---
content-type: overview
navigation-topic: notifications
title: イベント通知
description: イベント通知は、プロジェクト、タスク、イシューなどのオブジェクトに関する様々なタイプのイベントによってトリガーされる電子メールです。 他のユーザーが知っておく必要のあるプロジェクトで何かが発生したときに送信されます。 イベントに応じて、ユーザーは即座に、毎日、またはその旨の即時および毎日の電子メール通知を受け取ります。
author: Lisa
feature: Get Started with Workfront
exl-id: 09b70427-691d-437a-b9d2-86f78bd4d6a2
source-git-commit: f3ba39e02d690dd3a0d50ecdb22af0c12a3d4ffb
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# イベント通知

イベント通知は、プロジェクト、タスク、イシューなどのオブジェクトに関する様々なタイプのイベントによってトリガーされる電子メールです。 他のユーザーが知っておく必要のあるプロジェクトで何かが発生したときに送信されます。 イベントに応じて、ユーザーは即座に、毎日、またはその旨の即時および毎日の電子メール通知を受け取ります。

>[!NOTE]
>
>イベント通知は、次のいずれかのタイプです。 [!DNL Adobe Workfront] 通知。 以下に関する情報： [!DNL Workfront] 通知のタイプ： [[!DNL Adobe Workfront] 通知](../../workfront-basics/using-notifications/wf-notifications.md).

## イベント通知の設定

イベント通知 E メールは、以下に示すレベルで設定できます。 イベント通知の設定は、イベント通知のアクティブ化と非アクティブ化で構成されます。

* **システムレベル**:A [!DNL Workfront] 管理者は、イベント通知をシステムレベルでアクティブ化および非アクティブ化できます。詳しくは、 [システムの全員に対するイベント通知を設定する](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

   すべてのグループはデフォルトでシステム通知を継承しますが、グループ管理者は、 [!DNL Workfront] 管理者（下記の次の箇条書き項目で説明）

* **グループレベル**:グループ管理者は、 [!DNL Workfront] 管理者は、グループのこの機能をロック解除します。 管理するグループの上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。 同じことが～にも当てはまる [!DNL Workfront] 管理者（すべてのグループ）。 詳しくは、 [グループのイベント通知を表示および設定する](../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

   >[!NOTE]
   >
   >この機能は、最初は、段階的な展開の一環として、クラスター 4 のお客様のみが使用できます。 その後すぐに、他のクラスターで使用できるようになります。 この記事は、この場合に更新されます。

* **ユーザーレベル**:システム全体でアクティブ化されるすべてのイベント通知は、各ユーザーの [!UICONTROL 通知] 個々のプロファイルに関する節。 ユーザーは、ここで個々のイベント通知をアクティブ化および非アクティブ化できます。

   [!DNL Workfront] 他のユーザーを編集するアクセス権を持つ管理者やユーザーは、個々のユーザーのプロファイルで通知をアクティブ化または非アクティブ化することもできます。

   詳しくは、 [独自のイベント通知をアクティブ化または非アクティブ化する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

   >[!NOTE]
   >
   >ユーザーレベルの通知には、 [!DNL Workfront Goals] 通知。 ただし、 [!DNL Workfront] 管理者またはグループ管理者は、 [!DNL Workfront Goals]. 各ユーザーは、独自に設定する必要があります [!DNL Workfront Goals] 通知を含めることをお勧めします。 ユーザーを編集するアクセス権がある場合は、これらの通知を他のユーザーに変更することもできます。 有効にする場合 [!DNL Workfront Goals] 自分のプロファイルや、編集にアクセスできる他のユーザーに関する通知： [通知：目標](../../workfront-basics/using-notifications/notifications-goals.md).

   通知の詳細については、 [!DNL Workfront] 管理者が設定できます。詳しくは、 [システムの全員に対するイベント通知を設定する](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md). [!DNL Workfront Goals] は、新しい [!DNL Adobe Workfront] エクスペリエンス。

## イベント通知の内容

イベント通知 E メールには、発生したイベントに関する情報と、 [!DNL Workfront] ここで、システム内のイベントを確認できます。 電子メール通知の受信について詳しくは、 [[!DNL Adobe Workfront] 通知](../../workfront-basics/using-notifications/wf-notifications.md).

A [!DNL Workfront] 管理者は、電子メール通知の内容を変更できません。電子メール通知の内容は、 [!DNL Workfront]. ただし、イベント通知 E メールの件名行は変更できます。 詳しくは、 [イベント通知の電子メールの件名をカスタマイズする](../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md).

リストの場合、 [!DNL Workfront] イベント通知と各イベントの簡単な説明、およびデフォルトでアクティブか非アクティブかを確認するには、 [イベント通知はで使用可能 [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).
