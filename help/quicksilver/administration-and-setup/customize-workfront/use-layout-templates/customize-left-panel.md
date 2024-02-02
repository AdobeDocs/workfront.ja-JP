---
title: レイアウトテンプレートを使用した左パネルのカスタマイズ
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Adobe Workfront 全体を通して左パネル領域に表示される内容をレイアウトテンプレートでカスタマイズできます。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: ht
source-wordcount: '1025'
ht-degree: 100%

---

# レイアウトテンプレートを使用した左パネルのカスタマイズ

[!DNL Adobe Workfront] 全体を通して左パネルエリアに表示される内容をレイアウトテンプレートでカスタマイズできます。

例えば、ユーザーがタスクを表示する際に、左パネルで次の項目のうちどれを表示するかを決定できます。

![](assets/left-panel-adobe-branding.png)

>[!IMPORTANT]
>
>順序および表示に対する変更は、モバイルアプリに反映されます。

レイアウトテンプレートの作成について詳しくは、[レイアウトテンプレートを作成および管理](../use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

グループのレイアウトテンプレートについて詳しくは、[グループのレイアウトテンプレートを作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

レイアウトテンプレートを設定した後、変更を他のユーザーに表示するために、ユーザーに割り当てる必要があります。レイアウトテンプレートのユーザーへの割り当てについて詳しくは、[ユーザーをレイアウトテンプレートに割り当てる](../use-layout-templates/assign-users-to-layout-template.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> これらの手順をシステムレベルで実行するには、[!UICONTROL System Administrator]のアクセスレベルが必要です。<p>グループに対して実行するには、そのグループの管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか [!DNL Workfront] 管理者にお問い合わせください。[!DNL Workfront] 管理者がユーザーのアクセスレベルを変更する方法については、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## [!DNL Workfront] でエリアの左パネルをカスタマイズ

1. [レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)で説明されるように、レイアウトテンプレート上での作業を開始します。
1. **[!UICONTROL ユーザーの表示項目をカスタマイズする]**&#x200B;の下にある下向き矢印 ![](assets/dropdown-arrow.png) をクリックし、カスタマイズする左パネルをクリックします。

   >[!NOTE]
   >
   >ドロップダウンリストの「[!UICONTROL ホーム]」オプションについては、[レイアウトテンプレートを使用した[!UICONTROL ホーム]と[!UICONTROL 概要]のカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)を参照してください。「リスト」オプションについては、[レイアウトテンプレートを使用したフィルター、ビューおよびグループ化のカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)を参照してください。

1. **[!UICONTROL 左パネル]**&#x200B;リストで、次のいずれかを行って、ユーザーが選択したオプション（[!DNL Workfront] エリアまたはオブジェクトタイプ）の左パネルに何を表示するかを決定します。

   * 項目を表示するか（![](assets/add-secondary-nav-item.png) をクリック）非表示にするか（![](assets/delete-secondary-nav-item.png) をクリック）を選択します。![](assets/add-secondary-nav-item.png) や ![](assets/delete-secondary-nav-item.png) が付いていない項目は非表示にできません。

   * 項目の ![](assets/move-icon---dots.png) をドラッグして、左パネルでの順序を変更します。
   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>オプション</th> 
      <th>ユーザーが次をクリックすると...</th> 
      <th>次の中から選択した左パネル項目が表示される</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Project]</td> 
      <td>プロジェクト名</td> 
      <td>[!UICONTROL Tasks]、[!UICONTROL Project Details]、[!UICONTROL Business Case]、[!UICONTROL Updates]、[!UICONTROL Documents]、[!UICONTROL Issues]、[!UICONTROL Risks]、[!UICONTROL Approvals]、[!UICONTROL Baselines]、[!UICONTROL Billing Rates]、[!UICONTROL Billing Records]、[!UICONTROL Expenses]、[!UICONTROL Hours]、[!UICONTROL Workload Balancer]、[!UICONTROL People]、[!UICONTROL Utilization]、[!UICONTROL Queue Details]、[!UICONTROL Routing Rules]、[!UICONTROL Queue Topic]、[!UICONTROL Topic Group]、[!UICONTROL Metrics]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Task]</td> 
      <td>タスク名</td> 
      <td> [!UICONTROL Updates]、[!UICONTROL Documents]、[!UICONTROL Task Details]、[!UICONTROL Subtask]、[!UICONTROL Issues]、[!UICONTROL Hours]、[!UICONTROL Approvals]、[!UICONTROL Expenses]、[!UICONTROL Predecessors]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Issue]</td> 
      <td>イシュー名</td> 
      <td> [!UICONTROL Updates]、[!UICONTROL Documents]、[!UICONTROL Issue Details]、[!UICONTROL Hours]、[!UICONTROL Approvals]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Portfolio]</td> 
      <td>ポートフォリオ名</td> 
      <td>[!UICONTROL Projects]、[!UICONTROL Programs]、[!UICONTROL Portfolio Details]、[!UICONTROL Portfolio]、[!UICONTROL Optimization]、[!UICONTROL Documents]、[!UICONTROL Updates]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Program]</td> 
      <td>プログラム名</td> 
      <td>[!UICONTROL Projects]、[!UICONTROL Program Details]、[!UICONTROL Updates]、[!UICONTROL Documents]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Template]</td> 
      <td>プロジェクトテンプレート名</td> 
      <td>[!UICONTROL Template Tasks]、[!UICONTROL Template Details]、[!UICONTROL Updates]、[!UICONTROL Documents]、[!UICONTROL Risks]、[!UICONTROL Expenses]、[!UICONTROL People]、[!UICONTROL Approvals]、[!UICONTROL Billing Rates]、[!UICONTROL Queue Details]、[!UICONTROL Routing Rules]、[!UICONTROL Queue Topic]、[!UICONTROL Topic Group]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Template Task]</td> 
      <td>テンプレートタスクの名前</td> 
      <td>[!UICONTROL Updates]、[!UICONTROL Documents]、[!UICONTROL Template Task Details]、[!UICONTROL Subtasks]、[!UICONTROL Expenses]、[!UICONTROL Approvals]、[!UICONTROL Predecessors]</td>
     </tr>
     <!--
      <tr> 
       <td>Document</td> 
       <td>Document Details (for a document uploaded to Workfront)</td> 
       <td>Updates, Approvals, All Versions, Custom Forms</td> 
      </tr>
     --> 
     <tr> 
      <td> [!UICONTROL Billing Record]</td> 
      <td>プロジェクトの請求記録の名前</td> 
      <td>[!UICONTROL Billing Record Details]、[!UICONTROL Billable Hours]、[!UICONTROL Billable Expenses]、[!UICONTROL Fixed Revenues]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Projects]</td> 
      <td>[!UICONTROL Main menu] のプロジェクト <img src="assets/projects-in-main-menu.png"> <img src="assets/main-menu-icon.png"></td> 
      <td>[!UICONTROL Projects]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Requests]</td> 
      <td>リクエストの名前</td> 
      <td>[!UICONTROL New Request]、[!UICONTROL Submitted requests]、[!UICONTROL All Requests]、[!UICONTROL Drafts]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Dashboards]</td> 
      <td>ダッシュボードの名前</td> 
      <td>[!UICONTROL My Dashboards]、[!UICONTROL Shared Dashboards]、[!UICONTROL All Dashboards]<p><b>メモ</b>：[!DNL Adobe Workfront Classic] のレイアウトテンプレートを使用して [!UICONTROL Reports] エリアのカスタムタブを作成した場合、それらはこのリストの下部に表示されます。ユーザーの場合、[!UICONTROL Dashboards] エリアの左パネルの下部に表示されます。</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Scrum Team]</td> 
      <td>スクラムチームの名前</td> 
      <td><p>[!UICONTROL Iterations]、[!UICONTROL Current iteration]、[!UICONTROL Backlog]、[!UICONTROL Workload Balancer]、[!UICONTROL Updates]、[!UICONTROL Team Settings]</p> <p><strong>メモ：</strong><strong>[!UICONTROL Current iteration]</strong> 項目は、イテレーションに少なくとも 1 つのタスクまたはイシューがある場合にのみ、左側のパネルに表示されます。</p></td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Kanban Team]</td> 
      <td>かんばんチームの名前</td> 
      <td>[!UICONTROL Workload Balancer]、[!UICONTROL Kanban board]、[!UICONTROL Backlog]、[!UICONTROL Updates]、[!UICONTROL Team Settings]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Waterfal Team]</td> 
      <td>ウォーターフォールチームの名前</td> 
      <td>[!UICONTROL Workload Balancer]、[!UICONTROL Updates]、[!UICONTROL Team Requests]、[!UICONTROL Team Settings]</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Iteration]</td> 
      <td>イテレーションの名前</td> 
      <td>[!UICONTROL Stories]、[!UICONTROL Issues]、[!UICONTROL Story Board]、[!UICONTROL Overview]、[!UICONTROL Custom Forms]、[!UICONTROL Updates] </td> 
     </tr> 
     <!--
      <tr> 
       <td>Company</td> 
       <td>The name of the company</td> 
       <td> <p>People (cannot be hidden), Billing Rates, Custom Forms </p> </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>Timesheets</td> 
       <td>The name of the timesheet</td> 
       <td>My Timesheets, Timesheets I Approve, All Timesheets (cannot be hidden) </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>Resourcing</td> 
       <td>The name of the resource</td> 
       <td>Planner (cannot be hidden), Workload Balancer, Utilization, Resource Pools </td> 
      </tr>
     --> 
     <!--
      <tr> 
       <td>User Details</td> 
       <td>____________</td> 
       <td>Details (cannot be hidden), Org Chart, Time Off, Custom Forms </td> 
      </tr>
     --> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >「**[!UICONTROL ユーザーの表示項目をカスタマイズする]**」ドロップダウンリストの最後の 3 つの項目（[!UICONTROL リスト]、[!UICONTROL ホームと概要]、および[!UICONTROL ブランディング]）は、左側のパネル以外のエリアを設定するためのものです。詳しくは、次の記事を参照してください。
