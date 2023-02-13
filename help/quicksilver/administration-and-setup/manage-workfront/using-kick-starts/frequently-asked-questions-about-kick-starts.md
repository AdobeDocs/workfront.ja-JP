---
user-type: administrator
content-type: faq
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: キックスタートに関するよくある質問 (FAQ)
description: キックスタートを使用したWorkfrontデータのインポートとエクスポートに関するよくある質問に対する回答を見つけます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f286e03e-93a8-43f5-8c2d-2c36203776a8
source-git-commit: 1ebdb3797e30a7e06f4dfd4a7e0e5f540351c126
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# キックスタートに関するよくある質問 (FAQ)

以下は、キックスタートに関するよくある質問です。

## Kick-Start ファイルを読み込もうとすると、このエラーが表示されるのはなぜですか。「あなたのファイルは正しかったが、何も読み込まれなかった？」

### 回答

以下の 3 つのうちの 1 つが Kick-Start ファイルに見つからない可能性があります。

1. この **isNew** 列は **TRUE** を読み込むすべての項目に対して使用します。 **isNew** は、 **TRUE** 新しいデータを読み込むには、Kick-Start を使用する必要があります。 キックスタートを使用して既存のデータを変更することはできません。 スプレッドシートに他の行を追加する場合は、 **isNew = FALSE** ただし、これらの行はインポートされません。

1. &#x200B;ファイルでは、データのヘッダーを開始する前に空の行が 1 つ必要です。
1. Excel&#x200B;シートに正しい名前を付ける必要があります。

キックスタートを使用する場合は、まずキックスタートテンプレートをダウンロードし、正しいデータを手動で入力してから、Adobe Workfrontに再度読み込むことをお勧めします。

キックスタートを使用してWorkfrontでデータを正しく読み込む方法について詳しくは、 [キックスタートテンプレートを使用してAdobe Workfrontにデータを読み込む](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## Kick-Start ファイルを使用してWorkfrontに時間を読み込もうとすると、このエラーが表示されるのはなぜですか。&quot;プライマリキー値が&quot;null&quot;のユーザーが見つかりませんでしたか？&quot;

### 回答

エラーは、時間に関連付けられているユーザーの GUID を参照します。

これに対処するには：

1. 空のキックスタートテンプレートを **時間** オブジェクトのみ。\
   空のキックスタートファイルの書き出しについて詳しくは、  [キックスタートテンプレートを使用してAdobe Workfrontにデータを読み込む](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

1. 元の Kick-Start からデータを手動でコピーし、空のファイルに貼り付けます。\
   各列に対してこれを実行します。
1. 新しいファイルを再度読み込んでみてください。\
   Kick-Start は正常に読み込まれます。

## 「Kick-Start」インポートで、国フィールドにユーザープロファイルが入力されないのはなぜですか？

### 問題

ユーザーの読み込み時、「 」フィールドを使用してキックスタートを開始 **setCountry**&#x200B;の場合、そのデータはユーザープロファイル上の国には送信されません。

### 回答

ユーザーが統合ユーザー管理 (UUM) またはAdobeIdentity Managementシステム (IMS) に対して有効になっている場合、 **国** フィールドでは、国コードの値（例：米国、GB、IN）のみを使用できます。 を確認します。 **setCountry** キックスタートテンプレートのフィールドは、読み込む前に国コードの値を使用しています。

キックスタートを使用してWorkfrontでデータを正しく読み込む方法について詳しくは、 [キックスタートテンプレートを使用してAdobe Workfrontにデータを読み込む](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
