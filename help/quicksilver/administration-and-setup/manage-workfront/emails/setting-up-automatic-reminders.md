---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: 自動リマインダーの設定
description: 自動リマインダーの設定
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 37ad04a1-d3c8-48b2-aed8-fe40456196ec
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '609'
ht-degree: 1%

---

# 自動リマインダーの設定

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Adobe Workfront管理者は、すべてのタスクや問題が予定完了日、遅延または予定完了日付近になった場合の、トリガー電子メール通知に対する自動リマインダーを設定できます。 これらの設定を構成した後は、ユーザーは自動リマインダーを無効にできません。

遅延通知の場合、電子メールはタスクまたは問題が完了するまで毎晩送信されます。

自動リマインダーは、次の 1 つ以上に送信できます。

* タスクまたはイシューに割り当てられたユーザー
* ユーザーの即時管理者
* 即時支配人の支配人

>[!NOTE]
>
>自動リマインダーによってトリガーされる E メールの内容や件名は変更できません。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>システム管理者</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自動リマインダーの設定

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **電子メール** >**自動リマインダー**.

1. 内 **遅延通知の送信先** 「 」領域で、次のいずれかのオプションを選択します。

   <table>
    <tr>
        <td>「割り当て先」ユーザー</td>
        <td>タスクまたはタスクに割り当てられたユーザーが、作業項目が遅れていることに関する遅延通知を受け取る場合は、このオプションを選択します。</td>
        <td></td>
    </tr>
    <tr>
        <td>ユーザーのマネージャ</td>
        <td>ユーザーの管理者が直属の作業項目の遅延に関する通知を遅延で受け取る場合に、このオプションを選択します。</td>
        <td></td>
    </tr>
    <tr>
        <td>マネージャのマネージャ</td>
        <td>即時管理者の管理者が、直属の部下のユーザーの 1 つの作業項目に関する遅延通知を受け取る場合に、このオプションを選択します。</td>
        <td></td>
    </tr>
    <tr>
        <td>「割り当て先」ユーザー</td>
        <td>( <b>期限のリマインダーをに送信</b> 領域 ) タスクまたはイシューに割り当てられたユーザーが、期限が近づいている作業項目に関する通知を受け取る場合に、このオプションを選択します。</td>
        <td></td>
    </tr>
</table>

1. 作業項目の期限の前または後の時間を選択して、自動リマインダーが送信する時間を選択します。

   時間は、タスクまたはイシューの計画完了日から計算されます。

   タスクまたはタスクの計画完了日に時間を追加する時間を分、時間、日、週または月数で指定します。 選択 **経過分数**, **経過時間**, **経過日数**&#x200B;または **経過週間** ：スケジュールに示された週末、休日、非営業時間を含む時間を追加します。

   例えば、タスクが金曜日に割り当てられ、期間が 3 日の場合、タスクの完了日は月曜日（土曜日と日曜日が週末の場合）に設定されます。 タスクの期間が 3 日（経過日ではない）の場合、タスクの完了日は水曜日に設定されます。

   ![](assets/time-increments-for-automatic-reminder.png)

1. 「**保存**」をクリックします。

## 自動リマインダーを受信

自動リマインダー通知で指定されたエンティティである場合は、指定された期限を過ぎると電子メールを受け取ります。 遅延通知の場合、電子メールはタスクまたは問題が完了するまで毎晩送信されます。

特定の依存関係タイプを持つタスクは、期限を過ぎている場合でも、指定した開始日以降に配信される可能性があります。 たとえば、タスクに [ 終了 — 開始 ] (fs) 依存関係を持つ先行タスクがある場合、指定した開始日を過ぎても、先行タスクが完了するまでタスクを開始できないので、メールには含まれません。

自動リマインダーメールの受信の詳細については、 [自動リマインダー](../../../workfront-basics/using-notifications/wf-notifications.md#automatic-reminders) セクション [Adobe Workfront通知](../../../workfront-basics/using-notifications/wf-notifications.md).

## 自動リマインダーの送信

自動リマインダーは、Workfront管理者が選択した時間に達するとすぐに送信されます。

自動リマインダー電子メールの手動送信をトリガーにする場合は、診断を使用して送信できます。 Workfrontでの診断へのアクセスと使用について詳しくは、 [診断を使用して自動プロセスをトリガー化](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md).
