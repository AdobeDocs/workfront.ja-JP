---
user-type: administrator
content-type: faq
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: キックスタートに関するよくある質問
description: 詳しくは、キックスタートを使用した Workfront データの読み込みおよび書き出しに関するよくある質問に対する回答を参照してください。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f286e03e-93a8-43f5-8c2d-2c36203776a8
source-git-commit: 1ebdb3797e30a7e06f4dfd4a7e0e5f540351c126
workflow-type: ht
source-wordcount: '415'
ht-degree: 100%

---

# キックスタートに関するよくある質問

キックスタートに関するよくある質問を次に示します。

## キックスタートファイルを読み込もうとすると、「ファイルは正常ですが、何も読み込まれませんでした」というエラーが表示されるのはなぜですか？

### 回答

次の 3 つのうちの 1 つがキックスタートファイルから欠けている可能性があります。

1. **isNew** 列は、読み込むすべての項目に対して **TRUE** の値に設定する必要があります。キックスタートでは新しいデータに限り読み込むことができるので、**isNew** を **TRUE** にする必要があります。キックスタートを使用して既存のデータを変更することはできません。スプレッドシートに他の行に **isNew = FALSE** を指定できますが、これらの行は読み込まれません。

1. ファイルでは、データのヘッダーを開始する前に空の行が 1 行必要です。
1. Excel シートに正しい名前を付ける必要があります。

キックスタートを使用する場合は、まずキックスタートテンプレートをダウンロードし、正しいデータを手動で入力してから、Adobe Workfront に再度読み込むことをお勧めします。

キックスタートを使用して Workfront でデータを正しく読み込む方法について詳しくは、[キックスタートテンプレートを使用して Adobe Workfront にデータを読み込む](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)を参照してください。

## キックスタートファイルを使用して Workfront に時間を読み込もうとすると、「プライマリキー値が「null」のユーザーが見つかりません」というエラーが表示されるのはなぜですか？

### 回答

エラーは、時間に関連付けられているユーザーの GUID を参照します。

これに対処するには、次の手順に従います。

1. 空のキックスタートテンプレートを&#x200B;**時間**&#x200B;オブジェクトのみに書き出します。\
   空のキックスタートファイルの書き出しについて詳しくは、[キックスタートテンプレートを使用して Adobe Workfront にデータを読み込む](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)を参照してください。

1. 元のキックスタートからデータを手動でコピーし、空のファイルに貼り付けます。\
   各列に対してこれを実行します。
1. 新しいファイルを再度読み込んでみてください。\
   キックスタートは正常に読み込まれます。

## キックスタートの読み込みで、国フィールドにユーザープロファイルが入力されないのはなぜですか？

### 問題

「**setCountry**」フィールドを使用してユーザーキックスタートを読み込む場合、そのデータはユーザープロファイルの国には反映されません。

### 回答

ユーザーが統合ユーザー管理（UUM）またはAdobe Identity Management システム（IMS）に対して有効になっている場合、「**国**」フィールドでは、国コードの値（US、GB、IN など）のみを使用できます。読み込む前に、キックスタートテンプレートの「**setCountry**」フィールドで国コードの値が使用されていることを確認します。

キックスタートを使用して Workfront でデータを正しく読み込む方法について詳しくは、[キックスタートテンプレートを使用して Adobe Workfront にデータを読み込む](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)を参照してください。
