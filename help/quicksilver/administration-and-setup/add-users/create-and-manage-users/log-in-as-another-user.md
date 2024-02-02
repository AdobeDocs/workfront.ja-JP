---
title: 別のユーザーとしてのログイン
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Adobe Workfront の管理者は、別のユーザーの代わりに Workfront にアクセスする必要が生じる場合があります。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2f8dd132-1086-4980-9b56-993a68231e96
source-git-commit: bc7039bc4b8b257fc55e71e73f72327fdb417837
workflow-type: ht
source-wordcount: '809'
ht-degree: 100%

---

# 別のユーザーとしてのログイン


<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all users only in the Preview environment.</span> -->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. Also linked to other articles: Creating and Managing Groups, etc.</p>
-->

>[!IMPORTANT]
>
>このページで説明する手順は、まだ Adobe Admin Console にオンボーディングされていない組織にのみ適用されます。組織が Adobe Admin Console にオンボーディングされている場合、このアクションは使用できません。
>
>組織が Adobe Admin Console にオンボーディングされているかどうかに応じて異なる手順のリストについて詳しくは、[プラットフォームベースの管理上の違い（Adobe Workfront/Adobe Business Platform）](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md)を参照してください。

Adobe Workfront の管理者は、別のユーザーの代わりに Workfront にアクセスする必要が生じる場合があります。

また、グループ管理者は、管理対象のグループのメンバーであるユーザーに代わって Workfront にアクセスする必要が生じる場合があります。

例えば、休暇中のユーザーが特定のアクションを実行するまでタスクを進行できない場合、そのユーザーとしてログインし、代わりにアクションを実行できます。

<!--
<note type="note">
Some users, such as executives, need to be able to control which administrators can log in to their accounts, and for how long. Working with your organization, Workfront configures settings that allow this control for these users. When a Workfront administrator or group administrator (associated with one of the user's groups) tries to log in as one of these users, an on-screen message prompts the administrator to contact the user for access. From the user profile area, the user can then grant access to the administrator and specify an expiration time for it. For more information on how the user does this, see
<a href="../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md#access" class="MCXref xref">Access</a> in
<a href="../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">Configure My Settings</a>.
<span class="PinkDraftNote">[Add a note about this being only for the Enterprise package if they decide to do it that way]</span>
</note>
-->

>[!NOTE]
>
>ドキュメントの統合により、個人用の非公開ファイルに接続できるので、管理者は別のユーザーとしてログインしている間はドキュメントの統合にアクセスできません。
>
>ドキュメントの統合について詳しくは、[ドキュメント統合の設定](../../../administration-and-setup/configure-integrations/configure-document-integrations.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>システム管理者のアクセスレベルは、どのユーザーとしてもログインできます。このレベルのアクセスについて詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。 </p> <p>プランナーアクセスレベルでは、アクセスレベルの<b>ユーザー</b>設定が<b>編集</b>アクセス、<b>作成</b>および<b>設定の微調整</b><img src="assets/gear-icon-in-access-levels.png">で 2 つの<b>ユーザー管理者</b>オプションのうち少なくとも 1 つが有効になっていれば、下位のライセンスレベルのユーザーとしてログインできます。 </p> 
   <p><b>メモ</b>：これら 2 つのオプションのうち、ユーザー<b>管理者（グループユーザー）</b>が有効になっている場合は、ユーザーがメンバーであるグループのグループ管理者である必要があります。</p> 
   <p>アクセスレベルの<b>ユーザー</b>設定について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## ログインし、別のユーザーとしてアクションを実行する

1. Workfront 管理者またはグループ管理者としてWorkfront にログインします。

   >[!NOTE]
   >
   >* グループ管理者は、管理するグループのユーザーとしてのみログインできます。また、ユーザー管理（グループユーザー）権限をアクセスレベルで有効にする必要があります。
   >   
   >  ![](assets/group-admin-user.png)
   >   
   >  この設定は、デフォルトで無効になっています。詳しくは、[カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。
   >   
   >* Workfront 管理者のパスワードはリセットできません。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、**設定** ![](assets/gear-icon-settings.png) をクリックします。

1. 左側のパネルで、「**別のユーザーとしてログイン**」をクリックします。

1. 「**別のユーザーとしてログイン**」タブにある&#x200B;**ユーザー**&#x200B;ボックスで、ユーザーの名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。

   ユーザーは、Workfront で定義されたアクセスレベルを持っている必要があります。ログインする権限を持たないユーザーとしては Workfront システムにログインすることはできません。

   >[!NOTE]
   >
   >グループ管理者は、自分が管理するグループのメンバーであるユーザーとしてのみログインできます。Workfront 管理者としてログインすることはできません。

1. 「**ログイン**」をクリックします。

   <!--
   <p> Might come in a future story:</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">click an Access period and then click Request to ask the user for access to log as him or her for the specified period of time. Continue these steps after the user grants access. Specify somewhere here that this is only for the Enterprise package if they decide on that</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Or </p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">If a prompt appears indicating that the user has restricted access to their account, contact the user to request access.</p>
   -->

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">The user can then can grant you "Log in as" access in their user profile. They can also specify an expiration date and time for the access period. </p>
   -->

   <!--
   This triggers an email to let you know that you have access to log in as the user, depending on how your event notifications are enabled. For more information, see <a href="../../../workfront-basics/using-notifications/event-notifications.md" class="MCXref xref">Event notifications</a>.
   </div>
   -->

   別のユーザーとしてログインすると、画面の上部に通知が表示され、これを示します。

1. ユーザーとして必要なアクションを実行し、**ログアウト**&#x200B;します。

## 管理者が別のユーザーとしてログインしている間のアクティビティのトラッキングと監査

Workfront は、管理者が別のユーザーとしてログインしている間に実行される、トラッキングおよび監査アクティビティのメカニズムを提供します。

別のユーザーとしてログインした場合は、システム管理者またはグループ管理者がそのユーザーとしてログインした日付に最後ログイン日が変更されます。

* [項目の指標を表示](#view-indicators-on-items)
* [監査情報の表示](#view-audit-information)

### 項目の指標を表示 {#view-indicators-on-items}

別のユーザーとして Workfront にログインしてアクションを実行すると、Workfront ではログインしているユーザーの代理としてアクションを実行したことが明示されます。

例えば、別のユーザーとしてログインした項目に対してコメントを作成した場合、そのユーザーの代わりに自分がコメントを作成したことを示すステートメントが表示されます。

### 監査情報の表示 {#view-audit-information}

1. Workfront 管理者またはグループ管理者として Workfront にログインします。
1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、**設定** ![](assets/gear-icon-settings.png) の順にクリックします。

1. 「**別のユーザーとしてログイン**」、「**アクセスログ**」タブの順にクリックします。

   システム管理者またはグループ管理者が別のユーザーとして Workfront にログインするたびに、そのイベントは監査証跡に記録されます。また、管理者が別のユーザーとしてログインしている間に行われた監査可能なアクションは、監査証跡に記録されます。

1. （オプション）監査証跡に表示される結果は、次の方法でフィルタリングできます。

   * ログインしたユーザー別
   * 次のユーザーとしてログインしたユーザー別
   * 日付別
