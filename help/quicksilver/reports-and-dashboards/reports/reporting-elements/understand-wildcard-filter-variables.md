---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: ワイルドカードフィルター変数
description: フィルターでワイルドカードを使用すると、特定のユーザーや日付ではなく、一般的なユーザーや日付を参照できます。このようにして、作成する要素は動的で、使用するコンテキストに応じて結果が変わります。
author: Nolan
feature: Reports and Dashboards
exl-id: f99cd99e-c4c1-471d-8428-c680f0e73336
source-git-commit: d6094d944b7955db8a97b5e1ce0af8cb85f82a9e
workflow-type: tm+mt
source-wordcount: '1466'
ht-degree: 82%

---

# ワイルドカードフィルター変数の概要

<!-- Audited: 12/2023 -->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked to the training self-serve promted articles for user-based and date-based widlcards (how-to articles). This serves as the "overview/ reference" article for those articles. Consider renaming this when that is allowed.) </p>
<p>(NOTE: Alina: ***&gt;&gt;Linked in other articles - do not move/ delete.</p>
<p>&gt;&gt;This was included but it is not supported???:</p>
<p>The $$USER.roleIDs variable refers to all the job roles that are associated with the logged-in user. Using this variable, you can&nbsp; items assigned to all of the job roles associated with the logged-in user.</p>
<p>For example, if you want to display tasks assigned to any of the job roles associated with the logged-in user, you can use the following filter rule in a task filter:</p>
<p>AssignedToID Equals $$USER.roleIDs.)</p>
</div>
-->

ワイルドカードを使用すると、特定のユーザーや日付の代わりに、汎用のユーザーや日付を参照できます。 このようにして、作成する要素は動的で、結果は使用されるコンテキストに応じて変化します。

例えば、プロジェクトレポートで $$USER.homeGroupID に対してフィルターを適用すると、ログインしているユーザーのホームグループに関連付けられたプロジェクトのみが検索されます。

次の要素を作成する際に、フィルター変数（ワイルドカードとも呼ばれます）を使用できます。

<table>
    <tr>
        <td>リスト、レポートおよびリソースプランナーのフィルター</td>
        <td>Workfrontフィルターについて詳しくは、 <a href="../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md">フィルターの概要</a>.
</td>
    </tr>
    <tr>
        <td>詳細検索</td>
        <td>詳細検索について詳しくは、<a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md">Adobe Workfront での検索</a>の記事の<a href="../../../workfront-basics/navigate-workfront/search/search-workfront.md#using-advanced-search">詳細検索の使用</a>の節を参照してください。
    </tr>
    <tr>
        <td>ビューの計算列</td>
        <td></td>
    </tr>
    <tr>
        <td>ビューの条件付き形式</td>
        <td>条件付き形式について詳しくは、<a href="../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md">ビューで条件付き形式を使用</a>を参照してください。
    </tr>
    <tr>
        <td>計算済みカスタムフィールド</td>
        <td>計算列でネストされたコレクションを参照する場合、ワイルドカードフィルター変数はサポートされません。

計算済みのカスタムフィールドと列について詳しくは、<a hreft="../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md">計算カスタムフィールドと計算列の比較</a>を参照してください。
</td>
    </tr>
</table>

## 日付ベースのワイルドカードフィルター変数

日付ベースのワイルドカードオプションは、任意の日付フィルター属性と組み合わせて使用できます。 レポートに日付ベースのワイルドカードを追加する方法について詳しくは、[日付ベースのワイルドカードを使用したレポートの一般化](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md)を参照してください。

>[!NOTE]
>
>時間部分を含まない日付と時間の計算を作成した場合または $$TODAY や $$NOW の日付ワイルドカードを使用する場合、ローカルタイムゾーンではなく協定世界時（UTC）ゾーンに従って日付が使用されます。これは予期しない日付の結果を引き起こす可能性があります。

次の日付ベースのワイルドカードから選択できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$TODAY</strong> </p> </td> 
   <td> <p>明日、来週または来月に再度フィルターを作成することを避けるために、このワイルドカードを使用して日付指定のフィルターを作成することをお勧めします。</p> <p>例えば、今日までに期限を迎えるすべてのタスクを表示したい場合、タスクフィルターで <em>$$TODAY 以前の予定開始日</em>のルールを使用できます。</p> <p>$$TODAY は、常に現在の日付の午前 0時と等しいものとします。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$NOW</strong> </p> </td> 
   <td> <p>これは $$TODAY ワイルドカードに似ていますが、現在の日付と時間が含まれます。$$NOW は現在の日付と時間に等しいものとします。</p> <p>例えば、現在の時刻までに入力されたすべての時間エントリを表示する場合は、時間フィルターで <em>$$NOW 以前の予定開始日</em>のルールを使用します。</p> <p>メモ：このワイルドカードは、リソースプランナーではサポートされていません。</p> </td> 
  </tr> 
 </tbody> 
