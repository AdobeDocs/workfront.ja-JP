---
content-type: overview
navigation-topic: business-case-and-scorecards
title: ビジネスケースの財務フィールドの概要
description: 「ビジネスケース」サブタブには、プロジェクトの財務フィールドが含まれます。 一部の財務フィールドに値を設定するには、ビジネスケースの対応するエリアに入力する必要があります。
author: Becky
feature: Work Management
exl-id: d420fc3e-e98d-47a0-a456-b2df17d72f34
TQID: https://experienceleague.adobe.com/rtNmXiZoe-NqCa8neuASw1BDMl8OBBbsN6Jm0a6Z-90
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 746
ht-degree: 80%

---

# ビジネスケースの財務フィールドの概要

「ビジネスケース」サブタブには、プロジェクトの財務フィールドが含まれます。 一部の財務フィールドに値を設定するには、ビジネスケースの対応するエリアに入力する必要があります。

ビジネスケースには、次のプロジェクト財務フィールドが表示されます。

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
   <td>整合済み </td> 
   <td> <p>スコアカードに基づいてプロジェクトのアラインメントを表示します。 高い割合は、プロジェクトが組織の目的と目標に適切に合致していることを示します。 <br>スコアカードの使用の詳細については、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md" class="MCXref xref">スコアカードの作成</a>を参照してください。</p> <p>このフィールドは、ビジネスケースの概要領域に表示されます。 </p> </td> 
  </tr> 
  <tr> 
   <td>予算計上コスト</td> 
   <td> <p>プロジェクトの起動時にプロジェクトに関連付けられると推定される合計コストです。</p> <p>プロジェクトの予算計上コストは、次の式で計算されます。<br></p> <p><code>Budgeted Cost = Budgeted Expense Cost + Budgeted Labor Cost </code> <br> </p> <p>Adobe Workfrontでは、リソース プランナーの予算計上時間を使用して、予算計上労力コストを計算します。<br>予算計上費用の計算について詳しくは、<a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">予算計上費用の計算</a>を参照してください。 </p> <p>このフィールドは、ビジネスケースの概要領域に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>予算計上費用コスト</td> 
   <td> <p>プロジェクトのすべての費用の予算コスト。 </p> <p>これは次の数式で計算されます。</p> <p><code>Budgeted Expense Cost = SUM(Planned Amount of Expenses on the project) </code></p> <p>費用の計算について詳しくは、<a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">プロジェクト費用の管理</a>を参照してください。</p> <p>このフィールドは「費用」領域に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>予算計上労力コスト</td> 
   <td> <p>プロジェクトでの作業を完了するために割り当てられたリソースに関連付けられたコスト。</p> <p>プロジェクトの予算計上労力コストは、次の式で計算されます。<br></p> <p><code>Budgeted Labor Cost = SUM(Estimated/ Budgeted hours for each job role on the project * Cost per Hour rate of each job role on the project) </code><br></p> <p>Workfrontでは、リソース プランナーの予算計上時間を使用して、予算計上労力コストを計算します。<br>予算計上労力コストの計算について詳しくは、<a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref"> プロジェクトの予算計上労力コストと予算計上時間について</a>を参照してください。</p> <p>このフィールドは、ビジネスケースのリソース予算計上エリアに表示されます。 </p> </td> 
  </tr> 
  <tr> 
   <td>費用予定コスト</td> 
   <td> <p>これは予算計上費用コストと同じです。 </p> <p>メモ：費用予定コストは、プロジェクトの予定コストとは異なります。 費用予定コストは、プロジェクトの費用の予定金額を計算します。一方、予定コストは、プロジェクトの予定時間数を使用して計算されます。 </p> <p>このフィールドは、各費用の「費用」領域に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>純価</td> 
   <td> <p>これは、メリットを計算し、コストを削除した後のプロジェクトの期待値の合計です。</p> <p>プロジェクト純価は、次の式で計算されます。<br></p> <p><code>Net Value = Planned Benefit - Budgeted Cost - Potential Risk</code>。 <br></p> <p>純価の計算について詳しくは、<a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">純価の計算</a>を参照してください。<br></p> <p>このフィールドは、ビジネスケースの概要領域に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>予定利益</td> 
   <td>このプロジェクトが完了したときの、組織の金銭上の利益の手動見積もり。 任意の金額の通貨を指定でき、ユーザーや管理する各プロジェクトに固有です。 予定利益に負の値を設定することはできません。 このフィールドはビジネスケースの概要エリアに表示され、ビジネスケースのプロジェクト情報エリアで編集できます。 </td> 
  </tr> 
  <tr> 
   <td>潜在的なリスク費用</td> 
   <td> <p>これは、プロジェクトに関するすべてのリスクの潜在的なコストです。 </p> <p>これは、次の式を使用して計算されます。</p> <p><code>Potential Risk = SUM(Potential Cost * Probability of Risk) </code></p> <p>プロジェクトのリスクについて詳しくは、<a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref"> プロジェクトのリスクの作成と編集</a>を参照してください。</p> <p>このフィールドは、ビジネスケースの概要領域に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>潜在的な危険</td> 
   <td> <p>ビジネスケースの概要では、リスクが発生する可能性に基づいて、発生するすべてのリスクのコストを示します。 例えば、リスクの潜在的なコストが100 ドルで、発生する可能性が10%の場合、潜在的なリスクは10 ドルとなります。 ビジネスケースの概要での潜在的リスクは、次の式で計算されます。</p> <p><code>Potential Risk = SUM(Risk Potential Cost x Probability)</code> すべてのリスクに対して同じです。 </p> </td> 
  </tr> 
  <tr> 
   <td>リスク軽減コスト</td> 
   <td> <p>見積もっているリスクに対する緩和計画のコストは、プロジェクトで発生する可能性があります。<br>プロジェクトに関するリスクについて詳しくは、<a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">プロジェクトのリスクの作成と編集</a>を参照してください。</p> <p>このフィールドは、プロジェクトで指定された各リスクの「リスク」領域に表示されます。</p> </td> 
  </tr> 
  <tr> 
   <td>1 つのリスクに対する潜在的なコスト</td> 
   <td> <p>確率に関係なく、プロジェクトで定義されたリスクが実際に発生する場合の概算財務コスト。 </p> <p>これは手動で更新したフィールドで、ビジネスケースのリスクエリアで各リスクに対して表示されます。 </p> </td> 
  </tr> 
  <tr> 
   <td>リスク総潜在的コスト</td> 
   <td> <p>これは、実際に発生したプロジェクトで定義されたすべてのリスクの総概算財務コストです。 </p> <p>これは次の数式で計算されます。</p> <p><code>Risks Total Potential Cost = SUM(Potential Cost of all risks on the project) </code></p> <p>ビジネスケースのリスクエリアのタイトルの横に通貨番号として表示されます。</p> </td> 
  </tr> 
 </tbody> 
</table>
