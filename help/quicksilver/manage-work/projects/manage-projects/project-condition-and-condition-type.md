---
title: プロジェクトの状況と状況タイプの概要
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: プロジェクト状況は、プロジェクトの進行状況を視覚的に表したものです。これは、プロジェクトの予定日、見込み日、および推測日の関係によって決定されるレポート可能な変数です。
author: Alina
feature: Work Management
exl-id: 0c847b26-b0cb-49bb-84be-32534c72d5b6
source-git-commit: e4de185f172b173dcc3ad966afa69ffb3bc479eb
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 94%

---

# プロジェクトの状況と状況タイプの概要

<!-- Audited: 12/2023 -->

プロジェクト状況は、プロジェクトの進行状況を視覚的に表したものです。これは、プロジェクトの予定日、見込み日、および推測日の関係によって決定されるレポート可能な変数です。

## プロジェクトの状況の概要

プロジェクトの状況について理解するには、以下の点を考慮してください。

* プロジェクト所有者は、プロジェクトの状況を手動で設定するか、自動で設定するかを決定できます。プロジェクトの状況は、以下の方法で設定できます。

   * プロジェクトの「管理」へのアクセス権を持つユーザー、およびプロジェクトの「条件タイプ」が「手動」に設定されている場合に、手動でおこなう。
   * プロジェクトの「条件の種類」が「進行状況ステータス」に設定されている場合に、Adobe Workfrontによって自動的に表示されます。 プロジェクトの進捗ステータスは、プロジェクト上のタスクの進捗状況によって決まります。プロジェクトの進捗ステータスについて詳しくは、[プロジェクトの進捗ステータスの概要](../../../manage-work/projects/planning-a-project/project-progress-status.md)を参照してください。

  プロジェクトの状況タイプをアップデートする方法について詳しくは、[プロジェクトの状況タイプを設定](../../../manage-work/projects/manage-projects/set-condition-type-for-project.md)を参照してください。

* Workfront でプロジェクトの状況を自動的に見積りできるようにする場合は、タスクの進捗が実際の進捗とプロジェクトの進捗ステータスに反映されるように、タスクに先行タスクを使用することをお勧めします。
* プロジェクト所有者は、状況のタイプを進行状況ステータスから手動に変更することで、進捗ステータスを使用する代わりに手動状況タイプを使用するようにプロジェクトを変更できます。

  >[!NOTE]
  >
  >次のいずれかのステータスにあるプロジェクトは、タスクの日付や進捗状況に関係なく、常に「目標どおり」としてマークされます。
  >
  >* アイデア
  >* リクエスト日
  >* 承認済み
  >* 却下

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

## Workfront が進捗ステータスに基づいてプロジェクトの状況をアップデートする方法

プロジェクトの状況タイプが手動に設定されている場合、プロジェクトの進捗ステータスとは別にプロジェクトの状況を決定することができます。

ただし、タスクの進行状況に基づいてプロジェクトの実際の進行状況を明確に把握できるように、プロジェクトの状況タイプを「進捗ステータス」に設定することをお勧めします。Workfront がプロジェクトの進捗ステータスを計算する方法について詳しくは、[プロジェクトの進捗ステータスの概要](../../../manage-work/projects/planning-a-project/project-progress-status.md)を参照してください。

この場合、プロジェクトの状況の値は以下のようになります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>プロジェクト状況</strong></td> 
   <td><strong>プロジェクトの進捗ステータス</strong></td> 
   <td><strong>Workfront 状況インジケーター</strong></td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>目標どおり</td> 
   <td>進捗ステータスが予定どおりのプロジェクトの場合、プロジェクトの状況は<strong>予定どおり</strong>です。 </td> 
   <td> <img src="assets/on-target-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>リスクあり</td> 
   <td>プロジェクトの進捗ステータスが「<strong>遅れ</strong>」または「<strong>危険あり</strong>」の場合、プロジェクトの状況は「<strong>危険あり</strong>」になります。</td> 
   <td> <img src="assets/at-risk-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>トラブル発生中</td> 
   <td>プロジェクトの進捗ステータスが「<strong>遅延</strong>」の場合、プロジェクトの状況は「<strong>トラブル発生中</strong>」になります。 </td> 
   <td> <img src="assets/in-trouble-project-condition-icon.png"> </td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>状況は環境に合わせてカスタマイズできるので、お使いの環境で状況の選択肢が 4 つ以上ある場合もあります。状況の名前は、上記の名前とは異なる場合があります。状況のカスタマイズについて詳しくは、[カスタム状況の作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)を参照してください。

## プロジェクトの状況、プロジェクトの状況のアップデート、および最終状況メモに関するレポート

プロジェクトレポートのビューで、プロジェクトの状況に関連する以下のフィールドを表示できます。

* **プロジェクトの状況：**&#x200B;プロジェクトの現在の状況を表示します。
* **プロジェクトの状況の更新**：新しい状況と共に、プロジェクトの更新ストリームでプロジェクト所有者が提供した最新の更新を表示します。\
  状況の更新に対して行われたコメントは、**状況の更新**&#x200B;列に表示されます。主な更新のみが表示されます。

* **最終状況メモ**：オブジェクトの所有者が最後にオブジェクトに入力した更新を表示します。このフィールドは、オブジェクトに対する所有者の最新のアクティビティやインタラクションを表示するのに役立ちます。\
  **最終状況メモ**&#x200B;列は、オブジェクトの最終メモのメモテキストが削除されている場合、空になります。オブジェクトに新規メモを入力すると、それが最終メモになり、列に再び表示されます。

レポートの作成方法について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。
