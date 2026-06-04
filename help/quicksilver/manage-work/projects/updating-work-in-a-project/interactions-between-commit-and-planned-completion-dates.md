---
product-area: projects
navigation-topic: update-work-in-a-project
title: コミット日と予定完了日のインタラクション
description: 予定完了日とコミット日の両方は、タスクを完了すべきタイミングを示します。 しかし、これらの日付は誰が設定するかによって異なります。
author: Alina
feature: Work Management
exl-id: 1709c60c-ac75-48eb-9226-ec2cf556ebf0
TQID: https://experienceleague.adobe.com/iy-L6-ZnhDgVTJjhEBlqwdRH3TRA5OqT3Gj-LIoEgDA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 422
ht-degree: 80%

---

# コミット日と予定完了日の間のやり取り

<!--
this article has mostly information that is repeated from the articles linked from here. I left it in here for searchability's sake.
-->

予定完了日とコミット日の両方は、タスクを完了すべきタイミングを示します。 しかし、これらの日付は誰が設定するかによって異なります。

## コミット日と予定完了日の概要

タスクとイシューの両方に予定完了日とコミット日が存在します。

次の表に、コミット日と予定完了日の違いに関する情報を示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">コミット日</td> 
   <td> <p>コミット日は、タスクまたはイシューに割り当てられたユーザーがタスクまたはイシューの完了を手動で推定した日付です。</p> <p>コミット日について詳しくは、<a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">コミット日の概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">予定完了日</td> 
   <td> <p>予定完了日は、プロジェクトの所有者がタスクまたはイシューをいつ完了すると見込んでいるかを示します。 プロジェクト所有者によって手動で設定されるか、タスクまたはイシューに対する管理権限を持つ任意のユーザーによって設定されるか、Adobe Workfront によって自動的に計算される可能性があります。</p> <p>予定完了日について詳しくは、<a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">タスクの予定完了日の概要</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## コミット日と予定完了日の間のやり取り

プロジェクト所有者がタスクまたはイシューを作成して割り当てると、タスクまたはイシューには次の内容が割り当てられます。

* 予定完了日
* コミット日なし

タスクまたはイシューの担当者は、コミット日を手動で更新するか、作業を許可して自動的に更新することができます。 これは、プロジェクト所有者にとっていつタスクやイシューを完了するのが現実的なのかをプロジェクト所有者に示す視覚的な方法です。

>[!TIP]
>
>タスクまたはイシューのコミット日を更新できるのは担当者だけです。

コミット日を変更した担当者では、予定完了日が自動的に変更されません。 逆も同様で、予定完了日を変更しても、コミット日は変更されません。

コミット日が変更されると、この変更が発生したことをWorkfront アプリ内通知でプロジェクトオーナーに通知します。

担当者が提示したコミット日がプロジェクトオーナーにとって適切である場合、タスクの予定完了日を手動で更新し、プロジェクトのタイムラインに与える影響を把握する必要があります。 問題の予定完了日の変更は、プロジェクトのタイムラインには影響しません。

詳しくは、次の記事を参照してください。

* [コミット日の概要](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
* [タスクやイシューのコミット日の更新](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md)
