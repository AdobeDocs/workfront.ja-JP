---
title: レイアウトテンプレートを使用した左側のパネルのカスタマイズ
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Adobe Workfront 全体を通して左パネル領域に表示される内容をレイアウトテンプレートでカスタマイズできます。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: f7ad56375c20e26b0d45ae0966e2e156b5a200f1
workflow-type: tm+mt
source-wordcount: '1091'
ht-degree: 65%

---

# レイアウトテンプレートを使用した左パネルのカスタマイズ

<!--Audited: 10/2024-->

[!DNL Adobe Workfront] 全体を通して左パネルエリアに表示される内容をレイアウトテンプレートでカスタマイズできます。

例えば、ユーザーがタスクを表示する際に、左パネルで次の項目のうちどれを表示するかを決定できます。

![](assets/left-panel-adobe-branding.png)

>[!IMPORTANT]
>
>順序および表示に対する変更は、モバイルアプリに反映されます。

レイアウトテンプレートの作成について詳しくは、[レイアウトテンプレートを作成および管理](../use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

グループのレイアウトテンプレートについて詳しくは、[グループのレイアウトテンプレートを作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

レイアウトテンプレートを設定した後、変更を他のユーザーに表示するために、ユーザーに割り当てる必要があります。レイアウトテンプレートのユーザーへの割り当てについて詳しくは、[ユーザーのレイアウトテンプレートへの割り当て](../use-layout-templates/assign-users-to-layout-template.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td><p>新規：標準</p>
  <p> 現在：プラン</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>これらの手順をシステムレベルで実行するには、システム管理者のアクセスレベルが必要です。
グループに対して実行するには、そのグループの管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## [!DNL Workfront] でエリアの左パネルをカスタマイズ

1. [レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)で説明されるように、レイアウトテンプレート上での作業を開始します。
1. **[!UICONTROL ユーザーに表示する項目をカスタマイズ]** の下にある下向き矢印 ![](assets/dropdown-arrow.png) をクリックし、カスタマイズするオブジェクト タイプまたは [!DNL Workfront] 領域の名前をクリックします。

   左側のパネルをカスタマイズできるオブジェクトタイプと [!DNL Workfront] 領域を次の表に示します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>オブジェクトタイプまたは [!DNL Workfront] 領域</th> 
      <th>ユーザーが次をクリックすると...</th> 
      <th>左側のパネルのセクションで、レイアウトテンプレートに表示した後にユーザーに表示されるものは、次のとおりです。</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Project]</td> 
      <td>プロジェクト名</td> 
      <td>[!UICONTROL タスク ]、[!UICONTROL プロジェクトの詳細 ]、[!UICONTROL ビジネスケース ]、[!UICONTROL の更新 ]、[!UICONTROL ドキュメント ]、[!UICONTROL の問題 ]、[!UICONTROL リスク ]、[!UICONTROL 承認 ]、[!UICONTROL ベースライン ]、[!UICONTROL 請求レート ]、[!UICONTROL 請求レコード ]、[!UICONTROL 費用 ]、[!UICONTROL 時間 ]、[!UICONTROL ワークロードバランサー ]、[!UICONTROL 人物 ]、[!UICONTROL 使用率 ]、[!UICONTROL キューの詳細 ]、[!UICONTROL ルーティング規則 ]、[!UICONTROL キュートピック ]、[!UICONTROL トピック グループ ]、[!UICONTROL 指標 ]、[!UICONTROL l プランニング ]*</td> 
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
      <td>[!UICONTROL プロジェクト ]、[!UICONTROL プログラム ]、[!UICONTROLPortfolioの詳細 ]、[!UICONTROLPortfolio]、[!UICONTROL 最適化 ]、[!UICONTROL ドキュメント ]、[!UICONTROL 更新 ]、[!UICONTROL 計画 ]*</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Program]</td> 
      <td>プログラム名</td> 
      <td>[!UICONTROL プロジェクト ]、[!UICONTROL プログラムの詳細 ]、[!UICONTROL 更新 ]、[!UICONTROL ドキュメント ]、[!UICONTROL 計画 ]*</td> 
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

   *プロジェクト、ポートフォリオ、プログラムの左側のパネルにこの領域を追加するには、Workfront Planning のライセンスを追加購入する必要があります。 詳しくは、[Adobe Workfront計画の概要を参照してください ](/help/quicksilver/planning/general/planning-overview.md)


1. **[!UICONTROL 左側のパネル]** リストで、次のいずれかの操作を行って、選択した [!DNL Workfront] 領域またはオブジェクトタイプの左側のパネルに表示される内容を決定します。

   * 左側のパネルのセクションを表示または非表示にするには、「**表示** ![](assets/add-secondary-nav-item.png)」または「**非表示**」 ![](assets/delete-secondary-nav-item.png) イコンをクリックします。 **表示** または **非表示** アイコンのない項目は非表示にできません。

   * 項目の ![](assets/move-icon---dots.png) をドラッグして、左パネルでの順序を変更します。

   >[!NOTE]
   >
   >**[!UICONTROL ユーザーに表示する項目をカスタマイズ]** ドロップダウンリストの次の項目は、左側のパネル以外の領域を参照します。
   >* [!UICONTROL リスト]
   >* [!UICONTROL 概要パネル]
   >* [!UICONTROL ホーム]
   >* [!UICONTROL ブランディング]
   > 
   >その他の領域のカスタマイズ方法について詳しくは、次の記事を参照してください。
   >
   >* [レイアウトテンプレートを使用したフィルター、ビューおよびグループ化のカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   >* [ レイアウトテンプレートを使用した [!UICONTROL  概要パネル ] のカスタマイズ ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   >* [ レイアウトテンプレートを使用したホームのカスタマイズ ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-new-home-layout-template.md)
   >* [レイアウトテンプレートを使用して Adobe  [!DNL Workfront]  をブランディング](../../../administration-and-setup/customize-workfront/use-layout-templates/brand-wf-using-a-layout-template.md)


1. （オプション）組織のダッシュボードの 1 つにリンクする左側のパネル項目を追加する場合は、「**[!UICONTROL カスタムセクションを追加]**」をクリックし、項目の「**[!UICONTROL カスタムセクションのタイトル]**」を入力して、ダッシュボードを追加します。

   左側のパネルの下部にダッシュボード項目が表示されます。左側のパネルでダッシュボード項目にカーソルを合わせると、その項目の横に入力したカスタムセクションのタイトルが表示されます。

   >[!NOTE]
   >
   >ユーザーは、カスタムダッシュボードの項目を独自の左側のパネルに追加できます。レイアウトテンプレートにカスタムダッシュボード項目を追加すると、追加した項目に加えて項目が表示され、上書きまたはリセットされることはありません。 これは、ユーザーをカスタムのダッシュボード項目を含む新しいレイアウトテンプレートに割り当てる場合にも当てはまります。ユーザーが左側のパネルをカスタマイズする方法について詳しくは、[カスタムタブまたはセクションを作成](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md)を参照してください。
   >
   >ダッシュボードについて詳しくは、[ダッシュボード](../../../reports-and-dashboards/dashboards/dashboards-overview.md)を参照してください。

1. 引き続きレイアウトテンプレートをカスタマイズします。

   または

   カスタマイズが完了したら、「**[!UICONTROL 保存]**」をクリックします。

   >[!TIP]
   >
   >「[!UICONTROL **保存**]」をクリックすると、いつでも進行状況を保存できます。これによりレイアウトテンプレートエディターが閉じるので、後でテンプレートの変更を続行できます。
