---
content-type: reference
navigation-topic: workfront-navigation
title: ' [!DNL Workfront] のプロジェクト、タスクおよびイシューの日付の概要'
description: この記事では、のプロジェクト、タスク、イシューに関連する最も一般的な日付の定義を説明します [!DNL Adobe Workfront].
feature: Get Started with Workfront
author: Alina
exl-id: 3808200f-a573-4c39-8965-b254f69c893c
source-git-commit: 040dd446ff2b347dabf8a139feb17fd1a7d50e4e
workflow-type: tm+mt
source-wordcount: '1258'
ht-degree: 78%

---

# [!DNL Workfront] のプロジェクト、タスクおよびイシューの日付の概要

<!-- Audited: 05/2024 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider expanding on this article with ALL dates for PTIs - Hand off dates, Approval Dates, etc) </p>
-->

この記事では、[!DNL Adobe Workfront] のプロジェクト、タスクおよびイシューに関連する最も一般的な日付の定義を示します。ここに含まれる画像は、Workfront での日付の表示場所の例であり、すべてを網羅しているわけではありません。日付が表示されるエリアは他にもあります。すべての日付は、プロジェクト、タスク、イシューのレポートとリストにも表示されます。

レポートとリストについて詳しくは、次の記事を参照してください。

* [ [!DNL Adobe Workfront] のリストの基本を学ぶ](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)
* [レポートの基本を学ぶ](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)

