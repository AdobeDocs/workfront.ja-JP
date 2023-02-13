---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Adobe WorkfrontおよびMicrosoft Project の期間のタイプ
description: Adobe Workfrontで使用できる期間の種類は、Microsoftプロジェクト内のタスクの種類とは異なります。 WorkfrontとMicrosoft Project の間でプロジェクトをエクスポートまたは読み込むと、混乱が生じる場合があります。
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 2%

---

# Adobe WorkfrontおよびMicrosoft Project の期間のタイプ

Adobe Workfrontで使用できる期間の種類は、Microsoftプロジェクト内のタスクの種類とは異なります。 WorkfrontとMicrosoft Project の間でプロジェクトをエクスポートまたは読み込むと、混乱が生じる場合があります。

WorkfrontとMicrosoft Project の間でのプロジェクトの読み込みと書き出しについて詳しくは、次の記事を参照してください。

* [プロジェクトのMicrosoft Project への書き出し](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Microsoft Project からプロジェクトを読み込む](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)

## WorkfrontおよびMicrosoft Project の期間のタイプ

Workfrontには 4 つのタスク期間タイプがあります。

* シンプル
* 作業優先
* 算出した作業
* 算出した割り当て

詳しくは、 [タスクの期間と期間のタイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

これらの期間のタイプは、Microsoft Project では認識されません。 現在、Microsoft Project には、Workfrontの期間のタイプと同様に、次の 3 つのタスクタイプがあります。

* 固定単位
* 固定作業
* 固定期間

## Workfrontから MS Project に書き出す際の期間タイプの変更

WorkfrontからMicrosoft Project にプロジェクトをエクスポートする場合、労力に基づくタスクは固定作業になります。 [ 簡易 ]、[ 計算作業 ]、および [ 計算割り当て ] は [ 固定単位 ] になります。

## MS Project からWorkfrontに読み込む際の期間タイプの変更

Microsoft Project からWorkfrontにプロジェクトを読み込むと、固定単位が労力主導になります。 「 Fixed Work 」と「 Fixed Duration 」には、Workfront管理者がシステム用に選択したデフォルトの期間タイプが表示されます。 詳しくは、 [システム全体のタスクと問題の環境設定を構成](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--
<note type="warning">
When a task has Calculated Work as the Duration Type and the default Duration Type in Setup is set as Calculated Assignment, then MS Project assignment allocations will be lost during the import.
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(drafting this because it is misleading)
</MadCap:conditionalText>
</note>
-->
