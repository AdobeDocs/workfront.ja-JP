---
product-area: agile-and-teams
navigation-topic: iterations
title: 反復の作成
description: 反復は、スクラムアジャイルチームが作業キャパシティを計画する上で重要な要素です。 [!DNL Adobe Workfront] では、スクラムアジャイルチームが、チームのニーズに合わせて複数のイテレーションを作成することで、作業を管理できます。
author: Courtney
feature: Agile
exl-id: a25cdd4a-f2e3-4b8a-a7f4-3757940b635e
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 68%

---

# イテレーションを作成

反復は、スクラムアジャイルチームが作業キャパシティを計画する上で重要な要素です。 [!DNL Adobe Workfront]では、スクラムアジャイルチームが、チームのニーズに対応するために複数のイテレーションを作成して作業を管理できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>明るいまたはそれ以上</p> 
   <p>レビュー以上</p> </td> 
  </tr>
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## イテレーションを追加

リストにイテレーションを追加してイテレーションをすばやく作成し、後でタスクやイシューを追加することができます。

{{step1-to-team}}

1. （オプション）**[!UICONTROL チームの切り替え]**&#x200B;アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索します。

1. 「**[!UICONTROL 反復]**」タブで、「**[!UICONTROL 反復を追加]**」をクリックします。

   ![反復を追加をクリック ](assets/click-add-iteration.png)

1. 以下を指定します。

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Iteration Name]</strong></td> 
      <td>イテレーションの名前を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Goal]</strong></td> 
      <td>イテレーションの目標を追加します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Start Date]</strong></td> 
      <td>イテレーションを開始する日付を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL End Date]</strong></td> 
      <td><p>イテレーションを終了する日付を入力します。[!DNL Workfront] では、開始日から 4 週間以内の終了日を設定することをお勧めします。</p><p>ヒント：終了日は必ず稼働日にしてください。バーンダウンチャートの計算に使用されるのは稼働日のみです。<br>デフォルトでは、バーンダウンチャートはデフォルトのスケジュールを使用して稼働日を定義します（<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">スケジュールを作成</a>で説明しています）。または、チーム固有の非稼働日を組み込むために、アジャイルチームは代替スケジュールを使用できます（<a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref"> アジャイルチームを作成</a>の「バーンダウンチャートの代替チームスケジュールの定義」の説明に従って）。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Capacity]</strong></td> 
      <td> イテレーションの処理能力を指定します。これは、チームがイテレーションで達成できるポイントまたは時間の数です。入力する数は、そのイテレーションでの全ストーリーの合計からのポイント数または時間数以上である必要があります。<br>[!DNL Workfront] では、デフォルトでこのフィールドに 50 の処理能力が事前入力されます。 </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Focus]</strong></td> 
      <td>チームのフォーカス率を指定します。チームの全メンバーがこのイテレーションに完全にフォーカスすると、フォーカスは 100％になります。<br>[!DNL Workfront] ではこのフィールドに 100%をデフォルトで事前入力します。 </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL 反復を追加]**」をクリックします。 イテレーションを作成したら、ストーリーを追加する必要があります。詳しくは、[既存のイテレーションにストーリーを追加](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md)を参照してください。

## 「[!UICONTROL バックログ]」タブでのイテレーションの計画

[!UICONTROL イテレーションを計画]機能を使用し、バックログのタスクを使用してイテレーションを作成します。

{{step1-to-team}}

1. （オプション）**[!UICONTROL チームの切り替え]**&#x200B;アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索します。

1. 左側のパネルで「**[!UICONTROL バックログ]**」を選択します。

1. 「**ストーリー**」または「**問題**」タブで、イテレーションに追加する作業項目を選択し、**[!UICONTROL イテレーション計画]**」をクリックします。

