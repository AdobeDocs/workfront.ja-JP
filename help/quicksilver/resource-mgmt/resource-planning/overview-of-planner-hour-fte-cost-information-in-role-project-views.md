---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: リソースプランナーのプロジェクトビューと役割ビューの時間数、FTE およびコスト情報の概要
description: リソースプランナーのプロジェクトビューと役割ビューの時間数、FTE およびコスト情報の概要
author: Alina
feature: Resource Management
exl-id: 76de1945-3f19-4c91-801c-07dc79e646ad
source-git-commit: 3486a2523a038bdd83c3c2001001a119fd0508ad
workflow-type: ht
source-wordcount: '2973'
ht-degree: 100%

---

# リソースプランナーのプロジェクトビューと役割ビューの時間、FTE、コスト情報の概要

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this came from the budget-resources-project-role-views-resource-planner article)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: relink all articles pointing to this section to the new article)</p>
-->

プロジェクトで達成する必要のある作業に対してリソースを予算計上することが、リソースプランナーの主な機能です。リソースの空き時間を表示し、リソースが割り当てられているプロジェクトに時間を割り当てることができます。

リソースプランナーでのリソースの予算計上について詳しくは、[プロジェクトビューと役割ビューを使用したリソースプランナーでのリソースの予算計上](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)を参照してください。

この記事では、リソースプランナーでリソースの予算計上を開始する前に知っておく必要がある主要概念の一部を説明します。

## リソース予算計上の概要

リソースプランナーを使用してリソースを予算計上する際は、次の点に注意してください。

* リソースの割り当てを予算計上するには、リソースがプロジェクトでの作業完了に利用できる時間、FTE、またはコストの量を指定します。リソースの時間またはコストを予算計上すると、そのリソースの利用可能時間数、FTE、またはコストが、予算計上された量だけ減少します。その結果、予算計上するプロジェクトに従うプロジェクトの利用可能時間数、FTE またはコストの量が、該当するプロジェクトの該当するユーザーおよび役割に対して減少します。

  >[!IMPORTANT]
  >
  >リソースは 15 年の期間にわたって予算計上できます。期間が 15 年を超えるプロジェクトのリソースを予算計上すると、計上する情報が正確でなくなる可能性があります。

* プロジェクトのタイムラインに関係なく、リソースプランナーに表示される任意の時間枠のリソースの時間、FTE またはコストの予算を計上できます。例えば、（予定時間数に関連付けられた）プロジェクトのタイムラインではリソースが使用できないが別の時間では使用できる可能性があることを示す場合は、予定時間数がゼロの時間枠にリソースの予算を計上することができます（その期間にリソースが作業に使用できるようになる場合）。これを行った後に、リソースの空き時間に合わせてプロジェクトのタイムラインを手動で変更できます。

  >[!NOTE]
  >
  >まず、担当業務またはユーザーに対して、時間、FTE、またはコストを手動で予算計上することをお勧めします。自動オプションを使用してプロジェクトとリソースの時間を予算計上できるのは、予定の時間数、FTE またはコストの量が、予算計上された時間数、FTE またはコストと常に一致する場合のみです。\
  >リソースプランナーで予算計上の自動オプションを使用する方法について詳しくは、[Adobe Workfront Resource Planner を使用したリソースの可用性と割り当てのレビュー](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md)の記事の「プロジェクトと役割の自動予算計上」の節を参照してください。

* FTE またはコストの予算計上は、時間の予算計上と同じです。その場合、Adobe Workfront では、予算計上するリソースに関して、時間ではなく FTE とコストの値が使用されます。

  リソースプランナーでのコストの計算方法について詳しくは、[リソースプランナーでのコストの計算](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md)を参照してください。

* リソースプランナーでのリソースの割り当ての予算計上は、次の方法で行われます。

   * 手動

     または

   * 自動（**プロジェクト別に表示**&#x200B;ビューおよび&#x200B;**役割別に表示**&#x200B;ビューのプロジェクトと役割のオプションを使用）。

  詳しくは、[プロジェクトビューと役割ビューを使用したリソースプランナーでのリソースの予算計上](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)を参照してください。

