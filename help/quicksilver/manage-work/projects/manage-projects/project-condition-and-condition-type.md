---
title: プロジェクト条件と条件タイプの概要
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: プロジェクトの条件は、プロジェクトの進行状況を視覚的に表したものです。 これは、プロジェクトの計画日、予定日、および推定日の関係によって決定されるレポート可能な変数です。
author: Alina
feature: Work Management
exl-id: 0c847b26-b0cb-49bb-84be-32534c72d5b6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 1%

---

# プロジェクト条件と条件タイプの概要

プロジェクトの条件は、プロジェクトの進行状況を視覚的に表したものです。 これは、プロジェクトの計画日、予定日、および推定日の関係によって決定されるレポート可能な変数です。

## プロジェクト条件の概要

プロジェクトの条件について理解する際は、次の点に注意してください。

* プロジェクト所有者は、プロジェクトの条件を手動で設定するか、自動で設定するかを決定できます。 プロジェクトの条件は、次の方法で設定できます。

   * 手動：プロジェクトの管理へのアクセス権を持つユーザー、およびプロジェクトの条件の種類が手動に設定されている場合。
   * プロジェクトの「条件の種類」が「進捗状況ステータス」に設定されている場合に、Adobe Workfrontにより自動的に実行されます。 プロジェクトの進捗状況ステータスは、プロジェクト上のタスクの進捗状況によって決まります。 プロジェクトの進捗状況ステータスについて詳しくは、 [プロジェクトの進行状況ステータスの概要](../../../manage-work/projects/planning-a-project/project-progress-status.md).

   プロジェクトの条件タイプを更新する方法について詳しくは、 [プロジェクトの条件タイプの設定](../../../manage-work/projects/manage-projects/set-condition-type-for-project.md).

* Workfrontでプロジェクトの条件を自動的に推定する場合は、タスクの進捗状況が実際の進捗状況とプロジェクトの進捗状況ステータスに反映されるように、タスクに先行タスクを使用することをお勧めします。
* プロジェクトの所有者は、「条件の種類」を「進捗状況ステータス」から「手動」に変更することで、進捗状況ステータスを使用する代わりに手動の条件の種類を使用するようにプロジェクトを変更できます。

   >[!NOTE]
   >
   >次のいずれかのステータスのプロジェクトは、タスクの日付と進捗状況に関係なく、常に「ターゲット上」としてマークされます。
   >
   >* アイデア
   >* 要求済み
   >* 承認済み
   >* 拒否


<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Set the Condition Type for a project</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted here and moved it to a separate article: /Content/Manage work/Projects/Manage projects/set-condition-type-for-project.htm)</p>
<ol>
<li value="1">Go to the project for which you want to update the Condition Type. </li>
<li value="2"> <p>  Click the <strong>More</strong> menu <img src="assets/qs-more-menu.png"> to the right of the project name, then click <strong>Edit</strong>.  <br> </p> </li>
<li value="3">In the <strong>Condition Type</strong> field, choose one of the following:
<ul>
<li><p><strong>Manual:</strong> The project owner sets the Condition on the project manually.</p><p data-mc-conditions="QuicksilverOrClassic.Quicksilver">In this case, the project owner can update the Condition of the project in the project header, or the Project Details section. </p></li>
<li><p><strong>Progress Status:</strong> Workfront sets the Condition based on the Progress Status of the project. <br></p></li>
</ul></li>
<li value="4">Click <strong>Save Changes</strong>. </li>
</ol>
</div>
-->

## Workfrontが進行状況ステータスに基づいてプロジェクト条件を更新する方法

プロジェクトの「条件の種類」が「手動」に設定されている場合、プロジェクトの「条件」がプロジェクトの「進捗状況」ステータスとは独立して、どのような状態になるかを指定できます。

ただし、タスクの進捗状況に基づいてプロジェクトの真の進捗状況を明確に示すことができるように、プロジェクトの条件の種類を「進捗状況ステータス」に設定することをお勧めします。 Workfrontがプロジェクトの進捗状況ステータスを計算する方法について詳しくは、 [プロジェクトの進行状況ステータスの概要](../../../manage-work/projects/planning-a-project/project-progress-status.md).

この場合、プロジェクト条件の値は次のようになります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>プロジェクト条件</td> 
   <td>プロジェクトの進行状況ステータス</td> 
   <td>Workfront条件インジケーター</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>目標どおり</td> 
   <td> <li>プロジェクトの進捗状況ステータスがオンタイムの場合、プロジェクトの条件は次のようになります。 <strong>ターゲット時</strong>.</li> </td> 
   <td> <img src="assets/on-target-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>リスクあり</td> 
   <td>プロジェクトの進捗状況ステータスが <strong>後ろ</strong> または <strong>リスク</strong>を指定した場合、プロジェクトの条件は <strong>リスク</strong>.</td> 
   <td> <img src="assets/at-risk-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>トラブル発生中</td> 
   <td>プロジェクトの進捗状況ステータスが <strong>遅延</strong>を指定した場合、プロジェクトの条件は <strong>トラブル状態</strong>. </td> 
   <td> <img src="assets/in-trouble-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>条件は、お使いの環境に合わせてカスタマイズできるので、お使いの環境で条件に対して 3 つ以上のオプションを検索できます。 条件の名前は、上記の名前とは異なる場合があります。 の条件のカスタマイズについて詳しくは、この記事を参照してください。 [カスタム条件の作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## プロジェクト条件、プロジェクト条件の更新、および最終条件に関するレポート

プロジェクトレポートの表示で、プロジェクトの条件に関連する次のフィールドを表示できます。

* **プロジェクト条件：** プロジェクトの現在の条件を表示します。
* **プロジェクト条件の更新**:新しい条件と共に、プロジェクトの更新ストリームでプロジェクト所有者が提供した最新の更新を表示します。\
   条件の更新に対しておこなったコメントは、 **条件の更新** 列；メインの更新のみが表示されます。

* **最終条件のメモ**:オブジェクトの所有者が最後に入力した更新を表示します。 このフィールドは、オブジェクトに対する所有者の最新のアクティビティやインタラクションを表示するのに役立ちます。\
   この **最終条件のメモ** オブジェクトの最後のメモのメモテキストが削除されている場合、列は空になります。 オブジェクトに新しい注記を入力すると、その注記が最後の注記になり、列に再び表示されます。

レポートの作成方法について詳しくは、 [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
