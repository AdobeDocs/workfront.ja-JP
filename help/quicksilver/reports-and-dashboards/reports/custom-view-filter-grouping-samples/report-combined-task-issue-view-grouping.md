---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: レポート：タスクとイシューの組み合わせビューとグループ化
description: この作業アイテムレポートには、ユーザーが作業を承諾したタスクとイシューの両方が 1 つのレポートに表示されます。これは、カスタムグループ化と組み合わせる場合に最適です。
author: Nolan
feature: Reports and Dashboards
exl-id: 6eaae772-229d-44ea-b285-cbaf9e46eade
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 47%

---

# レポート：結合したタスクとイシューのビューとグループ化

<!--Audited: 10/2024-->

この作業項目レポートは、ユーザーが作業を承認したタスクと問題の両方を 1 つのレポートで表示します。 これは、カスタムグループ化と組み合わせる場合に最適です。

このレポートは、ビューに `sharecol=true` を使用して、同じ列ヘッダーの下にある複数のフィールドを組み合わせることができます。`sharecol` タグについて詳しくは、[表示：複数の列の情報を 1 つの共有列に結合](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-merge-columns.md)を参照してください。

>[!TIP]
>
>  作業項目ビューには、割り当てられたユーザーによって承認されたタスクと問題のみが表示されます。 このレポートには、[ 作業要求 ] または [ チーム要求 ] リストからユーザーの [ 作業割り当て ] リストに移動されていない作業項目は表示されません。

![work_item_report.png](assets/work-item-report-350x46.png)

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>フィルターの変更者または変更依頼 </p>
   <p>レポートを変更するための標準またはプラン</p>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルターを変更する場合は、フィルター、ビュー、グループ化への編集アクセス権</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## タスクとイシューのビューとグループ化を組み合わせたレポートを作成

このビューでレポートを作成するには、以下のように行います。

1. 右上隅の **メインメニュー** アイコン ![ メインメニューアイコン ](assets/main-menu-icon.png) をクリックするか、または右上隅の **メインメニュー** アイコン ![ メインメニューライン ](assets/lines-main-menu.png) をクリックして、可能であれば **レポート** をクリックします。

1. ドロップダウンメニューから **新規レポート**/**詳細**/**作業項目** をクリックします。

