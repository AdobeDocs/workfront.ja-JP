---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: ビュー：すべての日付の差異を含むタスク
description: このタスクビューは、Adobe Workfront アカウントで提供される「すべての日付」ビューに似ています。この特定のビューには、日付間の日数の差を計算する差異列が含まれます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 20df7cd8-113e-4c0d-b3f5-1def7db968a5
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '810'
ht-degree: 98%

---

# ビュー：「すべての日付」の差異を含むタスク

このタスクビューは、Adobe Workfront アカウントで提供される「すべての日付」ビューに似ています。このビューには、次の日付の間の日数の差を計算する&#x200B;*差異*&#x200B;列が含まれています。

* 開始予定日と見込み開始日
* 開始予定日と実際の開始日
* 完了予定日と見込み完了日
* 完了予定日と実際の完了日

このビューは、2 つの異なる列の値を入手して計算することで、3 つ目の値が取得される計算列の例を表します。ここでは、日付 2 から日付 1 が差し引かれます。

ビューでの計算の使用について詳しくは、[テキストモードの一般的な使用の概要](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)の[テキストモードの一般的な使用の概要](../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)を参照してください。

![Screen_Shot_2017-04-24_at_11.35.33_AM.png](assets/screen-shot-2017-04-24-at-11.35.33-am-350x95.png)

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>表示の変更をリクエスト </p>
   <p>レポートを変更するためのプラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルター、表示、グループ化へのアクセス権を編集して、表示を変更できるようにします。</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;自分のプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## すべての日付の差異を含むタスクの表示

1. タスクのリストに移動します。
1. **ビュー**&#x200B;ドロップダウンメニューから、**新規ビュー**&#x200B;を選択します。

