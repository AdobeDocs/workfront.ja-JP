---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 担当業務の作成と管理
description: ' [!DNL Adobe Workfront]  管理者、または担当業務の管理アクセス権を持つユーザーは、ユーザーに割り当て可能な担当業務を作成し、組織に関係のないデフォルトの担当業務を削除できます。'
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: 32441df90b915077f57ead791116dcbd32c9557a
workflow-type: tm+mt
source-wordcount: '1140'
ht-degree: 81%

---

# 担当業務の作成と管理

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

[!DNL Adobe Workfront] 管理者、または担当業務への管理アクセス権を持つユーザーは、ユーザーに割り当て可能な担当業務を作成し、組織に関係のないデフォルトの担当業務を削除できます。[!DNL Workfront] での管理アクセスについて詳しくは、[特定のエリアに対する管理アクセス権をユーザーに付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)を参照してください。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>
   <p>新規：標準</p>
   <p>現在： [!UICONTROL プラン ]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>担当業務の管理アクセス権</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 担当業務を作成

ジョブ・ロールを作成する手順は、次のとおりです。

{{step-1-to-setup}}

1. 左側のパネルで、「**[!UICONTROL 担当業務]**」をクリックします。
1. 「**[!UICONTROL 新規担当業務]**」をクリックします。
1. 以下を設定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>担当業務の名前を指定します。これは、[!DNL Workfront] で[!UICONTROL Job Role]フィールドが表示される場合に常に表示される名前です。 </p> <p>ヒント：担当業務の名前は 255 文字まで入力できます。ただし、名前が長い場合は、[!DNL Workfront] の一部の領域で省略される可能性があります。 </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>役割の一意性を示す説明を入力します。 </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Is Active]</span> </td> 
      <td> 
       <ul> 
        <li> <p>役割を [!DNL Workfront] のあらゆる場所でアクティブにでき、ユーザー、作業アイテムなどに関連付けられるようにする場合は、「<b>[!UICONTROL Yes]</b>」を選択します。 </p> </li> 
        <li> <p>役割を非アクティブ化し、ユーザーや作業アイテムなどに割り当てられないようにする場合は、「<b>[!UICONTROL No]</b>」を選択します。 </p> </li> 
       </ul> <p><span>担当業務の非アクティブ化について詳しくは、</span><a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">担当業務の非アクティブ化</a>を参照してください。 </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Base Currency]</span> </td> 
      <td> <p><span>これは、Workfront 管理者が[!UICONTROL Setup]エリアで設定した[!UICONTROL Base Currency]です。詳しくは、</span><a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">為替レートの設定</a>を参照してください。</p> <p>ヒント：<span>[!UICONTROL Base Currency]は、担当業務レベルでは編集できません。このフィールドはグレー表示で、システムの基本通貨を確認できます。</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL コストレート ]</td> 
      <td><p>これは、担当業務の 1 時間あたりのコスト率です。この値は、役割に関連するタスクとイシューの予定コストと実際のコスト、最終的にはプロジェクトの予定コストと実際のコストを計算します。[!UICONTROL Base Currency]を使用してレートを入力します。</p> 
      <p>日付が有効なコスト率の場合は、「<strong>[!UICONTROL Add Rate]</strong>」をクリックします。その期間の 1 時間当たりのコストの値を入力し、必要に応じて[!UICONTROL Start Date]と[!UICONTROL End Date]を割り当てます。最初のコスト率には開始日が設定されず、最後のコスト率には終了日が設定されません。</p> <p>一部の日付は自動的に追加されます。例えば、最初のコスト率に終了日が設定されていない場合に、2 番目のコスト率を追加して開始日を 2023年5月1日とすると、ギャップが生じないように、最初のコスト率に終了日 2023年4月30日が追加されます。</p> <p>ヒント：既存の担当業務を編集する際に、「<strong>開始日順に並べ替える</strong>」をクリックすると、最新の開始日がレートリストの上部に表示されます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 請求率 ] </td> 
      <td><p>これは、担当業務の 1 時間あたりの請求レートです。この値は、役割に関連するタスクの予定収益と実収益、最終的にはプロジェクトの予定収益と実収益を計算します。[!UICONTROL Base Currency]を使用してレートを入力します。</p> <p>日付が有効な請求レートを表示するには、「<strong>[!UICONTROL Add Rate]</strong>」をクリックします。その期間の 1 時間当たりの請求レートの値を入力し、必要に応じて[!UICONTROL Start Date]と[!UICONTROL End Date]を割り当てます。最初の請求レートには開始日が設定されず、最後の請求レートには終了日が設定されません。</p> <p>一部の日付は自動的に追加されます。例えば、最初の請求レートに終了日がなく、2 番目の請求レートを追加して開始日を 2023年5月1日とすると、ギャップが生じないように、最初の請求レートに終了日 2023年4月30日が追加されます。</p> <p>ヒント：既存の担当業務を編集する際に、「<strong>開始日順に並べ替える</strong>」をクリックすると、最新の開始日がレートリストの上部に表示されます。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency]</span> </td> 
      <td>
        <p>この担当業務に関連付けられている通貨を選択します。これは、[!DNL Workfront] でこの担当業務に関連付けられたコストと収益の計算に使用する通貨です。 </p> 
        <p><span>これは、 [!DNL Workfront] 管理者（[!UICONTROL 設定 ] 領域）で設定できます。プロジェクトに関連付けられている通貨とは異なる通貨を使用することもできます。</span> </p> 
        <p>ヒント：このフィールドは、システムの [!UICONTROL 為替レート ] 領域で使用できる通貨のみが表示されます。 設定されている通貨が 1 つだけの場合、このフィールドは表示されません。</p> 
       <p><span>[!DNL Workfront] での[!UICONTROL Base Currency]の設定について詳しくは、</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">為替レートの設定</a>を参照してください。</p> <p><span>プロジェクトの通貨の変更について詳しくは、</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">プロジェクトの通貨の変更</a>を参照してください。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL 通貨コストレートの上書き ]</span> </td> 
      <td>
        <p>これは、選択した「[!UICONTROL Override Currency]」を使用する担当業務の 1 時間あたりのコスト率です。[!DNL Workfront] はこの値を使用して、担当業務に関連するタスクおよびイシューの予定コストと実際のコストを計算します。 </p> 
        <p><span>上記の「[!UICONTROL Override Currency]」にレートを入力します。これにより、[!UICONTROL 基本通貨 ] を使用する際に、このジョブロールのコストレートも更新されます。</span> </p> 
        <p>[!DNL Workfront] のコストの計算について詳しくは、<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a>を参照してください。</p> 
       <p>ヒント：既にコスト・レートが関連付けられている既存のジョブ・ロールを更新する場合は、次の手順に従います。 [!DNL Workfront] は、システム内のコンバージョン率に基づいて [!UICONTROL 通貨の上書き ] 率を計算します。 [!UICONTROL Override Currency Cost Rate] を更新すると、ジョブロールのコストレートも自動的に更新されます。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL 通貨の請求率の上書き ]</span> </td> 
      <td>
        <p>これは、選択した「[!UICONTROL Override Currency]」を使用した担当業務の 1 時間あたりの請求レートです。[!DNL Workfront] はこの値を使用して、担当業務に関連するタスクおよびイシューの予定収益と実収益を計算します。 </p>
        <p><span>上記の「[!UICONTROL Override Currency]」にレートを入力します。これにより、[!UICONTROL 基本通貨 ] を使用する際に、このジョブの役割に対する請求率も更新されます。</span> </p>
        <p>[!DNL Workfront] の収益の計算方法について詳しくは、<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">請求と収益の概要</a>を参照してください。</p>
        <p>ヒント：既に請求率が関連付けられている既存のジョブロールを更新する場合は、次の手順に従います。 [!DNL Workfront] は、システム内の換算レートに基づいて「上書き通貨」レートを計算します。 「通貨請求レートの上書き」を更新すると、ジョブ・ロールの請求レートも自動的に更新されます。 </p>
       </td>
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >担当業務は、リソース管理に不可欠な要素です。リソース計画ツールを使用するには、担当業務に関連付けられたコストと請求レートが必要です。詳しくは、[リソース管理の概要](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md)を参照してください。

