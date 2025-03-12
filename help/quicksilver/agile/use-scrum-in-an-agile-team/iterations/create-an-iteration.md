---
product-area: agile-and-teams
navigation-topic: iterations
title: イテレーションを作成
description: イテレーションは、スクラムアジャイルチームが作業処理能力を計画する際の主要なコンポーネントです。 [!DNL Adobe Workfront]  を使ってチームのニーズに合わせて複数のイテレーションを作成することで、スクラムアジャイルチームが作業を管理できます。
author: Lisa
feature: Agile
exl-id: a25cdd4a-f2e3-4b8a-a7f4-3757940b635e
source-git-commit: 6fb0870b919baf49e17d48586b2a9661e5cb4b94
workflow-type: tm+mt
source-wordcount: '1119'
ht-degree: 83%

---

# イテレーションを作成

イテレーションは、スクラムアジャイルチームが作業処理能力を計画する際の主要なコンポーネントです。[!DNL Adobe Workfront] を使ってチームのニーズに合わせて複数のイテレーションを作成することで、スクラムアジャイルチームが作業を管理できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> <p>新規：[!UICONTROL ライト ] 以上</p> 
   または
   <p>現在：[!UICONTROL Review] 以上</p> </td> 
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

   ![ 「イテレーションを追加」をクリック ](assets/click-add-iteration.png)

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
      <td><p>イテレーションを終了する日付を入力します。[!DNL Workfront] では、開始日から 4 週間以内の終了日を設定することをお勧めします。</p><p>ヒント：終了日は必ず稼働日にしてください。バーンダウンチャートの計算に使用されるのは稼働日のみです。<br>デフォルトでは、バーンダウンチャートはデフォルトのスケジュールを使用して稼働日を定義します（<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">スケジュールを作成</a>で説明しています）。また、チーム固有の非稼働日を組み込むには、アジャイルチームが代替スケジュールを使用するように選択できます（<a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">アジャイルチームの作成</a>の「バーンダウンチャートの代替チームスケジュールの定義」で説明しています）。</p></td> 
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

1. **ストーリー** または **イシュー** タブで、少なくとも 1 つの作業項目を選択し、「**[!UICONTROL 反復を計画]**」をクリックします。

>[!NOTE]
>
> 「バックログ」タブでイテレーションを計画する際に、「ストーリー」タブまたは「イシュー」タブを切り替えることはできません。 イテレーションが作成されたら、既存のストーリーまたはイシューを追加できます。 詳しくは、[ バックログからイテレーションまたはボードへのストーリーの移動 ](/help/quicksilver/agile/work-in-an-agile-environment/manage-the-agile-backlog.md#move-stories-from-the-backlog-to-an-iteration-or-board) を参照してください。


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
      <td><p>イテレーションが終了する日付を指定します。[!DNL Workfront]では、終了日を開始日から 4 週間以内に設定することをお勧めします。</p><p>ヒント：終了日は必ず稼働日にしてください。バーンダウンチャートの計算に使用されるのは稼働日のみです。<br>デフォルトでは、バーンダウンチャートはデフォルトのスケジュールを使用して稼働日を定義します（<a href="../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">スケジュールを作成</a>で説明しています）。また、チーム固有の非稼働日を組み込むには、アジャイルチームが代替スケジュールを使用するように選択できます（<a href="../../../agile/use-scrum-in-an-agile-team/burndown/use-alt-team-schedule-burndown-charts.md" class="MCXref xref">バーンダウンチャートに代替のチームスケジュールを使用</a>で説明されています）。</p></td> 
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

1. （オプション）ストーリーを選択して今すぐイテレーションに追加するか、この手順をスキップして、後でイテレーションにストーリーを追加できます。バックログの先頭のストーリーの方が高い優先度を持ちます。ストーリーは、処理能力に収まると緑色でハイライト表示されます。収まらないと赤色でハイライト表示されます。
タスクとイシューの両方を 1 つのイテレーションに追加できます。

   * **タスクをイテレーションに追加するには：**「**[!UICONTROL バックログ]**」タブで、「**[!UICONTROL ストーリー]**」タブが選択されていることを確認します（バックログを表示する場合は、このタブがデフォルトで選択されています）。イテレーションに追加するストーリーを選択します。

     イテレーションにタスクを追加すると、タスクの開始日が「[[!UICONTROL イテレーションに追加された場合の]タスク開始日の計算方法について](#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration)」の説明に従って計算されます。

   * **イテレーションにイシューを追加するには：**「**[!UICONTROL バックログ]**」タブで、「**[!UICONTROL イシュー]**」タブをクリックします。イテレーションに追加するイシューを選択します。

1. 「**[!UICONTROL 保存]」をクリックします。**
イテレーションが作成されます。

1. （オプション）既存のイテレーションにストーリーを追加するには、[既存のイテレーションにストーリーを追加](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md)を参照してください。

## イテレーションに追加した場合のタスクの開始日の計算方法について {#understand-how-task-start-dates-are-calculated-when-added-to-an-iteration}

タスクをストーリーとしてイテレーションに追加する場合、[!UICONTROL 指定日に終了]の制約が、各ストーリーに使用されます。ほとんどの場合、タスクの予定開始日は以下の式に基づいて計算されます。

[!UICONTROL イテレーション終了日]マイナス（-）[!UICONTROL タスクの期間]は（=）[!UICONTROL タスクの予定開始日]

プロジェクト開始日がイテレーション開始日より後で、プロジェクト終了日がイテレーション終了日より後の場合、イテレーション終了日の代わりに [!UICONTROL  プロジェクト終了日 ] が使用されます。

個々のスクラムチームが、デフォルトではイテレーション日付よりも、プロジェクト日付を使用するように設定できます。詳しくは、[スクラムの設定](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)の記事の[作業アイテムをイテレーションに追加する際に日付を適用する方法を設定](../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration)を参照してください。
