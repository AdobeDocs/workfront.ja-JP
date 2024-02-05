---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: ' [!DNL Slack] での  [!DNL Adobe Workfront]  通知の受信'
description: ' [!DNL Slack] での  [!DNL Adobe Workfront]  通知の受信'
author: Becky
feature: Workfront Integrations and Apps
exl-id: bc1ce4ea-58be-4cd7-ab59-7dddb82949b9
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '582'
ht-degree: 97%

---

# [!DNL Slack] での [!DNL Adobe Workfront] 通知の受信

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: *** Linked to Accessing Workfront from Slack.***Some of this information is duplicating in Accessing Workfront from Slack (also screen shots))</p>
-->

[!DNL Adobe Workfront for Slack] をインストールすると、[!DNL Slack] で [!DNL Workfront] 通知を受信できるようになります。\
[!DNL Workfront for Slack] のインストールについて詳しくは、[設定 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)を参照してください。

[!DNL Workfront] のインターフェイスで通知バブルに表示される、選択した[!UICONTROL 通知]の数を [!DNL Slack] でも配信できるようにすることができます。

メール通知は、[!DNL Workfront] のインターフェイスでの通知とは独立して機能します。自分または [!DNL Workfront] 管理者はメール通知を無効にできますが、[!DNL Workfront] のインターフェイスでの通知は無効にできません。\
ただし、[!DNL Workfront] のインターフェイスだけに通知をフォーカスする場合は、[!DNL Slack] で受信する可能性のある [!DNL Workfront] 通知を無効にできます。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] プラン]</a>*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、またはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 前提条件

[!DNL Slack] で [!DNL Workfront] 通知を受信する前に、次のことが必要です。

* [!DNL Workfront for Slack] の設定\
   [!DNL Workfront for Slack] の設定の手順については、[設定 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)を参照してください。

## [!DNL Slack] 用に [!DNL Workfront] 通知を設定 {#configure-workfront-notifications-for-slack}

1. （条件付き）[!DNL Slack] インスタンスに [!DNL Workfront] が追加された後、[!DNL Slack] から [!DNL Workfront] にログインします。\
   [!DNL Slack] から [!DNL Workfront] へのログインについて詳しくは、[ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) から  [!DNL Adobe Workfront]  へのアクセスを参照してください。

1. 任意のチャネルから、メッセージフィールドに次のいずれかのコマンドを入力します。

   `/workfront settings`

   または

   `/wf settings`

1. デフォルトでは、すべての通知が有効になっています。\
   次のいずれかの通知を無効にします。

   * [!UICONTROL 自分に新しいタスクまたはイシューに割り当てられている]
   * [!UICONTROL チームに新しいタスクまたはイシューが割り当てられている]
   * [!UICONTROL 新しい承認またはアクセスリクエストを受け取る]
   * [!UICONTROL 自分が更新を受信する対象者として追加された]
   * [!UICONTROL 自分が参加中のスレッドに対して誰かがコメントした]
   * [!UICONTROL 購読しているタスク、イシュー、またはプロジェクトが更新された]
   * [!UICONTROL 誰かが自分の作業アイテムのいずれかに対してコメントした]
   * [!UICONTROL 誰かが自分のヘルプリクエストにコメントを投稿した]

   [!UICONTROL 通知]オプションに加えた変更はすぐに有効になります。\
   有効にした通知は、[!DNL Workfront] の [!DNL Slack] チャネルに表示されます。ここで通知を無効にすると、[!DNL Slack] の通知のみが無効になり、[!DNL Workfront] インターフェイスでは無効になりません。引き続き、インターフェイスの右上に [!DNL Workfront] 通知バブルとして表示されます。

## [!DNL Slack] からの [!DNL Workfront] 通知を管理

[!DNL Slack] から [!DNL Workfront] 通知を受信したり応答したりできます。

[!DNL Slack] で有効にした通知用のメール通知を無効にすることで、通知を重複して受け取らないようにすることができます。\
電子メール通知の設定について詳しくは、 [独自の電子メール通知を変更する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

[!DNL Slack] で [!DNL Workfront] 通知を有効または無効にしても、[!DNL Workfront] インターフェイス内で受信する通知に影響はありません。\
[!DNL Workfront] 内部の通知インターフェイスを無効にすることはできません。

[!DNL Slack] 用の [!DNL Workfront] 通知を管理するには：

1. [!UICONTROL Slack] にログインします。
1. [!DNL Slack] から [!DNL Workfront] にログインします。\
   [!DNL Slack] から [!DNL Workfront] へのログインについて詳しくは、[ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) から  [!DNL Adobe Workfront]  にアクセスの「[!DNL Slack] から [!DNL Workfront] へのログイン」節を参照してください。

1. [!DNL Slack] 用の [!DNL Workfront] 通知が有効になっていることを確認します。\
   どの [!DNL Workfront] 通知を [!DNL Slack] にも通知されるように設定できるかについて詳しくは、[ [!DNL Slack]](#configure-workfront-notifications-for-slack-configure-workfront-notifications-for-slack) 用の  [!DNL Workfront]  設定を参照してください。

1. **[!DNL Workfront]** チャネルにアクセスして [!DNL Workfront] 通知を検索します。
1. （条件付きおよびオプション）次のいずれかの操作を行います。

   * **[!UICONTROL 作業する]**&#x200B;をクリックして、タスクの作業を承認します。

   * （条件付きおよびオプション）コメントに返信するには「**[!UICONTROL [!DNL Workfront]]** で返信」をクリックし、返信内容を入力して「**[!UICONTROL 返信]**」をクリックします。

   * （条件付きおよびオプション）「**[!UICONTROL 承認]**」または「**[!UICONTROL 却下]**」をクリックして、承認待ちのタスク、イシューまたはプロジェクトを承認または却下します。

   * （条件付きおよびオプション）「**[!UICONTROL 承認]**」「**[!UICONTROL 変更]**」または「**[!UICONTROL 却下]**」をクリックして、承認、変更を加えて承認、またはドキュメントを拒否する場合は却下します。

     ドキュメントを承認する前に、ドキュメントのサムネイルの上にマウスを移動し、虫眼鏡アイコンをクリックして、ドキュメントの大きなプレビューを表示することもできます。\
      承認された Slack [ファイルタイプ](https://api.slack.com/types/file)のみプレビューできます。

   * （条件付きおよびオプション）「**[!UICONTROL 付与]**」または「**[!UICONTROL 無視]**」をクリックすると、他のユーザーからの追加アクセス要求を許可または無視します。

     通知内で決定するたびに、[!DNL Workfront] でアクションが完了したことを示す確認メッセージを受信します。
