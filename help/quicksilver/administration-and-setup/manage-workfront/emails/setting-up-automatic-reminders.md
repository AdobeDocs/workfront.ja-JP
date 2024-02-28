---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: 自動リマインダーを設定
description: 自動リマインダーを設定
author: Nolan
feature: System Setup and Administration
role: Admin
exl-id: 37ad04a1-d3c8-48b2-aed8-fe40456196ec
source-git-commit: 1c0a656f2603c5decabd2bb4e88da1b9530f9e1c
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 100%

---

# 自動リマインダーを設定

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

Adobe Workfront 管理者は、すべてのタスクやイシューが期日になったとき、遅れたとき、または完了予定日に近づいたときにメール通知をトリガーする自動リマインダーを設定できます。これらを設定成した後、ユーザーは自動リマインダーを無効にすることはできません。

遅延通知の場合、メールはタスクまたはイシューが完了するまで毎晩送信されます。

自動リマインダーは、次のいずれかの相手、または複数の相手に送信できます。

* タスクまたはイシューに割り当てられているユーザー
* ユーザーの直属のマネージャー
* 直属のマネージャーを管理するマネージャー

>[!NOTE]
>
>自動リマインダーによってトリガーされるメールの内容や件名は変更できません。

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
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>システム管理者</p> </td> 
  </tr> 
 </tbody> 
</table>

## 自動リマインダーを設定

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックして、「**設定**」![](assets/gear-icon-settings.png) をクリックします。

1. **電子メール**／**自動リマインダー**&#x200B;をクリックします。

1. **遅延通知の送信先**&#x200B;領域で、次のいずれかのオプションを選択します。

   <table>
    <tr>
        <td>「割り当て先」ユーザー</td>
        <td>タスクまたはイシューに割り当てられているユーザーに、作業項目の遅延に関する遅延通知を送信する場合は、このオプションを選択します。</td>
        <td></td>
    </tr>
    <tr>
        <td>ユーザーのマネージャ</td>
        <td>ユーザーのマネージャーに直属の部下の作業項目の遅延に関する遅延通知を送信する場合は、このオプションを選択します。</td>
        <td></td>
    </tr>
    <tr>
        <td>マネージャーのマネージャー</td>
        <td>直属の上司のマネージャーに、直属の部下のユーザーの 1 人の作業項目の遅延に関する遅延通知を送信する場合は、このオプションを選択します。</td>
        <td></td>
    </tr>
    <tr>
        <td>「割り当て先」ユーザー</td>
        <td>（<b>締切リマインダの送信先</b>領域内）タスクまたはイシューに割り当てられたユーザーに、期限が近づいている作業項目に関する通知を送信する場合は、このオプションを選択します。</td>
        <td></td>
    </tr>
</table>

1. 作業項目の期日の前後の時間を選択して、自動リマインダーを送信する時間を設定します。

   時間は、タスクまたはイシューの予定完了日から計算されます。

   分、時間、日、週または月数で、タスクまたはイシューの予定完了日に時間を指定します。**経過分数**、**経過時間数**、**経過日数**、または&#x200B;**経過週数**&#x200B;を選択して、スケジュールに示されている週末、祝日、非稼働時間を含む時間を追加します。

   例えば、タスクが金曜日に割り当てられ、期間が経過日数で 3 日の場合、タスクの完了日は月曜日（土曜日と日曜日が週末の場合）に設定されます。タスクの期間が 3 日（経過日数ではない）の場合、タスクの完了日は水曜日に設定されます。

   ![](assets/time-increments-for-automatic-reminder.png)

1. 「**保存**」をクリックします。

## 自動リマインダーを受信

自動リマインダー通知で指定されたエンティティは、指定された期限が来ると電子メールを受け取ります。遅延通知の場合、メールはタスクまたはイシューが完了するまで毎晩送信されます。

特定の依存関係を持つタスクは、期限を過ぎている場合でも、指定された開始日以降に配信される場合があります。例えば、タスクが終了 - 開始（fs）依存関係を持つ先行タスクを持っている場合、先行タスクが完了するまでタスクを開始できないため、指定された開始日を過ぎてもメールに含まれません。

自動リマインダーメールの受信について詳しくは、[Adobe Workfront 通知](../../../workfront-basics/using-notifications/wf-notifications.md)の[自動リマインダー](../../../workfront-basics/using-notifications/wf-notifications.md#automatic-reminders)セクションを参照してください。

## 自動リマインダーを送信

Workfront 管理者が選択した時刻になると直ちに自動リマインダーが送信されます。

自動リマインダーメールの送信を手動でトリガーしたい場合は、Diagnostics を使用して実行できます。Workfront Diagnostics へのアクセスと使用について詳しくは、[Diagnostics を使用した自動化プロセスのトリガー](../../../administration-and-setup/manage-workfront/run-diagnostics/use-diagnostics-to-trigger-automated-processes.md)を参照してください。
