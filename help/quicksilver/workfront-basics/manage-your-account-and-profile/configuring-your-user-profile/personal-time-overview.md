---
content-type: overview
product-area: user-management
navigation-topic: configure-your-user-profile
title: 個人の休暇の設定
description: 承認された休暇がいつ発生するかを Adobe Workfront で表示することが重要です。これはスケジュールに影響し、割り当てられているタスクの予定完了日に影響を与えるからです。
author: Becky
feature: Get Started with Workfront
exl-id: e7710495-c418-47b1-8598-725580054fc5
source-git-commit: 5d326776b9c5b4d9d24e802375df4630508c8bd0
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 75%

---

# 個人の休暇の設定

<!-- Audited: 12/2025 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment, and is being released in a phased rollout to Production.</span>-->

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

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 </col>
 <tbody> 
  <tr> 
   <td> Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td> <p>個人の休暇を設定するには、次の条件を満たす必要があります。</p>
        <p>標準（個人の休暇を設定するため）</p>
        <p>仕事以上（個人の休暇を設定するため）</p> </td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td><p>別のユーザーの休暇カレンダーを変更するには、そのユーザーのマネージャーで、ユーザーの編集アクセス権を持っている必要があります。</p>
   <p><strong> 注意：</strong> 管理者が別のユーザーの個人的な休暇カレンダーを編集した場合、すべてのエントリが管理者のタイムゾーンではなく、ユーザーのタイムゾーンで表示されます。</p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## [!DNL Workfront] における個人の休暇の設定

{{step1-click-profile-pic}}

>[!NOTE]
>
>Adobe統合エクスペリエンスを利用している場合は、上部のナビゲーション領域の右上隅にある **Adobe** のアカウントメニュー（プロファイル画像）をクリックし、**Workfrontのプロファイル** をクリックします。
>
>![workfront プロファイル &#x200B;](assets/aue-profile.png)

1. 左パネルの「**[!UICONTROL 休暇]**」をクリックします。
1. 個人の休暇に希望する日付を選択します。

   ![個人の休暇カレンダー](assets/personal-time-off-calendar-0925.png)

   <!--Sample image in the Production environment:
   ![Personal time off calendar](assets/personal-time-off-calendar.png)-->

1. 一日中休みを取る場合は、「**[!UICONTROL 一日中]**」を選択します。

   休暇が 1 日未満で、休暇の開始時間と終了時間を示す場合は、このチェックボックスをオフのままにします。

1. 「**[!UICONTROL 保存]**」をクリックします。

   休暇が、 [!DNL Workfront] システム全体でリソースプランナーやワークロードバランサーなどのリソース管理ツールに表示されるようになりました。この時間に作業が割り当てられると、休暇をスケジュールしたことをユーザーに通知するツールヒントが表示されます。
