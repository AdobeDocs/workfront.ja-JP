---
user-type: administrator
product-area: system-administration;user-management
keywords: ビュー,グループ,イベント,通知,設定,有効にする,無効にする
navigation-topic: create-and-manage-groups
title: グループのイベント通知の表示と設定
description: グループ管理者は、管理対象のグループに対してアクティブ化されているイベント通知を表示できます。また、Adobe Workfront 管理者がイベント通知のロックを解除した場合は、管理対象の最上位グループに対してイベント通知を設定できます。イベント通知の設定は、その設定の有効化と無効化で構成されます。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: a815aeb1-3403-4491-a8ad-7e47c519905c
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 83%

---

# グループのイベント通知を表示および設定

グループ管理者は、管理対象のグループに対してアクティブ化されているイベント通知を表示できます。

また、Adobe Workfront 管理者がイベント通知のロックを解除した場合は、管理対象の最上位グループに対してイベント通知を設定できます。イベント通知の設定は、その設定の有効化と無効化で構成されます。

Workfront 管理者は、任意のグループに対してこの操作を行うこともできます。

グループのイベント通知を設定すると、そのグループまたはそのサブグループの 1 つをホームグループとするユーザーに影響します。ユーザープロファイルには、システム全体でアクティブ化されたイベント通知ではなく、ホームグループに対してアクティブ化されたイベント通知が表示されます。

Workfront 管理者がイベント通知のロックを解除する方法については、[すべてのグループのイベント通知設定のロック解除またはロック](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)を参照してください。

イベントのデフォルトの通知設定については、[イベント通知のタイプ](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)を参照してください。

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
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：プラン</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>グループのグループ管理者またはシステム管理者である必要があります。</td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## グループのイベント通知の表示と設定

>[!TIP]
>
>Workfrontの管理者で、「Email Notifications」ページ（設定/メール/通知）を開いている場合は、以下の操作を行ってから、手順 6.に進みます。削除 **システムイベント通知** リスト上部のボックスに、グループの名前をボックスに入力し始め、表示されたらクリックします。

{{step-1-to-setup}}

1. 左側のパネルで、「**グループ**![&#x200B; グループ &#x200B;](assets/groups-icon.png)」をクリックします。

1. 最上位グループの名前をクリックします。
1. 左側のメニューで、「**イベント通知**」をクリックします。

   表示されるリストの左側の&#x200B;**アクティブ**&#x200B;列に、グループに対してアクティブな（青色）通知であるか、非アクティブな（灰色）通知であるかが示されます。

1. ロック解除されたイベント通知をアクティブ化または非アクティブ化するには、<strong>アクティブ</strong>列でボタンをクリックして、アクティブ化（ <img src="assets/email-notification-enabled-unlocked.png">）／非アクティブ化（ <img src="assets/email-notification-disabled-unlocked.png">）を切り替えます。

   >[!INFO]
   >
   >**例：**&#x200B;以下に示すような、グループに対してロック解除された、上位 2 つのマーケティンググループイベント通知を設定するとします。</p> <p> <img src="assets/configure-group-event-notifications.png">
   >* <strong>アクティブ</strong>列のボタンが灰色で淡色表示されている（ <img src="assets/email-notification-disabled-locked.png">）場合、イベント通知はすべてのユーザーに対して非アクティブ化されており、グループ管理者はこの通知をアクティブ化したり、メールの件名行を編集したりできません。
   >* <strong>アクティブ</strong>列のボタンが灰色で淡色表示ではない（ <img src="assets/email-notification-disabled-unlocked.png">）場合、イベント通知は<strong>すべてのユーザーに対して非アクティブ化されており</strong>、グループ管理者は自分のグループに対して通知をアクティブ化できます。
   >* <strong>アクティブ</strong>列のボタンが青色で淡色表示されている（ <img src="assets/email-notification-enabled-locked.png">）場合、イベント通知はすべてのユーザーに対してアクティブ化されており、グループ管理者は通知を非アクティブ化したり、自分のグループのメールの件名行を編集したりできません。
   >* <strong>アクティブ</strong>列のボタンが青色で淡色表示ではない（ <img src="assets/email-notification-enabled-unlocked.png">）場合、イベント通知は<strong>すべてのユーザーに対してアクティブ化されており</strong>、グループ管理者は自分のグループに対して通知を非アクティブ化できます。

<!--
This step (with substeps) is for functionality from a Sprint 3 2021 story that got put on hold. Also see the PDF on the story for some text earlier in the article that needs to be added. 

1. To customize the email subject line of an event notification,
  1. Click the name of the event notification.
  1. In the <strong>Event Notification</strong> box that displays, in the <strong>Email Subject Line</strong> box, change the text and fields, including custom fields, then click <strong>Update</strong> to save the new subject lines for your emails.
  IMPORTANT: The names of the fields added must match the camel case syntax of our database structure. For more information about how our objects and their fields are named in the Workfront database, see the <a href="../../../wf-api/workfront-api.md" class="MCXref xref">Adobe Workfront API</a>.
  For more information about customizing the email subject line of an event notification, see <a href="../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md" class="MCXref xref">Customize email subjects for event notifications</a>. 
-->

