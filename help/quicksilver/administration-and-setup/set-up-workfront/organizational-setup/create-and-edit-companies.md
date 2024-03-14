---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: 会社の作成と編集
description: 会社を  [!DNL Adobe Workfront]  に追加して、財務計画、レポートの目的、オブジェクトに関する権限の定義、情報の機密保持に使用することができます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bb597032-3395-4c9a-b622-5c920ba55131
source-git-commit: 155a2a8f5f266006629a28917a6a7565a95b37a9
workflow-type: tm+mt
source-wordcount: '1461'
ht-degree: 82%

---

# 会社の作成と編集

{{highlighted-preview}}

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

会社は、自分の組織、組織内の部門、または取引先の顧客を表す [!DNL Adobe Workfront] の組織単位です。会社を [!DNL Workfront] に追加して、財務計画、レポートの目的、オブジェクトに関する権限の定義、情報の機密保持に使用することができます。

## アクセス要件

[!DNL Workfront] で会社を管理するには、次が必要です。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] プラン</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] ライセンス*</p> </td> 
   <td><p>現在： [!UICONTROL プラン ]</p>
   または
   <p>新規： [!UICONTROL Standard]</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベルの設定</td> 
   <td> <p>次のうちのいずれか：</p> 
    <ul> 
     <li> <p>システム内の任意の会社を編集できる、[!UICONTROL System Administrator]のアクセスレベル。詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。 </p> </li> 
     <li> <p>システム内の任意の会社を編集できる、会社を管理するための管理者アクセス。詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md">特定のエリアに対する管理者アクセス権のユーザーへの付与</a>を参照してください。</p> </li> 
    </ul> <p><b>メモ</b>：  
     <ul> 
      <li> <p>また、自分がグループ管理者として割り当てられている任意のグループに関連する会社を管理することもできます。</p> </li> 
      <li> <p>[!DNL Workfront] システムでのユーザーの追加および削除を行うには、次のいずれかが必要です。</p> 
       <ul> 
        <li> <p>[!UICONTROL System Administrator] アクセスレベル。詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。 </p> </li> 
        <li> <p>アクセスレベルの [!UICONTROL Users] 設定で、[!UICONTROL Edit] が選択されている必要があります。また、[!UICONTROL Users] 設定の場合は、[!UICONTROL 設定の微調整 ] <img src="assets/gear-icon-in-access-levels.png">に設定されている場合は、[!UICONTROL 作成 ] オプションと、2 つの [!UICONTROL ユーザー管理 ] オプションのうち少なくとも 1 つを有効にする必要があります。 </p> <p> <img src="assets/access-req-users.png"> </p> <p>[!UICONTROL User Admin (Group Users)] オプションを使用している場合は、ユーザーがメンバーとなっているグループのグループ管理者である必要があります。</p> </li> 
       </ul> <p>アクセスレベルでのユーザー設定について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>を参照してください。</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセスレベルの設定を確認するには、 [!DNL Workfront] 管理者。 詳しくは、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

