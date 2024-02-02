---
user-type: administrator
product-area: system-administration
navigation-topic: organization-setup
title: 会社メンバーシップの管理
description: 設定の[!UICONTROL 会社]エリアで、会社のメンバーを追加および削除できます。また、ユーザープロファイルを編集して、ユーザーに  [!DNL Workfront], deactivate them in [!DNL Workfront], and remove them from the [!DNL Workfront]  システムで登録を促すこともできます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f0efd985-76e3-435e-bf19-87008f6a5e9d
source-git-commit: b6f6964bb80f172849434c669df2b0ecd735a590
workflow-type: ht
source-wordcount: '910'
ht-degree: 100%

---

# 会社メンバーシップの管理

[!UICONTROL 設定]の[!UICONTROL 会社]エリアで、会社のメンバーを追加および削除できます。また、ユーザープロファイルの編集、ユーザーに対する [!DNL Workfront] での登録のリマインド、[!DNL Workfront] で非アクティブ化および [!DNL Workfront] システムから削除もできます。

新しい会社の作成について詳しくは、[会社の作成と編集](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md)を参照してください。

## アクセス要件

[!DNL Workfront] で会社を管理するには、次が必要です。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Workfront] プラン*</p> </td> 
   <td>[!UICONTROL Team] 以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Adobe Workfront] ライセンス*</p> </td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong> </td> 
   <td> <p>次のうちのいずれか：</p> 
    <ul> 
     <li> <p>システム内の任意の会社を編集できる、[!UICONTROL System Administrator]のアクセスレベル。詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。 </p> </li> 
     <li> <p>システム内の任意の会社を編集できる、会社を管理するための管理者アクセス。詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定のエリアに対する管理者アクセス権のユーザーへの付与</a>を参照してください。</p> </li> 
    </ul> <p><b>メモ</b>：  
     <ul> 
      <li> <p>また、自分がグループ管理者として割り当てられている任意のグループに関連する会社を管理することもできます。</p> </li> 
      <li> <p>[!DNL Workfront] システムでのユーザーの追加および削除を行うには、次のいずれかが必要です。</p> 
       <ul> 
        <li> <p>[!UICONTROL System Administrator] アクセスレベル。詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。 </p> </li> 
        <li> <p>アクセスレベルの [!UICONTROL Users] 設定で、[!UICONTROL Edit] が選択されている必要があります。また、[!UICONTROL Users] 設定の場合は、[!UICONTROL Fine-tune your settings] <img src="assets/gear-icon-in-access-levels.png"> 下の [!UICONTROL Create] オプションと、2 つの [!UICONTROL User Admin] オプションのうち少なくとも 1 つを有効にする必要があります。 </p> <p> <img src="assets/access-req-users.png"> </p> <p>[!UICONTROL User Admin (Group Users)] オプションを使用している場合は、ユーザーがメンバーとなっているグループのグループ管理者である必要があります。</p> </li> 
       </ul> <p>アクセスレベルでのユーザー設定について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>を参照してください。</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプ、アクセスレベルの設定を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 会社メンバーシップの管理

1. [!DNL Adobe Workfront] の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、次に&#x200B;**[!UICONTROL 設定]** ![](assets/gear-icon-settings.png) をクリックします。

