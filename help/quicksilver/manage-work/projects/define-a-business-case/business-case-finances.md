---
content-type: overview
navigation-topic: business-case-and-scorecards
title: ビジネス事例の財務分野の概要
description: 「ビジネスケース」サブタブには、プロジェクトの財務フィールドが含まれます。 一部の財務分野に値を設定するには、ビジネスケースの対応する領域に入力する必要があります。
author: Alina
feature: Work Management
exl-id: d420fc3e-e98d-47a0-a456-b2df17d72f34
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 2%

---

# ビジネス事例の財務分野の概要

「ビジネスケース」サブタブには、プロジェクトの財務フィールドが含まれます。 一部の財務分野に値を設定するには、ビジネスケースの対応する領域に入力する必要があります。  

ビジネス事例には、次のプロジェクト財務フィールドが表示されます。

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="col">フィールド名</th> 
   <th scope="col">説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>整合済み </td> 
   <td> <p>スコアカードに従ったプロジェクトの配置を表示します。 割合が高い場合は、プロジェクトが組織の目的と目標に適切に合致していることを示します。 <br>スコアカードの使用の詳細については、「 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md" class="MCXref xref">スコアカードの作成</a>.</p> <p>このフィールドは、「ビジネス事例の概要」領域に表示されます。 </p> </td> 
  </tr> 
  <tr> 
   <td>予算計上コスト</td> 
   <td> <p>プロジェクトの起動時にプロジェクトに関連付けられると推定される合計コストです。</p> <p>プロジェクトの予算原価は、次の式で計算されます。<br></p> <p><code>Budgeted Cost =&nbsp;Budgeted Expense Cost + Budgeted Labor Cost </code> <br> </p> <p>Adobe Workfrontは、生産資源プランナの予算時間を使用して、予算労務費を計算します。<br>予算原価の計算の詳細は、次を参照してください： <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">予算コストの計算</a>. </p> <p>このフィールドは、「ビジネス事例の概要」領域に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>予算計上費用コスト</td> 
   <td> <p>プロジェクトのすべての費用の予算コスト。 </p> <p>これは次の数式で計算されます。</p> <p><code>Budgeted Expense Cost = SUM(Planned Amount of Expenses on the project) </code></p> <p>費用の計算について詳しくは、 <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">プロジェクト費用の管理 </a>.</p> <p>このフィールドは、「費用」領域に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>予算計上労力コスト</td> 
   <td> <p>プロジェクトでの作業を完了するために割り当てられたリソースに関連付けられたコスト。</p> <p>プロジェクトの予算労務費は、次の式で計算されます。<br></p> <p><code>Budgeted Labor Cost = SUM(Estimated/ Budgeted hours for each job role on the project * Cost per Hour rate of each job role on the project) </code></p> <p>Workfrontは、生産資源プランナの予算時間を使用して、予算労務費を計算します。<br>予算労務費の計算の詳細は、 <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">プロジェクトの予算労務費と予算時間の把握</a>.</p> <p>このフィールドは、ビジネスケースの「生産資源予算」領域に表示されます。 </p> </td> 
  </tr> 
  <tr> 
   <td>費用計画原価</td> 
   <td> <p>これは予算費用原価と同じです。 </p> <p>注意：費用計画原価は、プロジェクトの計画原価とは異なります。 「費用計画原価」はプロジェクトの費用の計画金額を計算し、「計画原価」はプロジェクトの計画時間を使用して計算します。 </p> <p>このフィールドは、費用ごとに「費用」領域に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>純価</td> 
   <td> <p>これは、メリットを計算し、コストを削除した後のプロジェクトの期待値の合計です。</p> <p>プロジェクトの正味値は、次の式で計算されます。<br></p> <p><code>Net Value = Planned Benefit - Budgeted Cost - Potential Risk</code>。 <br></p> <p>正味値の計算の詳細は、 <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">正味値を計算</a>.<br></p> <p>このフィールドは、「ビジネス事例の概要」領域に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>予定便益</td> 
   <td>このプロジェクトが完了したときの、組織の金銭上の利益の手動見積もり。 任意の金額の通貨を指定でき、ユーザーや管理する各プロジェクトに固有の通貨です。 計画福利厚生に負の値を設定することはできません。 このフィールドは「ビジネス事例の概要」領域に表示され、ビジネス事例の「プロジェクト情報」領域で編集できます。 </td> 
  </tr> 
  <tr> 
   <td>潜在的なリスクコスト</td> 
   <td> <p>これは、プロジェクトに関するすべてのリスクの潜在的なコストです。 </p> <p>これは、次の式を使用して計算されます。</p> <p><code>Potential Risk = SUM(Potential Cost * Probability of Risk) </code></p> <p>プロジェクトのリスクの詳細については、 <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">プロジェクトのリスクの作成と編集</a>.</p> <p>このフィールドは、「ビジネス事例の概要」領域に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>潜在的な危険</td> 
   <td> <p>「ビジネス・ケース・サマリ」では、リスクが発生する可能性に基づいて、発生するすべてのリスクのコストを示します。 例えば、リスクの潜在的なコストが 100 ドルで、発生する確率が 10%の場合、潜在的なリスクは 10 ドルになります。 「ビジネス・ケース・サマリー」の潜在的リスクは、次の式で計算されます。</p> <p><code>Potential&nbsp;Risk = SUM(Risk Potential Cost x Probability)</code> 全てのリスクに対して </p> </td> 
  </tr> 
  <tr> 
   <td>リスク軽減コスト</td> 
   <td> <p>見積もり中のリスクの緩和計画のコストは、プロジェクトで発生する可能性があります。<br>プロジェクトのリスクの詳細については、 <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">プロジェクトのリスクの作成と編集</a>.</p> <p>このフィールドは、プロジェクトで指定された各リスクの [ リスク ] 領域に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>1 つのリスクに対する潜在的なコスト</td> 
   <td> <p>確率に関係なく、プロジェクトで定義されたリスクが実際に発生する場合の概算財務コスト。 </p> <p>これは手動で更新したフィールドで、ビジネスケースの「リスク」領域の各リスクに表示されます。 </p> </td> 
  </tr> 
  <tr> 
   <td>リスク総潜在的コスト</td> 
   <td> <p>これは、実際に発生したプロジェクトで定義されたすべてのリスクの総概算財務コストです。 </p> <p>これは次の数式で計算されます。</p> <p><code>Risks Total Potential Cost = SUM(Potential Cost of all risks on the project) </code></p> <p>ビジネスケースの「リスク」領域のタイトルの横に通貨番号として表示されます。</p> </td> 
  </tr> 
 </tbody> 
</table>
