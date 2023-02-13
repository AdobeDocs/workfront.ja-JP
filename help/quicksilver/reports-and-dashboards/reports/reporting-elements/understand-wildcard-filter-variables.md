---
content-type: overview
product-area: reporting
navigation-topic: reporting-elements
title: ワイルドカードフィルター変数
description: フィルターでワイルドカードを使用すると、特定のユーザーや日付ではなく、汎用のユーザーや日付を参照できます。 このようにして、作成する要素は動的で、使用するコンテキストに応じて結果が変わります。
author: Lisa
feature: Reports and Dashboards
exl-id: f99cd99e-c4c1-471d-8428-c680f0e73336
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '1456'
ht-degree: 2%

---

# ワイルドカードフィルター変数

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

Adobe Workfrontでは、次の要素を作成する際にフィルター変数またはワイルドカードをサポートしています。

* リスト、レポートおよびリソースプランナーのフィルタ

   Workfrontフィルターについて詳しくは、 [Adobe Workfrontのフィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

* 詳細検索

   詳細検索について詳しくは、 [詳細検索を使用](../../../workfront-basics/navigate-workfront/search/search-workfront.md#using-advanced-search) 記事内 [検索Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

* ビュー内の計算列
* ビューの条件付き書式

   条件付き書式について詳しくは、 [ビューでの条件付き書式の使用](../../../reports-and-dashboards/reports/reporting-elements/use-conditional-formatting-views.md).

* 計算済みカスタムフィールド

   >[!NOTE]
   >
   >計算列でネストされたコレクションを参照する場合、ワイルドカードフィルター変数はサポートされません。

   計算されたカスタムフィールドと列の詳細については、 [計算カスタムフィールドと計算列](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-custom-fields-calculated-columns.md).

ワイルドカードを使用すると、特定のユーザーや日付の代わりに、汎用のユーザーや日付を参照できます。 このようにして、作成する要素は動的で、使用するコンテキストに応じて結果が変わります。

例えば、プロジェクトレポートで$$USER.homeGroupID に対してフィルタを適用すると、ログインしているユーザーのホームグループに関連付けられたプロジェクトのみが取得されます。

Workfrontでは、日付ベースまたはユーザーベースのフィルター変数を使用できます。

## 日付ベースのワイルドカードフィルター変数

Workfrontの日付ベースのワイルドカードオプションは、任意の日付フィルター属性と組み合わせて使用できます。

レポートに日付ベースのワイルドカードを追加する方法については、 [日付ベースのワイルドカードを使用してレポートを一般化する](../../../reports-and-dashboards/reports/reporting-elements/use-date-based-wildcards-generalize-reports.md).

>[!NOTE]
>
>時間部分を含まない日付と時間の計算を作成した場合、または$$TODAY や$$NOW の日付ワイルドカードを使用する場合、ローカルタイムゾーンではなく協定世界時 (UTC) ゾーンに従って日付が使用されます。 これは予期しない日付の結果を引き起こす可能性があります。

次の日付ベースのワイルドカードから選択します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$TODAY</strong> </p> </td> 
   <td> <p>明日、来週または来月に再度フィルターを作成するのを避けるために、このワイルドカードを使用して日付に依存するフィルターを作成することをお勧めします。</p> <p>例えば、今日より前に期限が切れたすべてのタスクを表示する場合は、タスクフィルタで次のルールを使用できます。 <em>$$TODAY 未満の予定開始日</em>.</p> <p>$$TODAY は、常に現在の日の午前 0 時と同じです。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td width="100" role="rowheader"> <p><strong>$$NOW</strong> </p> </td> 
   <td> <p>これは$$TODAY ワイルドカードに似ていますが、現在の日時が含まれます。 $$NOW は現在の日時と等しくなります。</p> <p>例えば、現在の時刻までに入力されたすべての時間エントリを表示する場合は、時間フィルターで次のルールを使用します。 <em>$$NOW 未満の計画開始日</em>.</p> <p>注意：このワイルドカードは、リソースプランナーではサポートされていません。</p> </td> 
  </tr> 
 </tbody> 
</table>

様々な期間と様々な時点（将来または過去）を指定するには、ワイルドカードを次のように組み合わせます。

| 属性 |   |
|---|---|
| **q** | 暦四半期 |
| **時間** | 時間 |
| **d** | 日 |
| **w** | 週 |
| **m** | 月 |
| **y** | 年 |

{style=&quot;table-layout:auto&quot;}

| **修飾子** |  |
|---|---|
| **b** | 週の最初（日曜日） |
| **e** | 週の終わり（土曜日） |

{style=&quot;table-layout:auto&quot;}

| **演算子** |  |
|---|---|
| **+** | ワイルドカード値に値を追加 |
| **-** | ワイルドカード値から値を減算 |

{style=&quot;table-layout:auto&quot;}

例えば、ワイルドカード `$$TODAYb+2w` は、「今週の初めから 2 週間」を指します。 ワイルドカード*`$$NOW+2h` は、「今から 2 時間後」を指します。

## ユーザーベースのワイルドカードフィルター変数

>[!IMPORTANT]
>
>フィルターまたはレポートにユーザーベースのワイルドカードフィルター変数が含まれる場合、結果には、現在ログインしているユーザーがフィルターした情報が常に表示されます。 このようなフィルターやレポートを別のユーザーと共有する場合、ワイルドカードを使用すると、そのレポートを閲覧するユーザーの情報が取得されます。 2 人のユーザーは、異なる結果を見ます。

レポートにユーザーベースのワイルドカードを追加する方法については、 [ユーザーベースのワイルドカードを使用してレポートを一般化する](../../../reports-and-dashboards/reports/reporting-elements/use-user-based-wildcards-generalize-reports.md).

Workfrontは、次のユーザーベースの変数を提供します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr valign="top"> 
   <td width="200" role="rowheader"> <p><strong>$$USER.ID</strong> </p> </td> 
   <td> <!--
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : should these be formatted with code?!) </p>
    --> <p>最も一般的なユーザーベースの変数は、$$USER.ID です。 これにより、常にログインしたユーザーの ID が返されます。 これは、各オブジェクトを作成したユーザーとその作業割り当てを識別するために使用される ID です。</p> <p>レポートでこのワイルドカードを使用すると、システムで作成する必要のあるレポートの数が少なくなります。 1 つのレポートを作成して複数のユーザーと共有でき、その結果は、ログインしたユーザーとレポートの閲覧者に応じて変化します。</p> <p>例えば、ログインしたユーザーに割り当てられたすべての問題に関するレポートを作成するには、問題フィルターで次のルールを使用できます。 <em>ID に$$USER.ID と等しい割り当て</em>.</p> <p>Workfrontは、この変数を次の組み込みフィルターで使用します。</p> 
    <ul> 
     <li>マイ報告書</li> 
     <li>マイプロジェクト</li> 
     <li>マイタスク</li> 
     <li>マイ問題</li> 
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
   <td> <p>$$USER.companyID 変数は、ログインしたユーザーに関連付けられた会社を表します。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.customerID</strong> </p> </td> 
   <td> <p>$$USER.customerID 変数は、環境に関連付けられた顧客アカウントの ID を参照します。 お使いの環境では、この変数に設定できる値は 1 つだけです。通常、この値は、API を介して統合を構築する場合にのみ使用されます。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.firstName</strong> </p> </td> 
   <td> <p>$$USER.firstName 変数は、ログインしているユーザーの名を参照します。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.lastName</strong> </p> </td> 
   <td> <p>$$USER.lastName 変数は、ログインしているユーザーの姓を参照します。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.name</strong> </p> </td> 
   <td> <p>$$USER.name 変数は、ログインしているユーザーのフルネームを参照します。</p> <p>メモ:   <p>このワイルドカード変数は、テキストモードでフィルターを変更する場合にのみ機能します。 このワイルドカードは、テキストモードをサポートしていないフィルターでは使用できません。 例えば、次の領域のフィルターでは、このワイルドカードを使用できません。</p> 
     <ul> 
      <li> <p>リソースプランナ</p> </li> 
      <li> <p>ワークロードバランサー</p> </li> 
      <li> <p>分析</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeGroupID</strong> </p> </td> 
   <td> <p>$$USER.homeGroupID 変数は、ログインしているユーザーのホームグループの ID を参照します。 グループ管理者は、この変数を使用して、ホームグループ内のユーザーに属するアイテムに対してのみフィルタリングできます。</p> <p>たとえば、財務グループのプロジェクトの未完了タスクをすべて表示するには、タスク・フィルタで次のフィルタ・ルールを使用します。<br><em>プロジェクト：グループ ID が$$USER.homeGroupID と等しい </em><br><em>完了率が 100 未満</em></p> <p>ログインしたユーザーのホームグループである特定のグループ内の個人に割り当てられているすべての不完全なタスクを表示するには、タスクフィルタで次のフィルタルールを使用します。</p> <p><em>割り当て先：グループ ID が$$USER.homeGroupID と等しい<br>完了率が 100 未満</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.otherGroupIDs</strong> </p> </td> 
   <td> <p>$$USER.otherGroupIDs 変数は、ログインしたユーザーのプロファイルに関連付けられているすべてのグループ（ホームグループを含む）を参照します。</p> <p>この変数の機能は、$$USER.homeGroupID 変数の機能に似ていますが、ログインしたユーザーに関連付けられたグループのいずれかに属するユーザーに関する情報が結果に表示される点が異なります。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.homeTeamID</strong> </p> </td> 
   <td> <p>$$USER.homeTeamID 変数は、ログインしたユーザーのホームチームの ID を参照します。 チームマネージャは、この変数を使用して、ホームチームのユーザに属するアイテムのみをフィルタリングできます。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.teamIDs</strong> </p> </td> 
   <td> <p>$$USER.teamIDs 変数は、ログインしたユーザーに関連付けられているすべてのチームのリストを返します。</p> <p>この変数の機能は、$$USER.homeTeamID 変数の機能に似ていますが、結果には、フィルターで識別された任意のチームに属するユーザーに関する情報が表示されます。</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader"> <p><strong>$$USER.roleID</strong> </p> </td> 
   <td> <p>$$USER.roleID 変数は、ログインしたプライマリのユーザーロールを参照します。 この変数を使用して、特定のジョブの役割に割り当てられたタスクや問題に関するレポートを作成できます。</p> <p>例えば、ログインしたプライマリのユーザーの役割に割り当てられているすべてのタスクを表示するには、タスクフィルタで次のフィルタルールを使用します。</p> <p><em>タスク：ロール ID が$$USER.roleID と等しい。</em> </p> </td> 
  </tr> 
  <tr valign="top"> 
   <td role="rowheader">$$USER.roleIDs</td> 
   <td> <p>$$USER.roleIDs 変数は、ログインしたユーザーに関連付けられているすべてのジョブロールを参照します。 この変数を使用して、ログインユーザーに関連する任意のジョブの役割に割り当てられたタスクや問題に関するレポートを作成できます。 </p> <p>例えば、ログインユーザーに関連付けられた任意の役割に割り当てられているすべてのタスクを表示するには、タスクフィルタで次のフィルタルールを使用します。</p> <p><i>タスク：ロール ID が$$USERID.roleIDs と等しい<br></i> </p> <p>ヒント：この <i>タスク：ロール ID が$$USERID.roleIDs と等しい</i> フィルタールールは、「自分の役割」の「未割り当てタスク」と「自分の役割」の「未割り当てタスク」の組み込みフィルターに存在します。 </p> </td> 
  </tr> 
 </tbody> 
</table>

## オブジェクトベースのワイルドカードフィルタ変数

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><b>$$OBJCODE</b> </td> 
   <td> 
    <div> 
     <p>$$OBJCODE 変数は、オブジェクトの型を参照します。 </p> 
     <p>カスタムフォームでは、選択したフォームのオブジェクトタイプが計算済みカスタムフィールドで参照されているフィールドと互換性がない場合は、このワイルドカードを使用して、これらのオブジェクトタイプで重複フォームを作成する回避策を回避できます。</p> 
     <p>計算されたカスタムフィールドでは、IF 式にワイルドカードを含めて、フォームのオブジェクトタイプごとに異なる値を計算で出力できるようにします。 </p> 
     <p>詳細および例については、「 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md#calculat" class="MCXref xref">複数オブジェクトカスタムフォームの計算済みカスタムフィールド</a> 記事内 <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">計算データをカスタムフォームに追加する</a>.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
