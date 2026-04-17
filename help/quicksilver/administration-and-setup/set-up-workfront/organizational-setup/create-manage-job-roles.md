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
source-git-commit: d8a01839b8f1332741f87be766f3ccb7d08cef96
workflow-type: tm+mt
source-wordcount: '1219'
ht-degree: 28%

---

# 担当業務の作成と管理

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

>[!IMPORTANT]
>
>25.11 リリースでは、ジョブロールの通貨の上書きは実稼動環境で廃止されました。 （廃止は10月30日にプレビュー環境で行われました）。 基本通貨とオーバーライド通貨を持つ代わりに、1つの通貨が担当業務で使用できるようになりました。コストと請求率は、その通貨を使用して定義されます。

[!DNL Adobe Workfront]管理者またはジョブロールへの編集アクセス権を持つ標準ユーザーは、ユーザーに割り当てることができるジョブロールを作成し、組織に関連しないデフォルトのジョブロールを削除できます。 [!DNL Workfront] での管理アクセスについて詳しくは、[特定のエリアに対する管理アクセス権をユーザーに付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)を参照してください。

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
   <td>[!DNL Adobe Workfront] パッケージ</td> 
   <td><p>担当業務を作成または編集するには：WorkfrontまたはWorkflow パッケージ</p>
   <p>レート属性を適用し、ジョブロールにカスタムフォームを追加するには：Workflow Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>担当業務へのアクセス権の編集</td>
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 担当業務を作成

担当業務を作成するには：

{{step-1-to-setup}}

1. 左側のパネルで、**[!UICONTROL 担当業務]**&#x200B;をクリックします。
1. **[!UICONTROL 新しい担当業務]/新しい担当業務を作成**&#x200B;をクリックします。
1. 次のフィールドに情報を入力します。

   * **名前**：担当業務の名前を指定します。 これは、「担当業務」フィールドが表示されるWorkfrontの任意の場所に表示される名前です。

     >[!TIP]
     >
     >担当業務の名前には、最大255文字を含めることができます。 ただし、Workfrontの特定の地域では、長い名前が切り捨てられる場合があります。

   * **説明**：役割の説明を入力します。この説明は、その役割に固有の内容を示します。
   * **はアクティブです**: ロールをアクティブにし、Workfront内のあらゆる場所で利用できるようにしたい場合は、**はい**&#x200B;を選択します。 役割を非アクティブにし、ユーザーや作業項目などに割り当てることができないようにする場合は、**No**&#x200B;を選択します。

     担当業務の非アクティブ化について詳しくは、[担当業務の非アクティブ化](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md)を参照してください。

1. 「**[!UICONTROL 担当業務を作成]**」をクリックします。担当業務をタスク、イシュー、承認に割り当てたり、レイアウトテンプレートや他のオブジェクトをタスクと共有したりできるようになります。[!DNL Workfront] でのすべての担当業務の使用に関する情報について詳しくは、[担当業務の概要](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md)を参照してください。担当業務の削除について詳しくは、[担当業務の削除](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md)を参照してください。

## 担当業務へのレートと属性の追加

担当業務の請求率と原価率は、財務計算で使用されます。

レート属性は、ジョブロールやユーザーなど、レートが存在するWorkfrontの領域でサポートされます。 担当業務に属性が適用されると、その割り当ては自動的に正しい率に解決されます。

詳しくは、[ レート属性の定義](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)を参照してください。

{{step-1-to-setup}}

1. 左側のパネルで、**[!UICONTROL 担当業務]**&#x200B;をクリックします。
1. 既存の担当業務の名前をクリックして編集します。
1. 担当業務の詳細を更新するには、左側のパネルで「**詳細**」をクリックします。
1. （オプション）カスタムフォームを担当業務に添付するには、詳細ページの右上隅にある「**カスタムフォームを追加**」フィールドをクリックし、表示されるリストからカスタムフォームを選択します。

   カスタムフォームの添付について詳しくは、[オブジェクトへのカスタムフォームの追加](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)を参照してください。

1. 左側のパネルで「[!UICONTROL **レート**]」をクリックします。
1. [!UICONTROL **請求**]&#x200B;または&#x200B;[!UICONTROL **コスト**]&#x200B;をクリックして、料金タイプを選択します。
1. 「[!UICONTROL **レートを追加**]」をクリックして、新しいレートを追加します。

   または

   既存のレートを選択し、**編集** アイコン ![編集アイコン ](assets/edit-icon.png)をクリックして更新します。

   >[!NOTE]
   >
   >各レートは、役割と属性の組み合わせに関連付けられて一意のレートを作成するため、レートを編集するときに属性を変更することはできません。

1. **新しいレート** ボックスで、代理店、場所、コストセンターなどのレートの属性を選択します。

   >[!NOTE]
   >
   >これらの属性は個別に定義され、収益とコストの計算に影響を与える可能性があります。 詳しくは、[ レート属性の定義](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md)を参照してください。

