---
title: プロジェクト制限の概要
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: Adobe Workfrontには、プロジェクトに関連付けるオブジェクトの数に制限があります。 製品のパフォーマンスを向上し、Workfrontでのエクスペリエンスを強化するために、プロジェクトの制限が設けられています。
author: Alina
feature: Work Management
exl-id: 60576107-89f1-4328-89e2-5b1e5e243fd9
source-git-commit: 11c4028038fe3d410ee0d4f238d2138435d9a3fa
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 0%

---

# プロジェクト制限の概要

Adobe Workfrontには、プロジェクトに関連付けるオブジェクトの数に制限があります。 製品のパフォーマンスを向上し、Workfrontでのエクスペリエンスを強化するために、プロジェクトの制限が設けられています。

プロジェクトに関連付けられた以下のオブジェクトには、次の制限があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>タスク</p></td> 
   <td>  <p>プロジェクトあたりのタスクの最大数は 5,000 です。 タスクの数がこの最大値に近づくと、警告メッセージが表示されます。 最大値に達すると、エラーメッセージが表示され、追加のタスクをプロジェクトに追加できなくなります。</p> <p>この最大値に達しないようにするには、閉じられたタスクを、閉じられたタスク用に指定された別のプロジェクトに移動します。 これらのプロジェクトに関するレポートは調整が必要になる場合があります。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>問題</p></td> 
   <td>  <p>プロジェクトあたりの最大問題数は 10,000 件です。 問題の数がこの値を超えると、警告メッセージが表示されます。 最大値に達すると、エラーメッセージが表示され、追加の問題をプロジェクトに追加できなくなります。</p> <p>この最大値に達しないようにするには、閉じられた問題を、閉じられた問題用に指定された別のプロジェクトに移動します。 これらのプロジェクトに関するレポートは調整が必要になる場合があります。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>期間</p></td> 
   <td> <p>Workfrontがタイムラインを自動的に計算するには、プロジェクトの最大期間を 15 年にする必要があります。 プロジェクト期間が最大値に近づくと、警告メッセージが表示されます。 最大値に達すると、警告メッセージが表示され、タイムラインの自動計算がおこなわれなくなります。</p> <p>プロジェクト内のタスクの日付を調整すると、プロジェクトの期間が 15 年を下回った時点で、自動タイムライン計算が再開されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>タイムラインの計算</p></td> 
   <td>Workfrontは、6 か月間更新されていないプロジェクトに対しては、自動タイムライン計算を実行しません。更新がおこなわれるまで再開されません。<p>3 か月間更新されていないプロジェクトの場合、Workfrontは夜間ではなく毎週タイムライン計算を実行します。</p><p>プロジェクトタイムラインの計算について詳しくは、 <a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">プロジェクトタイムラインを再計算</a>. </p></td> 
  </tr> 
 </tbody> 
</table>

<!-- Notes from the table: 
     <p>For tasks limits: (This is NOT TRUE , but the PMs always wanted this to stay the way it is because they don't want customers creating projects bigger than this.)</p>
    <p>For issue limits: (this is true only for some clusters; according to Anna A., some clusters are set to a million.)</p>
    -->