{#step-1-to-setup}

1. 「**[!UICONTROL 会社]**」をクリックします。

   会社のリストが表示されます。
1. 会社を追加する場合は、「**[!UICONTROL 新規会社]**」をクリックします。

   または

   既存の会社を編集する場合は、会社を選択し、 **[!UICONTROL 編集]** をクリックします。

1. 次の情報を更新します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Basic Info] セクション</td> 
      <td> 
       <ul> 
        <li> <p><b>[!UICONTROL Company Name]</b>：会社の名前を入力します。</p> </li> 
        <li> <p><b>[!UICONTROL Is Active]</b>：このオプションを有効にすると、ユーザーは会社を見つけて、作成および編集するプロジェクトに関連付けることができます。非アクティブな会社はプロジェクトに添付できません。このオプションは、デフォルトで有効になっています。</p> </li> 
        <li> <p><b>[!UICONTROL This is the Primary Company]</b>：会社を組織のプライマリ会社として割り当てます。通常、プライマリ会社は、[!DNL Workfront] のほとんどのユーザーが作業するアカウントです。</p> <p>1 つの会社をプライマリ会社として指定することも、プライマリ会社を指定しないこともできますが、複数の会社をプライマリ会社として指定することはできません。詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> <p><b>メモ</b>：アクセスレベルを変更することで、他のユーザーの表示を制限できます（プライマリ会社のみ、または関連する会社とプライマリ会社のみ）。プライマリ会社がユーザーのアクセスレベルでどのように機能するかについて詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </li> 
        <li> <p><b>[!UICONTROL Group]</b>：会社と取引を行うグループがある場合、ここにグループの名前を追加できます。これは、グループがビジネスを展開するすべての会社に関するレポートおよび管理を必要とするグループ管理者に役立ちます。</p> <p><b>重要</b>：この会社を使用するグループを関連付けない場合、グループの管理者は、アクセスレベルで会社に対する管理者アクセス権を持っていないと、会社にアクセスできません。 このアクセス権の付与方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定の領域に対する管理者アクセス権をユーザーに付与</a>を参照してください。</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">グループの名前を入力し始め、表示されたら <strong>[!UICONTROL Enter]</strong> を押します。</p> <p data-mc-conditions="SnippetConditions-wf-groups.system-level">グループを会社に割り当てると、そのグループの管理者は会社への [!UICONTROL Manage] アクセス権を取得します。詳しくは、この記事の<a href="#group-administrators-and-companies" class="MCXref xref">グループ管理者と会社</a>を参照してください。</p> </li> 
        <li> <p><b>[!UICONTROL Company Members]</b>：会社に既存のユーザーを追加します。これにより、これらのユーザーをこの会社に関連付けます。</p> <p>1 つの会社と関連付けるユーザー数に制限はありませんが、1 人のユーザーを複数の会社と関連付けることはできません。</p> </li> 
       </ul> </td> 
     </tr>
     <tr> 
      <td role="rowheader">[!UICONTROL Custom Forms] セクション</td> 
      <td> <p>会社に追加するフィールドが次の場所にない場合： [!DNL Workfront]を使用すると、カスタムフォームを作成して会社に関連付けることができます。 </p> <p>このフォームは、ドロップダウンメニューから選択して会社に添付できます。メニューには、アクティブなカスタムフォームのみが表示されます。</p> <p><span class="preview"><strong>注意：</strong> 「外部参照」フィールドやWorkfrontのネイティブフィールドなどの高度なカスタムフォーム機能は、会社の編集ダイアログではなく、詳細ページで会社レコードを開いたときにのみ使用できます。 （会社のリストで、会社名をクリックして詳細を開きます）。</span></p> <p> カスタムフォームの作成については、<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref">カスタムフォームの作成または編集</a>を参照してください。 </p> </td>
     </tr> 
    </tbody> 
   </table>

1. （条件付き）会社を作成する場合、 **[!UICONTROL 会社を作成]**.

   または

   既存の会社を編集している場合は、「**[!UICONTROL 変更を保存]**」をクリックします。

## 会社メンバーシップの管理

既存の会社のメンバーシップの管理について詳しくは、[会社メンバーシップの管理](../../../administration-and-setup/set-up-workfront/organizational-setup/manage-company-memberships.md)を参照してください。

## 請求レートの管理

会社レベルでの請求レートの上書きのについては、[会社レベルでの担当業務請求レートの上書き](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md)を参照してください。

## オブジェクトの会社との共有の概要

会社に関連付けられているユーザーは、特定の権限を使用できます（[ユーザーを会社に追加するメリット](#benefits-of-adding-users-to-a-company)の節を参照）。これらの権限に加えて、オブジェクトを会社と共有することで、[!DNL Workfront] 内のオブジェクトを表示、投稿、または編集する権限をユーザーに許可できます。

一度に 1 人のユーザーとオブジェクトを共有する代わりに、そのオブジェクトを会社全体と共有することができます。会社の各ユーザーは、そのオブジェクトに対して同じ権限を持ちます。

オブジェクトの共有について詳しくは、[オブジェクトに対する共有権限の概要](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

## グループ管理者と会社 {#group-administrators-and-companies}

[!DNL Workfront] 管理者がグループを会社に割り当てると、そのグループのグループ管理者は、[!UICONTROL 設定]で会社への[!UICONTROL 管理]権限を取得します。これには、[!UICONTROL 設定]の[!UICONTROL 会社]ページへのアクセスが含まれており、グループに関連付けられている会社を表示および管理できます。

この[!UICONTROL 会社]ページへのアクセスにより、グループ管理者はグループを会社に割り当てることができますが、その会社は同じグループ管理者が作成した会社である必要があります。グループ管理者のアクセスレベルが会社への管理アクセス権を持つように設定されていない場合、 [!UICONTROL グループ化] グループ管理者が会社を作成する場合は、フィールドが必須です。太字のタイトルは次のように示します。

![会社を編集](assets/group-admin-add-company.png)

ユーザーがアクセスレベルで会社に対して管理者アクセス権を取得する方法について詳しくは、[ユーザーへの特定の領域に対する管理者アクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)を参照してください。

[!UICONTROL 設定]領域での会社の管理については、[会社の作成または編集 [!DNL Workfront]](#create-or-edit-a-company-in-workfront)を参照してください。