1. レートの&#x200B;**通貨**&#x200B;を選択します。 Workfront管理者は、設定領域に基本通貨を追加します。 選択範囲を別の使用可能な通貨に変更したり、有効な日付範囲で通貨を変更したりできます。

   >[!TIP]
   >
   >このフィールドでは、システムの「為替レート」領域で使用可能な通貨のみが使用できます。 通貨が1つしか設定されていない場合は、その通貨のみが使用可能です。

   Workfrontでの基本通貨の設定について詳しくは、[為替レートの設定](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md)を参照してください。

   プロジェクトの通貨の変更について詳しくは、[ プロジェクトの通貨の変更](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md)を参照してください。

1. （条件付き）請求率については、この担当業務の&#x200B;**請求率**&#x200B;を入力してください。

   これは、担当業務の 1 時間あたりの請求レートです。この値は、役割に関連するタスクの予定収益と実収益、最終的にはプロジェクトの予定収益と実収益を計算します。選択した通貨を使用してレートを入力します。

   属性を使用する場合、属性と担当業務が組み合わされて一意のレートが定義されます。 例えば、エージェンシーAのニューヨークでのDesignerの役割は、エージェンシーBのパリでのDesignerの役割とは別の料金を設定できます。

   有効日の請求レートについては、「**レートを追加**」をクリックします。期間の請求/時間の値を入力し、必要に応じて開始日と終了日を割り当てます。 最初の請求レートには開始日が設定されず、最後の請求レートには終了日が設定されません。

   <!-- Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, an end date of April 30 is added to the first billing rate so that no gaps exist.-->

   Workfrontでは、日付範囲の間にギャップを残すことができますが、意図的であることを確認する警告が表示されます。

   Workfrontによる売上の計算方法について詳しくは、[請求と売上の概要](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md)を参照してください。

   >[!TIP]
   >
   >既存の担当業務を編集する場合、最新の開始日をレートリストの上部に表示するようにリストを並べ替えることができます。

1. （条件付き）原価率の場合は、この担当業務の&#x200B;**原価率**&#x200B;を入力します。

   これは、担当業務の 1 時間あたりのコスト率です。この値は、役割に関連するタスクとイシューの予定コストと実際のコスト、最終的にはプロジェクトの予定コストと実際のコストを計算します。選択した通貨を使用してレートを入力します。

   属性を使用する場合、属性と担当業務が組み合わされて一意のレートが定義されます。 例えば、エージェンシーAのニューヨークでのDesignerの役割は、エージェンシーBのパリでのDesignerの役割とは別の料金を設定できます。

   有効日のコスト率については、「**レートを追加**」をクリックします。期間のコスト/時間の値を入力し、必要に応じて開始日と終了日を割り当てます。 最初のコスト率には開始日が設定されず、最後のコスト率には終了日が設定されません。

   一部の日付は自動的に追加されます。例えば、最初の原価率に終了日がなく、開始日が5月1日の2番目の原価率を追加した場合、最初の原価率に4月30日の終了日が追加され、ギャップが存在しません。

   Workfrontでのコストの計算方法について詳しくは、[ コストの追跡](/help/quicksilver/manage-work/projects/project-finances/track-costs.md)を参照してください。

   >[!TIP]
   >
   >既存の担当業務を編集する場合、最新の開始日をレートリストの上部に表示するようにリストを並べ替えることができます。

1. 「[!UICONTROL **保存**]」をクリックします。

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

-->


<!--

   * **Currency**: The Base Currency is shown by default. The Workfront administrator adds the Base Currency in the Setup area. You can change the selection to another available currency, and you can change the currency on effective dated time ranges.

      >[!TIP]
      >
      >Only currencies available in the Exchange Rates area in your system are available in this field. If you only have one currency set up, only that currency is available.

      For information about setting up the Base Currency in Workfront, see [Set up exchange rates](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

      For information about changing the currency of a project, see [Change the project currency](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).
   
   * **Cost Rate**: This is the cost per hour rate of the job role. This value calculates the planned and the actual costs of tasks and issues associated with the role, and ultimately the planned and actual costs of the projects. Enter the rate using the selected currency.

      For date effective cost rates, click **Add Rate**. Enter the value of the cost/hour for the time period, and assign a Start Date and End Date as needed. The first cost rate will not have a start date and the last cost rate will not have an end date.

      Some dates are added automatically. For example, if the first cost rate does not have an end date, and you add a second cost rate with a start date of May 1, 2025, an end date of April 30, 2025 is added to the first cost rate so that no gaps exist.

      For information about how Workfront calculates cost, see [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

      >[!TIP]
      >
      >When editing an existing job role, you can sort the list to see the most recent start date at the top of the rate list.

   * **Billing Rate**: This is the billing per hour rate of the job role. This value calculates the planned and actual revenues of tasks and issues associated with the role, and ultimately the planned and actual revenues of the projects. Enter the rate using the selected currency.

      For date effective billing rates, click **Add Rate**. Enter the value of the billing/hour for the time period, and assign a Start Date and End Date as needed. The first billing rate will not have a start date and the last billing rate will not have an end date.

      Some dates are added automatically. For example, if the first billing rate does not have an end date, and you add a second with a start date of May 1, 2025, an end date of April 30, 2025 is added to the first billing rate so that no gaps exist.

      For information about how Workfront calculates revenue, see [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

      >[!TIP]
      >
      >When editing an existing job role, you can sort the list to see the most recent start date at the top of the rate list.

-->



