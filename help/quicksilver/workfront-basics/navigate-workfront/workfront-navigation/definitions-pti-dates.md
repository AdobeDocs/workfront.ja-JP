---
content-type: reference
navigation-topic: workfront-navigation
title: ' [!DNL Workfront] のプロジェクト、タスクおよびイシューの日付の概要'
description: この記事では、 [!DNL Adobe Workfront] のプロジェクト、タスクおよびイシューに関連する最も一般的な日付の定義を示します。
feature: Get Started with Workfront
author: Alina
exl-id: 3808200f-a573-4c39-8965-b254f69c893c
source-git-commit: 0a2ff1ab802b2bd08cd680376321552a8018cb74
workflow-type: tm+mt
source-wordcount: '2357'
ht-degree: 47%

---

# [!DNL Workfront] のプロジェクト、タスクおよびイシューの日付の概要

<!-- Audited: 05/2024 -->

<!--consider expanding on this article with ALL dates for PTIs - Hand off dates, Approval Dates, etc-->

<!-- there are dates below that need definition - ask Product-->

この記事では、[!DNL Adobe Workfront] のプロジェクト、タスクおよびイシューに関連する最も一般的な日付の定義を示します。ここに含まれる画像は、Workfront での日付の表示場所の例であり、すべてを網羅しているわけではありません。日付が表示されるエリアは他にもあります。すべての日付は、プロジェクト、タスク、イシューのレポートとリストにも表示されます。

レポートとリストについて詳しくは、次の記事を参照してください。

* [ [!DNL Adobe Workfront] のリストの基本を学ぶ](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)
* [レポートの基本を学ぶ](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)

プロジェクト、タスク、イシューの各フィールドについて詳しくは、[ 用語集  [!DNL Adobe Workfront]  用語 ](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md) を参照してください。


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

![ 編集タスクの実際の開始日 ](assets/actual-start-date-on-edit-task-highlighted-nwe-350x251.png)

![ タスクの実際の開始日 ](assets/actual-start-date-on-task-details-highlighted-nwe-350x191.png)

## [!UICONTROL 実際の完了日]

[!UICONTROL 実際の完了日]は、ユーザーがプロジェクト、タスクまたはイシューを実際に完了する日付です。[!UICONTROL 実際の完了日]は、プロジェクト、タスクまたはイシューを作成すると、空になります。

タスクまたは問題の作業が完了した日時を手動で指定するか、次のいずれかが発生した場合に [!UICONTROL  実際の完了日 ] が自動的に入力されるようにすることができます。

* プロジェクト、タスクまたはイシューのステータスが[!UICONTROL 完了]、[!UICONTROL クローズ]または[!UICONTROL 解決済み]に変更されます。
* タスクまたはプロジェクトの完了率は 100%です。

プロジェクトの[!UICONTROL 実際の完了日]は、プロジェクトの最後のタスクが完了した日付と一致します。

>[!TIP]
>
>[!UICONTROL 実際の完了日]が[!UICONTROL 予定完了日]と一致しない場合があります。

詳しくは、[プロジェクトの概要[!UICONTROL 実際の完了日]](../../../manage-work/projects/planning-a-project/project-actual-completion-date.md)を参照してください。

![ 詳細の実際の完了日 ](assets/actual-completion-date-task-details-highlighted-nwe-350x189.png)

## 承認パス完了日

承認パス完了日は、プロジェクト、タスクまたはイシューの承認が付与され、項目のステータスが変更された日付です。

承認パス完了日は、プロジェクト、タスク、問題のリストおよびレポートに表示されます。

## 承認パス開始日

承認パス開始日は、プロジェクト、タスクまたは問題の状態が「承認保留中」に変更され、プロジェクト承認要求が承認者に送信された日付です。

承認パス開始日は、プロジェクト、タスク、問題のリストおよびレポートに表示されます。

<!--## Auto Closure Date -->

## 予算計上完了日

これは、プロジェクトの非推奨フィールドです。 このフィールドでリストやレポートに表示される情報は、Workfrontによって削除された機能に関連しています。 このフィールドは更新できません。

このフィールドは、プロジェクトの報告書とリストに表示されます。

## 予算計上開始日

これは、プロジェクトの非推奨フィールドです。 このフィールドに表示される情報は、Workfrontによって削除された機能に関連しています。 このフィールドは更新できません。

このフィールドは、プロジェクトの報告書とリストに表示されます。