>[!NOTE]
>
> 「バックログ」タブでイテレーションを計画する際に、「ストーリー」タブまたは「イシュー」タブを切り替えたり、追加のタスクを追加したりすることはできません。 イテレーションが作成されたら、既存のストーリーまたはイシューを追加できます。 詳しくは、以下の「バックログ」タブ [の「](#add-tasks-or-issues-to-an-existing-iteration-on-the-backlog-tab)既存のイテレーションにタスクまたはイシューを追加する」を参照してください。


1. 次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Iteration Name]</strong></td> 
      <td>イテレーションの名前を指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Start Date]</strong></td> 
      <td> イテレーションを開始する日付を指定します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL End Date]</strong> </td> 
      <td><p>イテレーションが終了する日付を指定します。[!DNL Workfront]では、終了日を開始日から 4 週間以内に設定することをお勧めします。</p><p>ヒント：終了日は必ず稼働日にしてください。バーンダウンチャートの計算に使用されるのは稼働日のみです。<br>デフォルトでは、バーンダウンチャートはデフォルトのスケジュールを使用して稼働日を定義します（<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">スケジュールを作成</a>で説明しています）。または、チーム固有の非稼働日を組み込むために、アジャイルチームは代替スケジュールを使用できます（<a href="../../../agile/use-scrum-in-an-agile-team/burndown/use-alt-team-schedule-burndown-charts.md" class="MCXref xref"> バーンダウンチャートに代替チームスケジュールを使用</a>の説明に従って）。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Focus]</strong></td> 
      <td>チームのフォーカス率を指定します。チームの全メンバーがこのイテレーションに完全にフォーカスすると、フォーカスは 100％になります。<br>[!DNL Workfront]このフィールドに、チームの過去のイテレーションの平均値を事前入力します。これがチームの最初のイテレーションである場合、このフィールドの値はデフォルトでは 0 になります。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Capacity]</strong></td> 
      <td> イテレーションの処理能力を指定します。これは、チームがイテレーションで達成できるポイントまたは時間の数です。入力する数は、そのイテレーションでの全ストーリーの合計からのポイント数または時間数以上である必要があります。<br>[!DNL Workfront]このフィールドに、チームの過去のイテレーションの平均値を事前入力します。これがチームの最初のイテレーションである場合、このフィールドの値はデフォルトでは 0 になります。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><br><strong>[!UICONTROL Goal]</strong></td> 
      <td> イテレーションの目標を指定します。このフィールドは必須ではありません。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL 保存]」をクリックします。** イテレーションが作成されます。

## 「バックログ」タブの既存のイテレーションにタスクまたはイシューを追加する

1. 「**バックログ**」タブで、「**ストーリー**」または「**問題**」タブをクリックします。

1. イテレーションに追加するストーリーまたはイシューを選択します。 バックログの上部にあるストーリーの優先度が高くなります。

   ![作業項目を移動](assets/move-to-iteration.png)

   >[!NOTE]
   >
   >  イテレーションにタスクを追加すると、タスクの開始日が「[[!UICONTROL イテレーションに追加された場合の]タスク開始日の計算方法について](#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration)」の説明に従って計算されます。


## イテレーションに追加した場合のタスクの開始日の計算方法について {#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration}

タスクをストーリーとしてイテレーションに追加する場合、[!UICONTROL 指定日に終了]の制約が、各ストーリーに使用されます。ほとんどの場合、タスクの予定開始日は以下の式に基づいて計算されます。

[!UICONTROL イテレーション終了日]マイナス（-）[!UICONTROL タスクの期間]は（=）[!UICONTROL タスクの予定開始日]

プロジェクト開始日がイテレーション開始日より後で、プロジェクト終了日がイテレーション終了日より後の場合は、[!UICONTROL  プロジェクト終了日]がイテレーション終了日の代わりに使用されます。

個々のスクラムチームが、デフォルトではイテレーション日付よりも、プロジェクト日付を使用するように設定できます。詳しくは、[スクラムの設定](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)の記事の[作業アイテムをイテレーションに追加する際に日付を適用する方法を設定](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration)を参照してください。
