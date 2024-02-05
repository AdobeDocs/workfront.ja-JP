---
product-area: projects
navigation-topic: task-information
title: タスクの標準化遅延の更新
description: プロジェクトのタスクスケジュール間に競合が生じる場合があります。リソースとタスクを再スケジュールして、すべてのタスクを現実的なスケジュール内で完了できるように、リソースを標準化したり、リソースの競合に対処したりできます。タスクの標準化について詳しくは、ガントチャートのリソースの標準化を参照してください。
author: Alina
feature: Work Management
exl-id: 6695448c-76ce-460c-aa59-63a3d5e2e18d
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 100%

---

# タスクの標準化遅延の更新

プロジェクトのタスクスケジュール間に競合が生じる場合があります。リソースとタスクを再スケジュールして、すべてのタスクを現実的なスケジュール内で完了できるように、リソースを標準化したり、リソースの競合に対処したりできます。タスクの標準化について詳しくは、[ガントチャートのリソースの標準化](../../../manage-work/gantt-chart/use-the-gantt-chart/level-resources-in-gantt.md)を参照してください。

プロジェクトマネージャーまたはタスクの担当者として、個々のタスクに標準化の遅延を追加して、リソースまたはスケジュールの競合を考慮することもできます。つまり、Adobe Workfront のレベルでタスクをより現実的なスケジュールに従ってリソースの競合を回避するために、遅延を伴ってタスクをスケジュールする場合があります。

タスクに標準化の遅延を追加すると、タスクの完了予定日が調整されます。完了予定日について詳しくは、[プロジェクト、タスクおよびイシューに関する予定完了日の概要](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>ワークまたはそれ以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タスクおよびプロジェクトへのアクセスを編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクに対する権限の管理 </p> <p>プロジェクトへの参加権限またはそれ以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## タスクへの標準化の延期の追加

1. 標準化の延期を追加するタスクに移動します。
1. タスク名の右側ある&#x200B;**その他のアイコン**&#x200B;をクリックして、「**編集**」をクリックします。

1. 「**設定**」をクリックします。

   ![](assets/leveling-delay-edit-task-nwe-350x345.png)

1. 時間単位で、「**標準化の遅延**」を指定して、時間の単位を選択します。\
   リソースの競合が原因で、リソースがタスクの開始を遅らせる時間です。

   時間の単位に対して、次のオプションから選択します。

   * 分
   * 時間.これがデフォルトです。
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

 