## [!UICONTROL コミット日]

[!UICONTROL  コミット日 ] は、タスクまたは問題に割り当てられたユーザーがタスクまたは問題を完了するとコミットする日付です。 これは[!UICONTROL 予定完了日]とは異なり、作業を担当するユーザーが設定する、より現実的な予定完了日です。詳しくは、[[!UICONTROL コミット日]の概要](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)を参照してください。

>[!NOTE]
>
>[!UICONTROL コミット日]を変更すると、タスクやイシューの[!UICONTROL 見込み完了日]には影響しますが、[!UICONTROL 予定完了日]には影響しません。プロジェクトマネージャーは、担当者が変更した[!UICONTROL コミット日]を使用してタスクまたはイシューの[!UICONTROL 予定完了日]を更新します。

<!--## Completion Pending Date-->

## 制約の指定日

特定の日付に関連付けられているタスク制約を使用している場合、その特定の日付がタスクの制約の指定日になります。

「制約の指定日」フィールドを更新するタスク制約は次のとおりです。

* 指定日に開始
* 指定日に終了
* 指定日までに開始
* 指定日以降に開始

>[!TIP]
>
>固定日付の制約を持つタスクには、制約の指定日がありません。
>

制約の指定日はタスク リストまたはレポートに表示されます。

## 変換済みイシューのエントリ日

イシューがプロジェクトまたはタスクに変換された日付が作成されました。

変換されたイシューのエントリ日は、プロジェクト、タスクのリストおよびレポートに表示されます。

## 期日

タスクまたは問題の完了期日。 タスクまたは問題の期日が、予定完了日と同じ日です。

タスクと問題の期限は、タスクと問題のリストおよびレポートに表示されます。

