---
name: clean-el-traffic-csv
description: 生のExperience League/Adobe Analytics トラフィック CSVをページビュー別に並べ替えて、Workfront専用ページに書き出します。 ユーザーがExperience Leagueのページトラフィック CSV （「Page URL Generic」、「Unique Visitors」、「Visits」、「Page Views」などの列）を提供し、それをクリーニング、フィルタリング、処理するように求めるか、「ドキュメントのトラッキング」/「最も閲覧された記事」スプレッドシートに言及する場合に使用します。
source-git-commit: e22d43e9962b2b00793577fd14ac00587e8a2a6d
workflow-type: tm+mt
source-wordcount: '876'
ht-degree: 0%

---


# Experience Leagueのトラフィック CSVのクリーニング

Experience League ページトラフィックの生のAdobe Analytics フリーフォームテーブルの書き出しを、ページビューごとに並べ替えられたクリーンでWorkfront専用の重複排除されたCSVに変換し、元のファイルを上書きし、日付のあるコピーをデスクトップに保存します。

## 入力シェイプ

入力は、次の2つのシェイプのいずれかになります。

1. **Raw書き出し** — メタデータのコメント行（`#===`、`# Freeform`、`# Report suite: ...`、`"# Date: <range>"`など）で始まり、その後に階層的な分類テーブル（`Solution (v2)` → `workfront` → `Page URL Generic (v33)` →URL行など）が続きます。 リテラルセル `Page URL Generic (v33)` （または類似の`Page URL Generic ...` ラベル）は、2列目で部分的に下に表示されます。
2. **既にクリーンなCSV** – 最初の行は既に`Page URL Generic (v33),Unique Visitors,Visits,Page Views`のようなプレーンヘッダーであり、メタデータ行や追加の行送り列はありません。

開始する前に、どのシェイプを使用しているかを検出します。行1がシェイプ 2に一致するプレーンヘッダー行である場合は、手順2に直接スキップします（日付範囲は使用できません。ユーザーが日付範囲を個別に指定しない限り、手順7もスキップします）。

## ワークフロー

### 手順0：日付範囲をキャプチャする（未加工の書き出しのみ、何かを削除する前に）

`# Date: <range>`に一致する最上位のメタデータ行を検索します（例：`"# Date: Jul 1, 2026 - Jul 31, 2026"`）。 レコード `<range>` （例：`Jul 1, 2026 - Jul 31, 2026`） – 後の手順7で必要になります。 行が削除される前に、この操作を行います。

### 手順1：生の書き出しをプレーンテーブルに取り除く（生の書き出しのみ）

1. セル `Page URL Generic (...)`を含む行を検索します（標準書き出しの2番目の列にあります）。
2. メタデータのコメント行と`Solution (v2)` / `workfront`の小計行を含め、その行の上のすべての行を削除します。
3. `Page URL Generic` セルの左側にあるすべての列を削除します（標準的な書き出しでは、列Aのみです）。
4. 同じ行（現在はヘッダー行）で、数値の小計の値を`Page URL Generic (...)`の右側のリテラルヘッダーに置き換えます（順序：`Unique Visitors`、`Visits`、`Page Views`）。 `Page URL Generic (...)` セル自体は変更しないでください。

結果：ヘッダー`Page URL Generic (v33),Unique Visitors,Visits,Page Views`の後に1行/URLが続くプレーン CSV。

### 手順2:Workfront行のみを保持する

データ行ごとに、URLにリテラル部分文字列`/workfront/` （両側にスラッシュ）が含まれているかどうかを確認します。 ロケールのプレフィックスは問題ありません（`/en/`、`/zh-hans/`など – 製品セグメントが一致する限り、すべて維持されます）。

- URLが&#x200B;**not**&#x200B;に`/workfront/`がパスセグメントとして含まれている場合は、行を削除します。これにより、`workfront-fusion`、`workfront-learn`、`proofhqpapi`などの他の製品が削除されます（`tutorials-workfront`のような部分文字列は&#x200B;**not**&#x200B;件です。一致するセグメントは`/workfront/`と完全に一致する必要があります）。
- それ以外の場合は行を保持します。

### 手順3:URLのトリミング

残っている行ごとに、URLで`/using`を見つけ、その後に続く`/`の部分のみを保持し、`/using`の前と後のすべてを破棄します。

例：`https://experienceleague.adobe.com/ja/docs/workfront/using/home` → `/home`

Workfront行のURLに`/using`が見つからない場合は、そのURLを変更せずに、推測するのではなくユーザーにフラグを立てます。

### 手順4：フラグメント/クエリサフィックスの削除

トリミングされたURLに`#`または`?`が含まれている場合は、その文字とその後のすべての文字を削除します。

例：`/manage-scenarios/restore-a-scenario-version#compare-scenario-versions` → `/manage-scenarios/restore-a-scenario-version`

### 手順5：重複の結合

トリミング後、複数の行が同じURLを共有できるようになりました（例：同じパスに折りたたまれる2つの異なるロケール行）。 同一のURLを持つすべての行を1つの行に結合し、`Unique Visitors`、`Visits`および`Page Views`を個別に合計します。

例：`/home,2,2,3` and `/home,5,6,7` → `/home,7,8,10`

### 手順6：ページビューで並べ替え

すべてのデータ行を`Page Views`降順に並べ替えます（最初に最大）。 ヘッダー行は、並べ替えられたデータの上の上部に固定されたままになります。

### 手順7：日付範囲の行を追加する（手順0でキャプチャした場合は、未加工の書き出しのみ）

挿入する前に、取り込んだ日付範囲（例：`Jul 1, 2026 - Jul 31, 2026` → `Jul 1 2026 - Jul 31 2026`）からカンマを取り除きます。生の範囲には、その行のCSV列セパレータとして読み間違えられるカンマがあります。

