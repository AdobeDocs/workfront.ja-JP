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
source-git-commit: a30e505aa2061240f92642fda274be66e4947bce
workflow-type: tm+mt
source-wordcount: '864'
ht-degree: 50%

---

# 担当業務の作成と管理

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

>[!IMPORTANT]
>
>25.11 リリースでは、担当業務の通貨を上書きは実稼動環境では非推奨（廃止予定）になりました。 （非推奨（廃止予定）は 10 月 30 日にプレビュー環境で発生しました。） 基本通貨を設定して通貨を上書きするのではなく、担当業務で 1 つの通貨を使用できるようになり、コストと請求レートがその通貨を使用して定義されます。

[!DNL Adobe Workfront] 管理者、または担当業務への管理アクセス権を持つユーザーは、ユーザーに割り当て可能な担当業務を作成し、組織に関係のないデフォルトの担当業務を削除できます。[!DNL Workfront] での管理アクセスについて詳しくは、[特定のエリアに対する管理アクセス権をユーザーに付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)を参照してください。

>[!TIP]
>
>担当業務は、リソース管理に不可欠な要素です。リソース計画ツールを使用するには、担当業務に関連付けられたコストと請求レートが必要です。詳しくは、[リソース管理の概要](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>担当業務への管理アクセス</td>
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 担当業務を作成

担当業務を作成するには：

{{step-1-to-setup}}

1. 左側のパネルで、「**[!UICONTROL 担当業務]**」をクリックします。
1. 「**[!UICONTROL 新規担当業務]**」をクリックします。
1. 次のフィールドを設定します。

   * **名前**：担当業務の名前を指定します。 これは、担当業務フィールドが表示されるWorkfront内のすべての場所に表示される名前です。

     >[!TIP]
     >
     >担当業務の名前は、255 文字まで入力できます。 ただし、Workfrontの特定の領域では、長い名前が切り捨てられる場合があります。

   * **説明**：役割の一意の内容を示す役割の説明を入力します。
   * **アクティブ**：ロールをアクティブにして、Workfrontのすべての場所でユーザーや作業アイテムなどに関連付けて使用できるようにする場合は、「**はい**」を選択します。 役割をディアクティベートして、ユーザーや作業項目などに割り当てることができない場合は、「**いいえ**」を選択します。

     担当業務の非アクティブ化について詳しくは、[担当業務の非アクティブ化](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md)を参照してください。

   * **通貨**: ベース通貨がデフォルトで表示されます。 Workfront管理者が、設定エリアにベース通貨を追加します。 選択を別の使用可能な通貨に変更したり、発効日のある時間範囲の通貨を変更したりできます。

     >[!TIP]
     >
     >このフィールドで使用できるのは、システムの「為替レート」領域で指定した通貨のみです。 1 つの通貨のみを設定している場合は、その通貨のみを使用できます。

     Workfrontの基準通貨の設定については、「[&#x200B; 為替レートの設定 &#x200B;](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)」を参照してください。

     プロジェクトの通貨を変更する方法については、「[&#x200B; プロジェクトの通貨を変更する &#x200B;](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md)」を参照してください。

   * **コスト率**：これは担当業務の 1 時間あたりのコスト率です。 この値は、役割に関連するタスクとイシューの予定コストと実際のコスト、最終的にはプロジェクトの予定コストと実際のコストを計算します。選択した通貨を使用してレートを入力します。

     有効日のコスト率については、「**レートを追加**」をクリックします。期間の原価/時間の値を入力し、必要に応じて開始日と終了日を割り当てます。 最初のコスト率には開始日が設定されず、最後のコスト率には終了日が設定されません。

     一部の日付は自動的に追加されます。例えば、最初のコスト率に終了日が設定されていない場合に、2 番目のコスト率を追加して開始日を 2025年5月1日とすると、ギャップが生じないように、最初のコスト率に終了日 2025年4月30日が追加されます。

     Workfrontによるコストの計算方法について詳しくは、[&#x200B; コストの追跡 &#x200B;](/help/quicksilver/manage-work/projects/project-finances/track-costs.md) を参照してください。

     >[!TIP]
     >
     >既存の担当業務を編集する際に、最新の開始日を評価リストの先頭に表示するようにリストを並べ替えることができます。

   * **請求レート**：これは、担当業務の 1 時間あたりの請求レートです。 この値は、役割に関連するタスクの予定収益と実収益、最終的にはプロジェクトの予定収益と実収益を計算します。選択した通貨を使用してレートを入力します。

     有効日の請求レートについては、「**レートを追加**」をクリックします。期間の請求/時間の値を入力し、必要に応じて開始日と終了日を割り当てます。 最初の請求レートには開始日が設定されず、最後の請求レートには終了日が設定されません。

     一部の日付は自動的に追加されます。例えば、最初の請求レートに終了日がなく、2 番目の請求レートを追加して開始日を 2025年5月1日とすると、ギャップが生じないように、最初の請求レートに終了日 2025年4月30日が追加されます。

     Workfrontでの売上高の計算方法について詳しくは、[&#x200B; 請求と売上高の概要 &#x200B;](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md) を参照してください。

     >[!TIP]
     >
     >既存の担当業務を編集する際に、最新の開始日を評価リストの先頭に表示するようにリストを並べ替えることができます。

1. 「**[!UICONTROL 担当業務を作成]**」をクリックします。担当業務をタスク、イシュー、承認に割り当てたり、レイアウトテンプレートや他のオブジェクトをタスクと共有したりできるようになります。[!DNL Workfront] でのすべての担当業務の使用に関する情報について詳しくは、[担当業務の概要](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md)を参照してください。担当業務の削除について詳しくは、[担当業務の削除](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md)を参照してください。

<!--
   * **Override Currency Cost Rate**: This is the cost per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role.

     Enter the rate in the Override Currency specified above. This also updates the Cost Rate for this job role when using the Base Currency.

     For information about how Workfront calculates cost, see [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a cost rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Cost Rate, the cost rate of the job role also updates automatically.

   * **Override Currency Billing Rate**: This is the billing per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role.

      Enter the rate in the Override Currency specified above. This also updates the Billing Rate for this job role when using the Base Currency.

      For information about how Workfront calculates revenue, see [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a billing rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing Rate, the billing rate of the job role also updates automatically.


   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td> <p>Indicate a name for the job role. This is the name that displays everywhere in [!DNL Workfront] where the [!UICONTROL Job Role] field displays. </p> <p>Tip: The name of a job role may contain up to 255 characters. However, longer names might be truncated in certain areas of [!DNL Workfront]. </p> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Enter a description for the role that indicates what is unique about it. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Is Active]</span> </td> 
      <td> 
       <ul> 
        <li> <p>Select <b>[!UICONTROL Yes]</b> if you want the role to be active and available everywhere in [!DNL Workfront] to be associated with users, work items, etc. </p> </li> 
        <li> <p>Select <b>[!UICONTROL No]</b>, if you want the role to be deactivated and not available to assign to users, work items, etc. </p> </li> 
       </ul> <p><span>For information about deactivating job roles, see</span> <a href="../../../administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md" class="MCXref xref">Deactivate job roles</a>. </p> </td> 
     </tr>
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Base Currency]</span> </td> 
      <td> <p><span>This is the [!UICONTROL Base Currency], as set in the [!UICONTROL Setup] area by your Workfront administrator. For information, see</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a> .</p> <p>Tip: <span>You cannot edit the [!UICONTROL Base Currency] at the job role level. This field is dimmed and serves as a reminder for what the base currency is for your system.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Cost Rate]</td> 
      <td><p>This is the cost per hour rate of the job role. This value calculates the planned and the actual costs of tasks and issues associated with the role, and ultimately the planned and actual costs of the projects. Enter the rate using the [!UICONTROL Base Currency].</p> 
      <p>For date effective cost rates, click <strong>[!UICONTROL Add Rate]</strong>. Enter the value of the cost/hour for the time period, and assign a [!UICONTROL Start Date] and [!UICONTROL End Date] as needed. The first cost rate will not have a start date and the last cost rate will not have an end date.</p> <p>Some dates are added automatically. For example, if the first cost rate does not have an end date, and you add a second cost rate with a start date of May 1, 2023, an end date of April 30, 2023 is added to the first cost rate so that no gaps exist.</p> <p>Tip: When editing an existing job role, you can select <strong>Sort by start date</strong> to see the most recent start date at the top of the rate list.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Billing Rate] </td> 
      <td><p>This is the billing per hour rate of the job role. This value calculates the planned and actual revenues of tasks and issues associated with the role, and ultimately the planned and actual revenues of the projects. Enter the rate using the [!UICONTROL Base Currency].</p> <p>For date effective billing rates, click <strong>[!UICONTROL Add Rate]</strong>. Enter the value of the billing/hour for the time period, and assign a [!UICONTROL Start Date] and [!UICONTROL End Date] as needed. The first billing rate will not have a start date and the last billing rate will not have an end date.</p> <p>Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, 2023, an end date of April 30, 2023 is added to the first billing rate so that no gaps exist.</p> <p>Tip: When editing an existing job role, you can select <strong>Sort by start date</strong> to see the most recent start date at the top of the rate list.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency]</span> </td> 
      <td>
        <p>Select a currency associated with this job role. This is the currency that [!DNL Workfront] uses for calculating costs and revenue associated with this job role. </p> 
        <p><span>This is different than the [!UICONTROL Base Currency] set up by your [!DNL Workfront] administrator in the [!UICONTROL Setup] area, and can be different than the currency associated with a project.</span> </p> 
        <p>Tip: Only currencies available in the [!UICONTROL Exchange Rates] area in your system are available in this field. If you only have one currency set up, this field is does not appear.</p> 
       <p><span>For information about setting up the [!UICONTROL Base Currency] in [!DNL Workfront], see</span> <a href="../../../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Set up exchange rates</a>.</p> <p><span>For information about changing the currency of a project, see</span> <a href="../../../manage-work/projects/project-finances/change-project-currency.md" class="MCXref xref">Change the project currency</a>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Cost Rate]</span> </td> 
      <td>
        <p>This is the cost per hour rate of the job role using the selected [!UICONTROL Override Currency]. [!DNL Workfront] uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role. </p> 
        <p><span>Enter the rate in the [!UICONTROL Override Currency] specified above. This also updates the Cost Rate for this job role when using the [!UICONTROL Base Currency].</span> </p> 
        <p>For information about how [!DNL Workfront] calculates cost, see <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Track costs</a>.</p> 
       <p>Tip: When updating an existing job role that already has a Cost Rate associated with it, [!DNL Workfront] calculates the [!UICONTROL Override Currency] rate based on the conversion rate in your system. If you update the [!UICONTROL Override Currency Cost Rate], the Cost Rate of the job role also updates automatically.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>[!UICONTROL Override Currency Billing Rate]</span> </td> 
      <td>
        <p>This is the billing per hour rate of the job role using the selected [!UICONTROL Override Currency]. [!DNL Workfront] uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role. </p>
        <p><span>Enter the rate in the [!UICONTROL Override Currency] specified above. This also updates the Billing Rateate for this job role when using the [!UICONTROL Base Currency].</span> </p>
        <p>For information about how [!DNL Workfront] calculates revenue, see <a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Overview of Billing and Revenue</a>.</p>
        <p>Tip: When updating an existing job role that already has a Billing Rate associated with it, [!DNL Workfront] calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing Rate, the Billing Rate of the job role also updates automatically. </p>
       </td>
     </tr> 
    </tbody> 
   </table>
-->



