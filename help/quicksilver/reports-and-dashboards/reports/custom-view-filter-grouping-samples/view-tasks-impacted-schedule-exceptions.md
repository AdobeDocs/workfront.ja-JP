---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: '''表示：スケジュールの例外の影響を受けるタスク'
description: このタスクビューは、週末、個人のタイムオフ、または他のスケジュールの例外が発生した場合に、遅延完了する必要があるタスクを識別します。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7d7c77fa-d9a7-4e91-8dae-ad3aaca6f1da
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '722'
ht-degree: 0%

---

# 表示：スケジュールの例外の影響を受けるタスク

このタスクビューは、週末、個人のタイムオフ、または他のスケジュールの例外が発生した場合に、遅延完了する必要があるタスクを識別します。

このビューには、次の情報が表示されます。

* タスクの期間
* タスクの計画開始日と計画完了日
* タスクの計画開始日から計画完了日までの日数に応じたタスクの期間（カレンダー期間）
* タスクを開始するプロジェクトのスケジュールの日数（カレンダー開始日）
* タスクの計画開始日から計画完了日までの平日数に応じたタスクの曜日の期間（週日の期間）
* Week Day Duration がタスクの期間よりも長い場合は、タスクの期間に例外日数が含まれていることを示し、タスクは「例外」としてマークされます。\
   ![tasks_with_calendar_exceptions.png](assets/tasks-with-calendar-exceptions-350x51.png)

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

## スケジュールの例外の影響を受けるタスクを表示

1. タスクのリストに移動します。
1. 次の **表示** ドロップダウンメニューで、「 **新しいビュー**.

1. 内&#x200B;**列のプレビュー** 領域を選択し、1 つ以外のすべての列を削除します。
1. 残りの列のヘッダーをクリックし、 **テキストモードに切り替え**.
1. テキストモード領域の上にマウスを移動し、 **クリックしてテキストを編集**.
1. 検索したテキストを **テキストモード** 」ボックスに置き換えて、次のコードに置き換えます。
   <pre>column.0.descriptionkey=name<br>column.0.link.linkproperty.0.name=ID<br>column.0.link.linkproperty.0.valuefield=ID<br>column.0.link.linkproperty.0.valueformat=int<br>column.0.link.lookup=link.view<br>column.0.link.valuefield=objCode<br>column.0.link.valueformat=val<br>column.0.linkedname=direct<br>column.0.listsort=string(name)<br>column.0.namekey=name.abbr<br>column.0.querysort=name<br>column.0.shortview=false<br>column.0.stretch=100<br>column.0.valuefield=name<br>column.0.valueformat=HTML<br>column.0.width=150<br>column.1.descriptionkey=duration<br>column.1.linkedname=direct<br>column.1.listsort=intAsInt(durationMinutes)<br>column.1.namekey=duration.abbr<br>column.1.querysort=durationMinutes<br>column.1.shortview=false<br>column.1.stretch=0<br>column.1.valuefield=durationFieldLong<br>column.1.valueformat=compound<br>column.1.viewalias=duration<br>column.1.width=80<br>column.2.descriptionkey=plannedstartdate<br>column.2.linkedname=direct<br>column.2.listsort=atDateAsAtDate(plannedStartDate)<br>column.2.namekey=plannedstartdate.abbr<br>column.2.querysort=plannedStartDate<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=plannedStartDate<br>column.2.valueformat=atDate<br>column.2.width=80<br>column.3.descriptionkey=plannedcompletiondate<br>column.3.linkedname=direct<br>column.3.listsort=atDateAsAtDate(plannedCompletionDate)<br>column.3.namekey=plannedcompletiondate.abbr<br>column.3.querysort=plannedCompletionDate<br>column.3.shortview=false<br>column.3.stretch=0<br>column.3.valuefield=plannedCompletionDate<br>column.3.valueformat=atDate<br>column.3.width=80<br>column.4.aggregator.displayformat=int<br>column.4.aggregator.function=SUM<br>column.4.aggregator.namekey=id<br>column.4.aggregator.valueexpression=DATEDIFF({plannedCompletionDate},<br>{plannedStartDate})+1<br>column.4.aggregator.valueformat=intAsInt<br>column.4.descriptionkey=id<br>column.4.linkedname=direct<br>column.4.listsort=intAsInt(ID)<br>column.4.name=カレンダーの期間<br>column.4.querysort=ID<br>column.4.shortview=false<br>column.4.stretch=0<br>column.4.valueexpression=DATEDIFF({plannedCompletionDate},{plannedStartDate})+1<br>column.4.valueformat=int<br>column.4.width=80<br>column.5.aggregator.displayformat=int<br>column.5.aggregator.function=SUM<br>column.5.aggregator.namekey=id<br>column.5.aggregator.valueexpression=DATEDIFF({plannedStartDate},{project}.<br>{plannedStartDate})+0<br>column.5.aggregator.valueformat=intAsInt<br>column.5.descriptionkey=id<br>column.5.linkedname=direct<br>column.5.listsort=intAsInt(ID)<br>column.5.name=カレンダーの開始日<br>column.5.querysort=ID<br>column.5.shortview=false<br>column.5.stretch=0<br>column.5.valueexpression=DATEDIFF({plannedStartDate},{project}.{plannedStartDate})+0<br>column.5.valueformat=int<br>column.5.width=80<br>column.6.aggregator.displayformat=int<br>column.6.aggregator.function=SUM<br>column.6.aggregator.namekey=id<br>column.6.aggregator.valueexpression=WEEKDAYDIFF({plannedStartDate},<br>{plannedCompletionDate})+0<br>column.6.aggregator.valueformat=HTML<br>column.6.descriptionkey=id<br>column.6.linkedname=direct<br>column.6.listsort=intAsInt(ID)<br>column.6.name=曜日の期間<br>column.6.querysort=ID<br>column.6.shortview=false<br>column.6.stretch=0<br>column.6.valueexpression=WEEKDAYDIFF({plannedStartDate},{plannedCompletionDate})+0<br>column.6.valueformat=int<br>column.6.width=80<br>column.7.aggregator.displayformat=int<br>column.7.aggregator.expression=IF((WEEKDAYDIFF({plannedStartDate},{plannedCompletionDate})))&gt;({duration}/480),"Exception","")<br>column.7.aggregator.function=SUM<br>column.7.aggregator.namekey=id<br>column.7.aggregator.valueformat=HTML<br>column.7.linkedname=direct<br>column.7.listsort=intAsInt(ID)<br>column.7.name=Schedule<br>column.7.querysort=ID<br>column.7.shortview=false<br>column.7.stretch=0<br>column.7.valueexpression=IF((WEEKDAYDIFF({plannedStartDate},{plannedCompletionDate}))&gt;({duration}/480),"Exception","")<br>column.7.valueformat=HTML<br>column.7.width=80</pre>

1. クリック **ビューを保存**.
