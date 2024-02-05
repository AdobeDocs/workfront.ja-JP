---
content-type: overview;reference
navigation-topic: notifications
title: 通知の概要
description: Adobe Workfront は、モバイルデバイスでメール通知、アプリ内通知、および通知を送信します。
author: Lisa
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
source-git-commit: 6d2144732e5f47b670c2281d042a2dc950a2928f
workflow-type: tm+mt
source-wordcount: '1395'
ht-degree: 76%

---

# 通知の概要

<!--Audited: 12/2023-->

[!DNL Adobe Workfront] は、モバイルデバイスでメール通知、アプリ内通知、および通知を送信します。

## メール通知

[!DNL Workfront] は、Workfrontのアクティビティに関するユーザーに警告を出す電子メール通知を送信し、役に立つ情報やリンクを提供します。

電子メール通知の環境設定を変更するには、 [独自の電子メール通知を変更する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>サンドボックス環境からメール通知を受け取る場合は、その環境のユーザープロファイルからメールを有効にする必要があります。

[!DNL Workfront] から次のメール通知を受信することができます。

* [イベント通知](#event-notifications)
* [日次ダイジェスト通知](#daily-digest-notifications)
* [投稿されたコメントの通知](#notification-of-posted-comments)
* [自動リマインダ](#automatic-reminders)
* [リマインダー通知](#reminder-notifications)
* [ボード通知](#boards-notifications)
* [その他の  [!DNL Workfront]  メール](#other-workfront-emails)

### イベント通知

イベント通知は、通常、タスクを割り当てたり、自分がコメントに対して返信を受け取ったりするなど、事前定義された特定のイベントによってトリガーされます。

イベント通知が [!DNL Workfront] お客様のシステム [!DNL Workfront] 管理者またはグループ管理者は、 [!UICONTROL 通知] 環境設定がユーザープロファイルに表示されます。 また、イベントが発生したときに通知を受信するか、1 日の日次ダイジェストメールに要約されたイベントを受信するかを選択できます。

設定では、 [!DNL Workfront] 管理者がお客様に対するイベント通知を設定しました [!DNL Workfront] システム。 詳しくは、[システムの全員に対するイベント通知の設定](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)を参照してください。

デフォルトのステータスは、新しいユーザーを作成する際に、新しいユーザーに対してどの通知（日次、即時、または両方）がデフォルトで有効になっているかを示します。

イベント通知の完全なリスト、およびシステムレベル、グループレベル、ユーザーレベルでのイベント通知の有効化と設定方法について詳しくは、[ [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md) で使用可能なイベント通知を参照してください。

受信するイベント通知の選択方法について詳しくは、 [独自の電子メール通知を変更する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>イベント通知は、日次ダイジェスト更新で配信されるように設定できる唯一の通知です。

### 日次ダイジェスト通知

日別のダイジェスト通知は、電子メールの 24 時間前に受け取った特定のタイプの通知をすべて含む電子メールです。

日次ダイジェストメール配信で有効にされたメール通知の完全なリストと、メール通知のすべてのカテゴリに関する情報については、[イベント通知](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications)を参照してください。

>[!NOTE]
>
>[!UICONTROL Workfront] は、[!UICONTROL その他]および [!DNL Goals] カテゴリのイベントについては日次ダイジェスト通知を送信しません。これらのカテゴリの日次通知を無効にすることはできません。

日次ダイジェスト通知を受信する際に注意すべき点がいくつかあります。

* 「**[!UICONTROL 個人設定]**」パネルの各「[!UICONTROL 通知]」セクションでは、独自の日次ダイジェストメールが生成されます。日次ダイジェストメールに対して有効になっている通知設定と同数の日次ダイジェストメールを毎日送信できます。\
   例えば、**[!UICONTROL 所有プロジェクトに関する情報]**&#x200B;で、いくつかのアクションに関する日次ダイジェストメールを受信することを選択した場合、このエリアで発生したすべてのイベントをリストした 1 通のメール通知を受信します。

* 日次ダイジェストメールに含まれる通知は、様々な条件でグループ化されます。例えば、**[!UICONTROL 所有プロジェクトに関する情報]**&#x200B;の場合、イベントはプロジェクト名でグループ化されます。

  **[!UICONTROL コミュニケーション]**&#x200B;のカテゴリでは、通知は通信が発生したオブジェクト別にグループ化されます。

  >[!NOTE]
  >
  >「通信」カテゴリでは、インスタント配信の場合にのみ個々の通知を選択できます。 日刊ダイジェストで通知を配信するには、すべてを選択する必要があります。

* 日次ダイジェストメールには、配信対象として選択された時間の 24 時間前以内に、特定の 1 つのエリア（**所有プロジェクトに関する情報**&#x200B;など）のアクションに関して発生したイベントが一覧表示されます。
* 日次ダイジェスト配信で選択された時間のタイムゾーンは、ブラウザーで設定されているタイムゾーンと一致します。
* 日次ダイジェストメールには、件名行のセクションの名前と、配信日が含まれます。
* 日次ダイジェストを配信するには、少なくとも 1 つのイベントに通知をトリガーする必要があります。日次ダイジェストメールに対してマークされたイベントが満たされない場合、日次ダイジェストは送信されません。

### 投稿されたコメントの通知

[!UICONTROL コミュニケーション]のカテゴリの通知は、特定の項目の[!UICONTROL 更新]ストリームに投稿されたコメントを警告します。

[!UICONTROL コミュニケーション]のカテゴリの日次ダイジェストメールが、利用可能なすべての通知に対して選択されます。

情報は通信が発生したオブジェクトについて要約され、オブジェクトごとに通信メッセージの総数が表示されます。

Workfrontでコメントに返信または表示するには：

1. 次をクリック： **[!UICONTROL コメント]** 」ボタンをクリックします。

   The [!UICONTROL 更新] オブジェクトの領域が開き、特定のコメントが青で表示されます。

   返信ボックスが開き、コメントに返信できます。

毎日のダイジェスト通知の有効化を含め、電子メール通知の設定について詳しくは、 [電子メール通知設定を表示および変更する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view-and-modify-your-email-notification-settings) in [独自の電子メール通知を変更する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### 自動リマインダ

自動リマインダーは、[!DNL Workfront] 管理者によって、予定完了日の期限が迫っている、期限に遅れている、または予定完了日に近いタスクやイシューを警告することができます。遅延通知の場合、メールはタスクまたはイシューが完了するまで毎晩送信されます。管理者がこれらを設定した後で、無効にすることはできません。また、自動リマインダーによってトリガーされるメールの内容や件名を変更することはできません。

自動リマインダーは、次のいずれか、または複数の相手に送信できます。

* タスクまたはイシューに割り当てられているユーザー
* ユーザーの直属のマネージャー
* 直属のマネージャーを管理するマネージャー

自動リマインダーのメールは、[!DNL Workfront] 管理者が送信メールを処理するように選択したメールアドレスから送信されます。

どの自動リマインダーが有効になっているかに応じて、次の種類の情報を自動リマインダーメールで利用できます。

* タスクまたはイシューが作成された日付
* タスク名またはイシュー名
* タスクまたはイシューが存在するプロジェクトの名前
* タスクまたはイシューの説明
* タスクまたはイシューに割り当てられたユーザーのリスト
* タスクまたはイシューを入力したユーザーの名前
* タスクまたはイシューの優先度
* タスクまたはイシューが期限切れになった日付

自動リマインダーの有効化について詳しくは、[自動リマインダーの設定](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md)を参照してください。

### リマインダー通知

A [!DNL Workfront] 管理者 ( または [!UICONTROL プランナー] アクセスレベルと管理アクセス（リマインダー通知へのアクセス）は、近づく期限に関するリマインダー通知を設計し、プロジェクト、タスク、問題、およびタイムシートに手動で関連付けることができます。

>[!IMPORTANT]
>
>上記のいずれかのオブジェクトに関するリマインダー通知をユーザーが受け取った後に期限が変更された場合、ユーザーは他のリマインダー通知を受け取りません。

リマインダー通知は、[!DNL Workfront] 管理者が送信メールを処理するように選択したメールアドレスから送信されます。

リマインダー通知の設定と有効化について詳しくは、[リマインダー通知の設定](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md)を参照してください。

必要な管理アクセス権を取得する方法について詳しくは、 [特定の領域に対する管理者アクセス権をユーザーに付与する](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

### ボード通知

[!DNL Adobe Workfront] [!UICONTROL ボード]は、ボードに追加されたときや、カードが割り当てられたときにメールを送信します。ボードの環境設定で受信する電子メールを選択できます。

詳しくは、[ボードのメール通知と環境設定](/help/quicksilver/agile/get-started-with-boards/boards-emails.md)を参照してください。

### その他の [!DNL Workfront] メール

他にもメールが届いている可能性があります [!DNL Workfront] 設定できない

次のメールは、これらの条件が満たされた場合、[!DNL Workfront] によって自動的に送信されます。

* 項目を復元：[!DNL Workfront] 管理者は、ごみ箱からオブジェクトを復元する際に、メールが [!DNL Workfront] 管理者に送信されます。
* 復元に失敗：[!DNL Workfront] 管理者がごみ箱からオブジェクトを復元しようとして、復元に失敗した場合、メールが [!DNL Workfront] 管理者に送信されます。

次のメールは、ユーザープロファイルレベルでのみ設定できます。システムレベルで有効または無効にすることはできません。

* 個人タスクの完了：他のユーザーに割り当てた個人タスクが完了すると、メールが送信されます。
* ユーザーに追加されたコメント：ユーザープロファイルに対して誰かがコメントすると、メールが送信されます。

## アプリ内通知

特定のイベントが発生した場合、[!DNL Workfront] の web アプリケーション内で通知を受け取ることができます。

アプリ内通知について詳しくは、[アプリ内通知の表示と管理](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md)を参照してください。

## モバイルメールアプリでのメール通知

お使いのモバイルデバイスを使用して、モバイルメールアプリで [!DNL Workfront] メール通知を受信できます。

モバイルデバイスに [!DNL Workfront] モバイルアプリをインストールすると、メール内のリンクをタップすることで、[!DNL Workfront] モバイルアプリ内で通知を開くことができます。これには、次のいずれかのアクションボタンのタップが含まれます。

* [!UICONTROL 作業する]
* [!UICONTROL コメント]
* [!UICONTROL 承認決定する]
* [!UICONTROL すべての通知を表示]
* [!UICONTROL 追加]
* [!UICONTROL 開始]
* [!UICONTROL 詳細を表示]

[!DNL Workfront] のモバイルアプリについて詳しくは、[ [!DNL Adobe Workfront]  のモバイルアプリを使用](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md)を参照してください。
