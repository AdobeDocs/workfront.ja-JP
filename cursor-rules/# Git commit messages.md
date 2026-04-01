---
source-git-commit: b3148e5706abd75f2dd260f32507dedf8e259f57
workflow-type: tm+mt
source-wordcount: '171'
ht-degree: 1%

---
# Git コミットメッセージ

常にこのルールを適用する。 Git コミットメッセージをドラフトまたは生成する場合（Source Control コミットボックスやAgent チャットで要求されたときなど）、次のフォーマットに従います。

## 件名（1行目のみ）

- **50文字以下**&#x200B;程度です。
- **必須ムード**&#x200B;の変更を要約します（例：「追加…」、「修正…」、「リファクタリング…」）。

## 空白行

本文の前に件名の後ろに1行&#x200B;**空白行**&#x200B;を残します。

## 本文（詳細な説明）

- **72文字**&#x200B;程度で行を折り返します（箇条書きのプレフィックスとスペースを含む）。
- 説明には&#x200B;**箇条書き**&#x200B;を使用します。 各箇条書きは、次のいずれかから始める必要があります。
   - **📖** – 新しいファイル、新しいセクション、新しい機能、新しいヘッダー、新しい行、その他のグリーンフィールドコンテンツなど、変更&#x200B;**によって新しい項目が**&#x200B;追加された場合に使用します。
   - **✏️** – 変更&#x200B;**が**&#x200B;の既存の作業を変更する場合に使用します。既存の行の編集、既存のセクションの更新、既存のコードのリファクタリング、または現在のコンテンツの変更です。

**📖**&#x200B;または&#x200B;**✏️**&#x200B;を各ボディの弾丸に適用すると、何が導入されたか何が変更されたかがわかります。

## テンプレート

プレースホルダーを入力します（最後のメッセージでは角かっこを残さないでください）。

```
<Summarize change(s) in around 50 characters or less>

<More detailed explanatory description of the change wrapped into about 72
characters with bullets. >
```

## 例

```
Add refresh token rotation to auth flow

- 📖 Add refresh_tokens table and Alembic migration for schema v3.
- ✏️ Update session middleware to rotate secrets and revoke old tokens.
```