>   >   
* [レイアウトテンプレートを使用したフィルター、ビュー、およびグループ化のカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
>* [レイアウトテンプレートを使用して、[!UICONTROL ホーム]と[!UICONTROL 概要]をカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
* [レイアウトテンプレートを使用して Adobe  [!DNL Workfront]  をブランディング](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md)


1. （オプション）組織のダッシュボードの 1 つにリンクする左側のパネル項目を追加する場合は、「**[!UICONTROL カスタムセクションを追加]**」をクリックし、項目の「**[!UICONTROL カスタムセクションのタイトル]**」を入力して、ダッシュボードを追加します。

   左側のパネルの下部にダッシュボード項目が表示されます。ユーザーが左側のパネルにポインタを合わせると、ダッシュボード項目の横に入力したカスタムセクションのタイトルが表示されます。

   >[!NOTE]
   >
   ユーザーは、カスタムダッシュボードの項目を独自の左側のパネルに追加できます。レイアウトテンプレートにカスタムダッシュボード項目を追加すると、上書きやリセットなく、自分の項目がその項目と結合されます。これは、ユーザーをカスタムのダッシュボード項目を含む新しいレイアウトテンプレートに割り当てる場合にも当てはまります。ユーザーが左側のパネルをカスタマイズする方法について詳しくは、[カスタムタブまたはセクションを作成](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md)を参照してください。

   ダッシュボードについて詳しくは、[ダッシュボード](../../../reports-and-dashboards/dashboards/dashboards-overview.md)を参照してください。

1. 引き続きレイアウトテンプレートをカスタマイズします。

   または

   カスタマイズが終了したら、「**[!UICONTROL 保存]**」をクリックします。

   >[!TIP]
   >
   いつでも「[!UICONTROL 保存]」をクリックして進行状況を保存して、後でテンプレートの変更を続行できます。
