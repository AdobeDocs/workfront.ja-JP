---
title: レイアウトテンプレートを使用した左側のパネルのカスタマイズ
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Adobe Workfront 全体を通して左パネル領域に表示される内容をレイアウトテンプレートでカスタマイズできます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: b100ea35-e045-4021-b5be-2c9071b381da
source-git-commit: c037b4f9e5530d8dd796bed25021f7073f16061f
workflow-type: tm+mt
source-wordcount: '1095'
ht-degree: 50%

---

# レイアウトテンプレートを使用した左パネルのカスタマイズ

<!--Audited: 10/2024-->

[!DNL Adobe Workfront] 全体を通して左パネルエリアに表示される内容をレイアウトテンプレートでカスタマイズできます。

例えば、プロジェクトを表示するときに、左側のパネルに表示される項目を次の中から選択できます。

![ プロジェクトの左パネル ](assets/left-panel-in-project.png)

>[!IMPORTANT]
>
>順序および表示に対する変更は、モバイルアプリに反映されます。

レイアウトテンプレートの作成について詳しくは、[レイアウトテンプレートを作成および管理](../use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

グループのレイアウトテンプレートについて詳しくは、[グループのレイアウトテンプレートを作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

レイアウトテンプレートを設定した後、変更を他のユーザーに表示するために、ユーザーに割り当てる必要があります。レイアウトテンプレートのユーザーへの割り当てについて詳しくは、[ユーザーのレイアウトテンプレートへの割り当て](../use-layout-templates/assign-users-to-layout-template.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p>
       <p>メインメニューへのカスタムアプリケーションの追加は、Adobe App Builderでライセンスを取得している組織のみが使用できます。</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td><p>標準</p>
       <p>プラン</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>これらの手順をシステムレベルで実行するには、システム管理者のアクセスレベルが必要です。</p>
        <p>グループに対して実行するには、そのグループの管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## [!DNL Workfront] でエリアの左パネルをカスタマイズ

1. [レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)で説明されるように、レイアウトテンプレート上での作業を開始します。
1. ![ ユーザーに表示する項目をカスタマイズ ](assets/dropdown-arrow.png) の下にある下向き矢印 **[!UICONTROL 下向き矢印]** をクリックし、カスタマイズするオブジェクト タイプの名前または [!DNL Workfront] の領域をクリックします。

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
      <td>[!UICONTROL タスク ]、[!UICONTROL プロジェクトの詳細 ]、[!UICONTROL ビジネスケース ]、[!UICONTROL の更新 ]、[!UICONTROL ドキュメント ]、[!UICONTROL の問題 ]、[!UICONTROL リスク ]、[!UICONTROL 承認 ]、[!UICONTROL ベースライン ]、[!UICONTROL 請求レート ]、[!UICONTROL 請求レコード ]、[!UICONTROL 費用 ]、[!UICONTROL 時間 ]、[!UICONTROL ワークロードバランサー ]、[!UICONTROL 人物 ]、[!UICONTROL 使用率 ]、[!UICONTROL キューの詳細 ]、[!UICONTROL ルーティング規則 ]、[!UICONTROL キュートピック ]、[!UICONTROL トピック グループ ]、[!UICONTROL 指標 ]、[!UICONTROL uicontrol Planning]*, [!UICONTROL カスタム アプリケーション ]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Task]</td> 
      <td>タスク名</td> 
      <td> [!UICONTROL 更新 ]、[!UICONTROL ドキュメント ]、[!UICONTROL タスクの詳細 ]、[!UICONTROL サブタスク ]、[!UICONTROL 問題 ]、[!UICONTROL 時間 ]、[!UICONTROL 承認 ]、[!UICONTROL 費用 ]、[!UICONTROL 先行タスク ]、[!UICONTROL カスタム アプリケーション ]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Issue]</td> 
      <td>イシュー名</td> 
      <td> [!UICONTROL の更新 ]、[!UICONTROL ドキュメント ]、[!UICONTROL 問題の詳細 ]、[!UICONTROL 時間 ]、[!UICONTROL 承認 ]、[!UICONTROL カスタム アプリケーション ]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Portfolio]</td> 
      <td>ポートフォリオ名</td> 
      <td>[!UICONTROL プロジェクト ]、[!UICONTROL プログラム ]、[!UICONTROL Portfolioの詳細 ]、[!UICONTROL Portfolio]、[!UICONTROL 最適化 ]、[!UICONTROL ドキュメント ]、[!UICONTROL 更新 ]、[!UICONTROL Planning]*、[!UICONTROL カスタム アプリケーション ]**</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Program]</td> 
      <td>プログラム名</td> 
      <td>[!UICONTROL プロジェクト ]、[!UICONTROL プログラムの詳細 ]、[!UICONTROL 更新 ]、[!UICONTROL ドキュメント ]、[!UICONTROL 計画 ]*、[!UICONTROL カスタム アプリケーション ]**</td> 
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
      <td> [!UICONTROL 請求記録]</td> 
      <td>プロジェクトの請求記録の名前</td> 
      <td>[!UICONTROL 請求記録詳細]、[!UICONTROL 請求可能時間]、[!UICONTROL 請求可能な費用]、[!UICONTROL 固定収益]</td> 
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
      <td>[!UICONTROL My Dashboards]、[!UICONTROL Shared Dashboards]、[!UICONTROL All Dashboards]</td> 
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

   *プロジェクト、ポートフォリオ、プログラムの左側のパネルにこの領域を追加するには、Workfront Planning のライセンスを追加購入する必要があります。 詳しくは、[Adobe Workfrontの計画の概要 ](/help/quicksilver/planning/general/planning-overview.md) を参照してください

   **カスタムアプリケーションは、メインメニューオプションとして使用する前に、個別に作成する必要があります。 詳しくは、[Adobe App Builderを使用したWorkfrontのカスタムアプリケーションの作成 ](/help/quicksilver/app-builder/app-builder.md) を参照してください。


