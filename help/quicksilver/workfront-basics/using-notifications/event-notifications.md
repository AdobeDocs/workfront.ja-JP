---
content-type: overview
navigation-topic: notifications
title: イベント通知
description: イベント通知は、プロジェクト、タスク、イシューなどのオブジェクトに関する様々なタイプのイベントによってトリガーされるメールです。他のユーザーが知っておく必要のあることが何かプロジェクトで発生したときに送信されます。イベントに応じて、ユーザーは即時か1 日に 1 回、またはその両方のメール通知を受け取ります。
author: Lisa
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '554'
ht-degree: 98%

---

# イベント通知

イベント通知は、プロジェクト、タスク、イシューなどのオブジェクトに関する様々なタイプのイベントによってトリガーされるメールです。他のユーザーが知っておく必要のあることが何かプロジェクトで発生したときに送信されます。イベントに応じて、ユーザーは即時か1 日に 1 回、またはその両方のメール通知を受け取ります。

>[!NOTE]
>
>イベント通知は、[!DNL Adobe Workfront] 通知のいずれかのタイプです。すべての [!DNL Workfront] 通知タイプに関する情報については、[[!DNL Adobe Workfront] 通知](../../workfront-basics/using-notifications/wf-notifications.md)を参照してください。

## イベント通知の設定

イベント通知メールは、以下に示すレベルで設定できます。イベント通知の設定は、その設定の有効化と無効化で構成されます。

* **システムレベル**：[!DNL Workfront] 管理者は、イベント通知をシステムレベルでアクティベートおよびディアクティベートできます（[システムの全員へのイベント通知の設定](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)を参照）。

  すべてのグループはデフォルトでシステム通知を継承しますが、[!DNL Workfront] 管理者が許可した場合、グループ管理者はグループレベルで一部の設定を変更できる場合があります（以下の箇条書きを参照）。

* **グループレベル**：グループ管理者は、[!DNL Workfront] 管理者がグループに対してこの機能をアンロックをした後で、管理するグループのイベント通知を設定できます。管理するグループ上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。同じことが [!DNL Workfront] 管理者にも当てはまります（任意のグループ）。詳しくは、[グループのイベント通知の表示および設定](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)を参照してください。

  >[!NOTE]
  >
  >この機能は、段階的な展開の一環として、まずクラスター 4 のお客様のみが使用できます。その後すぐに、他のクラスターでも使用できるようになります。この記事は、その時点で更新されます。

* **ユーザーレベル**：システム全体でアクティベートされているすべてのイベント通知は、各ユーザーのプロファイルの[!UICONTROL 通知]セクションにリストされています。ユーザーは、ここで個々のイベント通知をアクティベートおよびディアクティベートできます。

  他のユーザーを編集するアクセス権を持つ [!DNL Workfront] 管理者やユーザーは、個々のユーザーのプロファイルで通知をアクティベートまたはディアクティベートすることもできます。

  詳しくは、 [独自の電子メール通知を変更する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

  >[!NOTE]
  >
  >ユーザーレベルの通知には [!DNL Workfront Goals] 通知も含まれます。ただし、[!DNL Workfront] 管理者またはグループ管理者は [!DNL Workfront Goals] の通知を設定することはできません。各ユーザーは、プロファイルで独自の [!DNL Workfront Goals] 通知を設定する必要があります。 他のユーザーを編集するアクセス権があるユーザーは、これらの通知を他のユーザーのために変更することもできます。自分のプロファイルまたは編集権限のある他のユーザーに対して [!DNL Workfront Goals] 通知を有効にする方法については、[通知：目標](../../workfront-basics/using-notifications/notifications-goals.md)を参照してください。

  [!DNL Workfront] 管理者が設定できる通知の詳細については、[システムの全員に対するイベント通知の設定](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)を参照してください。[!DNL Workfront Goals] は、新しい [!DNL Adobe Workfront] エクスペリエンスでのみ使用できます。

## イベント通知の内容

イベント通知メールには、発生したイベントに関する情報と [!DNL Workfront] へのリンクが含まれます。ここでは、システム内のイベントを確認できます。メール通知の受信について詳しくは、[[!DNL Adobe Workfront] 通知](../../workfront-basics/using-notifications/wf-notifications.md)を参照してください。

メール通知の内容は [!DNL Workfront] で設定されているため、[!DNL Workfront] 管理者が変更することはできません。ただし、イベント通知メールの件名行は変更できます。 詳しくは、[イベント通知メールの件名のカスタマイズ](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md)を参照してください。

すべての [!DNL Workfront] イベント通知のリストと各イベントの簡単な説明、デフォルトでアクティブか非アクティブかについては、「[ [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md) で使用可能なイベント通知」を参照してください。
