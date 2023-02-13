---
content-type: overview
product-area: resource-management
navigation-topic: resource-planning
title: リソースプランナーのプロジェクトビューとロールビューの時間、工数、コスト情報の概要
description: リソースプランナーのプロジェクトビューとロールビューの時間、工数、コスト情報の概要
author: Alina
feature: Resource Management
exl-id: 76de1945-3f19-4c91-801c-07dc79e646ad
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '2958'
ht-degree: 0%

---

# リソースプランナーのプロジェクトビューとロールビューの時間、工数、コスト情報の概要

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this came from the budget-resources-project-role-views-resource-planner article)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: relink all articles pointing to this section to the new article)</p>
-->

プロジェクトで実行する必要のある作業に対してリソースを予算を割り当てることは、リソースプランナーの主な機能です。 リソースの使用可能時間を表示し、リソースが割り当てられているプロジェクトに時間を割り当てることができます。

リソース・プランナでのリソース予算作成の詳細は、 [「プロジェクト」ビューと「ロール」ビューを使用する、リソースプランナーの予算リソース](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)

この記事では、リソース・プランナでリソースの予算を作成する前に知っておく必要がある主要概念の一部を説明します。

## 予算リソースの概要

リソース・プランナを使用してリソースを予算設定する際は、次の点を考慮します。

* リソースの割り当てを予算するには、リソースがプロジェクトでの作業を完了するのに使用できる時間数、工数、またはコストを指定します。 リソースの時間またはコストを予算すると、リソースの使用可能な時間、工数、またはコストが予算額の割合で減少します。 その結果、予算を作成するプロジェクトの「使用可能時間」、「工数」または「原価」の金額が、それらのプロジェクトのユーザーおよび役割に対して減少します。

   >[!IMPORTANT]
   >
   >15 年間のリソース予算を作成できます。 期間が 15 年を超えるプロジェクトのリソースを予算する場合、予算設定情報が正確でない可能性があります。

* プロジェクトのタイムラインに関係なく、リソースプランナーに表示される任意の期間のリソースの「時間」、「工数」または「コスト」を予算できます。 たとえば、プロジェクトのタイムライン（計画時間と関連付けられている）でリソースが使用できない可能性があるが、別の時間で使用できる場合は、計画時間がゼロの時間枠に予算を割り当てます。 この後、リソースの可用性に合わせて手動でプロジェクトのタイムラインを変更できます。

   >[!NOTE]
   >
   >まず、業務上の役割またはユーザーに対して、時間、工数、コストを手動で予算設定することをお勧めします。 自動オプションを使用して、計画時間、工数、原価の金額が常に予算時間、工数、原価と一致する必要がある場合にのみ、プロジェクトと生産資源の予算時間を設定できます。\
   >リソース・プランナで予算作成の自動オプションを使用する方法の詳細は、この記事の「予算プロジェクトと役割の自動化」の節を参照してください [Adobe Workfront Resource Planner を使用したリソースの可用性と割り当てのレビュー](../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md).

