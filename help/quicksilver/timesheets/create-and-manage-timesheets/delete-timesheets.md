---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: Adobe Workfront でのタイムシートの削除
description: タイムシートプロファイルの作成、編集、割り当てで説明しているように、タイムシートプロファイルに対して行った変更は、現在のタイムシートにすぐには有効になりません。既存のタイムシートで変更を表示するには、生成済みのタイムシートを削除し、新しいタイムシートを生成する必要があります。これは、タイムシートプロファイルをユーザーに関連付けて生成されたタイムシートにのみ当てはまります。
author: Alina
feature: Timesheets
exl-id: c6a86c1b-8580-4896-8933-d4e2818e98ed
source-git-commit: 210ca2e82286ff904bc7defb7b8c9c2559489d66
workflow-type: ht
source-wordcount: '810'
ht-degree: 100%

---

# Adobe Workfront でのタイムシートの削除

[タイムシートプロファイルの作成、編集、割り当て](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)で説明しているように、タイムシートプロファイルに対して行った変更は、現在のタイムシートにすぐには有効になりません。既存のタイムシートで変更を表示するには、生成済みのタイムシートを削除し、新しいタイムシートを生成する必要があります。これは、タイムシートプロファイルをユーザーに関連付けて生成されたタイムシートにのみ当てはまります。

>[!NOTE]
>
>手動で作成されたタイムシートは、それ以降、タイムシートプロファイルにユーザーが関連付けられていない限り、再生成によって再作成することはできません。手動で作成されたタイムシートを削除すると、データが失われる可能性があります。単一のタイムシートの作成については、[単一使用タイムシートの作成](../../timesheets/create-and-manage-timesheets/create-tmshts.md)を参照してください。

Adobe Workfront 管理者またはグループ管理者は、システム内の全員に対してタイムシートを生成できます。タイムシートの手動生成について詳しくは、以下を参照してください。

* [タイムシートの手動生成](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
* [グループのタイムシートプロファイルの作成と管理](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

>[!IMPORTANT]
>
>* 削除したタイムシートは復元できません。
>* 過去のタイムシートは、タイムシートプロファイルに基づいて自動的に生成されないので、削除しないことをお勧めします。現在および将来のタイムシートを削除し手動で生成すれば、タイムシートプロファイルに対する変更を新しいタイムシートに即座に表示することができます。
>* タイムシートを削除しても、タスク、イシューおよびプロジェクトに対して記録された時間数は削除されません。一般的な時間数のみがタイムシートと共に削除されます。別のテキストエディターで、タイムシートに関連付けられている一般的な時間数を書き留めておいてください。タイムシートを削除した後、新しいタイムシートに記録できます。
>

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タイムシートに対する管理アクセス権が必要です。 </p> <p>詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">ユーザーに対する特定の領域への管理アクセス権の付与</a>を参照してください。</p> <p>まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がユーザーのアクセスレベルを変更する方法については、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

## リスト内のタイムシートの削除

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックします。

1. 「**タイムシート**」をクリックします。「**すべて**」フィルターがデフォルトで選択されており、表示アクセス権のあるすべてのタイムシートが表示されます。

   ![](assets/timesheet-list-one-timesheet-selected-nwe-350x70.png)

1. （オプション）次のいずれかの操作を行って、タイムシートリストのフィルターを更新します。

   * ページの右上隅にある「**マイタイムシート承認**」を選択して、承認するタイムシートのみを表示する。

     または

     「**マイタイムシート**」を選択して、自分のタイムシートのみを表示する。

     これにより、「マイタイムシート承認」フィルターまたは「マイタイムシート」フィルターが、タイムシートリストに適用されます。

     ![](assets/my-timesheet-approvals-my-timesheets-pills-on-timesheets-list-nwe-350x58.png)

   * フィルターアイコン ![](assets/filter-nwepng.png) をクリックして別のフィルターを適用するか、新しいフィルターを作成します。フィルターの作成または更新については、[Adobe Workfront でのフィルターを作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)を参照してください。

   >[!NOTE]
   >
   >Workfront 管理者またはグループ管理者が、設定領域の「リスト制御」またはレイアウトテンプレートから「マイタイムシート承認」フィルターと「マイタイムシート」フィルターを削除した場合、「マイタイムシート承認」オプションと「マイタイムシート」オプションは、タイムシートリストの上部またはフィルターリストには表示されません。詳しくは、次の記事を参照してください。
   >
   >   
   >   
   >* [レイアウトテンプレートを使用したフィルター、ビューおよびグループ化のカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >   
   >

1. （オプション）**表示**&#x200B;アイコン ![](assets/view-icon.png) または&#x200B;**グループ化**&#x200B;アイコン ![](assets/grouping.png) をクリックして、別のビューやグループ化を適用するか、新しいビューやグループ化を作成します。

   フィルター、ビューまたはグループ化の作成については、次の記事を参照してください。

   * [Adobe Workfront でのフィルターの作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Adobe Workfront でのビューの作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Adobe Workfront でのグループ化の作成](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 削除する 1 つまたは複数のタイムシートを選択し、タイムシートリストの上部にある&#x200B;**削除**&#x200B;アイコン ![](assets/delete.png) をクリックします。

1. 「**削除**」をクリックします。

   選択したタイムシートは削除され、復元できません。

   新しいタイムシートを生成するには、ユーザーがタイムシートプロファイルに関連付けられていることを確認し、Workfront 管理者またはグループ管理者に、新しいタイムシートの生成を依頼します。

   詳しくは、以下を参照してください。

   * [タイムシートプロファイルの作成、編集、割り当て](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)
   * [タイムシートの手動生成](../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)
   * [グループのタイムシートプロファイルの作成と管理](../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md)

## タイムシートページからのタイムシートの削除

1. Adobe Workfront の右上隅にある&#x200B;[!UICONTROL **メインメニュー**]&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックします。
1. 削除するタイムシートをクリックして開きます。
1. タイムシート名の右にある&#x200B;[!UICONTROL **その他**]&#x200B;アイコン ![](assets/more-icon.png) をクリックしてから、「**削除**」をクリックします。

   ![タイムシートページからのタイムシートの削除](assets/delete-timesheet-from-timesheet-page.png)
1. 「[!UICONTROL **削除**]」をクリックして確定します。

   タイムシートは削除され、復元できません。
