---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Adobe Workfront および Microsoft Project の期間タイプ
description: Adobe Workfront で使用できる期間の種類は、Microsoft プロジェクト内のタスクの種類とは異なります。 Workfront と Microsoft Project の間でプロジェクトを書き出したり読み込んだりすると、混乱が生じる場合があります。
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
TQID: https://experienceleague.adobe.com/avh0ZuYJpsf7Ed5HiWuLkxEA-0PD-1iFvzHmWvpDZiI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 257
ht-degree: 78%

---

# Adobe Workfront および Microsoft Project の期間タイプ

Adobe Workfront で使用できる期間の種類は、Microsoft プロジェクト内のタスクの種類とは異なります。 Workfront と Microsoft Project の間でプロジェクトを書き出したり読み込んだりすると、混乱が生じる場合があります。

WorkfrontとMicrosoft プロジェクト間でのプロジェクトの読み込みと書き出しについて詳しくは、次の記事を参照してください。

* [プロジェクトの Microsoft Project への書き出し](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Microsoft Project からプロジェクトを読み込む](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)

## WorkfrontおよびMicrosoft プロジェクトの期間タイプ

Workfront には 4 つのタスク期間タイプがあります。

* シンプル
* 残存作業時間の優先
* 予定作業
* 予定割り当て時間

詳しくは、[タスク期間と期間タイプの概要](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)を参照してください。

これらの期間のタイプは、Microsoft Project では認識されません。 現在、Microsoft プロジェクトには、Workfrontの期間タイプと同様の3つのタスクタイプがあります。

* 固定単位
* 固定作業
* 固定期間

## WorkfrontからMS プロジェクトへの書き出し時に期間タイプが変更される

Workfront から Microsoft Project にプロジェクトを書き出す場合、残存作業時間を優先するタスクは固定作業になります。 簡易、予定作業、予定割り当て時間は、固定単位になります。

## MS プロジェクトからWorkfrontに読み込むと、期間タイプが変更される

Microsoft Project から Workfront にプロジェクトを読み込むと、固定単位が「残存作業時間の優先」になります。 固定作業と固定期間には、Workfront 管理者がシステム用に選択したデフォルトの期間タイプが表示されます。 詳しくは、[システム全体のタスクとイシューの環境設定を指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

<!--
<note type="warning">
When a task has Calculated Work as the Duration Type and the default Duration Type in Setup is set as Calculated Assignment, then MS Project assignment allocations will be lost during the import.
 
(drafting this because it is misleading)
 
</note>
-->