1. 「**列のプレビュー**」領域で、表示されている唯一の列のヘッダーをクリックします。 これは **外部参照** 列です。
1. 「**テキスト モードに切り替える**」をクリックします。
1. テキストモード領域にマウスポインターを置き、「**テキストモードを編集**」をクリックします。
1. テキストモードボックスで見つかったテキストを削除し、次のコードに置き換えます。

   ```
   column.0.description=Task or Issue 
   column.0.name=Issue or Task
   column.0.shortview=false
   column.0.stretch=0
   column.0.textmode=true
   column.0.type=image
   column.0.valueexpression=IF(ISBLANK({opTaskID}),'Task','Issue')
   column.0.valueformat=
   column.0.width=40
   column.1.description=Task or Issue Name
   column.1.isInlineEditable=false
   column.1.link.linkproperty.0.name=ID
   column.1.link.linkproperty.0.valuefield=task:ID
   column.1.link.linkproperty.0.valueformat=string
   column.1.link.lookup=link.view
   column.1.link.valuefield=task:objCode
   column.1.link.valueformat=val
   column.1.listsort=nested(task).string(name)
   column.1.name=Name
   column.1.sharecol=true
   column.1.shortview=false
   column.1.stretch=50
   column.1.textmode=true
   column.1.valuefield=task:name
   column.1.valueformat=HTML
   column.1.width=120
   column.2.isInlineEditable=false
   column.2.link.linkproperty.0.name=ID
   column.2.link.linkproperty.0.valuefield=opTask:ID
   column.2.link.linkproperty.0.valueformat=string
   column.2.link.lookup=link.view
   column.2.link.valuefield=opTask:objCode
   column.2.link.valueformat=val
   column.2.linkedname=opTask
   column.2.listsort=nested(opTask).string(name)
   column.2.shortview=false
   column.2.stretch=0
   column.2.textmode=true
   column.2.valuefield=opTask:name
   column.2.valueformat=HTML
   column.2.width=120
   column.3.description=Project Name
   column.3.isInlineEditable=false
   column.3.link.linkproperty.0.name=ID
   column.3.link.linkproperty.0.valuefield=task:projectID
   column.3.link.linkproperty.0.valueformat=string
   column.3.link.lookup=link.view
   column.3.link.valuefield=task:project:objCode
   column.3.link.valueformat=val
   column.3.listsort=nested(task).nested(project).string(name)
   column.3.name=Project Name
   column.3.sharecol=true
   column.3.shortview=false
   column.3.stretch=50
   column.3.textmode=true
   column.3.valuefield=task:project:name
   column.3.valueformat=HTML
   column.3.width=120
   column.4.isInlineEditable=false
   column.4.link.linkproperty.0.name=ID
   column.4.link.linkproperty.0.valuefield=opTask:projectID
   column.4.link.linkproperty.0.valueformat=string
   column.4.link.lookup=link.view
   column.4.link.valuefield=opTask:project:objCode
   column.4.link.valueformat=val
   column.4.linkedname=opTask
   column.4.listsort=nested(opTask).nested(project).string(name)
   column.4.shortview=false
   column.4.stretch=0
   column.4.textmode=true
   column.4.valuefield=opTask:project:name
   column.4.valueformat=HTML
   column.4.width=120
   column.5.displayname=Primary Assignee
   column.5.linkedname=assignment
   column.5.namekey=view.relatedcolumn
   column.5.namekeyargkey.0=assignment
   column.5.namekeyargkey.1=assignedToID
   column.5.querysort=assignment:assignedToID
   column.5.textmode=true
   column.5.valuefield=assignment:assignedTo:name
   column.5.valueformat=HTML
   column.6.displayname=Status
   column.6.enumclass=com.attask.common.constants.OpTaskStatusEnum
   column.6.enumtype=OPTASK
   column.6.linkedname=opTask
   column.6.namekey=view.relatedcolumn
   column.6.namekeyargkey.0=opTask
   column.6.namekeyargkey.1=status
   column.6.querysort=opTask:status
   column.6.sharecol=true
   column.6.textmode=true
   column.6.type=enum
   column.6.valuefield=opTask:status
   column.6.valueformat=val
   column.7.displayname=
   column.7.enumclass=com.attask.common.constants.TaskStatusEnum
   column.7.enumtype=TASK
   column.7.linkedname=task
   column.7.namekey=view.relatedcolumn
   column.7.namekeyargkey.0=task
   column.7.namekeyargkey.1=status
   column.7.querysort=task:status
   column.7.textmode=true
   column.7.type=enum
   column.7.valuefield=task:status
   column.7.valueformat=val
   column.8.displayname=Priority
   column.8.enumclass=com.attask.common.constants.TimelinePriorityEnum
   column.8.enumtype=OPTASK
   column.8.linkedname=opTask
   column.8.namekey=view.relatedcolumn
   column.8.namekeyargkey.0=opTask
   column.8.namekeyargkey.1=priority
   column.8.querysort=opTask:priority
   column.8.sharecol=true
   column.8.textmode=true
   column.8.type=enum
   column.8.valuefield=opTask:priority
   column.8.valueformat=val
   column.9.displayname=
   column.9.enumclass=com.attask.common.constants.TimelinePriorityEnum
   column.9.enumtype=TASK
   column.9.linkedname=task
   column.9.namekey=view.relatedcolumn
   column.9.namekeyargkey.0=task
   column.9.namekeyargkey.1=priority
   column.9.querysort=task:priority
   column.9.type=enum
   column.9.valuefield=task:priority
   column.9.valueformat=val
   column.10.isInlineEditable=false
   column.10.linkedname=task
   column.10.listsort=nested(task).atDateAsAtDate(plannedStartDate)
   column.10.name=Planned Start Date
   column.10.sharecol=true
   column.10.shortview=false
   column.10.stretch=0
   column.10.textmode=true
   column.10.valuefield=task:plannedStartDate
   column.10.valueformat=atDate
   column.10.width=100
   column.11.isInlineEditable=false
   column.11.linkedname=opTask
   column.11.listsort=nested(opTask).atDateAsAtDate(plannedStartDate)
   column.11.shortview=false
   column.11.stretch=0
   column.11.textmode=true
   column.11.valuefield=opTask:plannedStartDate
   column.11.valueformat=atDate
   column.11.width=1
   column.12.isInlineEditable=false
   column.12.linkedname=task
   column.12.listsort=nested(task).atDateAsAtDate(projectedCompletionDate)
   column.12.name=Planned Completion Date
   column.12.sharecol=true
   column.12.shortview=false
   column.12.stretch=0
   column.12.textmode=true
   column.12.valuefield=task:projectedCompletionDate
   column.12.valueformat=atDate
   column.12.width=100
   column.13.isInlineEditable=false
   column.13.linkedname=opTask
   column.13.listsort=nested(opTask).atDateAsAtDate(projectedCompletionDate)
   column.13.shortview=false
   column.13.stretch=0
   column.13.textmode=true
   column.13.valuefield=opTask:projectedCompletionDate
   column.13.valueformat=atDate
   column.13.width=1
   column.14.isInlineEditable=false
   column.14.linkedname=task
   column.14.listsort=nested(task).double(percentComplete)
   column.14.name=Percent Complete
   column.14.sharecol=true
   column.14.shortview=false
   column.14.stretch=0
   column.14.textmode=true
   column.14.valueexpression=IF(ISBLANK({taskID}),"",{task}.{percentComplete})
   column.14.valueformat=HTML
   column.14.width=100
   column.15.textmode=true
   column.15.value=
   column.15.valueformat=HTML
   column.15.width=1
   ```

1. 「**完了**」をクリックします。
1. （オプション）**グループ化**&#x200B;をクリックして、レポートにグループ化を追加します。
1. （オプションおよび条件付き）グループ化を追加する場合は、「**テキストモードに切り替え**」をクリックします。
1. （オプション）グループ化テキストモードエリア内のテキストを次のコードに置き換えます。

   ```
   group.0.name=
   group.0.valueexpression=IF(ISBLANK({opTaskID}),'Task','Issue')
   group.0.valueformat=string
   textmode=true
   ```

   このグループ化では、すべてのタスクをまとめてグループ化し、すべてのイシューをまとめてグループ化します。

1. 「**保存して閉じる**」をクリックします。
1. （オプション）レポートの名前を更新し、「**適用**」をクリックします。
