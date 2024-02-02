---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「ビューおよびグループ化：グループ化内の平均によって集計されたプロジェクトの実際の期間を表示」
description: プロジェクトレポートに以下の列を追加して、グループ化内の平均として集計された実際の期間を表示できます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 31794fe9-a04a-437d-8d2e-40e0cb6e6104
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: ht
source-wordcount: '358'
ht-degree: 100%

---

# ビューおよびグループ化：グループ化内の平均によって集計されたプロジェクトの実際の期間を表示

プロジェクトレポートに以下の列を追加して、グループ化内の平均として集計された実際の期間を表示できます。

![project_with_aggregate_actual_duration_in_grouping_view.png](assets/project-with-aggregate-actual-duration-in-grouping-view-350x65.png)

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

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## グループ化内の平均によって集計されたプロジェクトの実際の期間を表示

この列をプロジェクトビューに追加するには、以下のように行います。

1. （推奨）最適な結果を得るには、また実際の期間の集計平均値を確認するには、プロジェクトリストやレポートにグループ化を追加する必要があります。\
   グループ化の作成に関して詳しくは、[Adobe Workfront でのグループ化の概要](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)を参照してください。

1. 既存のプロジェクトビューに移動します。
1. 表示ドロップダウンメニューを展開し、「**表示をカスタマイズ**」を選択します。
1. 「**列を追加**」をクリックします。
1. 「**テキストモードに切り替え**」をクリックします。
1. **この列に表示**&#x200B;エリアにマウスを移動して、「**クリックしてテキストを編集**」をクリックします。

1. 「テキストモード」ボックスのすべてのテキストを削除し、次のコードに置き換えます。
   <pre>aggregator.displayformat=compound <br>aggregator.function=AVG <br>aggregator.namekey=view.relatedcolumn <br>aggregator.namekeyargkey=actualduration <br>aggregator.valuefield=actualDurationMinutes <br>aggregator.valueformat=val <br>displayname=Project Actual Duration <br>durationunitfield=durationUnit.value <br>linkedname=project <br>namekey=actualduration <br>namekeyargkey=actualduration <br>querysort=actualDurationMinutes <br>textmode=true <br>valuefield=actualDurationMinutes <br>valueformat=compound#M:D <br>viewalias=actualduration</pre>

1. 「**ビューを保存**」をクリックします。
