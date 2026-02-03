---
product-area: projects
navigation-topic: task-information
title: タスクの標準化の遅延の更新
description: プロジェクトのタスクスケジュール間に競合が生じる場合があります。リソースとタスクを再スケジュールして、すべてのタスクを現実的なスケジュール内で完了できるように、リソースを標準化したり、リソースの競合に対処したりできます。タスクの標準化について詳しくは、ガントチャートのリソースの標準化を参照してください。
author: Alina
feature: Work Management
exl-id: 6695448c-76ce-460c-aa59-63a3d5e2e18d
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 90%

---

# タスクの標準化遅延の更新

プロジェクトのタスクスケジュール間に競合が生じる場合があります。リソースとタスクを再スケジュールして、すべてのタスクを現実的なスケジュール内で完了できるように、リソースを標準化したり、リソースの競合に対処したりできます。タスクの標準化について詳しくは、[ガントチャートのリソースの標準化](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md)を参照してください。

プロジェクトマネージャーまたはタスクの担当者として、個々のタスクに標準化の遅延を追加して、リソースまたはスケジュールの競合を考慮することもできます。つまり、Adobe Workfrontでタスクを平準化するときに、より現実的なスケジュールでリソースの競合を解決できるように、タスクが遅れてスケジュールされる場合があります。

タスクに標準化の遅延を追加すると、タスクの完了予定日が調整されます。完了予定日について詳しくは、[プロジェクト、タスクおよびイシューに関する予定完了日の概要](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p>
   <p>Work またはそれ以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>タスクおよびプロジェクトへのアクセスを編集</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクに対する権限の管理 </p> <p>プロジェクトへの参加権限またはそれ以上の権限</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to Tasks </p> <p>Contribute or higher permissions to Projects</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## タスクへの標準化の延期の追加

1. 標準化の延期を追加するタスクに移動します。
1. タスク名の右側ある&#x200B;**その他のアイコン**&#x200B;をクリックして、「**編集**」をクリックします。

1. 「**設定**」をクリックします。

   ![&#x200B; タスク編集時の標準化の遅延 &#x200B;](assets/leveling-delay-edit-task-nwe-350x345.png)

1. 時間単位で、「**標準化の遅延**」を指定して、時間の単位を選択します。\
   リソースの競合が原因で、リソースがタスクの開始を遅らせる時間です。

   時間の単位に対して、次のオプションから選択します。

   * 分
   * 時間。 これがデフォルトです。
   * 日
   * 週
   * 月
   * 経過時間数 (分)
   * 経過時間数
   * 経過日数
   * 経過週数
   * 経過月数

   >[!TIP]
   >
   >経過時間は、タスクの期間の時間単位です。タスクの予定開始日から予定完了日までの時間で、休日、週末および休暇を含みます。つまり、経過時間はカレンダーの日数の経過です。

1. 「**保存**」をクリックします。