1. **[!UICONTROL 左側のパネル]** リストで、次のいずれかの操作を行って、選択した [!DNL Workfront] 領域またはオブジェクトタイプの左側のパネルに表示される内容を決定します。

   * **表示** ![ 表示アイコン ](assets/add-secondary-nav-item.png) または **非表示** ![ 非表示アイコン ](assets/delete-secondary-nav-item.png) アイコンをクリックして、左側のパネルのセクションを表示または非表示にします。 **表示** または **非表示** アイコンのない項目は非表示にできません。

   * 項目 ![ 移動アイコン ](assets/move-icon---dots.png) をドラッグして、左側のパネルでの順序を変更します。

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


1. （オプション）組織のダッシュボードのいずれかにリンクする左側のパネル項目を追加する場合は、「**[!UICONTROL ダッシュボードを追加]**」をクリックし、項目の **[!UICONTROL クイックリンク名]** を入力して、ダッシュボードを選択します。

   ダッシュボードがリストに表示される前に、ダッシュボードを作成する必要があります。

   ダッシュボード項目が左パネルの下部に表示されます。

   >[!NOTE]
   >
   >ユーザーは、カスタムダッシュボードの項目を独自の左側のパネルに追加できます。レイアウトテンプレートにカスタムダッシュボード項目を追加すると、追加した項目に加えて項目が表示され、上書きまたはリセットされることはありません。 これは、ユーザーをカスタムのダッシュボード項目を含む新しいレイアウトテンプレートに割り当てる場合にも当てはまります。左側のパネルをカスタマイズする方法については、[Workfront オブジェクトまたは領域の左側のパネルへのダッシュボードの追加 ](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md) を参照してください。
   >
   >ダッシュボードについて詳しくは、[ダッシュボード](../../../reports-and-dashboards/dashboards/dashboards-overview.md)を参照してください。

1. レイアウトテンプレートのカスタマイズを続行します。 「**適用**」をクリックすると、いつでも進捗を保存できます。

   または

   カスタマイズが終了したら、「保存して閉じる **をクリックし** す。