1. **列のプレビュー**&#x200B;領域で、1 つを除くすべての列を削除します。
1. 残りの列のヘッダーをクリックし、「**テキストモードに切り替え**」をクリックします。
1. テキストモード領域にカーソルを置き、「**クリックしてテキストを編集**」をクリックします。
1. 「**テキストモード**」ボックスにあるテキストを削除し、次のコードに置き換えます。
   <pre>column.1.descriptionkey=name<br>column.1.link.linkproperty.0.name=ID<br>column.1.link.linkproperty.0.valuefield=ID<br>column.1.link.linkproperty.0.valueformat=int<br>column.1.link.lookup=link.view<br>column.1.link.valuefield=objCode<br>column.1.link.valueformat=val<br>column.1.linkedname=direct<br>column.1.listsort=string(name)<br>column.1.namekey=name.abbr<br>column.1.querysort=name<br>column.1.shortview=false<br>column.1.stretch=95<br>column.1.styledef.case.0.comparison.attribute=css<br>column.1.styledef.case.0.comparison.isrowcase=true<br>column.1.styledef.case.0.comparison.leftmethod=intAsInt(numberOfChildren)<br>column.1.styledef.case.0.comparison.lefttext=numberOfChildren<br>column.1.styledef.case.0.comparison.operator=gt<br>column.1.styledef.case.0.comparison.operatortype=int<br>column.1.styledef.case.0.comparison.righttext=0<br>column.1.styledef.case.0.comparison.trueproperty.0.name=fontstyle<br>column.1.styledef.case.0.comparison.trueproperty.0.value=bold<br>column.1.styledef.case.0.comparison.truetext=<br>column.1.styledef.case.0.comparison.usefield=false<br>column.1.valuefield=name<br>column.1.valueformat=HTML<br>column.1.width=150<br>column.2.descriptionkey=plannedstartdate<br>column.2.linkedname=direct<br>column.2.listsort=atDateAsAtDate(plannedStartDate)<br>column.2.namekey=plannedstartdate.abbr<br>column.2.querysort=plannedStartDate<br>column.2.shortview=false<br>column.2.stretch=0<br>column.2.valuefield=plannedStartDate<br>column.2.valueformat=atDate<br>column.2.width=75<br>column.3.descriptionkey=projectedstartdate<br>column.3.linkedname=direct<br>column.3.listsort=atDateAsAtDate(projectedStartDate)<br>column.3.namekey=projectedstartdate.abbr<br>column.3.querysort=projectedStartDate<br>column.3.shortview=false<br>column.3.stretch=0<br>column.3.valuefield=projectedStartDate<br>column.3.valueformat=atDate<br>column.3.width=75<br>column.4.descriptionkey=plannedstartdate<br>column.4.displayname=Projected Start Variance<br>column.4.linkedname=direct<br>column.4.listsort=atDateAsAtDate(plannedStartDate)<br>column.4.namekey=plannedstartdate.abbr<br>column.4.querysort=plannedStartDate<br>column.4.shortview=false<br>column.4.stretch=0<br>column.4.styledef.case.0.comparison.attribute=css<br>column.4.styledef.case.0.comparison.isrowcase=false<br>column.4.styledef.case.0.comparison.leftmethod=atDateAsAtDate(plannedStartDate)<br>column.4.styledef.case.0.comparison.lefttext=plannedStartDate<br>column.4.styledef.case.0.comparison.operator=notnull<br>column.4.styledef.case.0.comparison.operatortype=date<br>column.4.styledef.case.0.comparison.righttext=<br>column.4.styledef.case.0.comparison.trueproperty.0.name=bgcolor<br>column.4.styledef.case.0.comparison.trueproperty.0.value=E1E1E1<br>column.4.styledef.case.0.comparison.truetext=<br>column.4.styledef.case.0.comparison.usefield=false<br>column.4.valueexpression=ROUND(DATEDIFF({projectedStartDate},{plannedStartDate}))<br>column.4.valueformat=HTML<br>column.4.width=75<br>column.5.descriptionkey=plannedstartdate<br>column.5.linkedname=direct<br>column.5.listsort=atDateAsAtDate(plannedStartDate)<br>column.5.namekey=plannedstartdate.abbr<br>column.5.querysort=plannedStartDate<br>column.5.shortview=false<br>column.5.stretch=0<br>column.5.valuefield=plannedStartDate<br>column.5.valueformat=atDate<br>column.5.width=75<br>column.6.descriptionkey=actualstartdate<br>column.6.linkedname=direct<br>column.6.listsort=atDateAsAtDate(actualStartDate)<br>column.6.namekey=actualstartdate.abbr<br>column.6.querysort=actualStartDate<br>column.6.shortview=false<br>column.6.stretch=0<br>column.6.valuefield=actualStartDate<br>column.6.valueformat=atDate<br>column.6.width=75<br>column.7.descriptionkey=plannedstartdate<br>column.7.displayname=Actual Start Variance<br>column.7.linkedname=direct<br>column.7.listsort=atDateAsAtDate(plannedStartDate)<br>column.7.namekey=plannedstartdate.abbr<br>column.7.querysort=plannedStartDate<br>column.7.shortview=false<br>column.7.stretch=0<br>column.7.styledef.case.0.comparison.attribute=css<br>column.7.styledef.case.0.comparison.isrowcase=false<br>column.7.styledef.case.0.comparison.leftmethod=atDateAsAtDate(plannedStartDate)<br>column.7.styledef.case.0.comparison.lefttext=plannedStartDate<br>column.7.styledef.case.0.comparison.operator=notnull<br>column.7.styledef.case.0.comparison.operatortype=date<br>column.7.styledef.case.0.comparison.righttext=<br>column.7.styledef.case.0.comparison.trueproperty.0.name=bgcolor<br>column.7.styledef.case.0.comparison.trueproperty.0.value=E1E1E1<br>column.7.styledef.case.0.comparison.truetext=<br>column.7.styledef.case.0.comparison.usefield=false<br>column.7.valueexpression=ROUND(DATEDIFF({actualStartDate},{plannedStartDate}))<br>column.7.valueformat=HTML<br>column.7.width=75<br>column.8.descriptionkey=plannedcompletiondate<br>column.8.linkedname=direct<br>column.8.listsort=atDateAsAtDate(plannedCompletionDate)<br>column.8.namekey=plannedcompletiondate.abbr<br>column.8.querysort=plannedCompletionDate<br>column.8.shortview=false<br>column.8.stretch=0<br>column.8.valuefield=plannedCompletionDate<br>column.8.valueformat=atDate<br>column.8.width=75<br>column.9.descriptionkey=projectedcompletiondate<br>column.9.linkedname=direct<br>column.9.listsort=atDateAsAtDate(projectedCompletionDate)<br>column.9.namekey=projectedcompletiondate.abbr<br>column.9.querysort=projectedCompletionDate<br>column.9.shortview=false<br>column.9.stretch=0<br>column.9.valuefield=projectedCompletionDate<br>column.9.valueformat=atDate<br>column.9.width=75<br>column.10.descriptionkey=plannedcompletiondate<br>column.10.displayname=Projected Completion Variance<br>column.10.linkedname=direct<br>column.10.listsort=atDateAsAtDate(plannedCompletionDate)<br>column.10.namekey=plannedcompletiondate.abbr<br>column.10.querysort=plannedCompletionDate<br>column.10.shortview=false<br>column.10.stretch=0<br>column.10.styledef.case.0.comparison.attribute=css<br>column.10.styledef.case.0.comparison.isrowcase=false<br>column.10.styledef.case.0.comparison.leftmethod=atDateAsAtDate(plannedCompletionDate)<br>column.10.styledef.case.0.comparison.lefttext=plannedCompletionDate<br>column.10.styledef.case.0.comparison.operator=notnull<br>column.10.styledef.case.0.comparison.operatortype=date<br>column.10.styledef.case.0.comparison.righttext=<br>column.10.styledef.case.0.comparison.trueproperty.0.name=bgcolor<br>column.10.styledef.case.0.comparison.trueproperty.0.value=E1E1E1<br>column.10.styledef.case.0.comparison.truetext=<br>column.10.styledef.case.0.comparison.usefield=false<br>column.10.valueexpression=ROUND(DATEDIFF({projectedCompletionDate},{plannedCompletionDate}))<br>column.10.valueformat=HTML<br>column.10.width=75<br>column.11.descriptionkey=plannedcompletiondate<br>column.11.linkedname=direct<br>column.11.listsort=atDateAsAtDate(plannedCompletionDate)<br>column.11.namekey=plannedcompletiondate.abbr<br>column.11.querysort=plannedCompletionDate<br>column.11.shortview=false<br>column.11.stretch=0<br>column.11.valuefield=plannedCompletionDate<br>column.11.valueformat=atDate<br>column.11.width=75<br>column.12.descriptionkey=actualcompletiondate<br>column.12.linkedname=direct<br>column.12.listsort=atDateAsAtDate(actualCompletionDate)<br>column.12.namekey=actualcompletiondate.abbr<br>column.12.querysort=actualCompletionDate<br>column.12.shortview=false<br>column.12.stretch=0<br>column.12.valuefield=actualCompletionDate<br>column.12.valueformat=atDate<br>column.12.width=75<br>column.13.descriptionkey=plannedcompletiondate<br>column.13.displayname=Actual Completion Variance<br>column.13.linkedname=direct<br>column.13.listsort=atDateAsAtDate(plannedCompletionDate)<br>column.13.namekey=plannedcompletiondate.abbr<br>column.13.querysort=plannedCompletionDate<br>column.13.shortview=false<br>column.13.stretch=0<br>column.13.styledef.case.0.comparison.attribute=css<br>column.13.styledef.case.0.comparison.isrowcase=false<br>column.13.styledef.case.0.comparison.leftmethod=atDateAsAtDate(plannedCompletionDate)<br>column.13.styledef.case.0.comparison.lefttext=plannedCompletionDate<br>column.13.styledef.case.0.comparison.operator=notnull<br>column.13.styledef.case.0.comparison.operatortype=date<br>column.13.styledef.case.0.comparison.righttext=<br>column.13.styledef.case.0.comparison.trueproperty.0.name=bgcolor<br>column.13.styledef.case.0.comparison.trueproperty.0.value=E1E1E1<br>column.13.styledef.case.0.comparison.truetext=<br>column.13.styledef.case.0.comparison.usefield=false<br>column.13.valueexpression=ROUND(DATEDIFF({actualCompletionDate},{plannedCompletionDate}))<br>column.13.valueformat=HTML<br>column.13.width=75<br>row.0.styledef.applyallcases=true<br>row.0.styledef.case.0.comparison.attribute=css<br>row.0.styledef.case.0.comparison.isrowcase=true<br>row.0.styledef.case.0.comparison.leftmethod=intAsInt(numberOfChildren)<br>row.0.styledef.case.0.comparison.lefttext=numberOfChildren<br>row.0.styledef.case.0.comparison.operator=gt<br>row.0.styledef.case.0.comparison.operatortype=int<br>row.0.styledef.case.0.comparison.righttext=0<br>row.0.styledef.case.0.comparison.trueproperty.0.name=fontstyle<br>row.0.styledef.case.0.comparison.trueproperty.0.value=bold<br>row.0.styledef.case.0.comparison.truetext=<br>row.0.styledef.case.0.comparison.usefield=false</pre>

1. 「**ビューの保存**」をクリックします。
