---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''表示：オブジェクトの詳細の解決に関する問題'
description: このイシュービューには、イシューの解決オブジェクトの名前と完了率が表示され、解決タスクやプロジェクトにアクセスしなくても、イシューの作成者はイシューの進行状況を把握できます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7f4c923a-01e4-4896-9f54-1f0c66d64bb5
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 0%

---

# 表示：オブジェクトの詳細の解決に関する問題

このイシュービューには、イシューの解決オブジェクトの名前と完了率が表示され、解決タスクやプロジェクトにアクセスしなくても、イシューの作成者はイシューの進行状況を把握できます。

このビューでは、

```
sharecol=true
```

タグを使用して、同じ列ヘッダーの下にある複数のフィールドを組み合わせることができます。 詳しくは、

```
sharecol
```

タグ、詳しくは、 [表示：1 つの共有列の複数の列から情報を結合](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md).

![issue_custom_view_with_resolving_object_name_and_percent_complete.png](assets/issue-custom-view-350x77.png)

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
   <td> <p>ビューの変更をリクエスト </p>
   <p>レポートの変更計画</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートを変更します</p> <p>フィルター、ビュー、グループへのアクセスを編集してビューを変更します</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## オブジェクトの詳細の解決に関する問題の表示

1. 問題のリストに移動します。
1. 次の **表示** ドロップダウンメニューで、「 **新しいビュー**.

1. 内&#x200B;**列のプレビュー** 領域を選択し、1 つ以外のすべての列を削除します。
1. 残りの列のヘッダーをクリックし、 **テキストモードに切り替え**.
1. テキストモード領域の上にマウスを移動し、 **クリックしてテキストを編集**.
1. 検索したテキストを **テキストモード** 」ボックスに置き換えて、次のコードに置き換えます。<pre>column.0.querysort=name</pre><pre>column.0.stretch=0<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=sourceobject<br>column.1.linkedname=direct<br>column.1.listsort=nested(referenceObject).HTML(name)<br>column.1.namekey=sourceobject.abbr<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=referenceObject:name<br>column.1.valueformat=HTML<br>column.1.viewalias=source<br>column.1.width=100<br>column.2.descriptionkey=assignedto<br>column.2.link.linkproperty.0.name=ID<br>column.2.link.linkproperty.0.valuefield=assignedTo:ID<br>column.2.link.linkproperty.0.valueformat=int<br>column.2.link.lookup=link.view<br>column.2.link.valuefield=assignedTo:objCode<br>column.2.link.valueformat=val<br>column.2.linkedname=assignedTo<br>column.2.listsort=nested(assignedTo).string(name)<br>column.2.namekey=assignedto<br>column.2.querysort=assignedTo:name<br>column.2.shortview=false<br>column.2.stretch=25<br>column.2.valuefield=assignedTo:name<br>column.2.valueformat=HTML<br>column.2.width=150<br>column.3.descriptionkey=entrydate<br>column.3.linkedname=direct<br>column.3.listsort=atDateAsAtDate(entryDate)<br>column.3.namekey=entrydate.abbr<br>column.3.querysort=entryDate<br>column.3.shortview=false<br>column.3.stretch=0<br>column.3.valuefield=entryDate<br>column.3.valueformat=atDate<br>column.3.width=150<br>column.4.descriptionkey=description<br>column.4.linkedname=direct<br>column.4.listsort=string(description)<br>column.4.namekey=description.abbr<br>column.4.querysort=description<br>column.4.shortview=false<br>column.4.stretch=75<br>column.4.valuefield=description<br>column.4.valueformat=HTML<br>column.4.width=150<br>column.5.descriptionkey=status<br>column.5.enumclass=com.attask.common.constants.OpTaskStatusEnum<br>column.5.linkedname=direct<br>column.5.listsort=string(status)<br>column.5.namekey=status.abbr<br>column.5.querysort=status<br>column.5.shortview=false<br>column.5.stretch=0<br>column.5.type=enum<br>column.5.valuefield=status<br>column.5.valueformat=val<br>column.5.width=150<br>column.6.displayname=Resolving Object Name<br>column.6.linkedname=resolveTask<br>column.6.namekey=view.relatedcolumn<br>column.6.namekeyargkey.0=resolveTask<br>column.6.namekeyargkey.1=name<br>column.6.querysort=resolveTask:name<br>column.6.sharecol=true<br>column.6.textmode=true<br>column.6.valuefield=resolveTask:name<br>column.6.valueformat=HTML<br>column.7.displayname=<br>column.7.linkedname=resolveOpTask<br>column.7.namekey=view.relatedcolumn<br>column.7.namekeyargkey.0=resolveOpTask<br>column.7.namekeyargkey.1=name<br>column.7.querysort=resolveOpTask:name<br>column.7.sharecol=true<br>column.7.textmode=true<br>column.7.valuefield=resolveOpTask:name<br>column.7.valueformat=HTML<br>column.8.displayname=<br>column.8.linkedname=resolveProject<br>column.8.namekey=view.relatedcolumn<br>column.8.namekeyargkey.0=resolveProject<br>column.8.namekeyargkey.1=name<br>column.8.querysort=resolveProject:name<br>column.8.textmode=true<br>column.8.valuefield=resolveProject:name<br>column.8.valueformat=HTML<br>column.9.displayname=Resolving Object Percent Complete<br>column.9.textmode=true<br>column.9.valueexpression=IF(ISBLANK({resolveTask}.{ID})、{resolveProject}。{percentComplete},IF(ISBLANK({resolveProject}.{ID})、{resolveTask}。{percentComplete},&quot;)<br>column.9.valueformat=doubleAsPercentRounded</pre>

1. クリック **ビューを保存**.