</table>

様々な期間と様々な時点（将来または過去）を指定するには、上記のワイルドカードを次と組み合わせます。

| 属性 |   |
|---|---|
| **q** | 四半期 |
| **時間** | 時間 |
| **d** | 日 |
| **w** | 週 |
| **m** | 月 |
| **y** | 年 |

{style="table-layout:auto"}

| **修飾子** | |
|---|---|
| **b** | 期間の初め ( 属性を指定せず、デフォルトで週の初め（日曜日）に設定されます。 |
| **e** | 期間の終わり ( 属性を指定せず、デフォルトで週の終わり（土曜日）に設定されます。 |

{style="table-layout:auto"}

| **演算子** | |
|---|---|
| **+** | ワイルドカード値に値を追加 |
| **-** | ワイルドカード値から値を減算 |

{style="table-layout:auto"}

例えば、ワイルドカード `$$TODAYb+2w` は、「今週の初めから 2 週間」を意味します。ワイルドカード *`$$NOW+2h` は、「今から 2 時間後」を意味します。

## ユーザーベースのワイルドカードフィルター変数

>[!IMPORTANT]
>
>フィルターまたはレポートにユーザーベースのワイルドカードフィルター変数が含まれる場合、結果には、現在ログインしているユーザーがフィルターした情報が常に表示されます。 このようなフィルターやレポートを別のユーザーと共有する場合、ワイルドカードはそのレポートを閲覧するユーザーの情報を取得します。2 人のユーザーには、異なる結果が表示されます。
>
>レポートにユーザーベースのワイルドカードを追加する方法について詳しくは、[ユーザーベースのワイルドカードを使用したレポートの一般化](../../../reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md)を参照してください。

次のユーザーベースの変数から選択できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.ID</strong> </p> </td> 
   <td> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : should these be formatted with code?!) </p>
    --> <p>最も一般的なユーザーベースの変数は、$$USER.ID です。これにより、常にログインしたユーザーの ID が返されます。これは、各オブジェクトを作成したユーザーとその作業割り当てを識別するために使用される ID です。</p> <p>レポートでこのワイルドカードを使用すると、システムで作成する必要のあるレポートの数が少なくなります。1 つのレポートを作成して複数のユーザーと共有でき、その結果は、ログインしたユーザーとレポートの閲覧者に応じて変化します。</p> <p>例えば、ログインしたユーザーに割り当てられたすべてのイシューに関するレポートを作成するには、イシューフィルターで<em>割り当て先 ID に等しい $$USER.ID</em> のルールを使用できます。</p> <p>Workfront は、この変数を次の組み込みフィルターで使用します。</p> 
    <ul> 
     <li>マイレポート</li> 
     <li>マイプロジェクト</li> 
     <li>マイタスク</li> 
     <li>マイイシュー</li> 
     <li>マイ時間数</li> 
    </ul> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.categoryID</strong> </p> </td> 
   <td> <p>$$USER.categoryID 変数は、ログインしたユーザーに関連付けられた特定のカスタムフォームを参照します。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelID</strong> </p> </td> 
   <td> <p>$$USER.accessLevelID 変数は、ログインしたユーザーに関連付けられたアクセスレベルの ID を参照します。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.accessLevelRank</strong> </p> </td> 
   <td> <p>$$USER.accessLevelRank 変数は、ログインしたユーザーに関連付けられたアクセスレベルのランクを参照します。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.companyID</strong> </p> </td> 
   <td> <p>$$USER.companyID 変数は、ログインしたユーザーに関連付けられた会社を参照します。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.customerID</strong> </p> </td> 
   <td> <p>$$USER.customerID 変数は、使用する環境に関連付けられた顧客アカウントの ID を参照します。お使いの環境では、この変数に設定できる値は 1 つだけで、通常、この値は、API を介して統合を構築する場合にのみ使用されます。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.firstName</strong> </p> </td> 
   <td> <p>$$USER.firstName 変数は、ログインしているユーザーの名前（名）を参照します。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.lastName</strong> </p> </td> 
   <td> <p>$$USER.lastName 変数は、ログインしているユーザーの名前（姓）を指します。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.name</strong> </p> </td> 
   <td> <p>$$USER.name 変数は、ログインしているユーザーのフルネームを指します。</p> <p>メモ：   <p>このワイルドカード変数は、テキストモードでフィルターを変更する場合にのみ機能します。このワイルドカードは、テキストモードをサポートしていないフィルターでは使用できません。例えば、次のエリアのフィルターでは、このワイルドカードを使用できません。</p> 
     <ul> 
      <li> <p>リソースプランナー</p> </li> 
      <li> <p>ワークロードバランサー</p> </li> 
      <li> <p>分析</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeGroupID</strong> </p> </td> 
   <td> <p>$$USER.homeGroupID 変数は、ログインしたユーザーのホームグループの ID を指します。グループ管理者は、この変数を使用して、ホームグループ内のユーザーに属するアイテムのみをフィルタリングできます。</p> <p>例えば、財務グループのプロジェクトの未完了タスクをすべて表示するには、タスクフィルターで次のフィルタールールを使用します。<br><em>プロジェクト：グループ ID が $$USER.homeGroupID と等しい</em><br><em>完了率が 100 未満</em></p> <p>ログインしたユーザーのホームグループである特定のグループ内の個人に割り当てられているすべての未完了タスクを表示するには、タスクフィルターで次のフィルタールールを使用します。</p> <p><em>割り当て先：グループ ID が $$USER.homeGroupID と等しい<br>完了率が 100 未満</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.otherGroupIDs</strong> </p> </td> 
   <td> <p>$$USER.otherGroupIDs 変数は、ログインしたユーザーのプロファイルに関連付けられているすべてのグループ（ホームグループを含む）を指します。</p> <p>この変数の機能は、$$USER.homeGroupID 変数と似ていますが、ログインしたユーザーに関連付けられているグループのいずれかに属するユーザーに関する情報が結果に表示される点が異なります。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeTeamID</strong> </p> </td> 
   <td> <p>$$USER.homeTeamID 変数は、ログインしたユーザーのホームチームの ID を指します。チームマネージャーは、この変数を使用して、ホームチームのユーザーに属するアイテムのみをフィルタリングできます。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.teamIDs</strong> </p> </td> 
   <td> <p>$$USER.teamIDs 変数は、ログインしたユーザーに関連付けられているすべてのチームのリストを返します。</p> <p>この変数の機能は、$$USER.homeTeamID 変数と似ていますが、フィルターで識別されたチームのいずれかに属するユーザーに関する情報が結果に表示される点が異なります。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.roleID</strong> </p> </td> 
   <td> <p>$$USER.roleID 変数は、ログインしたユーザーの主要役割を指します。この変数を使用すると、特定の担当業務に割り当てられたタスクやイシューに関するレポートを作成できます。</p> <p>例えば、ログインしたユーザーの主要役割に割り当てられているすべてのタスクを表示するには、タスクフィルターで次のフィルタールールを使用します。</p> <p><em>タスク：役割 ID が$$USER.roleID と等しい。</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"><p><strong>$$USER.roleIDs</strong></p></td> 
   <td> <p>$$USER.roleIDs 変数は、ログインしたユーザーに関連付けられているすべての担当業務を指します。この変数を使用すると、ログインしたユーザーに関連付けられている担当業務のいずれかに割り当てられたタスクやイシューに関するレポートを作成できます。 </p> <p>例えば、ログインしたユーザーに関連付けられている役割のいずれかに割り当てられたすべてのタスクを表示するには、タスクフィルターで次のフィルタールールを使用します。</p> <p><i>タスク：役割 ID が $$USERID.roleIDs と等しい<br></i> </p> <p>ヒント：<i>タスク：役割 ID が $$USERID.roleIDs と等しい</i>というフィルタールールは、組み込みのフィルター「マイ役割の未割り当てタスク」および「マイ役割の未割り当てイシュー」に存在します。 </p> </td> 
  </tr> 
 </tbody> 
</table>

## オブジェクトベースのワイルドカードフィルター変数

次のオブジェクトベースのワイルドカードから選択できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>$$OBJCODE</b> </td> 
   <td> 
    <div> 
     <p>$$OBJCODE 変数は、オブジェクトのタイプを指します。 </p> 
     <p>カスタムフォームでは、選択したフォームのオブジェクトタイプが、計算済みカスタムフィールドで参照されているフィールドと互換性がない場合、このワイルドカードを使用して、これらのオブジェクトタイプで重複フォームを作成する回避策を回避できます。</p> 
     <p>計算されたカスタムフィールドでは、IF 式にワイルドカードを含めて、フォームのオブジェクトタイプごとに異なる値を出力できるようにします。 </p> 
     <p>その詳細と例については、<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">カスタムフォームへの計算データの追加</a>の記事で<a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat" class="MCXref xref">複数オブジェクトのカスタムフォームにおける計算カスタムフィールド</a>の節を参照してください。</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