1. 「**[!UICONTROL 会社]**」をクリックします。
1. 会社の名前をクリックします。
1. 左側のパネルで選択した「**[!UICONTROL 会社メンバー]**」セクションを使用して、次のいずれかの操作を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">メンバーを追加</td> 
      <td> <p>「<b>[!UICONTROL Add member]</b>」をクリックして、表示されるドロップダウンメニューで次のいずれかのオプションを選択します。</p> 
       <ul> 
        <li> <p><b>[!UICONTROL New user]</b>：まだ [!DNL Workfront] に追加されていないユーザーを追加します。</p> <p>[!DNL Workfront] へのユーザーの追加について詳しくは、<a href="../../../administration-and-setup/add-users/create-and-manage-users/add-users.md" class="MCXref xref">ユーザーの追加</a>および<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">ユーザーのプロファイルの編集</a>を参照してください。</p> </li> 
        <li> <p><b>[!DNL Existing user]</b>：編集できるシステム内に既に存在するユーザーを追加します。</p> <p><b>重要</b>：ユーザーが既に別の会社のメンバーになっている場合は、新しい割り当てによって古い割り当てが上書きされます。ユーザーは、以前の会社と共有された項目へのアクセス権を失い、新たに割り当てられた会社と共有された項目へのアクセス権を取得します。</p> </li> 
        <li> <p><b>[!UICONTROL Import Users]</b>：スプレッドシートの読み込みファイルをアップロードして、ユーザーを読み込みます。詳しくは、<a href="../../../administration-and-setup/add-users/create-and-manage-users/import-users.md" class="MCXref xref">ユーザーの読み込み</a>を参照してください。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">メンバーの編集</td> 
      <td> 
       <ol> 
        <li value="1"> <p>少なくとも 1 人のユーザーを選択して、ツールバーの [!UICONTROL Edit] アイコン <img src="assets/edit-icon.png"> をクリックします。</p> </li> 
        <li value="2"> <p>表示される「<b>[!UICONTROL Edit User]</b>」ボックスで、オプションを設定します。</p> <p>これらのオプションについて詳しくは、<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">ユーザーのプロファイルの編集</a>を参照してください。</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">メンバーのコピー</td> 
      <td> <p>既存のメンバーをコピーして、会社メンバーを作成できます。 </p> <p><b>メモ</b>：  <p>この方法でユーザーを作成する場合、次の場合を除き、元のユーザーから新しく作成されたユーザーにすべての情報がコピーされます。</p> 
        <ul> 
         <li>「[!UICONTROL Personal Info]」セクションの情報。</li> 
         <li>[!UICONTROL When I log in, show]：このボックスでは、アクセスレベルのデフォルトのランディングタブが選択されています。</li> 
         <li>[!UICONTROL Direct Reports]</li> 
        </ul> </p> 
       <ol> 
        <li value="1"> <p>ユーザーを選択して、[!UICONTROL Copy] アイコン <img src="assets/copy-icon.png"> をクリックします。 </p> </li> 
        <li value="2"> <p>表示される「<b>[!UICONTROL New User]</b>」ボックスで、新しいユーザーが使用できるフィールドを編集します。</p> <p>ユーザーに関連付けられているすべてのフィールドについて詳しくは、<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">ユーザーのプロファイルの編集</a>を参照してください。</p> </li> 
        <li value="3"> <p>「<strong>[!UICONTROL Add This User]</strong>」をクリックします。</p> <p>または</p> <p>「<strong>[!UICONTROL Add Person User &amp; Start Another]</strong>」をクリックして、新しいユーザーを保存し、別のユーザーを追加します。</p> </li> 
       </ol> <p>これにより、[!DNL Workfront] にユーザーの新しいアカウントが作成されます。</p> <p>招待をユーザーに送信するオプションを選択した場合、そのユーザーにはメールが届き、ユーザーはリンクを使用して [!DNL Workfront] パスワードを作成できます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ユーザーの削除</td> 
      <td> 
       <div> 
        <p>少なくとも 1 人のユーザーを選択し、「<b>[!UICONTROL Remove users]</b>」を選択し、表示されるドロップダウンメニューで次のいずれかのオプションを選択します。</p> 
        <ul> 
         <li> <p><b>[!UICONTROL Remove from company]</b>：1 人または複数のユーザーを会社から削除します。</p> </li> 
         <li> <p><b>[!UICONTROL Delete]</b>：1 人または複数のユーザーを [!DNL Workfront] システムから削除します。</p> <p><b>重要</b>：システムからユーザーを削除すると、保持する予定のユーザーに関連付けられた情報も削除されてしまいます。ユーザーを削除する代わりに非アクティブ化することをお勧めします。詳しくは、<a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">ユーザーの非アクティブ化または再アクティブ化</a>を参照してください。</p> </li> 
        </ul> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ユーザーおよび [!UICONTROL Updates] エリアへのコメントの送信</td> 
      <td> 
       <ol> 
        <li value="1"> <p>少なくとも 1 人のユーザーを選択して、ツールバーの [!UICONTROL Comment] アイコン <img src="assets/comment-icon.png"> をクリックします。</p> </li> 
        <li value="2"> <p>ユーザーおよびユーザープロファイルの [!UICONTROL Updates] エリアに送信するコメントを入力します。</p> </li> 
       </ol> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">会社メンバーのリストの書き出し</td> 
      <td> <p>ツールバーの [!UICONTROL Export] アイコン <img src="assets/export.png"> をクリックして、書き出すファイルの形式を選択します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">システム内のメンバーの非アクティブ化</td> 
      <td> <p>少なくとも 1 人のユーザーを選択し、ツールバーの [!UICONTROL More] アイコン <img src="assets/more-icon.png"> をクリックして、「<b>[!UICONTROL Deactivate]</b>」を選択します。</p> <p>詳しくは、<a href="../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">ユーザーの非アクティブ化または再アクティブ化</a>を参照してください。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">ユーザーにシステム登録をリマインド</td> 
      <td> <p> <b>[!UICONTROL Name]</b> 列に、未登録の各ユーザーの名前の横に <b>[!UICONTROL Unregistered]</b> が表示されます。これらのユーザーにシステムへの登録を促すには、ユーザーを選択して、ツールバーで [!UICONTROL More] アイコン <img src="assets/more-icon.png"> をクリックして、「<b>[!UICONTROL Remind user to register]</b>」を選択します。</p> </td> 
     </tr> 
    </tbody> 
   </table>
