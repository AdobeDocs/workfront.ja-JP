---
title: システムの全員へのイベント通知を設定
description: イベント通知は、特定のイベントが発生したときにユーザーにメールを送信します。Adobe Workfront 管理者またはプランナーのアクセスレベルを持つユーザーは、システム内のすべてのユーザーに対するイベント通知を設定できます。イベント通知の設定は、その設定の有効化と無効化で構成されます。
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 027ecebd-d9de-4cdd-b15a-88de18367591
source-git-commit: 1c0a656f2603c5decabd2bb4e88da1b9530f9e1c
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 85%

---

# システムの全員へのイベント通知を設定

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS-->

イベント通知は、特定のイベントが発生したときにユーザーにメールを送信します。Adobe Workfront 管理者またはプランナーのアクセスレベルを持つユーザーは、システム内のすべてのユーザーに対するイベント通知を設定できます。イベント通知の設定は、その設定の有効化と無効化で構成されます。

<!--Alina annotation on the word "all" in 2nd sentence: abive, drafted and remains QS only-->

管理者が有効にし、ユーザーが自分のプロファイルでも有効にしているイベントについては、イベントが発生すると、即時、日次、または即時と日次の両方でメール通知がユーザーに送信されます。

まず、すべてのユーザーに届けたい通知を、Workfront インスタンスの設定エリアで指定する必要があります。設定エリアで通知を有効にすると、有効になった通知が各ユーザーのプロファイルページに表示されます。

通知が設定エリアで有効化され、ユーザーのプロファイルページに表示されると、それぞれのユーザーまたは Paln ライセンスのある別のユーザーは、有効化された通知をユーザープロファイルで設定することにより、特定のユーザーが受け取る通知とその通知頻度を制御することができます。詳しくは、 [独自の電子メール通知を変更する](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

アクティブ化および非アクティブ化できるすべてのイベント通知の一覧については、 [イベント通知タイプ](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

グループ管理者が自分のグループに対してイベント通知を設定できるように、イベント通知のロックを解除する方法について詳しくは、[すべてのグループに対するイベント通知の設定をロックまたはロック解除](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)と[グループのイベント通知の表示と設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)を参照してください。

## アクセス要件

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
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> <p>新規：標準</p>
 <p>または</p> 
<p>現在：プラン</p> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>リマインダー通知への管理アクセス権を持つ、プランナー以上の権限</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## すべてのユーザーへのイベント通知の設定

ユーザーが個々のプロファイルで通知を有効または無効にする前に、Workfrontの「セットアップ」領域で通知を有効にする必要があります。

>[!TIP]
>
>設定エリアで Workfront Goals の通知を有効にすることはできません。ユーザーは、自分のプロファイルでのみ、これらの通知をアクティブ化できます。Plan ライセンスを持つユーザーは、他のユーザーに対して通知をアクティブ化することができます。ユーザーへの Workfront Goals の通知の有効化について詳しくは、[通知：Goals](../../../workfront-basics/using-notifications/notifications-goals.md) を参照してください。

{{step-1-to-setup}}

1. **メール**／**通知**&#x200B;をクリックします。

   ![](assets/notifications-area-under-setup-emails.png)


1. 「**イベント通知**」タブが開くことを確認します。
1. イベント名の左側にあるスイッチをオンまたはオフに切り替えます。

   イベントのデフォルトの通知ステータスを確認するには、[イベント通知](../../../workfront-basics/using-notifications/event-notifications.md)を参照してください。

1. （オプション）イベント通知の名前をクリックすると、メール通知の件名行をカスタマイズできます。

   メール通知の件名行のカスタマイズについて詳しくは、[イベント通知のメール件名をカスタマイズする](../../../administration-and-setup/manage-workfront/emails/custom-email-subjects-event-notification.md)を参照してください。

1. （オプション）メール通知設定のロックを解除して、グループ管理者がグループごとに個別にメール通知を設定できるようにするには、通知の右側にあるボタン ![](assets/lock-toggle-button.png) をクリックしてロック解除位置 ![](assets/unlock-toggle-button.png) に切り替えます。

   >[!NOTE]
   >
   >この機能は、段階的な展開の一環として、まずクラスター 4 のお客様のみが使用できます。その後すぐに、他のクラスターでも使用できるようになります。この記事は、その時点で更新されます。

   詳しくは、[すべてのグループに対するイベント通知の設定をロックまたはロック解除](../../../administration-and-setup/manage-workfront/emails/unlock-configuration-of-event-notifications-for-groups.md)を参照してください。