プロジェクト、タスク、およびイシューの各フィールドについて詳しくは、 [!DNL Adobe Workfront] 用語集](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)内の[用語集を参照してください。

## [!UICONTROL 予定開始日]

[!UICONTROL 予定開始日]は、プロジェクト、タスク、またはイシューが開始される予定の日付です。

[!UICONTROL タスクの制約]によっては、タスクの[!UICONTROL 予定開始日]を編集できない場合があります。プロジェクトの[!UICONTROL スケジュールモード]によっては、プロジェクトの[!UICONTROL 予定開始日]を編集できない場合があります。

詳しくは、[プロジェクトの概要[!UICONTROL 予定開始日]](../../../manage-work/projects/planning-a-project/project-planned-start-date.md)を参照してください。

![](assets/planned-start-date-on-edit-task-highlighted-nwe.png)

![](assets/planned-start-date-in-task-list-highlighted-nwe-350x167.png)

## [!UICONTROL 予定完了日]

[!UICONTROL 予定完了日]または[!UICONTROL 期限]日とは、プロジェクト、タスク、またはイシューが完了する予定の日付です。

[!UICONTROL タスクの制約]によっては、タスクの[!UICONTROL 予定完了日]を編集できない場合があります。プロジェクトの[!UICONTROL スケジュールモード]によっては、プジェクトの[!UICONTROL 予定完了日]を編集できない場合もあります。

[!UICONTROL 予定完了日]は、[!DNL Workfront] の一部のエリアでは、期限日として表示されます。

詳しくは、次の記事を参照してください。

* [タスクの[!UICONTROL 予定完了日]の概要](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [プロジェクトの[!UICONTROL 予定完了日]を設定](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [問題の概要[!UICONTROL 予定完了日]](../../../manage-work/issues/issue-information/issue-planned-completion-date.md)

![](assets/project-header-planned-completion-date-highlighted-nwe-350x34.png)

![](assets/planned-completion-date-in-task-list-highlighted-nwe-350x183.png)

## [!UICONTROL エントリ日]

[!UICONTROL エントリ日]は、Workfront でプロジェクト、タスク、またはイシューが作成された日付です。

[!UICONTROL エントリ日]は、プロジェクト、タスクまたはイシューのタイムラインに影響しませんが、トラッキングやレポートの目的では重要です。[!DNL Workfront] は、オブジェクトの作成時に[!UICONTROL エントリ日]を自動的に生成しますが、手動でこの日付を編集することはできません。

![](assets/entry-date-in-task-details-highlighted-nwe.png)

## [!UICONTROL 実際の開始日]

[!UICONTROL 実際の開始日]は、ユーザーがプロジェクト、タスクまたはイシューで実際に作業を開始する日付です。[!UICONTROL 実際の開始日]は、プロジェクト、タスクまたはイシューを作成すると空になります。

タスクまたはイシューの作業がいつ開始されたかを手動で指定できます。または、またはタスクまたはイシューのステータスが「[!UICONTROL 新規]」から「[!UICONTROL 処理中]」または「[!UICONTROL 完了]」に変更された際、[!UICONTROL 実際の開始日]が自動的に入力されます。プロジェクトの[!UICONTROL 実際の開始日]は、プロジェクトの最初のタスクが開始する日付と一致します。

>[!TIP]
>
>ユーザーが予定日より遅くまたは早く作業を開始するため、プロジェクト、タスク、またはイシューの[!UICONTROL 実際の開始日]が[!UICONTROL 予定開始日]と一致しない場合があります。

詳しくは、[プロジェクトの概要[!UICONTROL 実際の開始日]](../../../manage-work/projects/planning-a-project/project-actual-start-date.md)を参照してください。

>[!NOTE]
>
>[!UICONTROL 開始日指定]タスクまたは固定日付制約は、タスクの[!UICONTROL 実際の開始日]ではなく、[!UICONTROL 予定開始日]に影響します。これにより、[!UICONTROL 予定開始日]を指定の日付に更新します。[!UICONTROL 実際の開始日]は、前述のとおり、[!UICONTROL 予定開始日]とは別にアップデートします。

![](assets/actual-start-date-on-edit-task-highlighted-nwe-350x251.png)

![](assets/actual-start-date-on-task-details-highlighted-nwe-350x191.png)

## [!UICONTROL 実際の完了日]

[!UICONTROL 実際の完了日]は、ユーザーがプロジェクト、タスクまたはイシューを実際に完了する日付です。[!UICONTROL 実際の完了日]は、プロジェクト、タスクまたはイシューを作成すると、空になります。

タスクまたはイシューの作業が完了したタイミングを手動で指定できます。 [!UICONTROL 実際の終了日] 次のいずれかが発生すると、が自動的に入力されます。

* プロジェクト、タスクまたはイシューのステータスが[!UICONTROL 完了]、[!UICONTROL クローズ]または[!UICONTROL 解決済み]に変更されます。
* タスクまたはプロジェクトの完了率は 100%です。

この [!UICONTROL 実際の終了日] のプロジェクトは、そのプロジェクトの最後のタスクを完了した日付と一致しています。

>[!TIP]
>
>[!UICONTROL 実際の完了日]が[!UICONTROL 予定完了日]と一致しない場合があります。

詳しくは、[プロジェクトの概要[!UICONTROL 実際の完了日]](../../../manage-work/projects/planning-a-project/project-actual-completion-date.md)を参照してください。

![](assets/actual-completion-date-task-details-highlighted-nwe-350x189.png)

## [!UICONTROL コミット日]

この [!UICONTROL コミット日] は、ユーザーがタスクまたは問題を完了するとコミットする日付です。 これは[!UICONTROL 予定完了日]とは異なり、作業を担当するユーザーが設定する、より現実的な予定完了日です。詳しくは、[[!UICONTROL コミット日]の概要](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)を参照してください。

>[!NOTE]
>
>[!UICONTROL コミット日]を変更すると、タスクやイシューの[!UICONTROL 見込み完了日]には影響しますが、[!UICONTROL 予定完了日]には影響しません。プロジェクトマネージャーは、担当者が変更した[!UICONTROL コミット日]を使用してタスクまたはイシューの[!UICONTROL 予定完了日]を更新します。

## [!UICONTROL 見込み開始日]

この [!UICONTROL 見込開始日] は、プロジェクト、タスク、または問題が開始され、すべての遅延が考慮されるリアルタイムの日付です。 これは[!UICONTROL 予定開始日]よりも正確なプロジェクト、タスクまたはイシューの開始日です。[!UICONTROL 予定開始日]では、遅延や過去の日付は考慮されません。

最初にプロジェクトを計画する際は、タスクとプロジェクトのタスクの[!UICONTROL 予定開始日]および[!UICONTROL 見込み開始日]は同じです。遅延が発生したり、タスクが早く完了したりする可能性があるので、[!UICONTROL 見込み開始日]と[!UICONTROL 予定開始日]は異なる場合があります。

タスクでは、先行タスクが予定より遅れている場合も、[!UICONTROL 見込み開始日]が[!UICONTROL 予定開始日]と異なる場合があります。

>[!TIP]
>
>イシューの[!UICONTROL 見込み開始日]は、リストまたはレポートでのみ表示できます。

詳しくは、[プロジェクトの概要[!UICONTROL 見込み開始日]](../../../manage-work/projects/planning-a-project/project-projected-start-date.md)を参照してください。

![](assets/projected-start-date-in-task-details-highlighted-nwe-350x188.png)

## [!UICONTROL 見込完了日]

[!UICONTROL 見込み完了日]は、プロジェクト、タスクまたはイシューが完了する日時を示すリアルタイムの計算指標です。プロジェクト、タスクまたはイシューが「完了」とマークされると、[!UICONTROL 見込み完了日]は[!UICONTROL 実際の完了日]の日付に変更されます。

すべてが計画どおりにスムーズに進む場合、 [!UICONTROL 見込完了日] 次と一致する必要があります [!UICONTROL 予定完了日]. それ以外の場合は、先行タスクの遅延により、 [!UICONTROL 見込完了日] は、と異なる場合があります。 [!UICONTROL 予定完了日].

詳しくは、[プロジェクト、タスクおよびイシューの[!UICONTROL 見込み完了日]の概要](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)を参照してください。

![](assets/projected-completion-date-in-task-details-highlighted-nwe-350x187.png)

## [!UICONTROL 時間エントリ日]

プロジェクト、タスクまたはイシューに費やした実際の時間（時間単位）を表すためにプロジェクト、タスクまたはイシューの時間を記録すると、記録した時間がプロジェクト、タスクまたはイシューの[!UICONTROL 実際の時間]になります。

時間を記録する日付は、 [!UICONTROL 時間エントリ日] 時間エントリのフィールド。 一部の時間リストおよびレポートでは、時間入力日が日付として表示されます。

>[!TIP]
>
>この [!UICONTROL 時間エントリ日] 次と異なる [!UICONTROL エントリ日] これは、時間ログを作成した日付ではなく、時間を関連付ける日付です。

Workfrontの次の領域で時間をログに記録し表示できます。

* での時間のログ記録と表示 [!UICONTROL プロジェクト], [!UICONTROL タスク]、または [!UICONTROL 問題更新] セクションまたは内 [!UICONTROL 時間] セクション。 「[!UICONTROL 時間]」セクションでログ時間を記録する際に、「時間エントリ日」とその該当ユーザーを手動で指定できます。

  ![](assets/log-time-box-task-hours-section-nwe-350x500.png)

  詳しくは、[時間の記録](../../../timesheets/create-and-manage-timesheets/log-time.md)を参照してください。

  >[!TIP]
  >
  >親タスクやプロジェクトではなく、作業タスクまたはイシューに関する時間を記録することをお勧めします。作業タスクに記録された時間は、親タスクとプロジェクトに[!UICONTROL 実際の時間]としてロールアップされます。イシューに記録した時間は、プロジェクトの[!UICONTROL 実際の時間数]としてプロジェクトにロールアップされます。

* タスクまたは問題の更新ストリームに時間を記録します。

  ![](assets/log-time-in-update-stream-task-nwe-350x185.png)

* を表示する [!UICONTROL 時間エントリ日] 時間レポートおよびリスト。

  ![](assets/hour-entry-date-in-view-nwe-350x173.png)
