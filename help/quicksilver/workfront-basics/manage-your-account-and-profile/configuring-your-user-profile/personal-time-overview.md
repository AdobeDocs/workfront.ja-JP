---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: 個人の休日を設定
description: 承認されたオフの発生時期をAdobe Workfrontで指定することが重要です。これは、スケジュールに影響し、割り当てられているタスクの予定完了日に影響を与えるからです。
author: Lisa
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: 16a34e4315d508e31859e962edd01026d01ee193
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 62%

---

# 個人の休日を設定

<!-- Audited: 12/2023 -->

[!DNL Adobe Workfront] は、個人の休暇を管理、累積または追跡するために、組織の既存システムを複製または置き換えるようには設計されていません。

ただし、承認されたオフのタイミングを指定することが重要です。これは、スケジュールと [!UICONTROL 計画完了日] 割り当てられているタスクの数を指定します。

例えば、ユーザーが 2 週間かかる予定のタスクに割り当てられていて、その間に 3 日間の休暇を取る予定がある場合、[!DNL Workfront] ではタスクタイムラインに 3 日を追加して、休暇を考慮します。

また、リソース管理ツールは、個人の休暇を使用して、いつ作業のスケジュールを入れることができるかを示します。

>[!NOTE]
>
>休暇のスケジュールを設定した日付との不一致が生じないようにするため、ユーザープロファイルのタイムゾーンをスケジュールのタイムゾーンと一致させることをお勧めします。詳しくは、次の記事を参照してください。
>
>* [スケジュールを作成](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [ユーザーのプロファイルを編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> <p>新規：標準（個人のオフ時間を設定）</p>
        <p>または</p>
        <p>現在：勤務先以上（個人の休日を設定する場合）</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!UICONTROL Edit User]アクセス権を持つ[!UICONTROL Manager]（他のユーザーの休暇カレンダーを変更する場合）<br>
   <strong>メモ：</strong>管理者が別のユーザーの個人の休暇カレンダーを編集した場合、すべてのエントリは、管理者のタイムゾーンではなく、ユーザーのタイムゾーンで表示されます。</td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## [!DNL Workfront] における個人の休暇の設定

{{step1-click-profile-pic}}

1. 左パネルの「**[!UICONTROL 休暇]**」をクリックします。
1. 個人の休暇に希望する日付を選択します。

   ![個人の休暇カレンダー](assets/personal-time-off-calendar.png)

1. 一日中休みを取る場合は、「**[!UICONTROL 一日中]**」を選択します。

   1 日未満の休日を取る場合は、このチェックボックスをオフのままにし、休日の開始時間と終了時間を指定します。

1. 「**[!UICONTROL 保存]**」をクリックします。

   休暇が、 [!DNL Workfront] システム全体でリソースプランナーやワークロードバランサーなどのリソース管理ツールに表示されるようになりました。この間に作業を割り当てられると、ツールヒントが表示され、予定時間がずれたことがユーザーに通知されます。
