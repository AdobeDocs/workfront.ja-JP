---
product-area: agile-and-teams
navigation-topic: iterations
title: イテレーションを作成
description: 反復は、スクラムアジャイルチームが作業処理能力を計画する際の重要なコンポーネントになります。 [!DNL Adobe Workfront]  スクラムアジャイルチームは、チームニーズに対応するために複数のイテレーションを作成することで、作業を管理できます。
author: Jenny
feature: Agile
exl-id: a25cdd4a-f2e3-4b8a-a7f4-3757940b635e
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '1022'
ht-degree: 68%

---

# イテレーションを作成

反復は、スクラムアジャイルチームが作業処理能力を計画する際の重要なコンポーネントになります。 [!DNL Adobe Workfront] を使用すると、スクラムアジャイルチームは、チームニーズに対応するために複数のイテレーションを作成して作業を管理できます。

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
   <td> <p>ライト以上</p> 
   <p>レビュー以上</p> </td> 
  </tr>
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## イテレーションを追加

リストでイテレーションを追加して素早くイテレーションを作成し、後でタスクと問題を追加できます。

{{step1-to-team}}

1. （オプション）**[!UICONTROL チームの切り替え]**&#x200B;アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索します。

1. 「**[!UICONTROL イテレーション]**」タブで、「**[!UICONTROL イテレーションを追加]**」をクリックします。

   ![&#x200B; 「イテレーションを追加」をクリック &#x200B;](assets/click-add-iteration.png)

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
      <td><p>イテレーションを終了する日付を入力します。[!DNL Workfront] では、開始日から 4 週間以内の終了日を設定することをお勧めします。</p><p>ヒント：終了日は必ず稼働日にしてください。バーンダウンチャートの計算に使用されるのは稼働日のみです。<br>デフォルトでは、バーンダウンチャートはデフォルトのスケジュールを使用して稼働日を定義します（<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">スケジュールを作成</a>で説明しています）。また、チーム固有の非稼働日を取り込むために、アジャイルチームは代替スケジュールを使用するように選択できます（「アジャイルチームの作成 <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref"> の「バーンダウンチャートに対する代替チームスケジュールの定義」を参照 </a> てください）。</p></td> 
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

1. **[!UICONTROL イテレーションを追加]** をクリックします。 イテレーションを作成したら、ストーリーを追加する必要があります。詳しくは、[既存のイテレーションにストーリーを追加](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md)を参照してください。

## 「[!UICONTROL バックログ]」タブでのイテレーションの計画

[!UICONTROL イテレーションを計画]機能を使用し、バックログのタスクを使用してイテレーションを作成します。

{{step1-to-team}}

1. （オプション）**[!UICONTROL チームの切り替え]**&#x200B;アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索します。

1. 左側のパネルで **[!UICONTROL バックログ]** を選択します。

1. **ストーリー** または **イシュー** タブで、反復に追加する作業項目を選択して「**[!UICONTROL 反復を計画]**」をクリックします。

>[!NOTE]
>
> 「バックログ」タブで反復を計画する際に、「ストーリー」タブまたは「イシュー」タブを切り替えたり、追加のタスクを追加したりすることはできません。 イテレーションが作成されたら、既存のストーリーまたはイシューを追加できます。 詳しくは、以下 [&#x200B; 「バックログ」タブの既存のイテレーションへのタスクまたは問題の追加 &#x200B;](#add-tasks-or-issues-to-an-existing-iteration-on-the-backlog-tab) を参照してください。


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
      <td><p>イテレーションが終了する日付を指定します。[!DNL Workfront]では、終了日を開始日から 4 週間以内に設定することをお勧めします。</p><p>ヒント：終了日は必ず稼働日にしてください。バーンダウンチャートの計算に使用されるのは稼働日のみです。<br>デフォルトでは、バーンダウンチャートはデフォルトのスケジュールを使用して稼働日を定義します（<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">スケジュールを作成</a>で説明しています）。また、チーム固有の非稼働日を取り込むために、アジャイルチームは代替スケジュールを使用するように選択できます（<a href="../../../agile/use-scrum-in-an-agile-team/burndown/use-alt-team-schedule-burndown-charts.md" class="MCXref xref"> バーンダウンチャートに代替チームスケジュールを使用 </a> を参照）。</p></td> 
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

## 「バックログ」タブで既存の反復にタスクまたは問題を追加

1. 「**バックログ**」タブで、「**ストーリー**」タブまたは「**イシュー**」タブをクリックします。

1. 反復に追加するストーリーまたはイシューを選択します。 バックログの上部にあるストーリーが優先されます。

   ![&#x200B; 作業項目の移動 &#x200B;](assets/move-to-iteration.png)

   >[!NOTE]
   >
   >  イテレーションにタスクを追加すると、タスクの開始日が「[[!UICONTROL イテレーションに追加された場合の]タスク開始日の計算方法について](#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration)」の説明に従って計算されます。


## イテレーションに追加した場合のタスクの開始日の計算方法について {#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration}

タスクをストーリーとしてイテレーションに追加する場合、[!UICONTROL 指定日に終了]の制約が、各ストーリーに使用されます。ほとんどの場合、タスクの予定開始日は以下の式に基づいて計算されます。

[!UICONTROL イテレーション終了日]マイナス（-）[!UICONTROL タスクの期間]は（=）[!UICONTROL タスクの予定開始日]

プロジェクト開始日がイテレーション開始日より後で、プロジェクト終了日がイテレーション終了日より後の場合、イテレーション終了日の代わりに [!UICONTROL &#x200B; プロジェクト終了日 &#x200B;] が使用されます。

個々のスクラムチームが、デフォルトではイテレーション日付よりも、プロジェクト日付を使用するように設定できます。詳しくは、[スクラムの設定](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)の記事の[作業アイテムをイテレーションに追加する際に日付を適用する方法を設定](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration)を参照してください。
