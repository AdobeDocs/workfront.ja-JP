---
content-type: overview
navigation-topic: notifications
title: イベント通知
description: イベント通知は、プロジェクト、タスク、イシューなどのオブジェクトに関する様々なタイプのイベントによってトリガーされるメールです。他のユーザーが知っておく必要のあることが何かプロジェクトで発生したときに送信されます。イベントに応じて、ユーザーは即時か1 日に 1 回、またはその両方のメール通知を受け取ります。
author: Courtney
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: c79d030ff2d05487e5f7e3457bf98df591822a80
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 67%

---

# イベント通知

<!-- Audited: 4/2025 -->

イベント通知は、プロジェクト、タスク、イシューなどのオブジェクトに関する様々なタイプのイベントによってトリガーされるメールです。他のユーザーが知っておく必要のあることが何かプロジェクトで発生したときに送信されます。イベントに応じて、ユーザーは即時か1 日に 1 回、またはその両方のメール通知を受け取ります。

>[!NOTE]
>
>イベント通知は、[!DNL Adobe Workfront] 通知のいずれかのタイプです。[!DNL Workfront] のすべての通知タイプについて詳しくは、[&#x200B; 通知の概要 &#x200B;](../../workfront-basics/using-notifications/wf-notifications.md) を参照してください。

## イベント通知の設定

イベント通知メールは、次のレベルで設定できます。

* **システムレベル**：[!DNL Workfront] 管理者は、イベント通知をシステムレベルでアクティベートおよびディアクティベートできます（[システムの全員へのイベント通知の設定](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)を参照）。

  すべてのグループはデフォルトでシステム通知を継承しますが、グループ管理者が許可した場合、グループ [!DNL Workfront] 理者はグループレベルの一部の設定を変更できる場合があります。

* **グループレベル**：グループ管理者は、[!DNL Workfront] 管理者がグループに対してこの機能をアンロックをした後で、管理するグループのイベント通知を設定できます。管理するグループ上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。同じことが [!DNL Workfront] 管理者にも当てはまります（任意のグループ）。詳しくは、[グループのイベント通知の表示および設定](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)を参照してください。

* **ユーザーレベル**：システム全体でアクティベートされているすべてのイベント通知は、各ユーザーのプロファイルの[!UICONTROL 通知]セクションにリストされています。ユーザーは、ここで個々のイベント通知をアクティベートおよびディアクティベートできます。

  管理者 [!DNL Workfront]、他のユーザーを編集するアクセス権を持つユーザーも、個々のユーザーのプロファイルの通知をアクティブ化および非アクティブ化できます。

  詳しくは、[自身のメール通知の変更](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md)を参照してください。

  >[!NOTE]
  >
  >ユーザーレベルの通知には [!DNL Workfront Goals] 通知も含まれます。ただし、[!DNL Workfront] 管理者またはグループ管理者は [!DNL Workfront Goals] の通知を設定することはできません。各ユーザーは、プロファイルで独自の [!DNL Workfront Goals] 通知を設定する必要があります。 ユーザーを編集するアクセス権を持っている場合は、他のユーザーに対してこれらの通知を変更することもできます。 自分のプロファイルまたは編集権限のある他のユーザーに対して [!DNL Workfront Goals] 通知を有効にする方法については、[通知：目標](../../workfront-basics/using-notifications/notifications-goals.md)を参照してください。

  [!DNL Workfront] 管理者が設定できる通知の詳細については、「[&#x200B; システム内の全員のイベント通知の設定 &#x200B;](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md) を参照してください。

## イベント通知の内容

イベント通知メールには、発生したイベントに関する情報と [!DNL Workfront] へのリンクが含まれます。ここでは、システム内のイベントを確認できます。メール通知の受信について詳しくは、「[&#x200B; 通知の概要 &#x200B;](../../workfront-basics/using-notifications/wf-notifications.md)」を参照してください。

[!DNL Workfront] 管理者は、[!DNL Workfront] で設定するメール通知の内容を変更することはできませんが、イベント通知メールの件名を変更できます。 詳しくは、[イベント通知メールの件名のカスタマイズ](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md)を参照してください。

[!DNL Workfront] のすべてのイベント通知のリスト、各イベントの簡単な説明、デフォルトでアクティブか非アクティブかについては、[&#x200B; イベント通知タイプ &#x200B;](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md) を参照してください。
