---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 更新時の他のユーザーへのタグ付け
description: Adobe Workfrontオブジェクトに更新コメントを付けると、プロジェクトのすべてのユーザーが、送信された情報を表示できます。 ただし、プロジェクトに参加していないユーザーがこの情報を表示する方がメリットが得られる場合があります。 これらのユーザーをプロジェクトに含める代わりに、更新時にタグ付けして、ユーザーと共有できます。 タグ付きユーザーは、イベント通知を受け取ります。
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: c4c0d74f-ac50-4fc5-89d6-28f004c25b29
source-git-commit: ba1d8d5a23da7e252e8c182a6bdb1cdd1e304eab
workflow-type: tm+mt
source-wordcount: '773'
ht-degree: 0%

---

# 更新時の他のユーザーへのタグ付け

<!--take "Beta" references out when we remove the beta-->

<!-- Drafted for commenting experience: 

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> 

>[!NOTE]
>
>We are currently redesigning the commenting experience in Adobe Workfront.
>For more information about the new updating experience, see [New commenting experience](../updating-work-items-and-viewing-updates/unified-commenting-experience.md). 
>
>You can access the new design for the following objects:
> * <span class="preview">Issues, when enabling the commenting Beta. </span>
> * Goals
>   The new commenting experience is the default for goals. You must have an additional license to access Workfront Goals. For more information, see [Requirements to uses Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md). 

-->
ユーザーが従わない可能性のあるオブジェクトに注意を向けたい場合は、オブジェクトの更新時にユーザーにタグを付けることができます。
これらのユーザーを割り当てたり、サブスクライブしたりして、オブジェクトに含めるのではなく、更新時にタグ付けしてユーザーと共有することができます。 タグ付きユーザーは、入力した更新に関する通知を受け取ります。

>[!NOTE]
>
>ユーザーが電子メール通知を受け取るには、イベント通知を有効にする必要があります。 管理者は、システム全体またはトップレベルグループに対する通知を有効にできます。 また、ユーザーは、独自のユーザープロファイルで個々のイベント通知を有効または無効にすることもできます。 詳しくは、次を参照してください。
>
>* [システムの全員に対するイベント通知を設定する](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).
>* [グループのイベント通知を表示および設定する](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)
>* [独自のイベント通知をアクティブ化または非アクティブ化する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).
>


更新をWorkfrontオブジェクトに追加する方法について詳しくは、 [作業を更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

>[!NOTE]
>
>イシューをプロジェクトまたはタスクに変換すると、更新内容は新しいプロジェクトまたはタスクにコピーされますが、タグ付けされたユーザーはコピーされません。 会話を続けるには、参加者に再度タグを付ける必要があります。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>問題およびドキュメントの要求以上その他のすべてのオブジェクトを確認するか、それ以上の値を設定します</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>問題およびドキュメントの要求者以上他のすべてのオブジェクトのレビュー担当者以上</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>オブジェクトへのアクセスの表示</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。

## 更新時の他のユーザーへのタグ付け

<!--
Tagging others in an update differs depending on which experience and which object you select.

### Tag others on updates in the current Updates section
-->

1. 作業項目の更新を開始します。詳しくは、 [作業を更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. 内 **通知** フィールドに、含めるユーザーまたはチームの名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。

   または

   @記号を **新しい更新を開始** 「 」領域で、更新に含めるユーザーまたはチームの名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。

   >[!TIP]
   >
   >類似または同一の名前を持つユーザーがいる場合に正しいユーザーを識別するには、アバター、ユーザーのプライマリの役割、またはその電子メールアドレスに注目します。 更新でタグ付けしたユーザーを表示するには、少なくとも 1 つのジョブの役割に関連付ける必要があります。

   ![](assets/tag-users-in-update.png)

1. （オプション）更新を非公開にするには、 **私の会社に対してプライベート** をクリックします。 これにより、会社のユーザーだけが更新を表示できるようになります。

   >[!NOTE]
   >
   >会社外のタグ付きユーザーは、「更新」タブに非公開コメントが表示されなくても、アプリ内通知や電子メールを引き続き受け取ることができます。 情報を共有したくない場合は、更新時に外部ユーザーにタグ付けしないことをお勧めします。

1. （オプション）複数のユーザーおよびチームを追加するには、手順 2 を繰り返します。

   >[!NOTE]
   >
   >「通知」フィールドに一覧表示されるすべてのユーザーとチームメンバーは、更新のアプリ内通知を受け取り、電子メール通知の設定に応じて電子メールを受け取る場合があります。 コメントまたは返信でタグ付けしたユーザーは、そのコメントまたは返信に関する通知を受け取り、スレッドの残りの部分の「通知」フィールドに名前を表示できますが、タグ付けし直さない限り、別の通知を受け取りません。 詳しくは、 [独自のイベント通知をアクティブ化または非アクティブ化する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) および [システムの全員に対するイベント通知を設定する](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. クリック **更新**.\
   更新に含まれるユーザーには、オブジェクトに対する表示権限が自動的に付与され、オブジェクトに対する更新の表示と応答が可能になります。

   更新スレッドの上部で、各返信でタグ付けされたユーザーを確認できます。 これらのユーザーは、オブジェクトを購読しているユーザーと共に、オブジェクトに対して更新または返信がおこなわれるたびに通知を受け取ります。

   ![](assets/tagging-transparency-350x192.png)

   作業項目の更新時に使用できる追加機能について詳しくは、 [作業を更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

<!--
<div class="preview">

### Tag others on updates in the commenting Beta experience

1. Begin updating a work item, as described in [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. In the **Tag people or teams** field, begin typing the name of the user or team you want to include, then click the name when it appears in the drop-down list.

   <!- ********************* this doesn't seem to work in Beta - keep drafted for now: 
   Or

   Type the @ symbol in the **Start a new update** area, begin typing the name of the user or team you want to include on the update, then click the name when it appears in the drop-down list. ************close draft

   >[!TIP]
   >
   >To identify the correct user when there are users with similar or identical names, notice the avatar, the user's Primary Role, or their email address. Users must be associated with at least one job role to view it as you tag them in an update.

   ![](assets/tag-others-unified-commenting.png)

      <!-******************* this might not be there for issues yet - keep drafted if not: 
      1. (Optional) To make the update private, enable **Private to my company** in the lower-right corner of the update box. This makes the update visible just to users in your company.

         >[!NOTE]
         >
         >* This option displays only when the user is associated with a Company.
         >* Tagged users outside the company could still receive an in-app notification or email, even though they will not see the private comments on the Updates tab. We recommend not to tag external users on an update if you do not want to share the information with them. - ************close draft 
      
1. (Optional) To add multiple users and teams, repeat step 2.

   >[!NOTE]
   >
   >All users and team members listed in the "Tag people or teams" field receive an in-app notification for the update and might receive an email, depending on the configuration of their email notification settings. Users who tag themselves in a comment or reply receive a notification for that comment or reply and can see their name in listed as a member of the thread for the remainder of the thread, but they do not receive another notification unless they tag themselves again. For more information, see [Activate or deactivate your own event notifications](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md) and [Configure event notifications for everyone in the system](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

1. Click **Submit**.  
   Users included in the update are automatically granted View permission to the object and can view and respond to updates made to the object.

   You can see who has been tagged in each reply under the text of the update, in the Members area. These users, along with any users subscribed to the object, receive a notification whenever an update or reply is made on the object.
1. (Optional) Cick the number of members included in the update to display a list of entities that the update you entered is shared with. 

   ![](assets/members-icons-expanded-unshimmed.png)

   For information about the additional functionality that is available when updating a work item, see [Update work](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

-->