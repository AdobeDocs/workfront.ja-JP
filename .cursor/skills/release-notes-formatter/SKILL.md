---
name: release-notes-formatter
description: Workfront リリースノートの書式と検証を行って、一貫性、正しい構造、適切なリンクを確認します。 製品リリースディレクトリ内のリリースノートファイル、またはユーザーがリリースノート、製品リリース、または四半期リリースについて言及した場合にのみ使用します。 ハウツー記事や一般的なドキュメントには適用されません。
source-git-commit: ec081e557ec48adcfcb3833bf11dcee91312ef4e
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 3%

---


# リリースノート形式

`help/quicksilver/product-announcements/product-releases/` ディレクトリのAdobe Workfront リリースノートをフォーマットして検証します。

## ページタイプ

ファイルパスとコンテンツからページタイプを特定します。

| ページ タイプ | ファイルパターン | テンプレート |
|-----------|-------------|----------|
| **概要** | `{YY}-q{N}-release-overview.md` | [reference.md#overview](reference.md#overview-page-template) |
| **製品エリア** | `{YY}-q{N}-{area}.md` | [reference.md#product-area](reference.md#product-area-page-template) |
| **計画中** | `planning-release-activity-{YY}-q{N}.md` | 商品エリアと同様 |
| **ルックアンドフィール** | `look-and-feel-updates-{YY}-q{N}.md` | [reference.md#look-and-feel](reference.md#look-and-feel-page-template) |

## 書式設定ワークフロー

### 手順1:Frontmatterの検証

すべてのリリースノートページの必須フィールド：

```yaml
---
title: <descriptive title>
description: <matches or summarizes the title>
author: <author name>
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: <existing UUID — never generate or change>
---
```

ルール：
- `feature`は正確に`Product Announcements`でなければなりません
- `recommendations`は正確に`noDisplay, noCatalog`でなければなりません
- `exl-id`を発明しない – 既に存在する場合にのみ含める
- 実際のページに`draft: Probably`を追加しない（テンプレートのみ）

### 手順2：ページタイプ別の構造の検証

#### 製品エリアページ

1. **H1**: `{Written Quarter} {Area} enhancements`
   - 例：`# Second Quarter 2026 Administrator enhancements`
   - 四半期には、「第1四半期」、「第2四半期」、「第3四半期」、「第4四半期」と記載する必要があります

2. **イントロパラグラフ**：概要のエリアとリンクを説明します
   - **四半期の**&#x200B;概要ファイルにリンクする必要があります
   - 一般的なバグ：前の四半期へのリンク（例：`26-q2`ではなく`26-q1`）

3. 機能ごとの&#x200B;**H2**：見出しとしての機能タイトル
   - **最新の機能が最初に** – 最新のリリースノートは、イントロパラグラフの後の最初のH2として表示される必要があります
   - 古い機能は時系列が逆になります

4. **各H2の後の日付コールアウトブロック**:

```markdown
>[!NOTE]
>
>Preview: {Month Day, Year}
>Production fast release: {Month Day, Year}
>Production for everyone: {Month Day, Year}
```

&#x200B;5. **Body**：機能の説明、ヘルプドキュメントへのリンク

#### 概要ページ

1. **H1**: `{Written Quarter} release overview`

2. 予定公開月を含む&#x200B;**イントロパラグラフ**

3. リリーススケジュール表を含む&#x200B;**`>[!IMPORTANT]`ブロック**

4. アンカーリンクの箇条書きリストを含む&#x200B;**H2`Adobe Workfront enhancements`**:

```markdown
* [Administrator enhancements](#administrator-enhancements)
* [Document enhancements](#document-enhancements)
```

&#x200B;5. HTML機能テーブルを含む製品領域&#x200B;**ごとの** H3 （[reference.md](reference.md#overview-feature-table)を参照）
   - 各テーブル内では、**最新の機能が最初に** – 最新の行がテーブルの上部（ヘッダー行の後）に表示されます

&#x200B;6. **後続セクション** （H2）：その他の領域のリリースノート、デスクトップ校正ビューアの更新、お知らせ、API バージョン、メンテナンスの更新、トレーニングの更新

### 手順3：リンクの検証

- **製品領域ページの概要リンク**：同じ四半期を指す必要があります
   - 正解：`26-q2-release-activity/26-q2-release-overview.md`
   - 間違っています：`26-q1-release-activity/26-q1-release-overview.md`
- **概要**&#x200B;のアンカーリンク：H3 ID （小文字、ハイフン）と一致する必要があります
- **概要テーブルの機能リンク**: `class="MCXref xref" xrefformat="{para}"`を使用する必要があります
- **ヘルプドキュメントのリンク**: `/help/quicksilver/`で始める必要があります

### 手順4：日付の検証

- 形式：`{Month} {Day}, {Year}` （例：「2026年3月12日」）
- 不明な日付に`TBD`を使用
- 製品領域ページ `>[!NOTE]` ブロックの日付は、対応する概要テーブル行と一致する必要があります
- プレビュー日は生産日より前にする必要があります

### 手順5：一般的な修正

書式設定時に次の修正を適用します。

| イシュー | 修正 |
|-------|-----|
| 不適切な概要リンク四半期 | ファイルの独自の四半期に一致するように更新 |
| `>[!NOTE]`日付ブロックがありません | H2機能見出しの後にブロックを追加 |
| 日付形式に一貫性がない | `Month Day, Year`に標準化 |
| `>[!NOTE]`の前に空白行がありません | 空白行を追加 |
| 吹き出し線内の余分なスペース | 末尾の空白をトリミング |
| HTMLの商品エリアページ | マークダウンとして保持（HTMLは概要テーブル専用） |
| `exl-id`がありません | そのままにしておきます。生成しないでください |

## ファイル命名規則

| タイプ | パターン | 例 |
|------|---------|---------|
| 概要 | `{YY}-q{N}-release-overview.md` | `26-q2-release-overview.md` |
| 製品エリア | `{YY}-q{N}-{area-slug}.md` | `26-q2-admin-and-setup.md` |
| ディレクトリ | `{YY}-q{N}-release-activity/` | `26-q2-release-activity/` |

標準領域スラグ：`admin-and-setup`、`documents`、`projects`、`reports`、`requests`、`other`

## 四半期マッピング

| 四半期 | 手書きフォーム | 月 |
|---------|-------------|--------|
| Q1 | 第1四半期 | ヤン=マール |
| Q2 | 第2四半期 | 4月 |
| Q3 | 第3四半期 | 7月 |
| Q4 | 第4四半期 | Oct-Dec |

四半期ごとの生産リリースは、通常、四半期の最後の月の第2週の木曜日にリリースされます。

## 検証チェックリスト

リリースノートファイルを確認する際は、次の点を確認します。

- [ ] Frontmatterには、すべての必須フィールドが正しい値で含まれています
- [ ] H1がページタイプ形式と一致しています
- [ ]概要リンクが正しい四半期を指しています
- [ ]各機能には`>[!NOTE]`個の日付ブロック （製品領域ページ）があります
- [ ]日付形式が一貫しています（`Month Day, Year`）
- [ 概要内の]機能テーブル行が製品領域ページのコンテンツに一致
- [ ]壊れた内部リンクはありません
- [ 概要の]個のアンカーリンクがH3 セクション IDと一致
- [ ]機能は、最新の順に並べられます（製品エリアページと概要テーブルの両方）

## その他のリソース

- HTMLのテンプレートと例について詳しくは、[reference.md](reference.md)を参照してください