* ユーザーが担当業務を変更した場合や、リソースプールから削除、非アクティブ化、または除去された場合、その役割に予算計上された時間は変更されず、その役割の残りのユーザーに再配分されます。担当業務に関連付けられているユーザーがいなくなった場合、その役割の予算計上時間数はゼロになります。

プロジェクトと役割のオプションについて詳しくは、この記事の[リソースプランナーの時間、FTE、コストの値について](#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner)の節を参照してください。

## リソースプランナーの時間、FTE、コストの値について {#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this needs to be broken into its own article and leave here just the how-to: see this article: overview-of-planner-hour-fte-cost-information-in-role-project-views)</p>
-->

リソースを予算計上し、リソースプランナーで予算計上時間数の情報を更新する前に、次の概念を理解しておく必要があります。

* **予定時間数、FTE またはコスト**：タスクとイシューに関する定義に従って行う必要がある作業。
* **利用可能時間数、FTE またはコスト**：ユーザーに関連付けられたスケジュールに従って、ユーザーまたは担当業務が利用可能な時間。

この情報は、リソース（ユーザーまたは役割）ごと、プロジェクトごとに、リソースプランナーに表示されます。

プロジェクトのプロジェクトビューと役割ビューに表示される内容について詳しくは、[リソースプランナーのナビゲーションの概要](../../resource-mgmt/resource-planning/resource-planner-navigation.md)の記事を参照してください。

リソースプランナーでのコストの計算方法について詳しくは、[リソースプランナーでのコストの計算](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md)の記事を参照してください。

>[!NOTE]
>
>コストによる予算計上は、時間または FTEによる予算作成と同じですが、Workfront がリソースプランナーのコストを計算する方法を理解する必要があります。
>
>リソースプランナーでのコストの計算方法について詳しくは、[リソースプランナーでのコストの計算](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md)の記事を参照してください。

次の表に、プロジェクトビューまたはロールビューを適用する際にリソースプランナーに表示される割り当てと空き時間の情報を示します。この情報は、時間別、FTE 別、またはコスト別に表示できます。

* [AVL（利用可能）列](#the-avl-available-column)
* [PLN（予定）列](#the-pln-planned-column)
* [BDG（予算計上）列](#the-bdg-budgeted-column)
* [VAR（差異）列](#the-var-variance-column)
* [NET 列](#the-net-column)

### AVL（利用可能）列 {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>表示対象</strong> </td> 
   <td><strong>説明</strong> </td> 
  </tr> 
  <tr> 
   <td>プロジェクト </td> 
   <td> <p>選択した時間枠で、プロジェクトのすべてのユーザーがスケジュールに従って作業できる時間数、FTE またはコストの合計。 </p> </td> 
  </tr> 
  <tr> 
   <td>役割</td> 
   <td> <p>選択した時間枠で、この役割に関連付けられているすべてのユーザーが、スケジュール、およびユーザーの特定の役割に対する <strong>FTE 使用可能時間の割合</strong>に従って作業できる時間数、FTE またはコストの合計。 </p> <p>次の点に注意してください。 </p> 
    <ul> 
     <li>担当業務に関連付けられているユーザーがいない場合、担当業務の利用可能時間数の値は 0 になります。 </li> 
     <li>ユーザーがプライマリ担当業務に関連付けられ、その役割の <strong>FTE 使用可能時間の割合</strong>が 0％の場合、利用可能時間数の値は 0 になります。</li> 
     <li>ユーザーがその他の役割に関連付けられていて、その役割の <strong>FTE 使用可能時間の割合</strong>が 0％の場合、その他の役割はリソースプランナーにリストされず、ユーザーはプライマリ担当業務の下にのみ表示されます。</li> 
    </ul> <p>担当業務の<strong>FTE 使用可能時間の割合</strong>について詳しくは、<a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">ユーザーのプロファイルの編集</a>の記事を参照してください。</p> <p>リソースプランナーでの担当業務の利用可能時間の計算方法について詳しくは、<a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">リソースプランナーでのユーザーおよび役割の時間と FTE の計算の概要</a>の記事の「リソースプランナーでの担当業務の利用可能時間数と FTE の計算」の節を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>ユーザー</td> 
   <td> <p>選択した時間枠で、ユーザーのスケジュールに基づき、ユーザーが作業できる時間数、FTE またはコスト。この数値は、次に関連する時間数を差し引いたものです。</p> 
    <ul> 
     <li>スケジュールの例外</li> 
     <li>ユーザーの休暇</li> 
     <li>その他のプロジェクトに対する予算計上時間数 </li> 
    </ul> <p>ユーザーの利用可能時間数、FTE またはコストは、次の内容に従って変更されます。 </p> 
    <ul> 
     <li>システムレベルでのリソース管理環境設定に基づいた、スケジュールと FTE の計算方法。<br><p>ユーザーと担当業務の利用可能時間の計算について詳しくは、<a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">リソースプランナーでのユーザーおよび役割の時間と FTE の計算の概要</a>を参照してください。</p>
     Workfront でのリソース管理環境設定について詳しくは、<a href="../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md">リソース管理環境設定の指定</a>を参照してください。</li> 
    </ul> 
    <ul> 
     <li><strong>プロジェクト計画の優先度</strong>（ユーザーの作業が予算に計上されている場合）<br>プロジェクト計画の優先度がユーザーの利用可能時間数に与える影響について詳しくは、<a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">リソースプランナーのナビゲーションの概要</a>を参照してください。 </li> 
    </ul> <p>ユーザーの非アクティブ化がスケジューリングされている場合、非アクティブ化日以降の利用可能時間数、FTE またはコストはゼロになります。<br>ユーザーの非アクティブ化について詳しくは、<a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">ユーザーの非アクティブ化または再アクティブ化</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>



### 「PLN（予定）」列 {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>表示対象</strong> </td> 
   <td><strong>説明</strong> </td> 
  </tr> 
  <tr> 
   <td>プロジェクト</td> 
   <td> <p>選択した時間枠で、プロジェクトのプロジェクト詳細タブに表示されるプロジェクトの下にリストされたすべての担当業務またはユーザーの予定時間数、FTE またはコストの合計（「<strong>役割なし</strong>」または「<strong>ユーザーなし</strong>」セクションも含む）。 </p> <p><b>メモ</b>

日次のユーザー割り当てを手動で調整すると、リソースプランナーの週次、月次または四半期の予定時間数の値が変更される場合があります。ワークロードバランサーを使用して、タスクとイシューに対する日次のユーザー割り当てを手動で調整できます。詳しくは、<a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">ワークロードバランサーでのユーザー割り当ての管理</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td>役割</td> 
   <td> <p>選択した時間枠内で、役割に割り当てられたすべてのタスクからの予定時間数の合計。 </p> <p>「<strong>役割なし</strong>」セクションには、未割り当てのタスク、チームに割り当てられているタスク（時間数は「<strong>ユーザーなし</strong>」セクションに一覧表示）、または担当業務に関連付けられていないユーザーに割り当てられたタスクのいずれかに関連付けられた予定時間数が表示されます。 </p> </td> 
  </tr> 
  <tr> 
   <td>ユーザー</td> 
   <td> <p>特定の役割のユーザーに割り当てられたすべてのタスクの、選択した時間枠での予定時間数。 </p> <p>「<strong>ユーザーなし</strong>」セクションには、未割り当てまたはチームに割り当てられているタスクに関連する予定時間数が表示されます。 </p> </td> 
  </tr> 
 </tbody> 
</table>

予定時間数を表示する際は、次の点を考慮してください。

* プロジェクトビューと役割ビューには、リソースプランナーでのタスクの割り当てに関する情報は表示されませんが、予定時間数の値は、プロジェクト内のタスクの予定時間数から取得されます。
* 予定時間数は、タスクの期間内の各日に、タスクに割り当てられたリソースに対して均等に配分されます。タスク期間は、タスクの予定開始日と完了日に基づき、その期間内のすべてのカレンダー日が含まれます。\
  Workfront では、ユーザーまたはプロジェクトに予定時間数を配分する際に、ユーザーまたはプロジェクトのスケジュールが考慮されます。この場合、予定時間数は、週末、休日、スケジュール例外を除くタスクの期間内の各日に均等に配分されます。\
  例えば、リソースプランナーを週別に表示していて、プロジェクトに複数週にわたるタスクがある場合、1 週間あたりの予定時間数は、その週の何日がタスク期間に含まれているかによって異なります。この動作は、月別または四半期別でリソースプランナーを表示する場合や、タスクが複数の月または四半期にまたがる場合と同様です。\
  週末、スケジュールの例外および休暇日は、この配分から除外されます。
* 各リソースの予定時間数の計算には、次のタスクのカテゴリが含まれます。

   * リソースプール、担当業務、またはプロジェクトのチームでユーザーに割り当てられたタスク\
     タスクがチームに割り当てられると、その割り当ては「**役割なし**」および「**ユーザーなし**」セクションに表示されます。チームに関連付けられた予定時間数は表示できますが、タスクに関連付けられた役割やユーザーがないので、時間数を予算計上することはできません。

   * 未割り当てタスク

* リソースプランナーの予定時間数には、次に関連する予定時間数は含まれません。

   * 親タスク
   * リソースプールを持たないユーザーに割り当てられたタスク
   * イシュー（**イシューの時間数を含める**&#x200B;の設定が無効の場合）。

* タスクの期間が 0 の場合、予定時間数はリソースプランナーに表示されません。
* 非アクティブ化されたユーザーに関連付けられた予定時間数は表示されません。

### BDG（予算）列 {#the-bdg-budgeted-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>表示対象</strong> </td> 
   <td><strong>説明</strong> </td> 
  </tr> 
  <tr> 
   <td>プロジェクト</td> 
   <td> <p>選択した時間枠に対するプロジェクトの予算計上時間数、FTE、またはコストを見積もるための手動入力。 </p> <p>プロジェクトビューでは、プロジェクトに予算を計上した時間数が、プロジェクトの下に一覧表示される担当業務に配分されます。各役割の予定時間数によって、予算計上時間数が役割にどのように配分されるかが決まります。 予算計上時間数は、「予定時間数」の値が高い役割に配分されます。 </p> <p>役割ビューでは、プロジェクトの予算計上時間数は、プロジェクト上の役割やユーザーに配分されません。 </p> </td> 
  </tr> 
  <tr> 
   <td>役割</td> 
   <td> <p>選択した時間枠に対する役割の予算計上時間数を見積もるための手動入力。 </p> <p>ユーザーが担当業務に関連付けられていない場合、その担当業務の予算計上時間を見積もることはできません。 </p> <p>役割ビューでは、その役割に予算計上した時間数が、その役割の下に一覧表示されるプロジェクトに配分されます。 各プロジェクトの予定時間数によって、予算計上時間数がプロジェクトにどのように配分されるかが決まります。予算計上時間数は、予定時間数の値が大きいプロジェクトに配分されます。</p> <p>プロジェクトビューでは、役割の予算計上時間数は、役割に関連付けられたプロジェクトやユーザーに配分されません。 </p> </td> 
  </tr> 
  <tr> 
   <td>ユーザー</td> 
   <td> <p>選択した時間枠に対するユーザーの予算計上時間数を見積もるための手動入力。 </p> <p> <p><b>メモ</b> タスクには割り当てられていないが、プロジェクトのリソースプールに関連付けられているユーザーの予算計上時間数を見積もることができます。これらのユーザーがリソースプランナーにも表示されるためです。ただし、タスクに割り当てられていない場合は、予定時間数はゼロにする必要があります。 </p> </p> </td> 
  </tr> 
 </tbody> 
</table>

予算計上時間数を使用する際は、次の点を考慮してください。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(Duplicated below ??)
</MadCap:conditionalText>
-->

* リソースを予算計上できるのは、プロジェクトに対するリソース管理、財務データの編集および財務管理の権限を持っている場合のみです。

  リソース予算計上に必要なアクセス権について詳しくは、[Adobe Workfront でのリソース予算計上に必要なアクセス権](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md)の記事を参照してください。

* デフォルトでは、すべてのリソースとすべてのプロジェクトに対する、リソースプランナーの予算計上時間数は 0 です。
* ユーザーと役割の予算計上時間数を手動で見積もることも、プロジェクトまたは担当業務の&#x200B;**その他**&#x200B;メニューのリンクの 1 つを使用して、予定時間数に応じて更新することもできます。\
  プロジェクトと役割のオプションについて詳しくは、[リソースプランナーのプロジェクトビューと役割ビューの時間、FTE、コスト情報の概要](#Budget)を参照してください。

* 時間数、FTE、コストを予算計上できる最短の期間は 1 週間です。 1 日の時間、FTE、コストを予算計上することはできません。
* 予算計上時間数は、タスクの期間内の各日に、タスクに割り当てられたリソースに対して均等に配分されます。タスク期間は、タスクの予定開始日と完了日に基づき、その期間内のすべてのカレンダー日が含まれます。\
  Workfront では、ユーザーまたはプロジェクトに予算計上時間数を配分する際に、ユーザーまたはプロジェクトのスケジュールが考慮されます。この場合、予算計上時間数は、週末を除くタスク期間内の各日に均等に配分されますが、休日やスケジュールの例外も含まれます。\
  例えば、リソースプランナーを週別に表示し、複数週にわたるタスクがある場合、1 週間あたりの予定時間数は、その週内のタスク期間に含まれる日数によって異なります。週末はこの配分から除外されます。 この動作は、月別または四半期別でリソースプランナーを表示する場合や、タスクが複数の月または四半期にまたがる場合と同様です。

* 新規レポートのレポートオブジェクトとして予算計上時間数を選択すると、予算計上時間数についてレポートを作成できます。\
  Workfront でレポートできるオブジェクトについて詳しくは、[Adobe Workfront のオブジェクトについて](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)の記事の「オブジェクトに関するレポート」の節を参照してください。\
  予算計上時間数のレポートの作成方法については、[レポート：予算計上時間数](../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md)の記事を参照してください。

* 後で非アクティブ化したユーザーに対して、以前に予算計上された時間は表示されません。

### VAR（平方偏差）列 {#the-var-variance-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>表示対象</strong> </td> 
   <td><strong>説明</strong> </td> 
  </tr> 
  <tr> 
   <td>プロジェクト</td> 
   <td> <p>時間、FTE、コスト差異は、プロジェクトの全予定時間数を完了するのに十分な予算計上時間数がプロジェクトにあるかどうかを示します。 </p> <p>プロジェクト時間、FTE、コスト差異は、次の式を使用して計算します。</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>役割</td> 
   <td> <p>時間、FTE、コスト差異は、役割に割り当てられた予定時間数を完了するのに十分な予算計上時間数、FTE、コストがあるかどうかを示します。 </p> <p>役割時間、FTE、コスト差異は、次の式を使用して計算します。</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>ユーザー</td> 
   <td> <p>時間、FTE、コスト差異は、ユーザーが割り当てられた予定時間数を完了するのに十分な予算計上時間数があるかどうかを示します。 </p> <p>ユーザー時間、FTE、コスト差異は、次の式を使用して計算します。</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>時間、FTE、コスト差異が赤色で表示される場合は、完了する必要がある実際の作業の予定時間数よりも少ない予算計上時間数が見積もられています。 この場合、この予算計上時間数では作業を完了するのに十分ではない可能性があります。

### NET 列  {#the-net-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>表示対象</strong> </td> 
   <td><strong>説明</strong> </td> 
  </tr> 
  <tr> 
   <td>プロジェクト</td> 
   <td> 
    <div> 
     <p>プロジェクトの純残存時間、FTE、コストには、次のいずれかが表示されます。 </p> 
     <ul> 
      <li> <p>使用可能な時間またはコストと、プロジェクトの予算計上時間またはコストの差異：</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p>「使用可能な時間またはコスト」と、「純残存計算で予定（PLN）値を使用」設定が有効な場合の、プロジェクトの予定時間数またはコストの差異： </p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code>
      </p>

<p><b>ヒント</b></p>        
  <p>このオプションは、選択した項目を表示セクションでビューをカスタマイズした場合にのみ適用されます。</p>
  <p>詳しくは、<a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" >Adobe Workfront Resource Planner を使用したリソースの可用性と割り当てのレビュー</a>を参照してください。 </p> 
      </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>役割</td> 
   <td> 
    <div> 
     <p>役割の正味時間、FTE、コストには、次のいずれかが表示されます。 </p> 
     <ul> 
      <li> <p>使用可能な時間またはコストと、役割の予算時間またはコストの差異：</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>「使用可能な時間またはコスト」と、「NET 計算で予定（PLN）値を使用」設定が有効な場合の役割の予定時間数またはコストの差異：</span> </p> <p><span><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <p><b>ヒント</b> <span>

このオプションは、選択した項目を表示セクションでビューをカスタマイズした場合にのみ適用されます。</span> </p> <p><span>詳しくは、</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Adobe Workfront Resource Planner を使用したリソースの可用性と割り当てのレビュー</a>を参照してください。 </p> </li>
</ul>
</div> </td>
</tr> 
  <tr> 
   <td>ユーザー</td> 
   <td> 
    <div> 
     <p>ユーザーの正味時間、FTE、コストの役割には、次のいずれかが表示されます。 </p> 
     <ul> 
      <li> <p>使用可能な時間またはコストと、ユーザーの予算時間またはコストの差異：</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>「使用可能な時間またはコスト」と、「NET 計算で予定（PLN）値を使用」設定が有効な場合のユーザーの予定時間数またはコストの差異：</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <p><b>ヒント</b> <span>

このオプションは、選択した項目を表示セクションでビューをカスタマイズした場合にのみ適用されます。</span> </p> <p><span>詳しくは、</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Adobe Workfront Resource Planner を使用したリソースの可用性と割り当てのレビュー</a>を参照してください。 </p> </li>
</ul>
</div> </td>
</tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**正味時間、FTE、またはコストが赤で表示される場合、予算をカバーするのに十分な使用可能な時間または予算** または作業に関連する予定時間またはコストがありません。この場合、リソースは割り当て超過になります。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(the table below is ideal but it does not transfer to Markdown)</p>
-->

<!--
<table style="table-layout:auto">
<col>
<col>
<col>
<tbody>
<tr>
<td><strong>Column Name (Hours, FTE, or Cost)</strong> </td>
<td><strong>Displayed by</strong> </td>
<td><strong>Description</strong> </td>
</tr>
<tr>
<td rowspan="3">AVL <br>(Available Hours, FTE, or Cost)</td>
<td>Project </td>
<td> <p>The total of Hours, FTEs, or Cost for which all the users on the project are available to work according to their schedule, for the time frame selected. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of Hours, FTEs, or Cost for which all the users associated with this role are available to work according to their schedule and their <strong>Percentage of FTE Availability</strong> for that specific role, for the time frame selected. </p> <p>Consider the following: </p>
<ul>
<li>If no user is associated with a job role, then the value for the Available Hours for the job role is zero. </li>
<li>If a user is associated with a Primary Job Role, but the <strong>Percentage of FTE Availability</strong> for the role is 0%, the job role Available Hours value is zero.</li>
<li>If the user is associated with Other Roles and the <strong>Percentage of FTE Availability</strong> for the roles is 0%, the Other Roles are not listed in the Resource Planner and the user displays only under their Primary Role.</li>
</ul> <p>For more information about the <strong>Percentage of FTE Availability</strong> for a job role, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">Edit a user's profile</a>.</p> <p>For more information about how the job role availability is calculated in the Resource Planner, see the section "Calculate the Available Hours and FTE for a job role in the Resource Planner" in the article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>Hours, FTEs, or Cost that the user is available to work, according to their schedule, for the time frame selected. This number subtracts the hours associated with the following:</p>
<ul>
<li>schedule exceptions</li>
<li>time off of the user</li>
<li>hours budgeted for other projects. </li>
</ul> <p>The Available Hours, FTEs, or Cost for a user change according the following: </p>
<ul>
<li>how their schedule and FTE are calculated based on the Resource Management Preferences at the system level.<br>For more information about calculating user and job role availability, see the article <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">Overview of calculating hours and FTE for users and roles in the Resource Planner</a>.</li>
</ul>
<ul>
<li>the <strong>Project Planning Priority</strong>, if the user is budgeted for work.<br>For more information about how Project Planning Priority affects the Available Hours of a user, see <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">Resource Planner navigation overview </a>. </li>
</ul> <p>If the user is scheduled for deactivation, the Available Hours, FTEs, or Cost for the days after the deactivation date are zero. <br>For more information about deactivating users, see the article <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">Deactivate or reactivate a user</a>.</p> </td>
</tr>
<tr>
<td rowspan="4">PLN <br>(Planned Hours, FTE, or Cost)</td>
<td>Project</td>
<td> <p>The total of the Planned Hours, FTEs, or Cost from all the job roles or users listed under the project, including in the <strong>No Role</strong> or <strong>No User</strong> sections, for the time frame selected, and as displayed in the Project Details tab of the project. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The total of the Planned Hours from all the tasks assigned to the role, during the time frame selected. </p> <p>The <strong>No Role</strong> section will show the Planned Hours associated with tasks that are either unassigned, assigned to teams (whose hours are listed in the <strong>No User</strong> section), or assigned to users who are not associated with a job role. </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>The Planned Hours from all the tasks assigned to the user in a specific role, during the time frame selected. </p> <p>The <strong>No User</strong> section will show the Planned Hours associated with tasks that are either unassigned or assigned to teams. </p> </td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when viewing Planned Hours:</p>
<ul>
<li>Although you cannot see information about task allocations in the Resource Planner in the Project and Role views, the amount of Planned Hours comes from the Planned Hours on the tasks in the projects. </li>
<li> <p>Planned Hours are equally distributed to each day within the Duration of tasks, for each resource assigned to them. The task Duration is based on the task Planned Start and Completion Dates and includes every calendar day within that period of time.<br>Workfront takes into account the schedule of the user or of the project when distributing Planned Hours to users or projects. In this case, Planned Hours are equally distributed to each day within the Duration of tasks excluding weekends, time-off days, and schedule exceptions.<br>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks on projects, the number of Planned Hours per week depends on how many days within that week are part of the task Duration. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters.<br>Weekend days, schedule exceptions, and time-off days are excluded from this distribution.</p> </li>
<li> The following categories of tasks are included in calculating the Planned Hours for each resource:
<ul>
<li> tasks assigned to users in Resource Pools, job roles, or teams on the project<br>If tasks are assigned to teams, their allocation will appear under <strong>No Role</strong> and <strong>No User</strong> sections. You can see the Planned Hours associated with teams, but you cannot budget the hours, because no roles nor users are associated with the tasks. </li>
<li> unassigned tasks </li>
</ul></li>
<li> Planned Hours in the Resource Planner do not include Planned Hours associated with the following:
<ul>
<li>parent tasks</li>
<li>tasks assigned to users with no Resource Pools</li>
<li>issues, when the <strong>Include hours from Issues</strong> setting is disabled.</li>
</ul></li>
<li>Planned Hours do not display in the Resource Planner if the task Duration is zero.</li>
<li>Planned Hours associated with deactivated users do not display. </li>
</ul> </td>
</tr>
<tr>
<td rowspan="4"> BDG <br>(BudgetedHours, FTE, or Cost) </td>
<td>Project</td>
<td> <p>A manual entry to estimate how many hours, FTE, or Cost you budget for a project, for a selected time frame. </p> <p>In the Project view, the hours you budget for the project are distributed to the job roles listed under the project. The amount of Planned Hours for each role determines how the Budgeted Hours are distributed to the roles. The Budgeted Hours are distributed to the roles with higher Planned Hours values. </p> <p>In the Role view, the hours you budget for the project are not distributed to the roles or the users on the project. </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>A manual entry to estimate how many hours you budget for a role, for a selected time frame. </p> <p>If no user is associated with the job role, you cannot estimate the Budgeted Hours for the job role. </p> <p>In the Role view, the hours you budget for the role are distributed to the projects listed under the role. The amount of Planned Hours for each project determines how the Budgeted Hours are distributed to the projects. The Budgeted Hours are distributed to the projects with higher Planned Hours values.</p> <p>In the Project view, the hours you budget for the role are not distributed to the projects or the users associated with the role. </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>A manual entry to estimate how many hours you budget for a user, for a selected time frame. </p> <p> <note type="note">  You can estimate the Budgeted Hours for users who are not assigned to tasks, but are associated with a Resource Pool on a project because these users also appear in the Resource Planner. Their Planned Hours should be zero, however, if they are not assigned to tasks.
</note> </p> </td>
</tr>
<tr>
<td colspan="2"> <p>Consider the following when working with Budgeted Hours:</p> <li>
<ul>
<li> <p>You can budget resources only when you have Edit access to Resource Management and Financial Data and Manage Finance permissions on the projects.</p> <p>For information about the access needed for budgeting resources, see the article <a href="../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Access needed to budget resources in&nbsp;Adobe Workfront</a>.</p> 
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this bullet: Duplicated below)</p>
</li>
</ul> </li>
<ul>
<li>By default, the Budgeted Hours in the Resource Planner are zero for all resources and for all the projects.</li>
<li>You can manually estimate the Budgeted Hours for users and roles, or you can use one of the links in the Project or Job Role <strong>More</strong> menus to update them according to the number of Planned Hours.<br>For more information about project and role options, see the section <a href="#Budget" class="MCXref xref">Overview of hours, FTE, and cost information in the Project and&nbsp;Role views of the Resource Planner</a> in this article.</li>
<li> The smallest period of time you can budget hours, FTE, or Cost for is a week. You cannot budget hours, FTE, or Cost for a day. </li>
<li> Budgeted Hours are equally distributed to each day within the Duration of tasks, for each resource assigned to them. The task Duration is based on the task Planned Start and Completion Dates and includes every calendar day within that period of time. <br>Workfront takes into account the schedule of the user or of the project when distributing Budgeted Hours to users or projects. In this case, Budgeted Hours are equally distributed to each day within the Duration of tasks excluding weekends, but including time-off and schedule exceptions. <br>If you display the Resource Planner by Week, for example, and you have tasks that span multiple weeks, the number of Budgeted Hours per week depends on how many days within that week are part of the task Duration. Weekend days are excluded from this distribution. This works similarly when displaying the Resource Planner by Month or Quarter and when tasks span multiple months or quarters. </li>
<li>You can report on Budgeted Hours, by selecting Budgeted Hour as your report object for a new report.<br>For information about what objects you can report on in Workfront, see the section "Report on objects" in the article <a href="../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md" class="MCXref xref">Understand objects in Adobe Workfront</a>. <br>For information about building a Budgeted Hour report, see the article <a href="../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md" class="MCXref xref">Report: Budgeted Hour</a>.</li>
<li>Hours previously budgeted for users who were later deactivated do not display. <br></li>
</ul> </td>
</tr>
<tr>
<td rowspan="4">VAR <br>(Hour, FTE, or ,Cost Variance)</td>
<td>Project</td>
<td> <p>The Hour, FTE, or Cost Variance shows whether you have enough Budgeted Hours for the project to accomplish all the Planned Hours for the project. </p> <p>The Project Hour, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td>Role</td>
<td> <p>The Hour, FTE, or Cost Variance shows whether you have enough Budgeted Hours, FTE, or Cost for the role to accomplish the Planned Hours assigned to it. </p> <p>The Role Hour, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td>User</td>
<td> <p>The Hours, FTE, or Cost Variance shows whether you have enough Budgeted Hours for the user to accomplish the Planned Hours assigned to them. </p> <p>The User Hours, FTE, or Cost Variance is calculated using the following formula:</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td>
</tr>
<tr>
<td colspan="2"> <note type="note">
When the Hours, FTE, or Cost Variance displays in red, you have estimated less Budgeted Hours than the Planned Hours of the actual work that needs to be completed. In this case, the Budgeted Hours might not be enough to complete the work.
</note> </td>
</tr>
<tr>
<td rowspan="4"> NET <br>(Net Hours, FTEs, or Cost) </td>
<td>Project</td>
<td>
<div>
<p>The project Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the project:</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the project, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td>Role</td>
<td>
<div>
<p>The role Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the role:</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the role, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span class="preview"><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td>User</td>
<td>
<div>
<p>The user Net Hours, FTE, or Cost may show one of the following: </p>
<ul>
<li> <p>The difference between the Available time or cost and the Budgeted time or cost for the user:</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li>
<li> <p><span>The difference between the Available time or cost and the Planned time or cost for the user, when the Use Planned (PLN) values in NET calculations setting is enabled:</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <note type="tip">
<span>This option is applied only when you customize the view in the Display selected items section.</span>
</note> <p><span>For more information, see</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Review resource availability and allocation using the Adobe Workfront Resource Planner</a> </p> </li>
</ul>
</div> </td>
</tr>
<tr>
<td colspan="2"> <note type="note">
<span>When the NET Hours,&nbsp;FTE, or Cost display in red, there is not enough Available time or budget to cover either the Budgeted</span> or the Planned time or cost associated with the work. In this case, the resources are overallocated.
</note> </td>
</tr>
</tbody>
</table>
-->
