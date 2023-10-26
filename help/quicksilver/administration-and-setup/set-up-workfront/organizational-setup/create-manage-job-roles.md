---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: 担当業務の作成と管理
description: As an [!DNL Adobe Workfront] 管理者またはジョブロールへの管理者アクセス権を持つユーザーは、ユーザーに割り当て可能なジョブロールを作成し、組織に関係のないデフォルトのジョブロールを削除できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: f66a6c340d8789db447c860d995d9836a30eeeb0
workflow-type: tm+mt
source-wordcount: '1168'
ht-degree: 1%

---

# 担当業務の作成と管理

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

As an [!DNL Adobe Workfront] 管理者またはジョブロールへの管理者アクセス権を持つユーザーは、ユーザーに割り当て可能なジョブロールを作成し、組織に関係のないデフォルトのジョブロールを削除できます。 での管理アクセスについて詳しくは、 [!DNL Workfront]を参照してください。 [特定の領域に対する管理者アクセス権をユーザーに付与する](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td>[!UICONTROL プラン ]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ジョブロールへの管理者アクセス</p> <p><b>注意</b>：まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## ジョブロールの作成

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) ～の右上隅に [!DNL Adobe] Workfront、 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、「 」をクリックしま&#x200B;す。 **[!UICONTROL ジョブの役割].**
1. クリック **[!UICONTROL 新しいジョブの役割].**
1. 以下を設定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 名前 ]</td> 
      <td> <p>ジョブの役割の名前を指定します。 これは、 [!DNL Workfront] [!UICONTROL ジョブロール ] フィールドが表示されます。 </p> <p>ヒント：ジョブの役割の名前は 255 文字までです。 ただし、 [!DNL Workfront]. </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL 説明 ]</td> 
      <td>ロールの一意性を示す説明を入力します。 </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL がアクティブです ]</span> </td> 
      <td> 
       <ul> 
        <li> <p>選択 <b>[!UICONTROL はい ]</b> 役割をアクティブにし、 [!DNL Workfront] ユーザー、作業項目などに関連付ける </p> </li> 
        <li> <p>選択 <b>[!UICONTROL いいえ ]</b>を無効にし、ユーザーや作業項目などに割り当てられないようにする場合。 </p> </li> 
       </ul> <p><span>ジョブの役割の非アクティブ化について詳しくは、</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">ジョブの役割の非アクティブ化</a>. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL 基本通貨 ]</span> </td> 
      <td> <p><span>これは、Workfront管理者が [!UICONTROL 設定 ] 領域で設定した [!UICONTROL 基本通貨 ] です。 詳しくは、</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">為替レートの設定</a> .</p> <p>ヒント： <span>[!UICONTROL 基本通貨 ] は、ジョブの役割レベルでは編集できません。 このフィールドは淡色表示になり、システムの基本通貨を確認する役割を果たします。</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL コストレート ]</td> 
      <td><p>これは、ジョブロールの 1 時間あたりのコスト率です。 この値は、ロールに関連するタスクとタスクの計画原価と実績原価、および最終的にはプロジェクトの計画原価と実績原価を計算します。 [!UICONTROL 基本通貨 ] を使用してレートを入力します。</p> 
      <p>有効な日付の原価率の場合は、 <strong>[!UICONTROL 追加率 ]</strong>. その期間のコスト/時間の値を入力し、必要に応じて [!UICONTROL 開始日 ] と [!UICONTROL 終了日 ] を割り当てます。 最初のコストレートには開始日が設定されず、最後のコストレートには終了日が設定されません。</p> <p>一部の日付は自動的に追加されます。 例えば、最初のコストレートに終了日が設定されていない場合に、開始日が 2023 年 5 月 1 日の 2 番目のコストレートを追加すると、ギャップが生じないように、2023 年 4 月 30 日の終了日が最初のコストレートに追加されます。</p> <p>ヒント：既存のジョブの役割を編集する際に、「 <strong>開始日で並べ替え</strong> をクリックすると、最新の開始日がレートリストの上部に表示されます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 請求率 ] </td> 
      <td><p>これは、ジョブロールの 1 時間あたりの請求率です。 この値は、ロールに関連するタスクとタスクの計画収益と実際の収益、および最終的にはプロジェクトの計画収益と実際の収益を計算します。 [!UICONTROL 基本通貨 ] を使用してレートを入力します。</p> <p>有効な請求率の日付を表示するには、 <strong>[!UICONTROL 追加率 ]</strong>. その期間の請求/時間の値を入力し、必要に応じて [!UICONTROL 開始日 ] と [!UICONTROL 終了日 ] を割り当てます。 最初の請求率には開始日が設定されず、最後の請求率には終了日が設定されません。</p> <p>一部の日付は自動的に追加されます。 例えば、最初の請求率に終了日がなく、開始日が 2023 年 5 月 1 日の 2 番目の請求を追加した場合、ギャップが生じないように、2023 年 4 月 30 日の終了日が最初の請求率に追加されます。</p> <p>ヒント：既存のジョブの役割を編集する際に、「 <strong>開始日で並べ替え</strong> をクリックすると、最新の開始日がレートリストの上部に表示されます。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL 通貨の上書き ]</span> </td> 
      <td>
        <p>このジョブの役割に関連付けられている通貨を選択します。 これが通貨です。 [!DNL Workfront] は、このジョブロールに関連付けられたコストと売上高の計算に使用します。 </p> 
        <p><span>これは、 [!DNL Workfront] 管理者（[!UICONTROL 設定 ] 領域）で設定できます。プロジェクトに関連付けられている通貨とは異なる通貨を使用することもできます。</span> </p> 
        <p>ヒント：このフィールドは、システムの [!UICONTROL 為替レート ] 領域で使用できる通貨のみが表示されます。</p> 
       <p><span>[!UICONTROL 基本通貨 ] の設定について詳しくは、 [!DNL Workfront]を参照してください。</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">為替レートの設定</a>.</p> <p><span>プロジェクトの通貨の変更について詳しくは、</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">プロジェクトの通貨を変更</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL 通貨コストレートの上書き ]</span> </td> 
      <td>
        <p>これは、選択した [!UICONTROL 通貨の上書き ] を使用するジョブロールの 1 時間あたりのコスト率です。 [!DNL Workfront] この値を使用して、ジョブロールに関連するタスクおよびタスクの計画コストと実際のコストを計算します。 </p> 
        <p><span>上記の [!UICONTROL 通貨上書き ] でレートを入力します。 これにより、[!UICONTROL 基本通貨 ] を使用する際に、このジョブロールのコストレートも更新されます。</span> </p> 
        <p>詳しくは、 [!DNL Workfront] コストの計算については、 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a>.</p> 
       <p>ヒント：既にコスト・レートが関連付けられている既存のジョブ・ロールを更新する場合は、次の手順に従います。 [!DNL Workfront] は、システム内のコンバージョン率に基づいて [!UICONTROL 通貨の上書き ] 率を計算します。 [!UICONTROL Override Currency Cost Rate] を更新すると、ジョブロールのコストレートも自動的に更新されます。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL 通貨の請求率の上書き ]</span> </td> 
      <td>
        <p>これは、選択した [!UICONTROL 通貨の上書き ] を使用したジョブロールの 1 時間あたりの請求率です。 [!DNL Workfront] この値を使用して、ジョブロールに関連するタスクおよびタスクの計画収益と実際の売上高を計算します。 </p>
        <p><span>上記の [!UICONTROL 通貨上書き ] でレートを入力します。 これにより、[!UICONTROL 基本通貨 ] を使用する際に、このジョブの役割に対する請求率も更新されます。</span> </p>
        <p>詳しくは、 [!DNL Workfront] 売上高の計算については、 <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">請求と売上高の概要</a>.</p>
        <p>ヒント：既に請求率が関連付けられている既存のジョブロールを更新する場合は、次の手順に従います。 [!DNL Workfront] は、システム内の換算レートに基づいて「上書き通貨」レートを計算します。 「通貨請求レートの上書き」を更新すると、ジョブ・ロールの請求レートも自動的に更新されます。 </p>
       </td>
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >ジョブの役割は、リソース管理に不可欠な要素です。 生産資源計画ツールを使用するには、製造オーダー・ロールに関連付けられた原価と請求率が必要です。 詳しくは、 [リソース管理の概要](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

1. クリック **[!UICONTROL ジョブロールを作成]**. これで、ジョブの役割をタスク、イシュー、承認に割り当てたり、レイアウトテンプレートや他のオブジェクトをタスクと共有したりできるようになりました。 でのジョブの役割のすべての使用に関する情報 [!DNL Workfront]を参照してください。 [ジョブロールの概要](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). ジョブの役割の削除について詳しくは、 [ジョブの役割を削除](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

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
