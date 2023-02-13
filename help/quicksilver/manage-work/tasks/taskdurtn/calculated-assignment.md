---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: '期間タイプの概要：計算された割り当て'
description: 計算された割り当ては、Adobe Workfrontのタスクに設定できる期間の種類です。 Workfrontの期間のタイプに関する一般情報については、タスク期間の概要および期間のタイプを参照してください。
author: Alina
feature: Work Management
exl-id: 5f1f6109-5d54-4c3f-9aa5-dc6ce165a1cd
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 0%

---

# 期間タイプの概要：計算された割り当て

計算された割り当ては、Adobe Workfrontのタスクに設定できる期間の種類です。 Workfrontの期間のタイプに関する一般情報については、 [タスクの期間と期間のタイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## 計算された割り当て期間タイプの概要

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This Hub issue has a powerpoint that highlights information that is useful to users when using Calculated Assignment duration type. I don't think we can use the powerpoint, because it's old. I also don't know if the things they discuss are still relevant, since the PP is from 2015. I've closed the issue, but I'm putting a link here just in case the info is useful. https://hub.workfront.com/issue/5a9dd7d5007d02a8966014557c23cc89/updates)</p>
-->

* 「割り当て期間タイプの計算」を使用する場合は、タスクの「期間」と「予定時間数」の両方を指定する必要があります。 次に、Workfrontは、計画時間数を期間内の時間数で割り、タスクに割り当てられたリソース数で割り当て率（割り当ての計算）を各リソースに対して計算します。 各リソースの配分率は同じ値になります。 この場合、各リソースの配分値を変更することはできません。
* Workfrontまたはグループ管理者は、システムまたはグループのデフォルトの期間タイプを計算割り当てに設定できます。 この場合、すべての新しいタスクは、この期間タイプで作成されます。 システムレベルまたはグループレベルのプロジェクト環境設定の一部として、タスクや問題の環境設定を変更する方法については、 [システム全体のタスクと問題の環境設定を構成](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

   この場合、タスクのデフォルトは「期間」が 1 日、デフォルトは「予定時間」が 0 時間になります。 プロジェクトマネージャがより正確な「期間」を設定し、「計画時間」フィールドに実際の見積もりを入力しない限り、リソースは未割り当てと表示されます。

次の状況では、「計算された割り当て」が推奨される期間の種類です。

* 割り当てにアクティビティウィンドウがあるが、割り当てられた期間全体を費やして作業を完了しない場合。 例えば、週の終わりまでにレポートをスーパーバイザーに配信するように割り当てられているとします。 期間は 5 日ですが、ドキュメントの下書きには 10 時間しかかかりません。
* 1 つのリソースがタスクに割り当てられる場合、プロジェクトマネージャは、計画期間と計画作業量を互いに関係なく見積もることができます。

   同じ結果に対して [ 計算された作業時間の期間の種類 ] を使用できますが、計画時間の計算値に影響を与えるには、プロジェクトマネージャがリソースの割合配分を入力する必要があります。 これにより、プロジェクトの計画がより難しく、時間がかかります。

各リソースの割り当て率は、次のように計算されます。

```
Planned Hours / Duration / Number of Resources = Allocation Percentage for each resource
```

例えば、以下に示すシナリオでは、各タスクの期間は 3 日です。 プロジェクト・マネージャは、「期間」（3 日または 24 時間）と「計画時間」の両方を手動で入力し、その結果、割り当て率（または割り当て率）が次のように計算されます。

![](assets/calcassign-350x80.png)

## タスクの期間の種類を計算割り当てに変更する

タスクの期間の種類の変更について詳しくは、 [タスクの期間タイプの更新](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3">Select <strong>Calculated Assignment</strong> from the drop-down menu.</li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong>.</li>
</ol>
-->
