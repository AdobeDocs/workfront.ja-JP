---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: タイムシートの合計時間の表示
description: タイムシートの合計時間数を表示できます。 この時間数には、プロジェクト、タスク、イシューに関して記録された時間とすべての一般的な時間が含まれます。
author: Lisa
feature: Timesheets
exl-id: ff0823f2-61d0-453f-ae1c-68f0f1465d73
TQID: https://experienceleague.adobe.com/oh6bBQz6sfxCpodHahZXtlMMuYYT-4U7-5MP6TQeuIs
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 64bb9e6dba8976ba413ec9b58e926da931bba1c5
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 56%
---
# タイムシートの合計時間の表示

<!--Audited: 8/2024-->

タイムシートの合計時間数を表示できます。 この時間数には、プロジェクト、タスク、イシューに関して記録された時間とすべての一般的な時間が含まれます。

合計時間数には、タイムシート、「更新」エリア、またはプロジェクト、タスク、イシューの「時間」エリアで提出された時間が反映されます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td> <p>明るいまたはそれ以上 </p>
   <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>タスクとイシューへのアクセス権を表示または高くする</p> </td> 
  </tr> 
  <tr> 
   <td>オブジェクト権限</td> 
   <td> <p>タスクとイシューに対する表示またはそれ以上の権限</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## タイムシートヘッダーのタイムシートの合計時間数の表示

タイムシートの合計時間数は、タイムシートのヘッダーに表示できます。

![合計時間数フィールド ](assets/timesheet-total-hours-in-header-highlighted-redesigned.png)

## タイムシートリストでのタイムシート合計時間数の表示

{{step1-to-timesheets}}

表示するアクセス権のあるタイムシートはすべて、デフォルトで表示されます。

![ タイムシート リスト ](assets/list-of-all-timesheets.png)

1. （オプション）次のいずれかの操作を行って、タイムシートリストのフィルターを更新します。

   * ページの右上隅にある「**自分のタイムシートの承認**」を選択して、承認したタイムシートのみを表示します。

     または

     「**マイタイムシート**」を選択して、自分のタイムシートのみを表示する。

     これは、**マイタイムシート承認**&#x200B;または&#x200B;**マイタイムシート** フィルターをタイムシートのリストに適用します。

   * **フィルター** アイコン ![ フィルターアイコン ](assets/filter-nwepng.png)をクリックして、フィルターを適用するか、新しいフィルターを作成します。 フィルターの作成または更新について詳しくは、[Adobe Workfront でのフィルターの作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)を参照してください。

   >[!NOTE]
   >
   >Workfrontの管理者またはグループ管理者が設定エリアのリストコントロールまたはレイアウトテンプレートからこれらのフィルターを削除した場合、タイムシートリストの上部またはフィルターのリストに「マイタイムシートの承認」オプションと「マイタイムシート」オプションが表示されません。 詳しくは、[レイアウトテンプレートを使用したフィルター、ビューおよびグループ化のカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)を参照してください。

1. （オプション）「**ビュー** ![ ビューのアイコン ](assets/view-icon.png)」または「**グループ化** ![ グループ化のアイコン ](assets/grouping.png)」アイコンをクリックして、ビューまたはグループ化を適用するか、新しいビューを作成します。

   フィルター、ビューまたはグループ化の作成については、次の記事を参照してください。

   * [Adobe Workfront でフィルターを作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Adobe Workfront でビューを作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Adobe Workfront でのグループ化の作成](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 各タイムシートの合計時間数は **合計時間数**&#x200B;列に表示されます。

   ![合計時間列](assets/total-hours-column.png)

   >[!TIP]
   >
   >タイムシートのリストに標準ビューを使用する場合、タイムシート上のアイテムのログ時間がタイムシートの時間枠の時間数を超えると、「合計時間」列が赤で表示されます。 詳しくは、[Adobe Workfront用語の用語集](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)の「合計時間数」フィールドを参照してください。
