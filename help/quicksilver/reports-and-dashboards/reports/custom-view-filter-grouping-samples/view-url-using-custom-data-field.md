---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: '''表示：カスタムデータフィールドを使用した外部 URL'
description: タスクビューで「カスタム URL」という名前の計算カスタムフィールドを使用して、内部カスタム URL へのリンクを表示できます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 5e402fed-71ce-438a-8da9-8f8d37550ea8
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 0%

---

# 表示：カスタムデータフィールドを使用した外部 URL

内部カスタム URL へのリンクを表示するには、 **計算済みカスタムフィールド** で「Custom URL」という名前が付けられている **タスクビュー**.

これにより、表示内の特定のオブジェクトからアプリケーションの特定の領域へ、レポートから直接リンクするのに役立ちます。

計算済みカスタムフィールドを作成する場合は、まずフィールドを作成してから、ビューを作成する必要があります。

次のセクションは、タスクの計算カスタムフィールドの例です。 カスタムフィールドはカスタム URL と呼ばれます。 カスタムビューには、フィールドの値と **URL** タスクのフィールド。

同じ手順を使用して、カスタムフォームを持つシステム内のすべてのオブジェクトに対して、類似した計算済みカスタムフィールドとカスタムビューを作成できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集</p> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 「カスタム URL」計算カスタムフィールドの作成

計算カスタムフィールドの作成について詳しくは、 [計算データをカスタムフォームに追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md).

カスタムフォームを作成するアクセス権がある場合は、「カスタム URL」と呼ばれるタスクの計算済みカスタムフィールドを作成できます。 このフィールドは、 **概要** 内のサブタブ **タスクの詳細** タブをクリックします。

1. 計算済みカスタムフィールドを作成します。
1. 「計算」フィールドに、次のコードを入力します。

   CONCAT(&quot;https://`<domain>`.my.workfront.com&quot;,&quot;/&quot;,&quot;task/&quot;,ID,&quot;/overview&quot;)

1. &quot;`<domain>`」と入力します。

   この

   ```
   /overview
   ```

   この URL の一部は、 **概要** セクションを追加します。

1. 作成後、 **計算済みカスタムフィールド**、 **カスタムフォーム** このフィールドをAdobe Workfrontの複数のタスクに設定し、新しいビューに表示する

## タスクの「カスタム URL」フィールドと「URL」フィールドを表示するビューを作成します

タスク **表示** 以下の例では、 **計算済みカスタムフィールド** 「カスタム URL」を **概要** タスク内のサブタブ&#x200B;**詳細** タブ、および **URL** タスクのフィールド。

![](assets/task-view-with-custom-url-field-quicksilver-350x70.png)

この表示をカスタマイズするには：

1. タスクのリストに移動します。
1. を展開します。 **表示** 」ドロップダウンを使用して、タスクリストの上部に表示されます。
1. クリック **表示をカスタマイズ**.
1. ビュー内の最初の列を除くすべての列を削除します。
1. 最初の列のヘッダーをクリックします。
1. クリック **テキストモードに切り替え** をクリックします。
1. クリック **クリックしてテキストを編集**.
1. 以下のテキストモードを 1 つの列に貼り付けます。\
   この例では、「column.1」となります。 「カスタム URL」フィールドの値をタスクの **概要**. &#39;Column.2.&#39; には、 **URL フィールド** タスクの
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat= int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield= objCode<br>column.0.link.valueformat= val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.description=カスタム URL<br>column.1.link.isnewwindow=true<br>column.1.link.url=customDataLabelsAsString(Custom URL)<br>column.1.linkedname=direct<br>column.1.listsort=customDataLabelsAsString(Custom URL)<br>column.1.name=Custom URL<br>column.1.querysort=URL<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=カスタム URL<br>column.1.valueformat=customDataLabelsAsString<br>column.1.width=150<br>column.2.descriptionkey=url<br>column.2.linkedname=direct<br>column.2.listsort=string(URL)<br>column.2.namekey=url.abbr<br>column.2.querysort=URL<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=URL<br>column.2.valueformat=HTML<br>column.2.width=150</pre>

1. クリック **ビューを保存**.
