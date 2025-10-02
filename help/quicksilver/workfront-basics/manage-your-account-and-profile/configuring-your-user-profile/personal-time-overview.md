---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: 個人の休暇の設定
description: 承認された休暇がいつ発生するかを Adobe Workfront で表示することが重要です。これはスケジュールに影響し、割り当てられているタスクの予定完了日に影響を与えるからです。
author: Becky
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: ce2f1ebe7ea97f3c25ac6a7ef33fd3c066727220
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 87%

---

# 個人の休暇の設定

<!-- Audited: 12/2023 -->

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。これはプレビューサンドボックス環境でのみ使用でき、実稼動環境への段階的なロールアウトでリリースされています。</span>

[!DNL Adobe Workfront] は、個人の休暇を管理、累積または追跡するために、組織の既存システムを複製または置き換えるようには設計されていません。

ただし、承認された休暇がいつ発生するかを示すことが重要です。これはスケジュールと割り当てられているタスクの[!UICONTROL 予定完了日]の両方に影響を与えるからです。

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
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> <p>新規：標準（個人の休暇を設定する場合）</p>
        <p>または</p>
        <p>現在：ワークまたはそれ以上（個人の休暇を設定する場合）</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!UICONTROL Edit User]アクセス権を持つ[!UICONTROL Manager]（他のユーザーの休暇カレンダーを変更する場合）<br>
   <strong>メモ：</strong>管理者が別のユーザーの個人の休暇カレンダーを編集した場合、すべてのエントリは、管理者のタイムゾーンではなく、ユーザーのタイムゾーンで表示されます。</td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## [!DNL Workfront] における個人の休暇の設定

{{step1-click-profile-pic}}

>[!NOTE]
>
>Adobe統合エクスペリエンスを利用している場合は、上部のナビゲーション領域でAdobe アカウント メニュー（プロファイル画像）をクリックし、「Workfront プロファイル」を選択すると、Workfront プロファイルにアクセスできます。
>
>![workfront プロファイル &#x200B;](assets/aue-profile.png)

1. 左パネルの「**[!UICONTROL 休暇]**」をクリックします。
1. 個人の休暇に希望する日付を選択します。

   <span class="preview"> プレビュー環境のサンプル画像：</span>
   ![個人の休暇カレンダー](assets/personal-time-off-calendar-0925.png)

   実稼動環境のサンプル画像：
   ![個人の休暇カレンダー](assets/personal-time-off-calendar.png)

1. 一日中休みを取る場合は、「**[!UICONTROL 一日中]**」を選択します。

   休暇が 1 日未満で、休暇の開始時間と終了時間を示す場合は、このチェックボックスをオフのままにします。

1. 「**[!UICONTROL 保存]**」をクリックします。

   休暇が、 [!DNL Workfront] システム全体でリソースプランナーやワークロードバランサーなどのリソース管理ツールに表示されるようになりました。この時間に作業が割り当てられると、休暇をスケジュールしたことをユーザーに通知するツールヒントが表示されます。
