---
title: プロジェクト制限の概要
content-type: overview
product-area: projects
navigation-topic: manage-projects
description: Adobe Workfront には、プロジェクトに関連付けることができるオブジェクトの数に制限があります。製品のパフォーマンスを向上させ、Workfront でのエクスペリエンスを強化するために、プロジェクトの制限が設けられています。
author: Alina
feature: Work Management
exl-id: 60576107-89f1-4328-89e2-5b1e5e243fd9
source-git-commit: 8be7534dfc0a1227bd2274ad093a88ae19b4691d
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 87%

---

# プロジェクト制限の概要

Adobe Workfront には、プロジェクトに関連付けることができるオブジェクトの数に制限があります。製品のパフォーマンスを向上させ、Workfront でのエクスペリエンスを強化するために、プロジェクトの制限が設けられています。

プロジェクトに関連付けられた以下のオブジェクトには、次の制限があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>タスク</p></td> 
   <td>  <p>プロジェクトあたりのタスクの最大数は 5,000 です。タスクの数がこの最大値に近づくと、警告メッセージが表示されます。最大値に達すると、エラーメッセージが表示され、追加のタスクをプロジェクトに追加できなくなります。</p> <p>この最大値に達しないようにするには、閉じられたタスクを、閉じられたタスク用に指定された別のプロジェクトに移動します。これらのプロジェクトに関するレポートは、調整が必要になる場合があります。</p>

<b>重要</b>

タスクに多くの依存関係があるプロジェクトの場合、タイムラインの計算時やプロジェクトでの作業時に、パフォーマンスが低下することがあります。

このため、複雑な依存関係を持つプロジェクトのタスクの数は、許容される最大タスク数の 5,000 個を大幅に下回ることをお勧めします。

プロジェクトのタイムラインの再計算に影響を与えたり、再計算を妨げたりする可能性のあるタスクの依存関係の例を以下に示します。

<ul><li>子の数</li>
   <li>複数レベルのタスクインデント</li>
   <li>先行タスクの数</li>
   <li>複数の割り当て</li>
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>イシュー</p></td> 
   <td>  <p>プロジェクトあたりの最大イシュー数は 10,000 件です。イシューの数がこの最大値に近づくと、警告メッセージが表示されます。最大値に達すると、エラーメッセージが表示され、追加のイシューをプロジェクトに追加できなくなります。</p> <p>この最大値に達しないようにするには、閉じられたイシューを、閉じられたイシュー用に指定された別のプロジェクトに移動します。これらのプロジェクトに関するレポートは、調整が必要になる場合があります。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>期間</p></td> 
   <td> <p>Workfront がタイムラインを自動的に計算するには、プロジェクトの最大期間を 15 年にする必要があります。プロジェクト期間が最大値に近づくと、警告メッセージが表示されます。最大値に達すると、警告メッセージが表示され、タイムラインの自動計算が行われなくなります。</p> <p>プロジェクト内のタスクの日付を調整すると、プロジェクトの期間が 15 年を下回った時点で、自動タイムライン計算が再開されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>タイムラインの計算</p></td> 
   <td>Workfront は、6 か月間更新されていないプロジェクトに対しては、自動タイムライン計算を実行せず、更新が行われるまで再開されません。<p>3 か月間更新されていないプロジェクトの場合、Workfront は夜間ではなく毎週タイムライン計算を実行します。</p><p>プロジェクトタイムラインの計算について詳しくは、<a href="../../../manage-work/projects/manage-projects/recalculate-project-timeline.md" class="MCXref xref">プロジェクトタイムラインの再計算</a>を参照してください。 </p></td> 
  </tr> 
 </tbody> 
</table>

<!-- Notes from the table: 
     <p>For tasks limits: (This is NOT TRUE , but the PMs always wanted this to stay the way it is because they don't want customers creating projects bigger than this.)</p>
    <p>For issue limits: (this is true only for some clusters; according to Anna A., some clusters are set to a million.)</p>
    -->