詳しくは、この記事の [ 予定完了日 ](#planned-completion-date) の節を参照してください。

## 期限

プロジェクトの完了期日。 プロジェクトの期限日が、プロジェクトの予定完了日と同じ日です。

プロジェクトの期限は、プロジェクトのリストおよびレポートに表示されます。

詳しくは、この記事の [ 予定完了日 ](#planned-completion-date) の節を参照してください。

## [!UICONTROL エントリ日]

[!UICONTROL  エントリ日 ] は、プロジェクト、タスクまたはイシューが [!DNL Workfront] で作成された日付です。

[!UICONTROL エントリ日]は、プロジェクト、タスクまたはイシューのタイムラインに影響しませんが、トラッキングやレポートの目的では重要です。[!DNL Workfront] は、オブジェクトの作成時に[!UICONTROL エントリ日]を自動的に生成しますが、手動でこの日付を編集することはできません。

![ タスク詳細のエントリ日 ](assets/entry-date-in-task-details-highlighted-nwe.png)

## 推定期限

タスクとプロジェクトの推定期限は、プロジェクトまたはタスクが完了する必要がある、より現実的な日付を示します。

推定日は、プロジェクトまたはタスクの実際の完了に影響を与える要因が考慮されるので、プロジェクトとタスクの実際の状況により近くなります。 見込期日は見込完了日に似ています。

詳しくは、[ 予定日と予定日の概要 ](/help/quicksilver/manage-work/tasks/task-information/differentiate-projected-estimated-dates.md) を参照してください。

プロジェクトとタスクの推定期限は、プロジェクト、タスクのリストおよびレポートに表示されます。

## 推定開始日

タスクとプロジェクトの推定開始日は、プロジェクトまたはタスクが開始できる、より現実的な日付を示します。

推定日付は、プロジェクトまたはタスクの実際の開始に影響を与える内容が考慮されるので、プロジェクトとタスクの実際の日付により近くなります。 推定開始日は見込み開始日に似ています。

詳しくは、[ 予定日と予定日の概要 ](/help/quicksilver/manage-work/tasks/task-information/differentiate-projected-estimated-dates.md) を参照してください。

プロジェクトおよびタスクの推定開始日は、プロジェクト、タスクのリストおよびレポートに表示されます。

<!--## Exchange Rate Date-->

## 固定終了日

プロジェクト依頼者または所有者は、ビジネス・ケースを完了するときに、プロジェクトの固定終了日を識別します。 期限は、プロジェクトの完了が必要なことを推奨する日付です。

これは手動の見積もりであり、プロジェクトのタスクの実際の進捗は考慮されません。

プロジェクトの固定終了日は、プロジェクトのビジネスケース セクション、およびプロジェクトリストとレポートに表示されます。

![ 固定終了日 ](assets/fixed-end-date-business-case-highlight.png)

## 固定開始日

プロジェクト依頼者または所有者は、ビジネス・ケースを完了するときに、プロジェクトの固定開始日を識別します。 期限は、プロジェクトの開始を推奨する日付です。

これは手動の見積もりであり、プロジェクトのタスクの実際の進捗は考慮されません。

プロジェクトの固定開始日は、プロジェクトのビジネスケース セクション、およびプロジェクトリストとレポートに表示されます。

![ 固定開始日 ](assets/fixed-start-date-business-case-highlight.png)

## ハンドオフ日

タスクが作業可能になる日付。つまり、すべての制約、承認および依存関係が完了し、ユーザーはそのタスクの作業を開始できます。

ハンドオフ日は計算であり、手動で設定することはできません。

ハンドオフ日について詳しくは、[ タスクのハンドオフ日の概要 ](/help/quicksilver/manage-work/tasks/task-information/handoff-task-date.md) を参照してください。

タスクのハンドオフ日は、タスクリストとレポートに表示されます。

## 財務の最終更新日

プロジェクトの財務情報が更新された日付。 これには、プロジェクトの「財務」セクションまたは「ビジネスケース」セクションの財務フィールドの更新が含まれます。

財務の最終更新日は、プロジェクト リストおよびレポートに表示されます。

## 最終更新日

プロジェクト、タスクまたは問題が最後に更新された日付。 更新とは、保存するプロジェクト、タスクまたはイシューをトリガーとするあらゆる変更と見なされます。 これには、ステータス、条件、タイムライン、財務、またはその他のフィールドの変更が含まれます。

最終更新日は、プロジェクト、タスク、問題のリストおよびレポートに表示されます。

## [!UICONTROL 時間エントリ日]

プロジェクト、タスクまたはイシューに費やした実際の時間（時間単位）を表すためにプロジェクト、タスクまたはイシューの時間を記録すると、記録した時間がプロジェクト、タスクまたはイシューの[!UICONTROL 実際の時間]になります。

時間を記録した日付は、時間入力の「[!UICONTROL 時間エントリ日]」フィールドです。

時間エントリ日は、時間リストおよびレポートに表示されます。

>[!TIP]
>
>時間の [!UICONTROL  エントリ日 ] は、時間ログが作成された日付ではなく、時間を関連付ける日付であるという点で、別のWorkfront オブジェクトの [!UICONTROL  エントリ日 ] とは異なります。
>
>例えば、9 月 5 日にタスクの時間を記録し、その時間を 9 月 1 日に関連付けることができます。 時間のエントリ日は 9 月 1 日です。

Workfrontに時間をログ記録する方法について詳しくは、[ 時間をログに記録 ](../../../timesheets/create-and-manage-timesheets/log-time.md) を参照してください。

>[!TIP]
>
>親タスクやプロジェクトではなく、作業タスクまたはイシューに関する時間を記録することをお勧めします。作業タスクに記録された時間は、親タスクとプロジェクトに[!UICONTROL 実際の時間]としてロールアップされます。イシューに記録した時間は、プロジェクトの[!UICONTROL 実際の時間数]としてプロジェクトにロールアップされます。

## [!UICONTROL 予定完了日]

[!UICONTROL 予定完了日]または[!UICONTROL 期限]日とは、プロジェクト、タスク、またはイシューが完了する予定の日付です。

[!UICONTROL タスクの制約]によっては、タスクの[!UICONTROL 予定完了日]を編集できない場合があります。プロジェクトの[!UICONTROL スケジュールモード]によっては、プジェクトの[!UICONTROL 予定完了日]を編集できない場合もあります。

[!UICONTROL 予定完了日]は、[!DNL Workfront] の一部のエリアでは、期限日として表示されます。

詳しくは、次の記事を参照してください。

* [タスクの[!UICONTROL 予定完了日]の概要](../../../manage-work/tasks/task-information/task-planned-completion-date.md)
* [プロジェクトの[!UICONTROL 予定完了日]を設定](../../../manage-work/projects/planning-a-project/project-planned-completion-date.md)
* [問題の概要[!UICONTROL 予定完了日]](../../../manage-work/issues/issue-information/issue-planned-completion-date.md)

![ ヘッダーの予定完了日 ](assets/project-header-planned-completion-date-highlighted-nwe-350x34.png)

![ タスクリストの予定完了日 ](assets/planned-completion-date-in-task-list-highlighted-nwe-350x183.png)


## 予定日付との整合性

これは、Workfrontがプロジェクト、タスクおよび問題を割り当て、予定完了日に対していつアイテムが完了するかを示す自動インジケーターです。

予定日整合性インジケーターには、次の値が使用できます。

* 計画完了日に完了します
* 計画完了日よりも前に完了します
* 計画完了日以降に完了します

予定日付の整合性は、プロジェクト、タスク、問題のリストおよびレポートに表示されます。

## [!UICONTROL 予定開始日]

[!UICONTROL 予定開始日]は、プロジェクト、タスク、またはイシューが開始される予定の日付です。

[!UICONTROL タスクの制約]によっては、タスクの[!UICONTROL 予定開始日]を編集できない場合があります。プロジェクトの[!UICONTROL スケジュールモード]によっては、プロジェクトの[!UICONTROL 予定開始日]を編集できない場合があります。

詳しくは、[プロジェクトの概要[!UICONTROL 予定開始日]](../../../manage-work/projects/planning-a-project/project-planned-start-date.md)を参照してください。

![ 編集タスクの予定開始日 ](assets/planned-start-date-on-edit-task-highlighted-nwe.png)

![ タスク リストの予定開始日 ](assets/planned-start-date-in-task-list-highlighted-nwe-350x167.png)

## [!UICONTROL 見込み完了日]

[!UICONTROL 見込み完了日]は、プロジェクト、タスクまたはイシューが完了する日時を示すリアルタイムの計算指標です。プロジェクト、タスクまたはイシューが「完了」とマークされると、[!UICONTROL 見込み完了日]は[!UICONTROL 実際の完了日]の日付に変更されます。

すべてが計画通りにスムーズに進む場合、[!UICONTROL  見込み完了日 ] は [!UICONTROL  計画完了日 ] と一致する必要があります。 そうしないと、先行タスクの遅延が原因で、[!UICONTROL  予定完了日 ] が [!UICONTROL  予定完了日 ] と異なる場合があります。

詳しくは、[プロジェクト、タスクおよびイシューの[!UICONTROL 見込み完了日]の概要](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md)を参照してください。

![ 完了予定日 ](assets/projected-completion-date-in-task-details-highlighted-nwe-350x187.png)

## [!UICONTROL 見込み開始日]

[!UICONTROL  予定開始日 ] は、プロジェクト、タスクまたは問題が開始され、すべての遅延が考慮されるリアルタイムの日付です。 これは[!UICONTROL 予定開始日]よりも正確なプロジェクト、タスクまたはイシューの開始日です。[!UICONTROL 予定開始日]では、遅延や過去の日付は考慮されません。

最初にプロジェクトを計画する際は、タスクとプロジェクトのタスクの[!UICONTROL 予定開始日]および[!UICONTROL 見込み開始日]は同じです。遅延が発生したり、タスクが早く完了したりする可能性があるので、[!UICONTROL 見込み開始日]と[!UICONTROL 予定開始日]は異なる場合があります。

タスクでは、先行タスクが予定より遅れている場合も、[!UICONTROL 見込み開始日]が[!UICONTROL 予定開始日]と異なる場合があります。

>[!TIP]
>
>イシューの[!UICONTROL 見込み開始日]は、リストまたはレポートでのみ表示できます。

詳しくは、[プロジェクトの概要[!UICONTROL 見込み開始日]](../../../manage-work/projects/planning-a-project/project-projected-start-date.md)を参照してください。

![ 見込み開始日 ](assets/projected-start-date-in-task-details-highlighted-nwe-350x188.png)

<!--## Rejection Date-->

## 余裕日

タスクの開始や完了が遅れても、プロジェクトの完了日に影響を及ぼさないことがあります。

余裕日には、タスクがプロジェクトの完了日に確実に影響を与える可能性がある正確な日付が表示されます。

タスクのSlack日について詳しくは、[ タスクのSlack日の概要 ](/help/quicksilver/manage-work/tasks/task-information/task-slack-date.md) を参照してください。

タスクのSlack日は、タスクリストとレポートに表示されます。

## 開始日

プロジェクトの開始予定日。 プロジェクトの開始日が、プロジェクトの予定開始日と同じ日付です。

このフィールドは、プロジェクトリストおよびレポートに表示されます。

詳しくは、この記事の [ 予定開始日 ](#planned-start-date) の節を参照してください。



