---
product-area: projects
navigation-topic: update-work-in-a-project
title: コミット日と予定完了日の間のインタラクション
description: 予定完了日とコミット日の両方は、タスクを完了すべきタイミングを示します。しかし、これらの日付は誰が設定するかによって異なります。
author: Alina
feature: Work Management
exl-id: 1709c60c-ac75-48eb-9226-ec2cf556ebf0
source-git-commit: 1eb1e919bede7e366956d8c0bd969329a641123f
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 80%

---

# コミット日と予定完了日の間のやり取り

<!--
this article has mostly information that is repeated from the articles linked from here. I left it in here for searchability's sake.
-->

予定完了日とコミット日の両方は、タスクを完了すべきタイミングを示します。しかし、これらの日付は誰が設定するかによって異なります。

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
   <td> <p>予定完了日は、プロジェクトの所有者がタスクまたはイシューをいつ完了すると見込んでいるかを示します。プロジェクト所有者によって手動で設定されるか、タスクまたはイシューに対する管理権限を持つ任意のユーザーによって設定されるか、Adobe Workfront によって自動的に計算される可能性があります。</p> <p>予定完了日について詳しくは、<a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">タスクの予定完了日の概要</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## コミット日と予定完了日の間のやり取り

プロジェクト所有者がタスクまたはイシューを作成して割り当てると、タスクまたはイシューには次の内容が割り当てられます。

* 予定完了日
* コミット日なし

タスクまたはイシューの担当者は、コミット日を手動で更新するか、作業を許可して自動的に更新することができます。これは、プロジェクト所有者にとっていつタスクやイシューを完了するのが現実的なのかをプロジェクト所有者に示す視覚的な方法です。

>[!TIP]
>
>タスクまたはイシューのコミット日を更新できるのは担当者だけです。

コミット日を変更した担当者では、予定完了日が自動的に変更されません。逆も同様で、予定完了日を変更しても、コミット日は変更されません。

コミット日が変更されると、プロジェクト所有者には、この変更が発生したことがWorkfrontのアプリ内通知で通知されます。

担当者が提供したコミット日がプロジェクト所有者にとって許容できる場合は、タスクの予定完了日を手動で更新して、プロジェクトのタイムラインに与える影響を示す必要があります。 イシューの予定完了日を変更しても、プロジェクトのタイムラインには影響しません。

詳しくは、次の記事を参照してください。

* [コミット日の概要](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
* [タスクやイシューのコミット日の更新](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md)
