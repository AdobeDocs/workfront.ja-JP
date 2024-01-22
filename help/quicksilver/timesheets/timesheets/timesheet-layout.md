---
content-type: overview
product-area: timesheets
navigation-topic: timesheets-navigation-topic
title: タイムシートレイアウトの概要
description: この記事では、Adobe Workfrontのタイムシートのレイアウトについて説明し、タイムシートをカスタマイズして時間を記録する方法をより深く理解できます。
author: Alina
feature: Timesheets
exl-id: 31c48a50-5235-495c-8e46-0974ed98ede1
source-git-commit: 71d5e15c38b26b9a833ac2418d5782afd249a24c
workflow-type: tm+mt
source-wordcount: '1049'
ht-degree: 1%

---

# タイムシートレイアウトの概要

<!-- Audited: 12/2023 -->

この記事では、Adobe Workfrontのタイムシートのレイアウトについて説明し、タイムシートをカスタマイズして時間を記録する方法をより深く理解できます。

タイムシートと時間の基本設定は、タイムシートに表示する内容を制御します。 この記事では、利用可能なすべてのオプションの概要を説明します。 オプションの選択について詳しくは、 [タイムシートと時間の基本設定を構成する](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

タイムシートの時刻を記録する方法については、 [ログ時間](../../timesheets/create-and-manage-timesheets/log-time.md).

![タイムシートのレイアウト](assets/timesheet-layout-unshimmed.png)

タイムシートの領域は次のとおりです。

* [タイムシートヘッダー](#timesheet-header)
* [左側のパネル](#the-left-panel)
* [作業項目](#work-items)
* [ツール バー](#toolbar)
* [タイムシートのフッター](#timesheet-footer)
* [ジョブの役割](#job-role)
* [時間タイプ](#hour-type)
* [左側のパネルの更新領域](#updates-area-in-the-left-panel)
* [概要パネル](#summary-panel)
* [時間枠と時間入口領域](#time-frame-and-hour-entry-area)
* [時間入力コメント](#hour-entry-comments)
* [時間](#hours)
* [合計](#totals)

## タイムシートヘッダー

![タイムシートヘッダー](assets/timesheet-title-unshimmed-redesign.png)

タイムシートヘッダーには、次の情報が含まれます。

* タイムシートの期間。
* 「アクション」領域には、次のものが含まれます。
   * [ お気に入り ] の一覧にタイムシートを追加する星形のアイコン。
   * タイムシートを削除できる [ 削除 ] オプションを含む [ その他 ] アイコン。
* タイムシートの所有者の名前。
* タイムシートに表示される項目に関して記録された時間の合計時間数。
* 残業時間数。 これは手動のエントリで、 **残業** の設定は、タイムシートで有効になっています。 詳しくは、 [タイムシート情報の編集](../create-and-manage-timesheets/edit-timesheets.md).

>[!TIP]
>
>タイムシートの現在の合計時間よりも長い時間の超過を記録することはできません。 たとえば、これまでにタイムシートに 7 時間記録した場合、8 時間の残業を記録することはできません。

* タイムシートの状態。

## 左側のパネル

![タイムシートの左パネル](assets/timesheet-left-panel-unshimmed-redesign.png)

次のセクションには、左側のパネルでアクセスできます。

* **タイムシート**：実際のタイムシートを表示します。
* **更新**：タイムシートのコメントとシステム更新を表示します。 詳しくは、 [左側のパネルの更新領域](#updates-area-in-the-left-panel) 」の節を参照してください。

## 作業項目

![タイムシートの作業項目](assets/timesheet-object-names-unshimmed-redesign.png)

作業項目は、時間を記録するプロジェクト、タスクおよび問題です。 ヘッダー行の下向き矢印をクリックすると、プロジェクトと、その下に表示されるタスクと問題が折りたたまれます。 プロジェクト名の横にある下向き矢印をクリックすると、そのプロジェクトの作業項目が折りたたまれます。

タイムシート外で時間が記録されるタスク、タスク、タスク、およびプロジェクト、またはタイムシートの期間中に予定された項目は、ここに自動的に表示されます。

## ツール バー

![タイムシートツールバー](assets/timesheet-toolbar-unshimmed-redesign.png)

ツールバーには次のオプションが含まれます。

* The **項目を追加** ボタンをクリックして、プロジェクト、タスクまたはタスクを追加できます。
* タイムシートのタスクまたは問題を検索するクイックフィルタアイコン。
* The **コメントを表示** プロジェクト、タスク、または発行時間のエントリで記録された時間コメントの表示/非表示を切り替える設定です。
* タイムシートをフルスクリーンモードで表示するためのフルスクリーンアイコン。
* The **概要を開く** ( または **概要を閉じる**) ボタンをクリックして Summary パネルを開くか閉じて、タスクや問題に関する追加情報を表示します。 このボタンは、プロジェクトでは使用できません。

詳しくは、 [ログ時間](../create-and-manage-timesheets/log-time.md).

## タイムシートのフッター

![タイムシートのフッター](assets/timesheet-footer-unshimmed-redesign.png)

次の項目をクリックします。 **承認用に送信**, **閉じる**, **承認**、および **拒否** この領域のボタンを使用して、タイムシートの承認を閉じるか拒否します。

この領域には、タイムシートが最後に保存された日時に関する情報も含まれます。 タイムシートの情報に対して行った変更はすべて自動的に保存されます。

## 担当業務

![ジョブの役割](assets/timesheet-job-role-area-unshimmed-redesign.png)

時間エントリに関連付ける別の役割を選択できます。 Workfront管理者が **時間エントリへのジョブロールの割り当て** を手動で設定します。 タスクに割り当てられたとき、またはタスクに問題が発生したときに指定されたジョブの役割がデフォルトで表示されます。 タスクまたは問題に対してプライマリの役割が割り当てられていない場合は、「ジョブの役割」がデフォルトとして表示されます。 詳しくは、 [タイムシートと時間の基本設定を構成する](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

異なるロールの同じ作業項目に対して、複数の時間エントリを記録できます。 詳しくは、 [ログ時間](../create-and-manage-timesheets/log-time.md).

## 時間タイプ

![時間タイプ](assets/timesheet-hour-type-unshimmed-redesign.png)

各項目の時間エントリに関連付ける時間タイプを選択できます。 このフィールドは、Workfront管理者がお使いの環境で有効にした場合にのみ表示されます。 詳しくは、 [タイムシートと時間の基本設定を構成する](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

異なる時間タイプの同じ作業項目に対して、複数の時間エントリを記録できます。 詳しくは、 [ログ時間](../create-and-manage-timesheets/log-time.md).

## 左側のパネルの更新領域

![左側のタイムシートパネルの更新領域](assets/timesheet-updates-section-unshimmed-redesign.png)

タイムシートにコメントを付けて、タイムシートの左側のパネルにある [ 更新 ] セクションで、タイムシートの承認者や他のユーザーと連絡を取ることができます。

タイムシートに対して行われたコメントは、この領域に表示されます。

## 概要パネル

![概要パネル](assets/timesheet-summary-panel-for-task-unshimmed-redesign.png)

タイムシートに表示されたタスクや問題に関する [ 概要 ] パネルにアクセスできます。 ここから、タスクや問題に対するコメントを作成したり、その情報を更新したりできます。 詳しくは、 [概要の概要](../../workfront-basics/the-new-workfront-experience/summary-overview.md).

タイムシートの [ 概要 ] パネルに入力した作業項目に対するコメントは、タスクまたは懸案事項の [ 更新 ] 領域に表示されます。 Summary パネルは、プロジェクトでは使用できません。

## 時間枠と時間入口領域

![タイムシートの期間](assets/timesheet-time-frame-log-time-area.png)

タイムシートの期間は、作業項目の右側に表示されます。

1 週間、2 週間、4 週間のタイムシートを作成できます。

期間は 1 週間単位で表示されます。 指定したタイムシート期間外の日数は淡色表示になります。 タイムシートの期間外の日の時間は記録できません。

詳しくは、 [単一使用のタイムシートを作成する](../create-and-manage-timesheets/create-tmshts.md) または [タイムシートプロファイルの作成、編集、割り当て](../create-and-manage-timesheets/create-timesheet-profiles.md).

<!--drafted for the resize columns in timesheets story - make this blurb a TIP when the story is released: 
You can resize the columns that display different weeks, the time frame, or the work item areas by dragging and dropping the vertical lines that separate them.-->

## 時間入力コメント

![時間入力コメント](assets/timesheet-hour-entry-comment-button-unshimmed-redesign.png)

タイムシートに追加する 1 時間ごとのエントリにコメントを追加できます。

時間入力のコメントボックスに入力したコメントは、タイムシートの各作業項目の下に表示され、タイムシートで、 **コメントを表示** 設定が有効になっている場合、ツールバーで有効になります。

![](assets/hour-entry-comment-under-task-in-timesheet-unshimmed-redesign.png)

## 時間

![タイムシート時間](assets/timesheet-hours-area-unshimmed-redesign.png)

タイムシートは、各作業項目とタイムシート範囲の日付に対する入力フィールドを提供し、項目の作業に費やした時間を記録します。 時刻を記録する際、時刻を記録する項目は、明るい青でハイライト表示され、時刻ボックスは暗い青でアウトライン表示されます。

## 合計

![タイムシートの合計](assets/timesheet-totals-column-and-header-unshimmed-redesign.png)

タイムシートに入力された全時間の合計を、日別（タイムシートのヘッダー）およびオブジェクト別（最後の列）にまとめて確認します。
