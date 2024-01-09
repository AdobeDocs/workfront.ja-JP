---
content-type: overview
product-area: projects
navigation-topic: task-information
title: タスクトラッキングモードの概要
description: タスクを作成または編集する際に、タスクの追跡モード設定を調整して、タスクの進捗状況ステータスインジケーターの表示方法と表示タイミングを制御できます。 Adobe Workfrontでは、タスクの進捗状況を追跡するための特定の設定を行うと、進捗状況ステータスフラグが表示されます。
author: Alina
feature: Work Management
exl-id: 397b5593-ac01-40cf-b683-fcf671a53d26
source-git-commit: d2836549ee3c615201ce5f3454258e9af31efa42
workflow-type: tm+mt
source-wordcount: '646'
ht-degree: 2%

---

# タスクトラッキングモードの概要

<!-- Audited: 01/2024 -->

タスクを作成または編集する際に、タスクの追跡モード設定を調整して、タスクの進捗状況ステータスインジケーターの表示方法と表示タイミングを制御できます。 Adobe Workfrontでは、タスクの進捗状況を追跡するための特定の設定を行うと、進捗状況ステータスフラグが表示されます。

タスクの進捗状況ステータスについて詳しくは、 [タスクの進捗状況ステータスの概要](../../../manage-work/tasks/task-information/task-progress-status.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set Tracking Mode for tasks</h2>
<p>(NOTE: drafted, because we created a new article and linked it below. Left this article as a "Overview" article only.) </p>
<p>To set the tracking mode:</p>
<ol>
<li value="1">Go to the task you want to set the tracking mode for.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the <strong>More</strong> icon <img src="assets/qs-more-icon-on-an-object.png">next to the name of the task, then click&nbsp;<strong>Edit</strong>.</p> <p>The Edit Task dialog box opens. </p> </li>
<li value="3"> <p>In the&nbsp;<strong>Settings</strong> section, use the&nbsp;<strong>Tracking Mode</strong> drop-down menu to select the Tracking Mode for the task.</p> <p>For more information about the tracking mode options, see the <a href="#tracking-mode-options" class="MCXref xref" xrefformat="{para}">Tracking Mode options</a> section in this article. </p> </li>
<li value="4">Click&nbsp;<strong>Save Changes.</strong></li>
</ol>
</div>
-->

## トラッキングモードのオプション {#tracking-mode-options}

タスクの所有者またはプロジェクトマネージャーは、各タスクの進捗状況の状態をWorkfrontが示す方法を選択できます。 タスクにトラッキングモードを設定する方法について詳しくは、 [タスクのトラッキングモードの設定](../../../manage-work/tasks/task-information/set-tracking-mode-for-tasks.md).

次のオプションから選択できます。

* [ユーザーは更新する必要があります](#user-must-update)
* [予定通り](#assume-on-time)
* [遅延警告を無視](#ignore-late-warnings)
* [オートコンプリート](#auto-complete)
* [先行タスク](#predecessor)

### ユーザーが更新する必要あり {#user-must-update}

このオプションを選択すると、Workfrontはタスクの完了率と実績時間を記録して、タスクの進捗状況ステータスを判断します。 これはデフォルトのオプションです。

### 予定通りを想定 {#assume-on-time}

Workfrontは、現在の完了ステータスに関係なく、タスクが時間通りに完了すると想定します。 タスクが（計画完了日に）予定どおりに完了しない場合、Workfrontは次の稼働日の計画完了日を自動的に仮定します。 タスクが完了するタイミングを指定する必要があります。 ユーザーが定期的にタスクを更新しない場合に、このオプションを使用します。

### 遅延警告を無視 {#ignore-late-warnings}

タスクの進捗状況ステータスは、[ 遅延 ] になるまで [ オンタイム ] になります。 例えば、10 日間のタスクをスケジュールし、完了する日にタスクの完了率が 60%と表示される場合、Workfrontは 4 日間を追加して完了予定日を更新し、タスクの進捗状況ステータスは「遅延」になります。

### 自動完了 {#auto-complete}

Workfrontは、タスクが予定どおりに完了し、期限または計画完了日に完了とマークされると仮定します。 それまでは、Workfrontは「完了率」と「実際のログ時間」を使用して、進捗状況ステータスを判断します。 ただし、Workfrontでは、予定完了日より前の進捗状況ステータスに関係なく、タスクが完了したとマークします。

次の例外が存在します。

* タスクに未完了の先行タスクがある場合、先行タスクがすべて完了するまで、自動的に完了しません。 先行タスクを適用する必要があります。
* タスクに固定日付の制約がある場合、先行タスクが完了しているかどうかに関係なく、タスクは常に計画完了日に完了します。

>[!IMPORTANT]
>
>タスクを自動完了するように選択すると、プロジェクト時間が再計算されたときにタスクが [ 完了 ] と表示されます。 プロジェクトの [ 更新の種類 ] が [ 自動 ] または [ 自動 ] に設定され、[ 変更時 ] に設定されている場合、プロジェクトのタイムラインは毎日計算されます。 プロジェクトでのタイムライン再計算の詳細については、 [プロジェクトタイムラインを再計算](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).
>
>実際の完了日の時刻は、タイムラインが自動的に計算される日の午前 0 時です。 このタイムスタンプの生成に使用される時間は、Workfront管理者がセットアップの「顧客情報」セクションで定義したシステムのタイムゾーンです。 システムのタイムゾーンの設定については、 [システムの基本情報を設定する](../../../administration-and-setup/get-started-wf-administration/configure-basic-info.md).

### 先行タスク {#predecessor}

Workfrontは、先行タスクの関係に基づいて、タスクの完了予定日を見積もります。 タスクの進捗状況ステータスは、この見積もりに基づいて決定されます。 たとえば、タスク B の期間は 1 日で、先行タスク A の 2 日後に完了するようにスケジュールされています。この処理には 5 日かかります。 次に、ユーザーがタスク B を 50%完了に更新しますが、先行タスク A はまだ開始されていません。 Workfrontは、先行タスクの開始日から 6 日後にタスク B を完了にスケジュールし、タスク A に 5 日、タスク B に 1 日を割り当てます。
