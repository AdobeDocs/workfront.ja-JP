---
title: 別のユーザーとしてログイン
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Adobe Workfront の管理者は、別のユーザーの代わりに Workfront にアクセスする必要が生じる場合があります。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 2f8dd132-1086-4980-9b56-993a68231e96
source-git-commit: 6068c9c53568d3ebec9fae294bfee1cbd365714b
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 56%

---

# 別のユーザーとしてのログイン

<!--Audited: 5/2025-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all users only in the Preview environment.</span> -->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. Also linked to other articles: Creating and Managing Groups, etc.</p>
-->

Adobe Workfront管理者は、別のユーザーに代わってWorkfrontにアクセスする必要が生じる場合があります。 また、グループ管理者は、管理対象のグループのメンバーであるユーザーに代わって Workfront にアクセスする必要が生じる場合があります。

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
>ドキュメント統合について詳しくは、「[&#x200B; ドキュメント統合の設定 &#x200B;](../../../administration-and-setup/configure-integrations/configure-document-integrations.md)」を参照してください。

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
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>新規：標準</p>
   <p>または</p>
   <p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>システム管理者のアクセスレベルを使用すると、任意のユーザーとしてログインできます。</p> <p>「Standard」または「Planner」のアクセスレベルでは、アクセスレベルの Users 設定が「Edit」アクセスに設定され、「Create」と「Fine-tune your settings」セクションの 2 つの User Admin オプションのうち少なくとも 1 つが有効になっている場合、より低いライセンスレベルでユーザーとしてログ <img src="assets/gear-icon-in-access-levels.png"> ンできます。 </p> 
   <p>メモ：これら 2 つのオプションのうち、ユーザー管理者（グループユーザー）が有効になっている場合、ユーザーがメンバーになっているグループのグループ管理者である必要があります。</p></td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ログインし、別のユーザーとしてアクションを実行する

1. Workfront 管理者またはグループ管理者として Workfront にログインします。

   >[!NOTE]
   >
   >* グループ管理者は、管理するグループのユーザーとしてのみログインできます。また、ユーザー管理（グループユーザー）権限をアクセスレベルで有効にする必要があります。
   >   
   >  ![&#x200B; グループ管理者ユーザー &#x200B;](assets/group-admin-user.png)
   >   
   >  この設定は、デフォルトで無効になっています。詳しくは、[カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。
   >   
   >* Workfront 管理者のパスワードはリセットできません。

{{step-1-to-setup}}

1. 左側のパネルで、「**ログイン名**」をクリックします。

1. **別名でログイン** タブの **名前の入力を開始…** ボックスにユーザーの名前の入力を開始し、ドロップダウンリストに表示される名前をクリックします。


   >[!NOTE]
   >* 選択するユーザーには、Workfrontで定義されたアクセスレベルが必要です。 ログインする権限を持たないユーザーとしては Workfront システムにログインすることはできません。
   >* グループ管理者は、自分が管理するグループのメンバーであるユーザーとしてのみログインできます。Workfront 管理者としてログインすることはできません。

1. 「**ログイン**」をクリックします。 別のユーザーとしてログインすると、これを示す通知が画面の上部に表示されます。

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



1. ユーザーとして必要なアクションを実行したら、画面上部の **ログアウト** をクリックします。

## 管理者が別のユーザーとしてログインしている間のアクティビティのトラッキングと監査

Workfront は、管理者が別のユーザーとしてログインしている間に実行される、トラッキングおよび監査アクティビティのメカニズムを提供します。

別のユーザーとしてログインすると、そのユーザーの最終ログイン日が、システム管理者またはグループ管理者がそのユーザーとしてログインした日付に変更されます。

* [項目の指標を表示](#view-indicators-on-items)
* [監査情報の表示](#view-audit-information)

### 項目の指標を表示 {#view-indicators-on-items}

別のユーザーとして Workfront にログインしてアクションを実行すると、Workfront ではログインしているユーザーの代理としてアクションを実行したことが明示されます。

例えば、別のユーザーとしてログインしている際に項目にコメントを付けると、オブジェクトの「更新」セクションを表示したときに、コメントがユーザーに代わってあなたが行ったことを示すステートメントが表示されます。

### 監査情報の表示 {#view-audit-information}

1. Workfront 管理者またはグループ管理者として Workfront にログインします。
   {{step-1-to-setup}}
   <!--1. Click the **Main Menu** icon ![Main menu icon](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![Gear settings icon](assets/gear-icon-settings.png).-->

1. 左側のパネルで「**別名でログイン**」をクリックし、「**アクセスログ**」タブをクリックします。

   >[!NOTE]
   >
   >システム管理者またはグループ管理者が別のユーザーとして Workfront にログインするたびに、そのイベントは監査証跡に記録されます。また、管理者が別のユーザーとしてログインしている間に行われた監査可能なアクションは、監査証跡に記録されます。

1. （オプション）監査記録に表示される結果は、次の方法でフィルタリングできます。

   * ログインしたユーザー別
   * 次のユーザーとしてログインしたユーザー別
   * 日時別
