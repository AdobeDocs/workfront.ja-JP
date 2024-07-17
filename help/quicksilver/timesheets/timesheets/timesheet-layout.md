---
content-type: overview
product-area: timesheets
navigation-topic: timesheets-navigation-topic
title: タイムシートレイアウトの概要
description: この記事では、Adobe Workfront のタイムシートのレイアウトについて説明します。タイムシートをカスタマイズして利用し、時間を記録する方法をより深く理解できます。
author: Alina
feature: Timesheets
exl-id: 31c48a50-5235-495c-8e46-0974ed98ede1
source-git-commit: 4c17466705873b06e7ea7bb08bb78a7e68078f8b
workflow-type: tm+mt
source-wordcount: '1049'
ht-degree: 100%

---

# タイムシートレイアウトの概要

<!-- Audited: 12/2023 -->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers or in Production for customers who enabled fast releases. </span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release schedule, see [Second Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>-->

この記事では、Adobe Workfront のタイムシートのレイアウトについて説明します。タイムシートをカスタマイズして利用し、時間を記録する方法をより深く理解できます。

「タイムシートおよび時間設定」は、タイムシートに表示される内容を制御します。この記事では、利用可能なすべてのオプションの概要を説明します。オプションの選択については、[タイムシートおよび時間設定の指定](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)を参照してください。

タイムシートで時刻を記録する方法については、[時間の記録](../../timesheets/create-and-manage-timesheets/log-time.md)を参照してください。

![タイムシートのレイアウト](assets/timesheet-layout-unshimmed.png)

タイムシートのエリアは次のとおりです。

* [タイムシートのヘッダー](#timesheet-header)
* [左パネル](#the-left-panel)
* [作業項目](#work-items)
* [ツール バー](#toolbar)
* [タイムシートのフッター](#timesheet-footer)
* [担当業務](#job-role)
* [時間タイプ](#hour-type)
* [左パネルの更新エリア](#updates-area-in-the-left-panel)
* [概要パネル](#summary-panel)
* [時間枠と時間エントリエリア](#time-frame-and-hour-entry-area)
* [時間エントリのコメント](#hour-entry-comments)
* [時間](#hours)
* [合計](#totals)

## タイムシートのヘッダー

![タイムシートのヘッダー](assets/timesheet-title-unshimmed-redesign.png)

タイムシートのヘッダーには、次の情報が含まれます。

* タイムシートの時間枠。
* 「アクション」エリアには、次のものが含まれます。
   * タイムシートをお気に入りのリストに追加する星形のアイコン。
   * タイムシートを削除できる「削除」オプションを含んだその他アイコン。
* タイムシートの所有者の名前。
* タイムシートに表示される項目に関して記録された時間の合計時間数。
* 超過作業時間数。これは手動のエントリで、**超過作業時間**&#x200B;の設定がタイムシートで有効になっている場合にのみ表示されます。詳しくは、[タイムシート情報の編集](../create-and-manage-timesheets/edit-timesheets.md)を参照してください。

>[!TIP]
>
>タイムシートの現在の合計時間数よりも長い時間の超過作業時間数を記録することはできません。例えば、これまでにタイムシートに 7 時間記録した場合、超過作業時間数を 8 時間の記録することはできません。

* タイムシートのステータス。

## 左パネル

![左パネルのタイムシート](assets/timesheet-left-panel-unshimmed-redesign.png)

左パネルでは、次のセクションにアクセスできます。

* **タイムシート**：実際のタイムシートを表示します。
* **更新**：タイムシートのコメントとシステム更新を表示します。詳しくは、この記事の[左パネルの「更新」エリア](#updates-area-in-the-left-panel)の節を参照してください。

## 作業項目

![タイムシートの作業アイテム](assets/timesheet-object-names-unshimmed-redesign.png)

作業項目は、時間を記録するプロジェクト、タスクおよびイシューです。ヘッダー行の下向き矢印をクリックすると、プロジェクトと、その下に表示されるタスクとイシューが折りたたまれます。プロジェクト名の横にある下向き矢印をクリックすると、そのプロジェクトの作業アイテムが折りたたまれます。

タイムシート外で時間が記録されるタスク、イシューおよびプロジェクト、またはタイムシートの期間中に予定された項目は、ここに自動的に表示されます。

## ツール バー

![タイムシートのツールバー](assets/timesheet-toolbar-unshimmed-redesign.png)

ツールバーには次のオプションが含まれます。

* プロジェクト、タスクまたはイシューを追加できる「**項目を追加**」ボタン。
* タイムシートのタスクまたはイシューを検索できる、クイックフィルターアイコン。
* プロジェクト、タスク、またはイシューの時間のエントリに記録された時間コメントの表示と非表示を切り替えられる、「**コメントの表示**」設定。
* タイムシートをフルスクリーンモードで表示するためのフルスクリーンアイコン。
* タスクまたはイシューの追加情報を確認するための概要パネルを開くまたは閉じることができる、「**概要を開く**」または「**概要を閉じる**」ボタン。このボタンは、プロジェクトでは使用できません。

詳しくは、[時間の記録](../create-and-manage-timesheets/log-time.md)を参照してください。

## タイムシートのフッター

![タイムシートのフッター](assets/timesheet-footer-unshimmed-redesign.png)

このエリアにある「**承認用に送信**」、「**閉じる**」、「**承認**」および「**拒否**」ボタンをクリックして、タイムシートの承認を閉じるか、却下することができます。

この領域には、タイムシートが最後に保存された日時に関する情報も含まれます。タイムシートの情報に加えた変更はすべて自動的に保存されます。

## 担当業務

![担当業務](assets/timesheet-job-role-area-unshimmed-redesign.png)

時間エントリに関連付ける別の担当業務を選択できます。Workfront 管理者が「**手動で担当業務を時間エントリに割り当てます**」設定を有効にする必要があります。タスクやイシューに割り当てられたときに指定された担当業務がデフォルトで表示されます。タスクやイシューの担当業務が割り当てられていない場合は、主要役割がデフォルトで表示されます。詳しくは、[タイムシートと時間の環境設定を指定](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)を参照してください。

別々の役割の同じ作業項目に対して、複数の時間エントリを記録できます。詳しくは、[時間の記録](../create-and-manage-timesheets/log-time.md)を参照してください。

## 時間タイプ

![時間タイプ](assets/timesheet-hour-type-unshimmed-redesign.png)

各項目の時間エントリに関連付ける別々の時間タイプを選択できます。このフィールドは、Workfront 管理者がお使いの環境向けに有効にしている場合にのみ表示されます。詳しくは、[タイムシートと時間の環境設定](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)を参照してください。

別々の時間タイプの同じ作業項目に対して、複数の時間エントリを記録できます。詳しくは、[時間の記録](../create-and-manage-timesheets/log-time.md)を参照してください。

## 左パネルの更新エリア

![左側のタイムシートパネルの更新エリア](assets/timesheet-updates-with-all-tab.png)

タイムシートの左パネルの「更新」セクションでタイムシートにコメントを付けると、タイムシートの承認者や他のユーザーとコミュニケーションを取ることができます。

タイムシートに付けられたコメントは、このエリアに表示されます。

## 概要パネル

![概要パネル](assets/timesheet-summary-panel-on-updates.png)

タイムシートに表示されたタスクやイシューの概要パネルにアクセスできます。ここから、タスクやイシューにコメントを付けたり、情報を更新したりできます。詳しくは、[概要について](../../workfront-basics/the-new-workfront-experience/summary-overview.md)を参照してください。

タイムシートの概要パネルで作業項目に対して入力したコメントは、タスクまたはイシューの「更新」領域に表示されます。概要パネルは、プロジェクトでは使用できません。

## 時間枠と時間エントリエリア

![タイムシートの時間枠](assets/timesheet-time-frame-log-time-area.png)

タイムシートの時間枠は、作業項目の右側に表示されます。

1 週間、2 週間、4 週間のタイムシートを作成できます。

時間枠は 1 週間単位で表示されます。指定したタイムシートの時間枠に含まれない日付は淡色表示になります。タイムシートの時間枠に含まれない日付の時間は記録できません。

詳しくは、[単一回使用のタイムシートの作成](../create-and-manage-timesheets/create-tmshts.md)または[定期タイムシートの作成、編集、割り当て](../create-and-manage-timesheets/create-timesheet-profiles.md)を参照してください。

<!--drafted for the resize columns in timesheets story - make this blurb a TIP when the story is released: 
You can resize the columns that display different weeks, the time frame, or the work item areas by dragging and dropping the vertical lines that separate them.-->

## 時間エントリのコメント

![時間エントリコメント](assets/timesheet-hour-entry-comment-button-unshimmed-redesign.png)

タイムシートに追加するそれぞれの時間エントリにコメントを追加できます。

時間エントリのコメントボックスに入力したコメントは、タイムシートの各作業項目の下に表示されます。ツールバーの「**コメントの表示**」設定が有効になっている場合は、ここから時間を記録できます。

![](assets/hour-entry-comment-under-task-in-timesheet-unshimmed-redesign.png)

## 時間

![タイムシート時間](assets/timesheet-hours-area-unshimmed-redesign.png)

タイムシートには、タイムシートの範囲内の作業項目と日付のそれぞれに入力フィールドが用意されており、その項目の作業に費やした時間を記録できます。時刻を記録する際、時間を記録する行が水色でハイライト表示され、時間ボックスは濃い青色でアウトライン表示されます。

## 合計

![タイムシート合計](assets/timesheet-totals-column-and-header-unshimmed-redesign.png)

タイムシートに入力されたすべての時間の合計を、日別（タイムシートのヘッダー）およびオブジェクト別（最後の列）に確認できます。
