---
content-type: reference
product-area: setup
navigation-topic: use-the-gantt-chart
title: '[!UICONTROL ガント]チャートでの情報の表示方法の設定'
description: タスクリストのガントチャートとプロジェクトリストのガントチャートに表示される情報を設定できます。
author: Alina
feature: Work Management
exl-id: 465365a2-d94b-47b6-a393-16770fca2714
source-git-commit: 2db4a79cad71b550b7de573c5b27293b6582858f
workflow-type: ht
source-wordcount: '948'
ht-degree: 100%

---

# [!UICONTROL ガントチャート]での情報の表示方法の設定

タスクリストの[!UICONTROL ガントチャート]とプロジェクトリストの[!UICONTROL ガントチャート]に表示される情報を設定できます。

## アクセス要件

この記事の手順に従うには、以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Review] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトとタスクに対する[!UICONTROL View]以上のアクセス権</p> <p>メモ：まだアクセス権がない場合は、[!DNL Workfront] 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する[!UICONTROL View]以上のアクセス権</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 表示オプションについて

[!UICONTROL ガントチャート]の表示オプションの詳細を次の表に示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Actual Dates]</td> 
   <td> <img src="assets/actual-dates-in-gantt-183x213.png" alt="actual_dates_in_gantt.png" style="width: 183;height: 213;"> </td> 
   <td> <p>[!UICONTROL Actual Start Date]と[!UICONTROL Actual Completion Date]が三角形のアイコンと共に表示されます。[!UICONTROL Actual Completion Date]が null の場合は、[!UICONTROL Actual Start Date]のみが表示されます。</p> <p>開始日と完了日について詳しくは、<a href="../../../manage-work/projects/planning-a-project/project-actual-completion-date.md" class="MCXref xref">プロジェクトの[!UICONTROL Actual Completion Date]の概要</a>と<a href="../../../manage-work/projects/planning-a-project/project-actual-start-date.md" class="MCXref xref">プロジェクトの[!UICONTROL Actual Start Date]の概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assignments]</td> 
   <td> <img src="assets/assignments-in-gantt-312x203.png" alt="assignments_in_gantt.png" style="width: 312;height: 203;"> </td> 
   <td> <p>タスクの割り当て先を表示します。割り当て先の名前の横にある「<strong>[!UICONTROL Details]</strong>」リンクにマウスを置くと、タスクへの割り当ての割合など、割り当て先に関する詳細情報が表示されます。</p> <p>[!UICONTROL Gantt chart]を PDF に書き出すと、[!UICONTROL Gantt chart]に割り当て先が表示されません。[!UICONTROL Gantt chart]を PDF に書き出すと、割り当て先はタスクリストにのみ表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Baseline]</td> 
   <td> <img src="assets/baselines-sandbox-gantt.png" alt="baselines_sandbox_gant.png"> </td> 
   <td> <p>初期のプロジェクト計画に含まれる、プロジェクトに関する主要なデータを表すプロジェクトスナップショット。ベースラインは、プロジェクトの全期間を通じて取得できます。[!UICONTROL Gantt chart]にベースラインを表示できるようにする場合は、表示するベースラインを選択します。[!UICONTROL Gantt chart]では、一度に 1 つのベースラインのみ表示でき、グレーのバー形式で表示されます。</p> <p>ベースラインについて詳しくは、<a href="../../../manage-work/projects/create-projects/create-baselines.md" class="MCXref xref">プロジェクトのベースラインの作成</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Commit Date]</td> 
   <td> <img src="assets/commit-dates-sandbox-243x226.png" alt="commit_dates_sandbox.png" style="width: 243;height: 226;"> </td> 
   <td> <p>割り当て先がタスクの完了時期として約束した日付が、[!UICONTROL Gantt chart]にマーカーで表示されます。 </p> <p>コミット日の詳細について詳しくは、<a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">[!UICONTROL Commit Date]の概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL % Complete]</td> 
   <td> <img src="assets/percent-complete-gantt.png" alt="percent_complete_gantt.png"> </td> 
   <td> 完了したタスクの割合がタスクラインに表示されます。<br><br></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Critical Path]</td> 
   <td> <img src="assets/critical-path-2.png" alt="Critical_path_2.png"> </td> 
   <td>プロジェクトのタイムラインに影響を与える可能性のあるタスクは、クリティカルパスの一部と見なされ、赤ではっきりとマークされます。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone] ダイヤモンド</td> 
   <td> <img src="assets/milestone-diamonds.png" alt="milestone_diamonds.png"> </td> 
   <td> <p>マイルストーンに関連付けられたタスクの後にダイヤモンドのアイコンが表示されます。マイルストーンの上にポインタを合わせると、マイルストーンの名前と日付が表示されます。[!DNL Workfront] 管理者が、各マイルストーンのダイヤモンドの色を決定します。</p> <p>マイルストーンについて詳しくは、<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">マイルストーンパスを作成</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Milestone] 行</td> 
   <td> <img src="assets/milestone-line-more-info-in-gantt-270x209.png" alt="milestone_line_more_info_in_gant.png" style="width: 270;height: 209;"> </td> 
   <td> <p>マイルストーンに関連付けられているタスクの後に線が表示されます。マイルストーンの上にポインタを合わせると、マイルストーンの名前と日付が表示されます。[!DNL Workfront] 管理者が、各マイルストーン行の色を決定します。</p> <p> マイルストーンに関して詳しくは、<a href="../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md" class="MCXref xref">マイルストーンパスを作成</a>を参照</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Predecessors]</td> 
   <td> <img src="assets/predecessor-2-269x200.png" alt="predecessor_2.png" style="width: 269;height: 200;"> </td> 
   <td> <p>2 つのタスク間の先行関係を示す、1 つのタスクから別のタスクへの行。先行タスク関係を個別にハイライト表示するには、その上にマウスを移動します。クリックすると、ハイライト表示されたままになります。先行タスク関係は、一度に 1 行だけハイライト表示できます。</p> <p>「<strong>[!UICONTROL Predecessor]</strong>」アイコンは、ガントチャート上の複数のページにまたがる先行タスク関係を持つタスク、またはプロジェクト間の先行タスク関係を持つタスクの横に表示されます。</p> <p><strong>[!UICONTROL Predecessor]</strong> アイコンをクリックして、すべての先行タスクと後続タスク、およびタスク名、先行タスクのタイプ、主要な日付など、各タスクの詳細を表示します。</p> <p>メモ：プロジェクトのリストの [!UICONTROL Gantt Chart] には、プロジェクトをまたいだ先行タスクに関する情報が表示されます。異なるプロジェクト間で先行タスク関係を作成する方法に関して詳しくは、<a href="../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md" class="MCXref xref">プロジェクト間の先行タスクを作成</a>を参照</p> <p>先行タスクに関して詳しくは、「<a href="../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md" class="MCXref xref">先行タスクを強制的に実行</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Progress Status]</td> 
   <td> <p>[!UICONTROL On Time]<img src="assets/task-on-time--oct.-2017.png" alt="task_on_time_Oct._2017.png"></p> <p>[!UICONTROL Behind]<img src="assets/task-behind--oct.-2017.png" alt="task_behind_Oct._2017.png"></p> <p>[!UICONTROL At Risk]<img src="assets/task-at-risk.png" alt="task_at_risk.png"></p> <p>遅延        <img src="assets/task-late-oct.2017.png" alt="task_late_Oct.2017.png"></p> </td> 
   <td> <p> </p> <p>特定のタスクの現在の進捗状況のステータス。 </p> <p>それぞれの [!UICONTROL Progress Status] タイプに関する詳細情報は、<a href="../../../manage-work/tasks/task-information/task-progress-status.md" class="MCXref xref">タスク [!UICONTROL Progress Status] の概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Projected Dates]</td> 
   <td> <img src="assets/gantt-projected-dates-272x152.png" alt="gantt_projected_dates.png" style="width: 272;height: 152;"> </td> 
   <td> <p>現在完了した作業と残りの作業量の合計に基づいて、[!UICONTROL Projected Start] および [!UICONTROL Completion dates] をマークする見込タイムライン。 </p> <p>見込み完了日に関して詳しくは、<a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">プロジェクト、タスクおよびイシューに関する [!UICONTROL Projected Completion Date] の概要</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 表示オプションを設定

1. [!UICONTROL ガントチャート]タスクリスト、または[!UICONTROL ガントチャート]プロジェクトリストに移動します。\
   [!UICONTROL ガントチャート]の場所に関して詳しくは、[[!UICONTROL ガントチャートの概要]](../../../manage-work/gantt-chart/use-the-gantt-chart/get-started-with-gantt.md)を参照してください。

1. （オプション）**[!UICONTROL 見込日に切り替え]**&#x200B;設定を選択し、タスクを[!UICONTROL 見込日]ごとに表示します。デフォルトでは、タスクは[!UICONTROL ガントチャート]の[!UICONTROL 予定日]ごとに表示されます。
1. 「オプション」アイコンをクリックして、**[!UICONTROL オプション]**&#x200B;ダイアログボックスを表示します。\
   ![Options.png](assets/options-350x129.png)

1. [!UICONTROL ガントチャート]に表示する「設定」オプションを選択します。

   >[!NOTE]
   > すべての「設定」オプションがプロジェクトリストの[!UICONTROL ガントチャート]で使用できるわけではありません。

1. [!UICONTROL ガントチャート]内の任意の場所をクリックして、**[!UICONTROL オプション]**&#x200B;ダイアログボックスを閉じます。
