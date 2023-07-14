---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: タスク制約の概要
description: タスクの制約は、タスクをプロジェクトで開始および終了するタイミングを決定します。
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '684'
ht-degree: 6%

---

# タスク制約の概要

タスクの制約は、タスクをプロジェクトで開始および終了するタイミングを決定します。

## タスク制約の概要

プロジェクト計画を立てる際には、プロジェクト上のタスクの順序と時間枠を決定します。 タスクは、どのタスクシーケンスとも独立して機能できますが、プロジェクトタイムラインに影響を与える場合があります。 タスク制約を使用すると、プロジェクトマネージャは、特定のタスクをプロジェクト上で開始または完了できるタイミングを計画できます。

使用する制約に応じて、タスクに対して「計画開始日」、「計画完了日」、またはその両方を指定する必要があります。

定義済みの日付を必要とする制約タイプは、先行関係に影響を与えます。

>[!TIP]
>
>タスク間で先行タスクの関係を使用する場合は、特定の日付を必要としない制約タイプを使用することを検討します。

次の表に、各拘束とその省略形を示します。 省略形は、タスクリストと Kick-Start インポートファイルの作成時に使用されます。 制約の種類の詳細については、各タスク制約のリンクされたタイトルをクリックしてください。

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col>
 <thead> 
  <tr> 
   <th> <p><strong>制約名</strong> </p> </th> 
   <th> <p><strong>省略形</strong> </p> </th> 
   <th> <p><strong>説明</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-soon-as-possible.md" class="MCXref xref">タスク制約の概要：できるだけ早く</a> </p> </td> 
   <td scope="col"> <p>ASAP</p> </td>
   <td scope="col"> <p>タスクの開始時刻を、できるだけプロジェクトの開始時刻に近い位置に配置します。</p> 
   <p>プロジェクトで「開始日からのスケジュール・モード」を使用し、新しいタスクのシステムのデフォルトの開始日が「プロジェクト計画日に基づく」に設定されている場合は、デフォルトの制約です。 </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">タスク制約の概要：できるだけ遅く </a> </p> </td> 
   <td scope="col"> <p>ALAP</p> </td> 
   <td scope="col"> <p>タスクの完了時間を、できるだけプロジェクトの終わり近くに配置します。</p> 
   <p>これは、プロジェクトスケジュールモードが「完了日」からで、タスクの開始日のシステムまたはグループのデフォルトが「プロジェクト計画日に基づく」の場合のデフォルトの制約です。 </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">タスク制約の概要：最古の利用可能時間</a> </p> </td> 
   <td scope="col"> <p>EAT</p> </td> 
 <td scope="col"> <p>先行タスクの関係を考慮した後、使用可能な最も早い時間にタスクをスケジュールします。</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">タスク制約の概要：最新の利用可能時間</a> </p> </td> 
   <td scope="col"> <p>LAT</p> </td> 
   <td scope="col"> <p>プロジェクト内の前任者と後続者の関係を考慮した後、利用可能な最新の時間にタスクを開始するようにスケジュールします。</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">タスク制約の概要：次の日までに開始</a> </p> </td> 
   <td scope="col"> <p>SNET</p> </td> 
   <td scope="col"> <p>指定した日付の後に開始するタスクをスケジュールします。</p> 
   <p>プロジェクトの [ スケジュールモード ] が [ 開始日 ] から、新しいタスクの既定の [ 開始日 ] が [ 今日 ] に設定されている場合は、既定の制約です。   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">タスク制約の概要：次の日までに開始</a> </p> </td> 
   <td scope="col"> <p>SNLT</p> </td> 
   <td scope="col"> <p>指定した日付より前に開始するようにタスクをスケジュールします。</p> 
   <p>プロジェクトの [ スケジュールモード ] が [ 完了日 ] からで、タスクの [ 開始日 ] の既定が [ 今日 ] の場合は、既定の制約が設定されます。 
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">タスク制約の概要：次よりも前に完了</a> </p> </td> 
   <td scope="col"> <p>FNET</p> </td>
   <td scope="col"> <p>指定した日付以降にタスクを完了するようにスケジュールを設定します。</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">タスク制約の概要：次の日までに完了</a> </p> </td> 
   <td scope="col"> <p>FNLT</p> </td> 
   <td scope="col"> <p>指定した日付より前にタスクを完了するようにスケジュールを設定します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">タスク制約の概要：開始日</a> </p> </td> 
   <td scope="col"> <p>MSO</p> </td> 
   <td scope="col"> <p>特定の日付に正確に開始するようにタスクをスケジュールします。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">タスク制約の概要：終了日</a> </p> </td> 
   <td scope="col"> <p>MFO</p> </td> 
   <td scope="col"> <p>特定の日付に終了するようにタスクをスケジュールします。</p> </td>
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">タスク制約の概要：固定日付</a> </p> </td> 
   <td> <p>FIXT</p> </td> 
   <td> <p>特定の日付に開始および終了するタスクをスケジュールします。</p> </td> 
  </tr> 
 </tbody> 
</table>

## デフォルト制約の概要

新しいタスクを作成すると、Workfrontによってタスク制約が自動的に選択されます。

Workfrontは、2 つの変数を使用して、新しいタスクに対してデフォルトで選択されるタスク制約を決定します。

* この **プロジェクトスケジュールの開始日** フィールドに値を入力します。

  [ プロジェクトスケジュールの開始 ] フィールドの詳細については、 [プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md).

* この **開始日** Workfrontまたはグループ管理者が、 **タスクと問題** ～の面積 **設定**.

  タスクとタスクの環境設定について詳しくは、 [システム全体のタスクと問題の環境設定を構成](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

次の表に、プロジェクトと新しいタスクに対して異なる変数を選択する場合の既定のタスク制約を示します。

| プロジェクトスケジュールの開始日 | タスク開始日 | タスク制約のデフォルト |
|---|---|---|
| 開始日 | プロジェクト予定日に基づく | できるだけ早く |
| 開始日 | 今日 | 指定日以後に開始 |
| 完了日 | プロジェクト予定日に基づく | できるだけ遅く |
| 完了日 | 今日 | 指定日までに開始 |
