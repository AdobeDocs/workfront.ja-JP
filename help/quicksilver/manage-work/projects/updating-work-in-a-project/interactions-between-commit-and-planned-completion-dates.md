---
product-area: projects
navigation-topic: update-work-in-a-project
title: コミット日と予定完了日の間のやり取り
description: 予定完了日とコミット日の両方は、タスクを完了すべきタイミングを示します。しかし、これらの日付は誰が設定するかによって異なります。
author: Alina
feature: Work Management
exl-id: 1709c60c-ac75-48eb-9226-ec2cf556ebf0
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 70%

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

タスクまたはイシューを担当する担当者は、コミット日を手動で更新するか、作業を許可して自動的に更新することができます。 これは、タスクやイシューを完了させるのが現実的な場合に、プロジェクト所有者に示す視覚的な方法です。

>[!TIP]
>
>タスクまたはイシューのコミット日を更新できるのは担当者だけです。

コミット日を変更した担当者は、計画完了日を自動的に変更しません。 逆も同様です。計画完了日を変更しても、コミット日は変更されません。

「コミット日」が「計画完了日」より後の日付に変更されると、プロジェクト所有者は、この変更が発生したことを通知され、プロジェクト所有者が従来のコメント作成機能を使用している場合は、プロジェクトのタイムラインに影響を与えます。 この機能は、新しいコメントエクスペリエンスではサポートされていません。 詳しくは、[新しいコメントエクスペリエンス](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md)を参照してください。

担当者が指定したコミット日がプロジェクト所有者によって許可された場合は、タスクまたはイシューに関する予定完了日を手動で更新する必要があります。詳しくは、次の記事を参照してください。

* [コミット日の概要](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
* [タスクやイシューのコミット日の更新](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md)
