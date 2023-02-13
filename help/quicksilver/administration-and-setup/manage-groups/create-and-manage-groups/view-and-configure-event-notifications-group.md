---
user-type: administrator
product-area: system-administration;user-management
keywords: 表示，グループ，イベント，通知，設定，有効，無効
navigation-topic: create-and-manage-groups
title: グループのイベント通知を表示および設定する
description: グループ管理者は、管理しているグループに対して有効化されているイベント通知を表示できます。 また、Adobe Workfrontの管理者がイベント通知のロックを解除した場合、管理対象の最上位グループに対して設定できます。 イベント通知の設定は、イベント通知のアクティブ化と非アクティブ化で構成されます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a815aeb1-3403-4491-a8ad-7e47c519905c
source-git-commit: 306d6493ff0413d5814f4aed8ab44fb897f3568d
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 0%

---

# グループのイベント通知を表示および設定する

グループ管理者は、管理しているグループに対して有効化されているイベント通知を表示できます。

また、Adobe Workfrontの管理者がイベント通知のロックを解除した場合、管理対象の最上位グループに対して設定できます。 イベント通知の設定は、イベント通知のアクティブ化と非アクティブ化で構成されます。

Workfrontの管理者は、任意のグループに対してこの操作を実行することもできます。

グループのイベント通知を設定すると、そのグループのユーザー（またはそのサブグループの 1 つ）がホームグループに影響を与えます。 ユーザープロファイルには、システム全体でアクティブ化されたイベント通知の代わりに、ホームグループに対してアクティブ化されたイベント通知が表示されます。

Workfront管理者がイベント通知のロックを解除する方法について詳しくは、 [すべてのグループのイベント通知の設定をロック解除またはロックします](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md).

イベントのデフォルトの通知設定について詳しくは、 [Adobe Workfrontで使用可能なイベント通知](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Workfrontプラン</a>*</td> 
   <td> <p>Pro 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="https://one.workfront.com/s/document-item?bundleId=the-new-workfront-experience&amp;topicId=Content%2FAdministration_and_Setup%2FAdd_users%2FAccess_levels_and_object_permissions%2Fwf-licenses.html&amp;_LANG=en" target="_blank">Adobe Workfrontライセンス</a>*</td> 
   <td> <p>計画 </p> <p>グループのグループ管理者またはWorkfront管理者である必要があります。 詳しくは、 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a> および <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランまたはライセンスの種類を確認する必要がある場合は、Workfront管理者にお問い合わせください。

## グループのイベント通知の表示と設定

1. （条件付きおよびオプション）Workfrontの管理者で、既に電子メール通知ページ（設定/電子メール/通知）にいる場合は、次の操作を実行してから、手順 6 にスキップできます。削除 **システムイベント通知** リストの上のボックスで、ボックスにグループの名前を入力し、表示されたらクリックします。
1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **グループ** ![](assets/groups-icon.png).

1. 最上位グループの名前をクリックします。
1. 左側のメニューで、 **イベント通知**.

   表示されるリストで、 **アクティブ** 左側の列には、グループに対してアクティブ（青）と非アクティブ（灰色）の通知が表示されます。

1. ロック解除されたイベント通知を有効または無効にするには：「 <strong>アクティブ</strong> 有効化する列 <img src="assets/email-notification-enabled-unlocked.png"> または無効化 <img src="assets/email-notification-disabled-unlocked.png"> それは。

   >[!INFO]
   >
   >**例：** 以下に示す、グループのロックが解除された、上位 2 つのマーケティンググループイベント通知を設定できます。</p> <p> <img src="assets/configure-group-event-notifications.png">
   >* ボタンが <strong>アクティブ</strong> 列が灰色で淡色表示になります <img src="assets/email-notification-disabled-locked.png">の場合、すべてのユーザーおよびグループ管理者に対するイベント通知は無効化されます。この通知を有効化したり、電子メールの件名行を編集したりすることはできません。
   >* ボタンが <strong>アクティブ</strong> 列が灰色で淡色表示になっていない <img src="assets/email-notification-disabled-unlocked.png">の場合、イベント通知は <strong>すべてのユーザーで非アクティブ、</strong> グループ管理者は、自分のグループに対してこの機能をアクティブ化できます。
   >* ボタンが <strong>アクティブ</strong> 列が青色で淡色表示になります <img src="assets/email-notification-enabled-locked.png">の場合、すべてのユーザーおよびグループ管理者に対して、イベント通知がアクティブ化されます。非アクティブ化したり、自分のグループの電子メールの件名行を編集したりすることはできません。
   >* ボタンが <strong>アクティブ</strong> 列が青で淡色表示になっていません <img src="assets/email-notification-enabled-unlocked.png">の場合、イベント通知は <strong>すべてのユーザーに対して有効化され、</strong> グループ管理者は、自分のグループに対してこの権限を無効にすることができます。


<!--
This step (with substeps) is for functionality from a Sprint 3 2021 story that got put on hold. Also see the PDF on the story for some text earlier in the article that needs to be added. 

1. To customize the email subject line of an event notification,
  1. Click the name of the event notification.
  1. In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.
  IMPORTANT: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.
  For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. 
-->

