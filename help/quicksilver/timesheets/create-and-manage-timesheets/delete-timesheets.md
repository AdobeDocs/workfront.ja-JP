---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Adobe Workfront でのタイムシートの削除
description: タイムシートプロファイルの作成、編集、割り当てで説明しているように、タイムシートプロファイルに対して行った変更は、現在のタイムシートにすぐには有効になりません。 既存のタイムシートで変更を表示するには、生成済みのタイムシートを削除し、新しいタイムシートを生成する必要があります。 これは、タイムシートプロファイルをユーザーに関連付けて生成されたタイムシートにのみ当てはまります。
author: Alina
feature: Timesheets
exl-id: c6a86c1b-8580-4896-8933-d4e2818e98ed
TQID: https://experienceleague.adobe.com/kgFaOSFwNQIjArobJBWf5kT19pS8k0an1O05IIYxg9E
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 0a3a49ff0e6347e0a0b327fcd692d5e1d9598f08
workflow-type: tm+mt
source-wordcount: 742
ht-degree: 79%

---

# Adobe Workfront でのタイムシートの削除

[タイムシートプロファイルの作成、編集、割り当て](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)で説明しているように、タイムシートプロファイルに対して行った変更は、現在のタイムシートにすぐには有効になりません。 既存のタイムシートで変更を表示するには、生成済みのタイムシートを削除し、新しいタイムシートを生成する必要があります。 これは、タイムシートプロファイルをユーザーに関連付けて生成されたタイムシートにのみ当てはまります。

>[!NOTE]
>
>手動で作成されたタイムシートは、それ以降、タイムシートプロファイルにユーザーが関連付けられていない限り、再生成によって再作成することはできません。 手動で作成されたタイムシートを削除すると、データが失われる可能性があります。 単一のタイムシートの作成については、[単一使用タイムシートの作成](../../timesheets/create-and-manage-timesheets/create-tmshts.md)を参照してください。

Adobe Workfront 管理者またはグループ管理者は、システム内の全員に対してタイムシートを生成できます。 タイムシートの手動生成について詳しくは、以下を参照してください。

* [タイムシートの手動生成](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
* [グループのタイムシートプロファイルの作成と管理](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

>[!IMPORTANT]
>
>* 削除したタイムシートは復元できません。
>* 過去のタイムシートは、タイムシートプロファイルに基づいて自動的に生成されないので、削除しないことをお勧めします。 現在および将来のタイムシートを削除し手動で生成すれば、タイムシートプロファイルに対する変更を新しいタイムシートに即座に表示することができます。
>* タイムシートを削除しても、タスク、イシューおよびプロジェクトに対して記録された時間数は削除されません。 一般的な時間数のみがタイムシートと共に削除されます。 別のテキストエディターで、タイムシートに関連付けられている一般的な時間数を書き留めておいてください。 タイムシートを削除した後、新しいタイムシートに記録できます。
>

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td>
   <p>標準</p>
   <p>プラン</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td><p>タイムシートへの管理アクセス</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## リスト内のタイムシートの削除

{{step1-to-timesheets}}

「**すべて**」フィルターがデフォルトで選択されており、表示アクセス権のあるすべてのタイムシートが表示されます。

1つのタイムシートが選択された![&#x200B; タイムシート リスト &#x200B;](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （オプション）次のいずれかの操作を行って、タイムシートリストのフィルターを更新します。

   * ページの右上隅にある「**マイタイムシート承認**」を選択して、承認するタイムシートのみを表示する

     または

     「**マイタイムシート**」を選択して、自分のタイムシートのみを表示する。

     これにより、「マイタイムシート承認」フィルターまたは「マイタイムシート」フィルターが、タイムシートリストに適用されます。

     ![&#x200B; タイムシート リスト ページのタイムシート フィルターのボタン &#x200B;](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * フィルターアイコン ![&#x200B; フィルターアイコン &#x200B;](assets/filter-nwepng.png)をクリックして、別のフィルターを適用するか、新しいフィルターを作成します。 フィルターの作成または更新について詳しくは、[Adobe Workfront でのフィルターの作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)を参照してください。

   >[!NOTE]
   >
   >Workfrontの管理者またはグループ管理者が設定エリアのリストコントロールまたはレイアウトテンプレートからこれらのフィルターを削除した場合、タイムシートリストの上部またはフィルターのリストに「マイタイムシートの承認」オプションと「マイタイムシート」オプションが表示されません。 詳しくは、[レイアウトテンプレートを使用したフィルター、ビューおよびグループ化のカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)を参照してください。

1. （オプション）別のビューまたはグループ化を適用したり、新しいビューを作成したりするには、**ビュー** ![&#x200B; ビューのアイコン &#x200B;](assets/view-icon.png)または&#x200B;**グループ化** ![&#x200B; グループ化のアイコン &#x200B;](assets/grouping.png)をクリックします。

   フィルター、ビューまたはグループ化の作成については、次の記事を参照してください。

   * [Adobe Workfront でフィルターを作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Adobe Workfront でビューを作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Adobe Workfront でのグループ化の作成](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 削除する1つまたは複数のタイムシートを選択し、タイムシートのリストの上部にある&#x200B;**削除** アイコン ![削除アイコン &#x200B;](assets/delete.png)をクリックします。

1. 「**削除**」をクリックします。

   選択したタイムシートは削除され、復元できません。

   新しいタイムシートを生成するには、ユーザーがタイムシートプロファイルに関連付けられていることを確認し、Workfront 管理者またはグループ管理者に、新しいタイムシートの生成を依頼します。

   詳しくは、以下を参照してください。

   * [タイムシートプロファイルの作成、編集、割り当て](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)
   * [タイムシートの手動生成](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
   * [グループのタイムシートプロファイルの作成と管理](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

## タイムシートページからのタイムシートの削除

{{step1-to-timesheets}}

1. 削除するタイムシートをクリックして開きます。
1. タイムシート名の右側にある&#x200B;[!UICONTROL **詳細**] アイコン ![詳細アイコン &#x200B;](assets/more-icon.png)をクリックし、**削除**&#x200B;をクリックします。

   ![タイムシートページからのタイムシートの削除](assets/delete-timesheet-from-timesheet-page.png)
1. 「[!UICONTROL **削除**]」をクリックして確定します。

   タイムシートは削除され、復元できません。