* 予算の工数またはコストは予算の時間と同じです。Adobe Workfrontでは、予算するリソースに対して時間ではなく FTE とコストの値が使用されます。

   リソース・プランナでのコストの計算方法の詳細は、次を参照してください： [リソースプランナーでコストを計算する](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

* リソース・プランナでのリソースの予算割当は、次の方法で行われます。

   * 手動

      または

   * 自動的に ( **プロジェクト別に表示** および **ロール別に表示** ビュー。
   詳しくは、 [「プロジェクト」ビューと「ロール」ビューを使用する、リソースプランナーの予算リソース](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

* ユーザーがジョブの役割を変更し、リソースプールから削除、非アクティブ化、または削除した場合、その役割に予算された時間は変更されず、役割の残りのユーザーに再配分されます。 ジョブ・ロールに関連付けられたユーザーがいなくなった場合、ロールの予算時間は 0 になります。

プロジェクトと役割のオプションの詳細については、「 [生産資源プランナの時間、工数および原価の値の把握](#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner) 」を参照してください。

## 生産資源プランナの時間、工数および原価の値の把握 {#understand-the-values-of-hours-fte-and-cost-in-the-resource-planner}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this needs to be broken into its own article and leave here just the how-to: see this article: overview-of-planner-hour-fte-cost-information-in-role-project-views)</p>
-->

リソースを予算編成し、リソース・プランナの予算時間情報を更新する前に、次の概念に精通している必要があります

* **計画時間、工数またはコスト**:タスクと問題に関する定義に従って実行する必要がある作業。
* **利用可能な時間数、工数、コスト**:ユーザーに関連付けられたスケジュールに従って、ユーザーまたはジョブの役割が機能できる時間。

この情報は、各リソース（ユーザーまたはロール）および各プロジェクトのリソースプランナーに表示されます。

プロジェクトのプロジェクトビューと役割ビューに表示される内容については、この記事を参照してください。 [リソースプランナーのナビゲーションの概要](../../resource-mgmt/resource-planning/resource-planner-navigation.md).

リソース・プランナでのコストの計算方法の詳細は、「 [リソースプランナーでコストを計算する](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

>[!NOTE]
>
>原価による予算作成は、時間または工数による予算作成と同じですが、Workfrontが生産資源プランナの原価を計算する方法を理解する必要があります。
>
>リソース・プランナでのコストの計算方法の詳細は、「 [リソースプランナーでコストを計算する](../../resource-mgmt/resource-planning/calculate-costs-resource-planner.md).

次の表に、「プロジェクト」ビューまたは「ロール」ビューを適用する際に「リソース・プランナ」に表示される割付情報と可用性情報を示します。 この情報は、時間、工数またはコストで表示できます。

* [AVL (Available) 列](#the-avl-available-column)
* [「PLN （計画済み）」列](#the-pln-planned-column)
* [BDG （予算）列](#the-bdg-budgeted-column)
* [「VAR （平方偏差）」列](#the-var-variance-column)
* [NET 列](#the-net-column)

### AVL (Available) 列 {#the-avl-available-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>表示順</strong> </td> 
   <td><strong>説明</strong> </td> 
  </tr> 
  <tr> 
   <td>プロジェクト </td> 
   <td> <p>選択した期間で、プロジェクトのすべてのユーザーがスケジュールに従って作業できる時間、工数、コストの合計。 </p> </td> 
  </tr> 
  <tr> 
   <td>役割</td> 
   <td> <p>この役割に関連付けられているすべてのユーザーが、スケジュールとそのユーザーのスケジュールに従って作業できる時間数、工数、またはコストの合計 <strong>FTE の可用性の割合</strong> 選択した時間枠に対する特定の役割の。 </p> <p>次の点に注意してください。 </p> 
    <ul> 
     <li>ジョブロールに関連付けられているユーザーがない場合、ジョブロールの「使用可能時間」の値は 0 になります。 </li> 
     <li>ユーザーがプライマリジョブロールに関連付けられ、 <strong>FTE の可用性の割合</strong> 役割が 0%の場合、「Available Hours」の値は 0 です。</li> 
     <li>ユーザーが他のロールと関連付けられている場合、 <strong>FTE の可用性の割合</strong> ロールが 0%の場合、「その他のロール」は「リソース・プランナ」にリストされず、ユーザーは「プライマリ・ロール」の下にのみ表示されます。</li> 
    </ul> <p>詳しくは、 <strong>FTE の可用性の割合</strong> 役割については、この記事を参照してください。 <a href="../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">ユーザーのプロファイルの編集</a>.</p> <p>リソース・プランナでのジョブ・ロールの可用性の計算方法の詳細は、この記事の「リソース・プランナでのジョブ・ロールの使用可能時間と工数の計算」の項を参照してください <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">リソース・プランナのユーザーとロールの時間と工数の計算の概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>ユーザー</td> 
   <td> <p>選択した期間に対して、ユーザーが作業できる時間、工数、コスト（スケジュールに従って）が表示されます。 この数値は、次に関連する時間を引きます。</p> 
    <ul> 
     <li>スケジュールの例外</li> 
     <li>ユーザーの休暇</li> 
     <li>他のプロジェクトで予算に計上された時間数。 </li> 
    </ul> <p>ユーザーの利用可能な時間、工数またはコストは、次の項目に従って変更されます。 </p> 
    <ul> 
     <li>システム・レベルでのリソース管理プリファレンスに基づいて、スケジュールと FTE を計算する方法。<br>ユーザーとジョブの役割の可用性の計算の詳細については、「 <a href="../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md" class="MCXref xref">リソース・プランナのユーザーとロールの時間と工数の計算の概要</a>.</li> 
    </ul> 
    <ul> 
     <li>の <strong>プロジェクト計画の優先順位</strong>（ユーザーが予算で作業する場合）<br>プロジェクト計画優先度がユーザーの使用可能時間に与える影響の詳細は、 <a href="../../resource-mgmt/resource-planning/resource-planner-navigation.md" class="MCXref xref">リソースプランナーのナビゲーションの概要 </a>. </li> 
    </ul> <p>ユーザーが非アクティブ化をスケジュールされている場合、非アクティブ化の日からの使用可能な時間、FTE またはコストはゼロになります。 <br>ユーザーの非アクティブ化について詳しくは、 <a href="../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md" class="MCXref xref">ユーザーを非アクティブ化または再アクティブ化する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### 「PLN （計画済み）」列 {#the-pln-planned-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>表示順</strong> </td> 
   <td><strong>説明</strong> </td> 
  </tr> 
  <tr> 
   <td>プロジェクト</td> 
   <td> <p>プロジェクトの下にリストされたすべてのジョブロールまたはユーザーからの計画時間、工数、またはコストの合計 ( <strong>ロールなし</strong> または <strong>ユーザーなし</strong> セクション、選択した期間、およびプロジェクトの「プロジェクトの詳細」タブに表示されるもの。 </p> <p><b>メモ</b>

日次ユーザー割当の手動調整により、生産資源プランナの週次、月次または四半期の計画時間の値が変更される場合があります。 ワークロード・バランサを使用して、タスクと問題に対する日次ユーザー割り当てを手動で調整できます。 詳しくは、 <a href="../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md" class="MCXref xref">ワークロードバランサーでのユーザー割り当ての管理</a>.</p> </td>
</tr> 
  <tr> 
   <td>役割</td> 
   <td> <p>選択した期間内の、ロールに割り当てられたすべてのタスクからの計画時間の合計。 </p> <p>この <strong>ロールなし</strong> 「 」セクションには、未割り当てのタスク ( 時間が <strong>ユーザーなし</strong> （セクション）、またはジョブロールに関連付けられていないユーザーに割り当てられます。 </p> </td> 
  </tr> 
  <tr> 
   <td>ユーザー</td> 
   <td> <p>特定の役割のユーザーに割り当てられたすべてのタスクの、選択した期間の計画時間。 </p> <p>この <strong>ユーザーなし</strong> 「 」セクションには、未割り当てまたはチームに割り当てられているタスクに関連する計画時間が表示されます。 </p> </td> 
  </tr> 
 </tbody> 
</table>

計画時間を表示する際は、次の点を考慮してください。

* [ プロジェクト ] ビューと [ ロール ] ビューの [ リソースプランナ ] にタスクの割り当てに関する情報は表示されませんが、[ 計画時間 ] の値は、プロジェクト内のタスクの [ 計画時間 ] から取得されます。
* 予定時間は、タスクの期間内の各日に、タスクに割り当てられたリソースに対して均等に配分されます。 タスク期間は、タスクの「計画開始日」と「完了日」に基づき、その期間内の各カレンダー日が含まれます。\
   Workfrontは、ユーザーまたはプロジェクトに予定時間を配分する際に、ユーザーまたはプロジェクトのスケジュールを考慮に入れます。 この場合、計画時間は、週末、休日、スケジュール例外を除くタスクの期間内に、各日に均等に配分されます。\
   たとえば、リソース・プランナを週別に表示し、プロジェクトに複数週間のタスクがある場合、1 週間の予定時間数は、その週内の日数がタスク期間の一部であるかどうかによって異なります。 これは、「月別」または「四半期別」で「生産資源プランナ」を表示する場合と、タスクが複数の月または四半期にまたがる場合に同様に機能します。\
   週末、スケジュールの例外、およびタイムオフ日は、この配分から除外されます。
* 各リソースの予定時間の計算には、次のタスクのカテゴリが含まれます。

   * リソースプール、ジョブロール、またはプロジェクトのチームでユーザーに割り当てられたタスク\
      タスクがチームに割り当てられると、その割り当てが以下に表示されます。 **ロールなし** および **ユーザーなし** セクション。 チームに関連付けられた「計画時間」は表示できますが、タスクに関連付けられた役割もユーザーもないので、時間を予算できません。

   * 未割り当てタスク

* 生産資源計画担当の計画時間には、次に関連する計画時間は含まれません。

   * 親タスク
   * リソースプールを持たないユーザーに割り当てられたタスク
   * 問題、 **問題からの時間数を含める** の設定は無効です。

* タスクの期間が 0 の場合、計画時間はリソース・プランナに表示されません。
* 非アクティブなユーザーに関連付けられた計画時間は表示されません。

### BDG （予算）列 {#the-bdg-budgeted-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>表示順</strong> </td> 
   <td><strong>説明</strong> </td> 
  </tr> 
  <tr> 
   <td>プロジェクト</td> 
   <td> <p>選択した期間に対してプロジェクトに予算した時間数、工数、コストを見積もる手動入力。 </p> <p>[ プロジェクト ] ビューでは、プロジェクトの予算時間が、プロジェクトの下に表示されるジョブの役割に配分されます。 各ロールの計画時間数によって、予算時間がロールにどのように配分されるかが決まります。 予算時間は、「計画時間」の値が高い役割に配分されます。 </p> <p>[ 役割 ] ビューでは、プロジェクトの予算時間は、プロジェクト上の役割やユーザーに配分されません。 </p> </td> 
  </tr> 
  <tr> 
   <td>役割</td> 
   <td> <p>選択した期間に対して、ロールの予算時間数を見積もるための手動入力。 </p> <p>ジョブ・ロールに関連付けられているユーザーがない場合は、ジョブ・ロールの予算時間を見積もることはできません。 </p> <p>[ 役割 ] ビューでは、その役割に予算を割り当てた時間が、その役割の下に一覧表示されるプロジェクトに配分されます。 各プロジェクトの計画時間数によって、予算時間がプロジェクトにどのように配分されるかが決まります。 予算時間は、「計画時間」の値が大きいプロジェクトに配分されます。</p> <p>[ プロジェクト ] ビューでは、ロールの予算時間は、ロールに関連付けられたプロジェクトやユーザーに配分されません。 </p> </td> 
  </tr> 
  <tr> 
   <td>ユーザー</td> 
   <td> <p>選択した期間に対してユーザーが予算した時間数を見積もるための手動入力。 </p> <p> <p><b>注意</b>   タスクに割り当てられていないが、プロジェクト上の資源プールに関連付けられているユーザーの予算時間を見積もることができます。これは、これらのユーザーが資源プランナにも表示されるためです。 ただし、タスクに割り当てられていない場合は、「計画時間」はゼロにする必要があります。 </p> </p> </td> 
  </tr> 
 </tbody> 
</table>

予算時間を使用する際は、次の点に注意してください。

<!--
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(Duplicated below ??)
</MadCap:conditionalText>
-->

* リソースを予算設定できるのは、プロジェクトに対するリソース管理および財務データの編集および財務の管理の権限を持っている場合のみです。

   予算リソースの割り当てに必要なアクセスの詳細については、この記事を参照してください [Adobe Workfrontの予算リソースに必要なアクセス](../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md).

* デフォルトでは、すべてのリソースとすべてのプロジェクトに対して、リソース・プランナの予算時間は 0 です。
* ユーザーとロールの予算時間を手動で見積もるか、プロジェクトロールまたはジョブロールのいずれかのリンクを使用できます **詳細** メニューを使用して、予定時間数に従って更新できます。\
   プロジェクトと役割のオプションの詳細については、「 [リソースプランナーのプロジェクトビューとロールビューの時間、工数、コスト情報の概要](#Budget) 」を参照してください。

* 時間、工数、コストを予算できる最小の期間は 1 週間です。 1 日の時間、工数、コストは予算できません。
* 予算時間は、タスクに割り当てられた各リソースに対して、タスクの期間内の各日に均等に配分されます。 タスク期間は、タスクの「計画開始日」と「完了日」に基づき、その期間内の各カレンダー日が含まれます。\
   Workfrontでは、予算時間をユーザーまたはプロジェクトに配分する際に、ユーザーまたはプロジェクトのスケジュールが考慮されます。 この場合、予算時間は、週末を除くタスク期間内の各日に均等に配分されますが、タイムオフやスケジュール例外も含まれます。\
   たとえば、リソース・プランナを週別に表示し、複数週間にわたるタスクがある場合、1 週間あたりの予算時間数は、その週内の日数がタスク期間の一部であるかどうかによって異なります。 週末はこの配布から除外されます。 これは、「月別」または「四半期別」で「生産資源プランナ」を表示する場合と、タスクが複数の月または四半期にまたがる場合に同様に機能します。

* 新しいレポートのレポート・オブジェクトとして「予算時間」を選択すると、予算時間に関するレポートを作成できます。\
   Workfrontでレポートできるオブジェクトについて詳しくは、この記事の「オブジェクトのレポート」の節を参照してください [Adobe Workfrontのオブジェクトについて](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).\
   予算時間レポートの作成方法については、この記事を参照してください [レポート：予算時間](../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/report-budgeted-hour.md).

* 後で非アクティブ化したユーザーに対して予算された時間は表示されません。

### 「VAR （平方偏差）」列 {#the-var-variance-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>表示順</strong> </td> 
   <td><strong>説明</strong> </td> 
  </tr> 
  <tr> 
   <td>プロジェクト</td> 
   <td> <p>「時間」、「工数」または「原価差異」は、プロジェクトの全計画時間を完了するのに十分な予算時間があるかどうかを示します。 </p> <p>プロジェクト時間、工数または原価差異は、次の式を使用して計算されます。</p> <p><code>Project Hour, FTE, or Cost Variance = Project Budgeted Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>役割</td> 
   <td> <p>「時間」、「工数」または「原価差異」は、割り当てられた計画時間を完了するのに十分な予算時間、工数、原価のどれがロールにあるかを示します。 </p> <p>「役割時間」、「工数」または「原価差異」は、次の式を使用して計算されます。</p> <p><code>Role Hour, FTE, or Cost Variance = Role Budgeted Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
  <tr> 
   <td>ユーザー</td> 
   <td> <p>「時間」、「工数」または「原価差異」は、ユーザーが割り当てられた計画時間を達成するのに十分な予算時間があるかどうかを示します。 </p> <p>「ユーザー時間」、「工数」または「原価差異」は、次の式を使用して計算されます。</p> <p><code>User Hours, FTE, or Cost Variance = User Budgeted Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>「時間」、「工数」または「原価差異」が赤で表示される場合は、完了する必要のある実際の作業の計画時間よりも予算時間の方が少なく見積もられています。 この場合、予算時間では作業を完了するのに十分でない場合があります。

### NET 列  {#the-net-column}

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>表示順</strong> </td> 
   <td><strong>説明</strong> </td> 
  </tr> 
  <tr> 
   <td>プロジェクト</td> 
   <td> 
    <div> 
     <p>プロジェクトの「正味時間」、「工数」または「原価」には、次のいずれかが表示されます。 </p> 
     <ul> 
      <li> <p>使用可能な時間またはコストと、プロジェクトの予算時間またはコストの差。</p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p>NET 計算設定で計画済 (PLN) 値を使用できる場合の、使用可能な時間またはコストと、プロジェクトの計画済時間またはコストの違い： </p> <p><code>Project Net Hours, FTE, or Cost = Project Available Hours, FTE, or Cost - Project Planned Hours, FTE, or Cost</code>
      </p>

<p><b>ヒント</b></p>        
  <p>このオプションは、「選択した項目を表示」セクションでビューをカスタマイズした場合にのみ適用されます。</p>
  <p>詳しくは、 <a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" >Adobe Workfront Resource Planner を使用したリソースの可用性と割り当てのレビュー</a> </p> 
      </li> 
     </ul> 
    </div> </td> 
  </tr> 
  <tr> 
   <td>役割</td> 
   <td> 
    <div> 
     <p>「正味時間」、「工数」または「原価」の役割には、次のいずれかが表示されます。 </p> 
     <ul> 
      <li> <p>使用可能な時間またはコストと、ロールの予算時間またはコストの差異：</p> <p><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>「使用可能な時間または原価」と、「NET 計算で計画 (PLN) 値を使用」設定が有効な場合のロールの計画時間または原価の差異：</span> </p> <p><span><code>Role Net Hours, FTE, or Cost = Role Available Hours, FTE, or Cost - Role Planned Hours, FTE, or Cost</code></span> </p> <p><b>ヒント</b> <span>

このオプションは、「選択した項目を表示」セクションでビューをカスタマイズした場合にのみ適用されます。</span> </p> <p><span>詳しくは、</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Adobe Workfront Resource Planner を使用したリソースの可用性と割り当てのレビュー</a> </p> </li>
</ul>
</div> </td>
</tr> 
  <tr> 
   <td>ユーザー</td> 
   <td> 
    <div> 
     <p>ユーザーの正味時間、工数または原価には、次のいずれかが表示されます。 </p> 
     <ul> 
      <li> <p>「使用可能な時間またはコスト」と、ユーザーの予算時間またはコストの差。</p> <p><code>User Net Hours, FTE, or Cost = USer Available Hours, FTE, or Cost - User Budgeted Hours, FTE, or Cost</code> </p> </li> 
      <li> <p><span>NET 計算設定で計画済 (PLN) 値を使用可能にした場合の、使用可能な時間またはコストと、ユーザーの計画済時間またはコストの差異：</span> </p> <p><span><code>User Net Hours, FTE, or Cost = User Available Hours, FTE, or Cost - User Planned Hours, FTE, or Cost</code></span> </p> <p><b>ヒント</b> <span>

このオプションは、「選択した項目を表示」セクションでビューをカスタマイズした場合にのみ適用されます。</span> </p> <p><span>詳しくは、</span><a href="../../resource-mgmt/resource-planning/resource-availability-allocation-resource-planner.md" class="MCXref xref">Adobe Workfront Resource Planner を使用したリソースの可用性と割り当てのレビュー</a> </p> </li>
</ul>
</div> </td>
</tr> 
 </tbody> 
</table>

>[!NOTE]
>
>**NET Hours、FTE、または Cost が赤で表示される場合、予算をカバーするのに十分な使用可能な時間または予算がありません** または作業に関連する計画時間またはコスト。 この場合、リソースは割り当て超過になります。

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
