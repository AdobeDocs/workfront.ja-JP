---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: 会社の作成および編集
description: 会社を  [!DNL Adobe Workfront]  に追加して、財務計画、レポートの目的、オブジェクトに関する権限の定義、情報の機密保持に使用することができます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: 2e86369ae4c8e9fe2678773c20c02f6dbf8d5247
workflow-type: tm+mt
source-wordcount: '1399'
ht-degree: 74%

---

# 会社の作成と編集

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

会社は、自分の組織、組織内の部門、または取引先の顧客を表す [!DNL Adobe Workfront] の組織単位です。会社を [!DNL Workfront] に追加して、財務計画、レポートの目的、オブジェクトに関する権限の定義、情報の機密保持に使用することができます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Workfront] package</p> </td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] ライセンス</p> </td> 
   <td><p>[!UICONTROL Plan]</p>
   <p>[!UICONTROL Standard]</p>
   </td> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>次のいずれかが必要です。</p> 
    <ul> 
     <li> <p>[!UICONTROL システム管理者 ] アクセス レベル。システム内の任意の会社を編集できます。</p> </li> 
     <li> <p>会社を管理するための管理者アクセス。システム内の任意の会社を編集できます。</p> </li> 
    </ul> <p><b>メモ</b>：  
     <ul> 
      <li> <p>また、自分がグループ管理者として割り当てられている任意のグループに関連する会社を管理することもできます。</p> </li> 
      <li> <p>[!DNL Workfront] システムにユーザーを追加したり、システムからユーザーを削除したりするには、次のいずれかが必要です。</p> 
       <ul> 
        <li> <p>[!UICONTROL System Administrator] アクセスレベル。 </p> </li> 
        <li> <p>アクセスレベルの <b>[!UICONTROL ユーザー ]</b> 設定が <b>[!UICONTROL 編集 ]</b> アクセスに設定され、<b>[!UICONTROL 作成 ]</b> と、<b> </b>[!UICONTROL 設定 ]<b> で有効になっている 2 つの </b>[!UICONTROL ユーザー管理者 ]<img src="assets/gear-icon-in-access-levels.png"> オプションのうち少なくとも 1 つが設定されています。 </p> <p> <img src="assets/access-req-users.png"> </p> <p>これら 2 つのオプションのうち、<b>[!UICONTROL User Admin （Group Users） ]</b> が有効になっている場合、ユーザーがメンバーになっているグループのグループ管理者である必要があります。</p> </li> 
       </ul>
       </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ユーザーを会社に追加するメリット {#benefits-of-adding-users-to-a-company}

* ユーザーを直属の部下に関連付けることで、会社の組織図を作成できます。同じ会社のユーザーのみを、その会社の別のユーザーの直属の部下として追加できます。
* プロジェクトマネージャーは、同じ会社内で利用可能リソースを識別できます。
* 以下の設定の 1 つまたはすべてを選択して、企業間で情報を非公開に保つことができます。

   * 同じ会社のユーザーはお互いのリクエストを表示可能。

     ユーザーの会社に基づいて [!DNL Workfront] 管理者がリクエストに対して同様のアクセス権を付与する方法について詳しくは、[システム全体のタスクとイシューの環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)の記事にある [ [!DNL Workfront]](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#changing-task-and-issue-preferences) の全員に対するタスクとイシューの環境設定の指定の節を参照してください。

     ユーザーの会社に基づいて管理者がリクエストに対して同様のアクセス権を付与する方法について詳しくは、[グループのタスクとイシューの環境設定の指定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)を参照してください。

   * ユーザーは自分の会社に関連付けられているリクエストキューのみを表示可能。リクエストキューの表示を制限する方法について詳しくは、[リクエストキューへのアクセス権の提供](../../../manage-work/requests/create-and-manage-request-queues/provide-access-to-request-queues.md)を参照してください。
   * ユーザーに対して、自分の会社または自分の会社とプライマリ会社のユーザーのみを表示するように制限できます。ユーザーのプライバシーに関するプライマリ会社の機能について詳しくは、[カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。
   * ユーザーは項目に加えた更新を自分の会社ユーザーのみが表示できるように制限可能。会社で更新を非公開にする方法について詳しくは、[作業の更新](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)を参照してください。

## [!DNL Workfront] で会社を作成または編集 {#create-or-edit-a-company-in-workfront}

追加できる会社の数に制限はありません。ただし、オブジェクトの権限に問題が発生する可能性があるため、使用する会社の数を制限することをお勧めします。細分化しすぎると、作業アイテムに対するユーザーの可視性が損なわれる可能性があります。

デフォルトでは、[!DNL Workfront] のインスタンスに関連付けられた会社は [!DNL Workfront] システムに既に作成されており、これが組織のプライマリ会社です。顧客名と同じ名前を持ちます。[!DNL Workfront] の顧客情報について詳しくは、[システムの基本情報の設定](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md)を参照してください。

会社を追加または編集するには、以下のように行います。

{{step-1-to-setup}}

1. 「**[!UICONTROL 会社]**」をクリックします。

   会社のリストが表示されます。

1. 会社を追加する場合は、「**[!UICONTROL 新規会社]**」をクリックします。

   または

   既存の会社を編集する場合は、会社を選択し、会社リストの上部にある **[!UICONTROL 編集]** アイコン ![ 編集アイコン ](assets/edit-icon.png) をクリックします。

1. 「**基本情報**」セクションで次の情報を更新します。

   * **会社名**<!--<span class="preview"> or **Name**</span>-->：会社の名前を入力します。
   * **アクティブ**：このオプションを有効にすると、ユーザーは会社を見つけて、作成および編集するプロジェクトに参加させることができます。非アクティブな会社はプロジェクトに添付できません。このオプションは、デフォルトで有効になっています。
   * **これがプライマリ会社です**<!--<span class="preview">or **Is Primary**</span>-->：会社を組織のプライマリ会社として割り当てます。通常、プライマリ会社は、ほとんどのユーザーが作業する Workfront アカウントを表します。

     1 つの会社をプライマリ会社として指定することも、プライマリ会社を指定しないこともできますが、複数の会社をプライマリ会社として指定することはできません。詳しくは、[カスタムアクセスレベルを作成および変更](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。

     >[!NOTE]
     >
     >アクセスレベルを変更することで、ユーザーが他のユーザー（プライマリ会社のみ、または関連する会社およびプライマリ会社のみ）を表示するように制限できます。 プライマリ会社がユーザーのアクセスレベルをどのように操作するかについて詳しくは、[ カスタムアクセスレベルの作成と変更 ](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md) を参照してください。

   * **グループ**：会社と取引を行うグループがある場合、ここにグループの名前を追加できます。これは、グループがビジネスを展開するすべての会社に関するレポートおよび管理を必要とするグループ管理者に役立ちます。

     この会社で作業するグループを関連付けない場合、グループの管理者は、アクセス レベル内の会社に対する管理アクセス権を持っていない限り、その会社にアクセスできません。 このアクセス権の付与方法について詳しくは、[特定の領域に対する管理者アクセス権をユーザーに付与](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)を参照してください。

     グループの名前の入力を開始し、表示されたら選択します。

     グループを会社に割り当てると、そのグループのグループ管理者は、会社に対する管理アクセス権を取得します。 詳しくは、この記事の[グループ管理者と会社](#group-administrators-and-companies)を参照してください。

   * **会社メンバー**：会社に既存のユーザーを追加します。これにより、これらのユーザーをこの会社に関連付けます。

     ユーザーの名前の入力を開始し、表示されたら選択します。

     1 つの会社と関連付けるユーザー数に制限はありませんが、1 人のユーザーを複数の会社と関連付けることはできません。

1. 「**カスタムForms**」セクションで、カスタムフォームを追加または更新します。

   Workfrontで使用できない、会社に追加するフィールドがある場合は、カスタムフォームを作成して会社に関連付けることができます。

   このフォームは、ドロップダウンメニューから選択して会社に添付できます。アクティブなカスタムフォームのみが、メニューに表示されます。

   >[!NOTE]
   >
   >外部検索フィールドやWorkfront ネイティブフィールドなどの高度なカスタムフォーム機能は、会社を編集ダイアログではなく、詳細ページで会社レコードを開いた場合にのみ使用できます。 （会社のリストで、会社名をクリックすると詳細が開きます）。

   カスタムフォームの作成について詳しくは、「[ カスタムフォームの作成 ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)」を参照してください。

1. （条件付き）新しい会社を作成する場合は、「**[!UICONTROL 会社を作成]**<!--<span class="preview">or **Save**</span>-->」をクリックします。

   または

   既存の会社を編集している場合は、「**[!UICONTROL 変更を保存]**<!--<span class="preview">or **Save**</span>-->」をクリックします。

## 会社メンバーシップの管理

既存の会社のメンバーシップの管理について詳しくは、[会社メンバーシップの管理](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md)を参照してください。

## 請求レートの管理

会社レベルでの請求レートの上書きのについては、[会社レベルでの担当業務請求レートの上書き](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md)を参照してください。

## 会社とのオブジェクトの共有の概要

会社に関連付けられているユーザーは、特定の権限を使用できます（[ユーザーを会社に追加するメリット](#benefits-of-adding-users-to-a-company)の節を参照）。これらの権限に加えて、オブジェクトを会社と共有することで、[!DNL Workfront] 内のオブジェクトを表示、投稿、または編集する権限をユーザーに許可できます。

一度に 1 人のユーザーとオブジェクトを共有する代わりに、そのオブジェクトを会社全体と共有することができます。会社の各ユーザーは、そのオブジェクトに対して同じ権限を持ちます。

オブジェクトの共有について詳しくは、[オブジェクトに対する共有権限の概要](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

## グループ管理者と会社 {#group-administrators-and-companies}

[!DNL Workfront] 管理者がグループを会社に割り当てると、そのグループのグループ管理者は、[!UICONTROL 設定]で会社への[!UICONTROL 管理]権限を取得します。これには、[!UICONTROL 設定]の[!UICONTROL 会社]ページへのアクセスが含まれており、グループに関連付けられている会社を表示および管理できます。

この[!UICONTROL 会社]ページへのアクセスにより、グループ管理者はグループを会社に割り当てることができますが、その会社は同じグループ管理者が作成した会社である必要があります。グループ管理者のアクセスレベルが会社への管理アクセスを含むように設定されていない場合、グループ管理者が会社を作成する際に「[!UICONTROL グループ]」フィールドが必要になります。太字のタイトルはこれを示しています。

![会社を編集](assets/group-admin-add-company.png)

ユーザーがアクセスレベルで会社に対して管理者アクセス権を取得する方法について詳しくは、[ユーザーへの特定の領域に対する管理者アクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)を参照してください。

[!UICONTROL 設定]領域での会社の管理については、[会社の作成または編集 [!DNL Workfront]](#create-or-edit-a-company-in-workfront)を参照してください。

<!-- OLD HTML TABLE
<table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic Info] section</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL Company Name]</b>: Type a name for the company.</p> </li> 
        <li> <p><b>[!UICONTROL Is Active]</b>: When this option is enabled, users can find the company and attach it to projects that they create and edit. An inactive company cannot be attached to projects. This option is enabled by default.</p> </li> 
        <li> <p><b>[!UICONTROL This is the Primary Company]</b>: Assigns the company as your organization's primary company. The primary company typically represents your [!DNL Workfront] account where most of your users work.</p> <p>You can have one company or no company designated as a primary company, but you cannot have multiple companies designated as primary companies. For more information, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> <p><b>NOTE</b>: By modifying their access levels, you can restrict users to see other users: only in their primary company, or in their associated company and the primary company. For information about how the primary company works with users' access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </li> 
        <li> <p><b>[!UICONTROL Group]</b>: If there is a group that conducts business with the company, you can add the name of the group here. This is useful for group administrators who need to report on and manage all the companies that their groups do business with.</p> <p><b>IMPORTANT</b>: If you don't associate the group that will be working with this company, administrators for the group can't access the company unless they have administrative access to companies in their access level. For information about how this access is granted, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Grant users administrative access to certain areas</a>.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">Start typing the name of the group, then press <strong>[!UICONTROL Enter]</strong> when it appears.</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">When you assign a group to a company, the group administrators for the group gain [!UICONTROL Manage] access to the company. For more information, see <a href="#group-administrators-and-companies" class="MCXref xref">Group administrators and companies</a> in this article.</p> </li> 
        <li> <p><b>[!UICONTROL Company Members]</b>: Add existing users to the company. By doing this, you are associating these users with this company.</p> <p>There is no limit to how many users you associate with one company, but a user cannot be associated with more than one company.</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Custom Forms] section</td> 
      <td> <p>If there are fields that you want to add to your company that are not available in [!DNL Workfront], you can build a custom form and associate it with your company. </p> <p>You can attach this form to your company by selecting it from the drop-down menu. Only active custom forms are listed in the menu.</p> <p><strong>Note:</strong> Advanced custom form features such as External lookup fields and Workfront native fields are only available when you open the company record on the details page, not on the Edit Company dialog. (From the list of companies, click the company name to open the details.)</p> <p> For information about creating custom forms, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md">Create a custom form</a>. </p> </td>
     </tr> 
    </tbody> 
   </table>
   -->
