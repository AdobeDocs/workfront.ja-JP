---
content-type: overview;reference
navigation-topic: notifications
title: Adobe Workfront通知
description: Adobe Workfrontは、モバイルデバイスで電子メール通知、アプリ内通知および通知を送信します。
author: Lisa
feature: Get Started with Workfront
exl-id: 118677e9-a13f-47e6-96a3-6f5e93b005e9
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '1307'
ht-degree: 2%

---

# [!DNL Adobe Workfront] 通知

[!DNL Adobe Workfront] は、モバイルデバイスで電子メール通知、アプリ内通知および通知を送信します。

## メール通知

[!DNL Workfront] は、Workfrontのアクティビティについてユーザーに警告する電子メール通知を多数送信し、役に立つ情報やリンクを提供します。

電子メール通知の環境設定を変更するには、 [独自の電子メール通知を変更する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>サンドボックス環境から電子メール通知を受け取る場合は、その環境のユーザープロファイルから電子メールを有効にする必要があります。

次の電子メール通知をから受け取ることができます。 [!DNL Workfront]:

* [イベント通知](#event-notifications)
* [1 日のダイジェスト通知](#daily-digest-notifications)
* [投稿されたコメントの通知](#notification-of-posted-comments)
* [自動リマインダー](#automatic-reminders)
* [リマインダ通知](#reminder-notifications)
* [ボード通知](#boards-notifications)
* [その他 [!DNL Workfront] 電子メール](#other-workfront-emails)

### イベント通知

イベント通知は、 [!DNL Workfront]. 通常、特定のイベントによってトリガーされます。

イベント通知が [!DNL Workfront] 管理者またはグループ管理者は、 [!UICONTROL 通知] 環境設定がユーザープロファイルに表示されます。 また、イベントが発生したときに通知を受け取るか、1 日のダイジェスト電子メールに要約されたイベントを受け取るかを選択できます。

を [!DNL Workfront] 管理者がお客様に対するイベント通知を設定しました [!DNL Workfront] システム ( [システムの全員に対するイベント通知を設定する](../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)) の場合、設定には、これらの通知のサブセットのみが表示されることがあります。

デフォルトのステータスは、新しいユーザーを作成する際に、新しいユーザーに対してデフォルトで有効にされる通知（日別、即時またはその両方）を示します。

イベント通知の完全なリスト、およびシステムレベル、グループレベル、ユーザーレベルでのイベント通知の有効化と設定方法について詳しくは、 [イベント通知はで使用可能 [!DNL Adobe Workfront]](../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md).

受信するイベント通知の選択方法について詳しくは、 [独自の電子メール通知を変更する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>イベント通知は、毎日のダイジェスト更新で配信されるように設定できる唯一の通知です。

### 1 日のダイジェスト通知

日々のダイジェスト電子メール配信で有効にされた電子メール通知の完全なリストと、電子メール通知のすべてのカテゴリに関する情報については、 [イベント通知](../../workfront-basics/using-notifications/event-notifications.md#understanding-instant-and-daily-digest-notifications).

>[!NOTE]
>
>[!UICONTROL Workfront] は、 [!UICONTROL その他] および [!DNL Goals] イベントのカテゴリ。 これらのカテゴリの Daily 通知を無効にすることはできません。

日別のダイジェスト通知を受信する際に注意すべき点がいくつかあります。

* 各 [!UICONTROL 通知] 」セクションに **[!UICONTROL マイ設定]** パネルは、独自の日次ダイジェスト電子メールを生成します。 1 日に 1 件のダイジェスト電子メールに対して有効にする通知設定と同じ数のダイジェスト電子メールを 1 日に 1 通ずつ送信することができます。\
   例えば、「 **[!UICONTROL プロジェクト ID に関する情報] 所有者** 1 通の電子メール通知が届き、この領域で満たされたすべてのイベントが一覧表示されます。

* 日別ダイジェスト電子メールに含まれる通知は、様々な条件でグループ化されます。 例えば、 **[!UICONTROL 自分が所有するプロジェクトに関する情報]**&#x200B;の場合、イベントはプロジェクト名でグループ化されます。

  の **[!UICONTROL 通信]** カテゴリに分類すると、通知は通信が発生したオブジェクト別にグループ化されます。

* 日次ダイジェスト電子メールには、特定の領域で発生したイベント ( **所有しているプロジェクトに関する情報**) を、配信に選択された時間の 24 時間以内に設定します。
* 日別のダイジェスト配信で選択された時間のタイムゾーンは、ブラウザーで設定されているタイムゾーンと一致します。
* 日別のダイジェスト E メールには、件名行のセクションの名前と、配信日が含まれます。
* 日別のダイジェストを配信するには、少なくとも 1 つのイベントに通知をトリガーする必要があります。 日別のダイジェスト電子メールに対してマークされたイベントが満たされない場合、日別ダイジェストは送信されません。

### 投稿されたコメントの通知

通知は、 [!UICONTROL 通信] カテゴリには、で投稿されたコメントに対する警告が表示されます [!UICONTROL 更新] 特定の項目のストリーム。

の日別ダイジェスト電子メール [!UICONTROL 通信] カテゴリが選択され、使用可能なすべての通知が表示されます。

通信が発生したオブジェクトに対して情報を要約し、各オブジェクトに対して通信メッセージの総数を表示する。

電子メール通知の設定について詳しくは、 [独自の電子メール通知を変更する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

に対するコメントの説明 [!UICONTROL 通信] 電子メール、詳しくは、 [作業を更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

詳しくは、以下を参照してください。 [!UICONTROL 通信] 電子メール、詳しくは、 [独自の電子メール通知を変更する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

日別のダイジェスト通知を有効にする方法について詳しくは、 [独自の電子メール通知を変更する](../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

### 自動リマインダー

自動リマインダーは、 [!DNL Workfront] 管理者：予定完了日に期限が切れている、遅れている、または予定完了日に近いタスクや問題を警告します。 遅延通知の場合、電子メールはタスクまたは問題が完了するまで毎晩送信されます。 管理者が設定した後で、無効にすることはできません。 また、自動リマインダーによってトリガーされる E メールの内容や件名を変更することはできません。

自動リマインダーは、次のいずれか、または複数の相手に送信できます。

* タスクまたはイシューに割り当てられたユーザー
* ユーザーの即時管理者
* 即時支配人の支配人

自動リマインダーの電子メールは、 [!DNL Workfront] 送信メールを処理するように選択された管理者。

自動リマインダーが有効化されている場合、自動リマインダー電子メールでは次の種類の情報を使用できます。

* タスクまたはタスクが作成された日付
* タスク名または懸案事項名
* タスクまたはタスクが存在するプロジェクトの名前
* タスクまたはイシューの説明
* タスクまたはイシューに割り当てられたユーザーのリスト
* タスクまたはタスクを入力したユーザーの名前
* タスクまたはタスクの優先度
* タスクまたは問題が期限切れになった日付

自動リマインダーの有効化について詳しくは、 [自動リマインダーの設定](../../administration-and-setup/manage-workfront/emails/setting-up-automatic-reminders.md).

### リマインダ通知

A [!DNL Workfront] 管理者 ( または [!UICONTROL プランナー] アクセスレベルと管理アクセス（リマインダー通知へのアクセス）は、近づく期限に関するリマインダー通知を設計し、プロジェクト、タスク、問題、およびタイムシートに関連付けることができます。 必要な管理アクセス権を取得する方法について詳しくは、 [特定の領域に対する管理者アクセス権をユーザーに付与する](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

>[!IMPORTANT]
>
>上記のいずれかのオブジェクトに関するリマインダー通知をユーザーが受け取った後に期限が変更された場合、ユーザーは別のリマインダー通知を受け取りません。

リマインダー通知は、 [!DNL Workfront] 送信メールを処理するように選択された管理者。

リマインダー通知の設定と有効化について詳しくは、 [リマインダー通知の設定](../../administration-and-setup/manage-workfront/emails/set-up-reminder-notifications.md).

### ボード通知

[!DNL Adobe Workfront] [!UICONTROL ボード] は、あなたがボードに追加されたとき、およびカードが割り当てられたときに電子メールを送信します。

ボードの環境設定で受信する電子メールを選択できます。 詳しくは、 [電子メール通知と環境設定をボード](/help/quicksilver/agile/get-started-with-boards/boards-emails.md).

### その他 [!DNL Workfront] 電子メール

他にもメールが届いている可能性があります [!DNL Workfront] 設定できない 次の E メールは、によって自動的に送信されます [!DNL Workfront] これらの条件が満たされた場合：

* 項目を復元： [!DNL Workfront] 管理者は、 [!UICONTROL リサイクル] bin：電子メールが [!DNL Workfront] 管理者。
* 復元に失敗しました： [!DNL Workfront] 管理者がごみ箱からオブジェクトを復元しようとしましたが、復元に失敗した場合、電子メールが [!DNL Workfront] 管理者。

次の電子メールは、ユーザープロファイルレベルでのみ設定できます。 システムレベルで有効または無効にすることはできません。

* 個人タスクの完了：他のユーザーに割り当てた個人タスクが完了すると、電子メールが送信されます。
* ユーザーに追加されたコメント：ユーザープロファイルに対して誰かがコメントをすると、電子メールが送信されます。

## アプリ内通知

通知は、 [!DNL Workfront] 特定のイベントが発生した場合の Web アプリケーション。

アプリ内通知について詳しくは、 [アプリ内通知の表示と管理](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

## モバイル電子メールアプリでの電子メール通知

以下を受け取ることができます： [!DNL Workfront] モバイル電子メールアプリでの電子メール通知を設定できます。

次の条件を満たす [!DNL Workfront] 携帯電話にインストールされたモバイルアプリが、電子メールのリンクをタップすると、 [!DNL Workfront] モバイルアプリ。 これには、次のいずれかのアクションボタンをタップすることも含まれます。

* [!UICONTROL 作業]
* [!UICONTROL コメント]
* [!UICONTROL 承認決定する]
* [!UICONTROL 全ての通知を表示]
* [!UICONTROL 追加]
* [!UICONTROL 開始]
* [!UICONTROL 詳細を表示]

詳しくは、 [!DNL Workfront] モバイルアプリ ( [以下を使用します。 [!DNL Adobe Workfront] モバイルアプリ](../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md).