1. 「**[!UICONTROL 担当業務を作成]**」をクリックします。担当業務をタスク、イシュー、承認に割り当てたり、レイアウトテンプレートや他のオブジェクトをタスクと共有したりできるようになります。[!DNL Workfront] でのすべての担当業務の使用に関する情報について詳しくは、[担当業務の概要](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md)を参照してください。担当業務の削除について詳しくは、[担当業務の削除](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md)を参照してください。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Delete a job role</h2>
<ol data-mc-continue="false">
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront, then click <strong>Setup</strong> <img src="assets/gear-icon-settings.png">.</li>
<li value="2">Click<strong>Job Roles.</strong></li>
<li value="3">Select the job role that you want to delete, then click <strong>Delete.</strong></li>
<li value="4">If there are any objects (users, tasks, issues) that are assigned to the job role, do one of the following:<br>
<ul>
<li><p><strong>Replace the job role with a different job role:</strong> Select the new job role from the drop-down list.</p><p>Any current and past resource allocations that are associated with the deleted job role are transferred to the job role that you select.</p><p>Users who have only one job role assigned to them are reassigned to the job role that you select; users who have a secondary job role assigned to them are not reassigned to the job role that you select.</p></li>
<li><p><strong>Delete the job role and its resource allocation:</strong> Select<strong>None</strong> from the drop-down list.</p><note type="important">
Deleting a job role deletes all current and past resource allocation related to that job role for all projects.
</note><p>​For example, if a task or issue is assigned to only that job role, the task or issue is unassigned after the job role is deleted.</p></li>
</ul></li>
<li value="5">Click  <strong>Yes, Delete It</strong>. </li>
</ol>
</div>
-->
