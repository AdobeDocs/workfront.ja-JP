---
product-area: projects
navigation-topic: issue-information
title: イシューを参照する際の「opTask」と「issue」の使用
description: イシューの名前は、Adobe Workfront データベースに opTask として現れます。場合によっては、issue フィールド名を使用してイシューを参照する必要がありますが、ほとんどの場合、イシューの参照時には issue ではなく opTask フィールド名を使用する必要があります。
author: Alina
feature: Work Management
exl-id: 91107c04-616c-49b2-aa78-10e373d11f6b
source-git-commit: 813b97ee0979e29a90293d9ddaba12a33c99f64d
workflow-type: ht
source-wordcount: '252'
ht-degree: 100%

---

# イシューを参照する際の「opTask」と「issue」の使用

イシューの名前は、Adobe Workfront データベースに `opTask` として現れます。場合によっては、`issue` フィールド名を使用してイシューを参照する必要がありますが、ほとんどの場合、イシューの参照時には `issue` ではなく `opTask` フィールド名を使用する必要があります。

Workfront データベースでオブジェクトがどのように現れるかについて詳しくは、[API エクスプローラー](https://developer.adobe.com/workfront/api-explorer/)を参照してください。

## `opTask` フィールド名

次のコンテキストでイシューを参照する場合は、`opTask` フィールド名を使用します。

* イシューのテキストモードのカスタムレポートを作成し、イシューをビュー、フィルター、グループ化またはプロンプトで参照する場合。

  レポートでのテキストモードの使用について詳しくは、[テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)を参照してください。

<!--* When you pull information about issues using our API.  
  For more information about the Workfront API, see [Adobe Workfront API](../../../wf-api/workfront-api.md)-->

* キックスタートデータインポーターシートのイシューフィールドを更新する場合。

  キックスタートを使用して Workfront にデータを読み込む方法について詳しくは、[キックスタートテンプレートを使用した Adobe Workfront へのデータの読み込み](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md)を参照してください。

## `issue` フィールド名

次のコンテキストでイシューを参照する場合は、`issue` フィールド名を使用します。

* レポートでテキストモードを使用してコレクション内のイシューを参照する場合。
* Workfront API を使用してイシューコレクションを参照する場合。

コレクションに関するレポートについては、[レポートでのコレクションの参照](../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)を参照してください。

<!--
<note type="tip">
For information about how issues appear in a collection, see the
<a href="https://developer.adobe.com/workfront/api-explorer/" target="_blank">API Explorer</a> and select the API Unsupported option from the upper-right corner of the page.
<br>(NOTE: Drafted because this might not be needed.)
</note>
-->