ヘッダー行の上の一番上に、コンマで区切った日付範囲のみを含む1つの新しい行を挿入します。

最終行の順序：日付範囲の行→ヘッダー行→並べ替えられたデータ行。

### ステップ 8：保存

元の入力ファイルを、クリーニングされた結果で上書きします。

### 手順9：日付のコピーをデスクトップに保存（手順0で日付範囲がキャプチャされた場合のみ、未加工の書き出し）

日付範囲のファイル名に安全なバージョンを作成します。コンマを削除し、`\ / : * ? " < > |`のいずれかを`-`に置き換えます（これらの文字はWindows ファイル名では無効であり、書き出しロケールや形式によっては日付範囲に表示される可能性があります）。

現在のユーザーのデスクトップに、クリーニングされたCSV （手順8と同じ内容）の追加コピーを保存します。次の名前を付けます。

`Documentation tracking report <filename-safe date range>.csv`

例：`Apr 1, 2026 - Apr 30, 2026`のキャプチャ範囲は`Documentation tracking report Apr 1 2026 - Apr 30 2026.csv`になります。

ユーザーが日付範囲を個別に指定しない限り、既にクリーンなCSV （シェイプ 2）に対してこの手順をスキップします。

## 範囲外

クレンジングしたCSVを投稿または共有する（例：Slackへ）は、未定義の個別の手順です。この手順の一部として、ファイルを添付したり、アップロードしたりしないでください。

## 実装（未加工エクスポート）

生の書き出しを行う場合は、手動で行を編集するのではなく、このテスト済みのPowerShell スクリプトを使用して手順0 ～ 8を実行します。数百行のファイルでは、より高速でエラーが発生しやすくなります。 実際のファイル パスを`$path`に置き換えます。

実行する前に、ファイルがロックされているかどうかを確認します（例：Excelで開く）。「`Set-Content`」が「別のプロセスで使用されている」場合に失敗した場合は、ユーザーにファイルを閉じるよう依頼してから、再実行します。

```powershell
$path = "<full path to the CSV>"
$lines = Get-Content -Path $path -Encoding UTF8

# Step 0: capture the date range
$dateLine = $lines | Where-Object { $_ -match '# Date:\s*(.+?)"?\s*$' } | Select-Object -First 1
$null = $dateLine -match '# Date:\s*(.+?)"?\s*$'
$dateRange = $matches[1].Trim('"').Trim()

# Step 1: find the "Page URL Generic" row and strip everything above/left of it
$headerIdx = -1
for ($i = 0; $i -lt $lines.Count; $i++) {
    if ($lines[$i] -match 'Page URL Generic') { $headerIdx = $i; break }
}
$headerParts = $lines[$headerIdx].Split(',')
$urlHeaderLabel = $headerParts[1]
$newHeader = "$urlHeaderLabel,Unique Visitors,Visits,Page Views"

$dataLines = $lines[($headerIdx + 1)..($lines.Count - 1)] | Where-Object { $_.Trim() -ne '' }

$rows = @()
foreach ($line in $dataLines) {
    $comma1 = $line.IndexOf(',')
    $rest = $line.Substring($comma1 + 1)   # drop column(s) left of the URL
    $parts = $rest.Split(',')
    if ($parts.Count -ne 4) { continue }
    $url = $parts[0]
    $uv = [int]$parts[1]
    $vi = [int]$parts[2]
    $pv = [int]$parts[3]

    # Step 2: keep only /workfront/ rows
    if ($url -notmatch '/workfront/') { continue }

    # Step 3: trim to from "/using" onward
    $usingIdx = $url.IndexOf('/using')
    if ($usingIdx -lt 0) { continue }   # flag/report these separately if any occur
    $trimmed = $url.Substring($usingIdx + 6)   # 6 = length of "/using"

    # Step 4: strip # or ? suffix
    $hashIdx = $trimmed.IndexOfAny(@('#', '?'))
    if ($hashIdx -ge 0) { $trimmed = $trimmed.Substring(0, $hashIdx) }

    $rows += [PSCustomObject]@{ URL = $trimmed; UV = $uv; Visits = $vi; PV = $pv }
}

# Step 5: merge duplicates
$grouped = $rows | Group-Object URL | ForEach-Object {
    [PSCustomObject]@{
        URL    = $_.Name
        UV     = ($_.Group | Measure-Object UV -Sum).Sum
        Visits = ($_.Group | Measure-Object Visits -Sum).Sum
        PV     = ($_.Group | Measure-Object PV -Sum).Sum
    }
}

# Step 6: sort by Page Views descending
$sorted = $grouped | Sort-Object -Property PV -Descending

# Step 7 + 8: prepend date range (commas stripped) + header, then save
$dateRangeNoCommas = $dateRange -replace ',', ''
$outLines = @()
$outLines += $dateRangeNoCommas
$outLines += $newHeader
$outLines += $sorted | ForEach-Object { "$($_.URL),$($_.UV),$($_.Visits),$($_.PV)" }

Set-Content -Path $path -Value $outLines -Encoding UTF8

# Step 9: also save a dated copy to the Desktop
$safeDateRange = ($dateRange -replace ',', '') -replace '[\\/:*?"<>|]', '-'
$desktopPath = Join-Path ([Environment]::GetFolderPath('Desktop')) "Documentation tracking report $safeDateRange.csv"
Set-Content -Path $desktopPath -Value $outLines -Encoding UTF8
```

既にクリーンなCSV （入力シェイプ 2）の場合は、ヘッダーの再配置、日付範囲ロジック、およびステップ 9をスキップして、既存のヘッダー/行をそのまま実行します。
