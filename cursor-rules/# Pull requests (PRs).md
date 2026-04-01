---
source-git-commit: b3148e5706abd75f2dd260f32507dedf8e259f57
workflow-type: tm+mt
source-wordcount: '400'
ht-degree: 0%

---
# プルリクエスト（PR）

プルリクエストのタイトルまたは説明（GitHub/GitLabやエージェントチャットで要求されたときなど）をドラフトまたはレビューする場合は、次の規則に従います。

## Jiraの問題の導出

- **Source of truth:** Jiraの課題IDを&#x200B;**現在のGit ブランチ名**&#x200B;から取得します（例：`FFENT-8796`など、プロジェクトキーパターンに一致するセグメント）。
- **ブランチ名にJira IDが含まれる場合：** PR タイトルにそのIDを使用し（以下を参照）、`# Context`→`## Jira`にリンクします。
- **ブランチ名にJira IDが含まれていない場合：** PRをチケットに関連付けられていないとして扱います。 **Jira キーをPR タイトルから削除**&#x200B;します（チケットは作成しないでください）。 まだ`# Context` → `## Jira`が含まれており、コンテンツは正確に`No ticket` （リンクなし）です。

## PR タイトル

**ブランチ名にJira課題ID**&#x200B;が含まれる場合は、**両方**&#x200B;を含めます。

1. **Jira課題ID** （例：`FFENT-8001`）。
2. このパターンを使用した&#x200B;**コミットの種類** （以下のリストを参照）:

`{type}/{JIRA-ID}- {short task description}`

例：

`feat/FFENT-8001- Add validation for numVariations in OCAPI request`

IDの後に簡潔な必須スタイルの説明を使用します。 表示される間隔パターンの末尾にハイフン、スペース、説明を含む文字、スラッシュ、Jira キーを一致させます。

**ブランチ名にJira課題ID**&#x200B;が含まれていない場合は、タイトルからチケットを省略して、次を使用します。

`{type}- {short task description}`

例：

`docs- Refresh Object Composite API changelog`

### 使用可能なコミットタイプ（`/`の前にこれらのラベルを使用）

- **feat** – 新機能を追加します。 新しい目次アイテムが追加されたり、JIRAが別の`feat`- ラベル付きJiraに接続されたりすると。
- **fix** — バグの修正
- **refactor** – 動作を変更せずにコードを書き換えたり再構築したりします
- **perf** — パフォーマンスの向上（特殊リファクタリング）
- **style** – 書式設定/空白のみ。意味の変更はありません。 編集内容のみ
- **test** — テストの追加または修正
- **docs** – 新しいコンテンツが追加されました。 ドキュメントのみ
- **ビルド** — ビルドツール、CI、依存関係、プロジェクトバージョンなど。
- **ops** — インフラストラクチャ、デプロイメント、バックアップ、リカバリなど。
- **chore** – その他（例：`.gitignore`）

## PR body — required sections

次のトップレベルのセクション **を正確に使用する** （マークダウン見出し）:

### 1. `# Summary`

**何**&#x200B;が変更されたか、なぜ&#x200B;**なぜ**&#x200B;の概要（ビジネスまたは技術的な意図）を簡単に説明します。

### 2. `# Changes`

**ファイル**&#x200B;で整理します。 タッチされた各ファイルに対して、バックティック内のパスにレベル 2の見出しを付け、編集内容を説明する箇条書きを付けます。

フォーマット：

```markdown
# Changes

## `path/to/file.ext`
* Concise bullet describing the change in that file.

## `another/file.ts`
* Another bullet for that file.
```

### 3. `# Context`

常に&#x200B;**の下に** Jira`# Context` サブセクションを含めます。

**ブランチ名にJira IDが含まれている場合：** クリック可能な問題へのリンクを使用します（ブランチ名からキーを取得します）。

フォーマット：

```markdown
# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

キーとURLを実際のチケットに置き換えます。 複数のチケットが適用される場合は、各チケットを同じサブセクション内の個別の行にリストします。

**ブランチ名にJira IDが含まれていない場合：** `## Jira`を保持し、正確に使用します：

```markdown
# Context

## Jira
No ticket
```

## 例（PRの詳細な説明）

```markdown
# Summary
Adds minimum and maximum constraints for numVariations in the Object Composite API v4 OpenAPI spec.

# Changes

## `static/object-composite-v4.json`
* numVariations in OCAPIRequest now includes minimum: 1 and maximum: 3 to align with the allowed range (number of variations to generate).

# Context

## Jira
[FFENT-8796](https://jira.corp.adobe.com/browse/FFENT-8796)
```

## 例（完全なPR説明、Jira IDのないブランチ）

**タイトル：** `docs- Refresh Object Composite API changelog`

```markdown
# Summary
Refreshes the changelog for the Object Composite API.

# Changes

## `CHANGELOG.md`
* Documents the latest OCAPI v4 constraint updates.

# Context

## Jira
No ticket
```
