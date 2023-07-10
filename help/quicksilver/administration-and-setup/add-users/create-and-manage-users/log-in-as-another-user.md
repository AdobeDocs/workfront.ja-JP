---
title: 別のユーザーとしてのログイン
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: Adobe Workfrontの管理者は、別のユーザーの代わりにWorkfrontにアクセスする必要が生じる場合があります。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2f8dd132-1086-4980-9b56-993a68231e96
source-git-commit: 82f42d81970c7572f43519423ec3a8c0889aaff4
workflow-type: tm+mt
source-wordcount: '895'
ht-degree: 1%

---

# 別のユーザーとしてのログイン


<span class="preview">このページで強調表示されている情報は、まだ一般に利用できない機能を示しています。 この機能は、プレビュー環境でのみ、すべてのユーザーが使用できます。</span>
<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. Also linked to other articles: Creating and Managing Groups, etc.</p>
-->

>[!IMPORTANT]
>
>このページで説明する手順は、まだAdobe Admin Consoleにオンボーディングされていない組織にのみ適用されます。 組織がAdobe Admin Consoleにオンボーディングされている場合、このアクションは使用できません。
>
>組織がAdobe Admin Consoleにオンボーディングされているかどうかに応じて異なる手順のリストについては、 [プラットフォームベースの管理上の違い (Adobe Workfront/Adobeビジネスプラットフォーム )](../../../administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).

Adobe Workfrontの管理者は、別のユーザーの代わりにWorkfrontにアクセスする必要が生じる場合があります。

また、グループ管理者は、管理対象のグループのメンバーであるユーザーに代わってWorkfrontにアクセスする必要が生じる場合があります。

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
>ドキュメントの統合は個人用の非公開ファイルに接続できるので、管理者は別のユーザーとしてログインしている間はドキュメントの統合にアクセスできません。
>
>ドキュメントの統合について詳しくは、 [ドキュメント統合の設定](../../../administration-and-setup/configure-integrations/configure-document-integrations.md)

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>システム管理者のアクセスレベルでは、誰でもログインできます。 このレベルのアクセスについて詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>. </p> <p>Planner のアクセス・レベルでは、ライセンス・レベルが低いユーザーとしてログインできます ( <b>ユーザー</b> の設定は、 <b>編集</b> アクセス、 <b>作成</b> そして少なくとも 2 つのうち 1 つは <b>ユーザー管理者</b> 以下で有効になるオプション <b>設定を微調整する</b> <img src="assets/gear-icon-in-access-levels.png">. </p> 
   <p><b>注意</b>:この 2 つのオプションのうち、ユーザー <b>管理者（グループユーザー）</b> が有効になっている場合は、ユーザーがメンバーであるグループのグループ管理者である必要があります。</p> 
   <p>詳しくは、 <b>ユーザー</b> アクセスレベルでの設定については、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## ログインし、別のユーザーとしてアクションを実行する

1. Workfront管理者またはグループ管理者としてWorkfrontにログインします。

   >[!NOTE]
   >
   >* グループ管理者は、管理するグループのユーザーとしてのみログインできます。 また、ユーザー管理（グループユーザー）権限をアクセスレベルで有効にする必要があります。
   >   
   >  ![](assets/group-admin-user.png)
   >   
   >  この設定は、デフォルトでは無効です。 詳しくは、 [カスタムアクセスレベルの作成または変更](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
   >   
   >* Workfront管理者のパスワードはリセットできません。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **ログイン名**.

1. 内 **ユーザー** ～の箱 **ログイン名** 「 」タブで、ユーザーの名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。

   ユーザーは、Workfrontで定義されたアクセスレベルを持っている必要があります。 ログインする権限を持たないユーザーとしてWorkfrontシステムにログインすることはできません。

   >[!NOTE]
   >
   >グループ管理者は、自分が管理するグループのメンバーであるユーザーとしてのみログインできます。 Workfront管理者としてログインすることはできません。

1. クリック **ログインします。**

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Might come in a future story:</p>
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

1. ユーザーとして必要なアクションを実行したら、「 **ログアウトします。**

## 管理者が別のユーザーとしてログインしている間のアクティビティの追跡と監査

Workfrontは、管理者が別のユーザーとしてログインしている間に実行される、追跡および監査アクティビティのメカニズムを提供します。

別のユーザーとしてログインした場合は、システム管理者またはグループ管理者がそのユーザーとしてログインした日付まで、最後のログイン日が変更されます。

* [項目の指標の表示](#view-indicators-on-items)
* [監査情報の表示](#view-audit-information)

### 項目の指標の表示 {#view-indicators-on-items}

別のユーザーとしてWorkfrontにログインし、アクションを実行すると、Workfrontは、ログインしているユーザーに代わって、実行するアクションがおこなわれたことを明確に示します。

例えば、別のユーザーとしてログインした項目に対してコメントを作成した場合、そのユーザーの代わりに自分がコメントを作成したことを示すステートメントが表示されます。

>[!NOTE]
>
><span class="preview">新しいコメントエクスペリエンスを使用する場合、コメントは別のユーザーとしてログインしたユーザーとして追加され、他のユーザーに代わってコメントを追加していることを示すものではありません。
>
>例えば、Workfront管理者が別のユーザーとしてログインした場合、コメントに関連付けられているユーザーはWorkfront管理者になります。 詳しくは、 [新しいコメントエクスペリエンス](../../../product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). </span>


### 監査情報の表示 {#view-audit-information}

1. Workfront管理者またはグループ管理者としてWorkfrontにログインします。
1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **ログイン名、** 次に、 **アクセスログ** タブをクリックします。

   システム管理者またはグループ管理者が別のユーザーとしてWorkfrontにログインすると、そのイベントは監査記録に記録されます。 さらに、管理者が別のユーザーとしてログインしている間に行われた監査可能なアクションは、監査記録に記録されます。

1. （オプション）監査記録に表示される結果は、次の方法でフィルタリングできます。

   * ログインしたユーザー別
   * 次のユーザーとしてログインしたユーザー別
   * 日付別
