---
content-type: overview
product-area: projects
navigation-topic: task-constraints
title: タスクの制約の概要
description: タスクの制約は、プロジェクト上でタスクを開始および終了するタイミングを決定します。
author: Alina
feature: Work Management
exl-id: 91b0844b-95a3-4d18-9fdb-a907dd42e1bf
source-git-commit: 91d757513792604677d6285baafa795629b4506d
workflow-type: tm+mt
source-wordcount: '691'
ht-degree: 77%

---

# タスクの制約の概要

<!-- Audited: 12/2023 -->

タスクの制約は、プロジェクト上でタスクを開始および終了するタイミングを決定します。

## タスク制約の概要

プロジェクト計画を立てる際には、プロジェクト上のタスクの順序と時間枠を決定します。タスクは、どのタスクシーケンスとも独立して機能できますが、プロジェクトタイムラインに影響を与える場合があります。タスク制約を使用すると、プロジェクトマネージャーは、特定のタスクをプロジェクト上で開始または完了できるタイミングを計画できます。

使用する制約に応じて、タスクに対して予定開始日、予定完了日、またはその両方を指定する必要があります。

定義された日付を必要とする制約タイプは、先行タスクの関係に影響を与えます。

>[!TIP]
>
>タスク間で先行タスク関係を使用する場合は、特定の日付を必要としない制約タイプを使用することを検討します。

次の表に、各制約とその省略形を示します。省略形は、タスクリスト上や、キックスタート読み込みファイルの作成時に使用されます。制約タイプについて詳しくは、各タスク制約のリンクされたタイトルをクリックしてください。

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
   <td scope="col"> <p>タスクの開始時間を、プロジェクトの開始時間にできるだけ近づけます。</p> 
   <p>プロジェクトで開始日からのスケジュールモードを使用し、新規タスクのシステムのデフォルトの開始日が「プロジェクト予定日に基づく」に設定されている場合、これがデフォルトの制約になります。 </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/as-late-as-possible.md" class="MCXref xref">タスク制約の概要：できるだけ遅く</a> </p> </td> 
   <td scope="col"> <p>ALAP</p> </td> 
   <td scope="col"> <p>タスクの完了時間を、できるだけプロジェクトの終了に近づけます。</p> 
   <p>これは、プロジェクトスケジュールモードが「完了日」からで、タスクの開始日のシステムまたはグループのデフォルトが「プロジェクト計画日に基づく」に設定されている場合のデフォルトの制約です。 </p>
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/earliest-available-time.md" class="MCXref xref">タスク制約の概要：最も早い空き時間</a> </p> </td> 
   <td scope="col"> <p>EAT</p> </td> 
 <td scope="col"> <p>先行タスクの関係を考慮した後で、最も早い空き時間にタスクを開始するようスケジュール設定します。</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/latest-available-time.md" class="MCXref xref">タスク制約の概要：最も遅い空き時間</a> </p> </td> 
   <td scope="col"> <p>LAT</p> </td> 
   <td scope="col"> <p>プロジェクト内の先行者と後続者の関係を考慮した後に、利用可能な最新の時間にタスクを開始するようにスケジュールを設定します。</p> </td>
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-earlier-than.md" class="MCXref xref">タスク制約の概要：指定日以後に開始</a> </p> </td> 
   <td scope="col"> <p>SNET</p> </td> 
   <td scope="col"> <p>指定した日付より後にタスクを開始するようスケジュール設定します。</p> 
   <p>プロジェクトのスケジュールモードが開始日からで、新規タスクのデフォルトの開始日が「今日」に設定されている場合のデフォルトの制約です。   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/start-no-later-than.md" class="MCXref xref">タスク制約の概要：指定日までに開始</a> </p> </td> 
   <td scope="col"> <p>SNLT</p> </td> 
   <td scope="col"> <p>指定した日付より前にタスクを開始するようスケジュール設定します。</p> 
   <p>プロジェクトのスケジュールモードが [ 完了日 ] からで、タスクの [ 開始日 ] が [ 今日 ] に設定されている場合は、既定の制約です。 
   </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-earlier-than.md" class="MCXref xref">タスク制約の概要：これよりも早く終了しない</a> </p> </td> 
   <td scope="col"> <p>FNET</p> </td>
   <td scope="col"> <p>指定した日付より後にタスクを完了するようスケジュール設定します。</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"> <p><a href="../../../manage-work/tasks/task-constraints/finish-no-later-than.md" class="MCXref xref">タスク制約の概要：これよりも遅く終了しない</a> </p> </td> 
   <td scope="col"> <p>FNLT</p> </td> 
   <td scope="col"> <p>指定した日付より前にタスクを完了するようスケジュール設定します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-start-on.md" class="MCXref xref">タスク制約の概要：指定日に開始</a> </p> </td> 
   <td scope="col"> <p>MSO</p> </td> 
   <td scope="col"> <p>指定した日付に正確にタスクを開始するようスケジュール設定します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/must-finish-on.md" class="MCXref xref">タスク制約の概要：指定日に終了</a> </p> </td> 
   <td scope="col"> <p>MFO</p> </td> 
   <td scope="col"> <p>指定した日付にタスクを終了するようスケジュール設定します。</p> </td>
  </tr> 
  <tr> 
   <td> <p><a href="../../../manage-work/tasks/task-constraints/fixed-dates.md" class="MCXref xref">タスク制約の概要：固定日付</a> </p> </td> 
   <td> <p>FIXT</p> </td> 
   <td> <p>特定の日付で開始および終了するタスクをスケジュールします。</p> </td> 
  </tr> 
 </tbody> 
</table>

## デフォルト制約の概要

新規タスクを作成すると、Workfront によってタスクの制約が自動的に選択されます。

Workfrontは、2 つの変数を使用して、新しいタスクに対してデフォルトで選択されるタスク制約を決定します。

* プロジェクトの「**プロジェクトスケジュールの開始日**」フィールド。

  「プロジェクトスケジュールの開始日」フィールドについて詳しくは、[プロジェクトの編集](../../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。

* Workfront またはグループ管理者が、**設定**&#x200B;の&#x200B;**タスクとイシュー**&#x200B;エリアで設定した&#x200B;**開始日**&#x200B;環境設定。

  タスクと問題の環境設定について詳しくは、 [新規タスクのデフォルト](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md#new-task-defaults) のセクション [システム全体のタスクと問題の環境設定を構成する](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

次の表に、プロジェクトおよび新規タスクに対して異なる変数を選択する場合のデフォルトのタスクの制約を示します。

| プロジェクトスケジュールの開始日 | タスクの開始日 | タスクの制約のデフォルト |
|---|---|---|
| 開始日 | プロジェクト予定日に基づく | できるだけ早く |
| 開始日 | 今日 | 指定日以降に開始 |
| 完了日 | プロジェクト予定日に基づく | できるだけ遅く |
| 完了日 | 今日 | 指定日までに開始 |
