---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Adobe Workfront および Microsoft Project の期間タイプ
description: Adobe Workfront で使用できる期間の種類は、Microsoft プロジェクト内のタスクの種類とは異なります。Workfront と Microsoft Project の間でプロジェクトを書き出したり読み込んだりすると、混乱が生じる場合があります。
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 78%

---

# Adobe Workfront および Microsoft Project の期間タイプ

Adobe Workfront で使用できる期間の種類は、Microsoft プロジェクト内のタスクの種類とは異なります。Workfront と Microsoft Project の間でプロジェクトを書き出したり読み込んだりすると、混乱が生じる場合があります。

WorkfrontとMicrosoft プロジェクトの間でのプロジェクトの読み込みおよび書き出しについて詳しくは、以下の記事を参照してください。

* [プロジェクトの Microsoft Project への書き出し](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Microsoft Project からプロジェクトを読み込む](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)

## WorkfrontとMicrosoft プロジェクトの期間タイプ

Workfront には 4 つのタスク期間タイプがあります。

* シンプル
* 残存作業時間の優先
* 予定作業
* 予定割り当て時間

詳しくは、[タスク期間と期間タイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)を参照してください。

これらの期間のタイプは、Microsoft Project では認識されません。現在、Microsoft プロジェクトには、Workfrontの期間タイプに似た 3 つのタスクタイプがあります。

* 固定単位
* 固定作業
* 固定期間

## Workfrontから MS Project に書き出す際の期間タイプの変更

Workfront から Microsoft Project にプロジェクトを書き出す場合、残存作業時間を優先するタスクは固定作業になります。簡易、予定作業、予定割り当て時間は、固定単位になります。

## MS Project からWorkfrontに読み込むと、期間タイプが変更される

Microsoft Project から Workfront にプロジェクトを読み込むと、固定単位が「残存作業時間の優先」になります。固定作業と固定期間には、Workfront 管理者がシステム用に選択したデフォルトの期間タイプが表示されます。詳しくは、[システム全体のタスクとイシューの環境設定を指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

<!--
<note type="warning">
When a task has Calculated Work as the Duration Type and the default Duration Type in Setup is set as Calculated Assignment, then MS Project assignment allocations will be lost during the import.
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(drafting this because it is misleading)
</MadCap:conditionalText>
</note>
-->
