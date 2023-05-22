---
product-area: projects
navigation-topic: issue-information
title: 問題を参照する際には、「opTask」と「issue」を使用します
description: イシューの名前は、Adobe Workfrontデータベースに opTask と表示されます。 問題を参照する際に、問題フィールド名を使用する必要がある場合がありますが、ほとんどの場合、問題を参照する際には、問題ではなく opTask フィールド名を使用する必要があります。
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
source-git-commit: 813b97ee0979e29a90293d9ddaba12a33c99f64d
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 1%

---

# 問題を参照する際には、「opTask」と「issue」を使用します

問題の名前は、 `opTask` をAdobe Workfrontデータベースに追加します。 ただし、 `issue` ほとんどの場合、 `opTask` フィールド名の代わりに `issue` 問題を参照する場合。

Workfrontデータベースでのオブジェクトの表示について詳しくは、 [API エクスプローラ](https://developer.adobe.com/workfront/api-explorer/).

## `opTask` filename

以下を使用： `opTask` 次のコンテキストで問題を参照する際のフィールド名：

* テキストモードのカスタムレポートを作成して問題を表示、フィルタ、グループ化、プロンプトで参照する場合。

   レポートでのテキストモードの使用について詳しくは、 [テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

<!--* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)-->

* 「キックスタート」データインポーターシートの問題フィールドを更新する場合。

   キックスタートを使用してWorkfrontにデータを読み込む方法について詳しくは、 [キックスタートテンプレートを使用してAdobe Workfrontにデータを読み込む](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## `issue` フィールド名

以下を使用： `issue` 以下のコンテキストでの問題を参照するフィールド名：

* レポートのテキストモードを使用してコレクションで問題を参照する場合。
* Workfront API を使用して問題コレクションを参照する場合。

コレクションのレポートについて詳しくは、 [レポート内のコレクションの参照](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md).

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://developer.adobe.com/workfront/api-explorer/" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->
