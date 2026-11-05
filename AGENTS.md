---
source-git-commit: 59deddd679267d10059f19cfd2d86b164903500e
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 0%
---
# AGENTS.md

**workfront.en** リポジトリの担当者ガイダンス （Adobe Workfront英語）
documentation）。 このファイルは正規の命令を指しているので、どんなエージェントでも – 
読み込むコンベンションファイルに関係なく、同じルールに従います。

## 正規命令ファイル

- **リポジトリ全体のルール**: [.github/copilot-instructions.md](.github/copilot-instructions.md)
— candidate-article search, propose-before-edit, commit-message and PR formats,
「ギャップをインテリジェントに埋める」ことです。
- **標準の作成** （自動的に`help/**/*.md`に適用）:
  [.github/instructions/writing-quality.instructions.md](.github/instructions/writing-quality.instructions.md),
の詳細を含む
  [.cursor/skills/writing-quality/reference.md](.cursor/skills/writing-quality/reference.md)。
- **リリースノート** （`product-announcements/product-releases/**`に自動的に適用）:
  [.github/instructions/release-notes-formatter.instructions.md](.github/instructions/release-notes-formatter.instructions.md)。
- **クリーンアップのプレビュー強調表示** （オンデマンドワークフロー）:
  [.github/prompts/remove-preview-highlighting.prompt.md](.github/prompts/remove-preview-highlighting.prompt.md)。

## 交渉不可能な行動

1. **新しい記事を作成する前に、候補となる記事を検索します。** 新しいコンテンツが来たら
で、`help/`を検索し、それが当てはまる可能性のある既存の記事のランク付けリストを表示します。
作成する前に、どこにあるかを尋ねます。
2. **ヘルプ `.md`の記事を編集する前に変更点を提案します。** 提案を表示
diffを指定して、明示的な承認を待ちます。 唯一の例外は、「ただ修正する」と言う場合です
同じ順番に「要求しない、編集する」ことができます。 読み取り専用のリサーチとインチャット
描き方は常に大丈夫です。
3. **ギャップをインテリジェントに埋める。** 明確な意図があれば
ベストプラクティスに従って回答し、周囲の記事の見出しに一致させ，
オプションメニューではなく、用語、構造が表示されます。
4. **作成基準を`help/`の編集ごとに積極的に**&#x200B;適用します。待ってはいけません
思い出してもらう。

## コミットおよびPR規則

詳細については、[.github/copilot-instructions.md](.github/copilot-instructions.md)を参照してください
commit-message形式（必須件名≤最大50文字、追加部分は📖、追加部分は✏️
修正）とPR構造（ブランチ名のJira ID、`# Summary`、
`# Changes` （ファイル別、`# Context` → `## Jira`）。
