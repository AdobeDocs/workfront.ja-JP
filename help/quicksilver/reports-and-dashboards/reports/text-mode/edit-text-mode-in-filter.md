---
product-area: reporting
navigation-topic: text-mode-reporting
title: テキストモードを使用したフィルターの編集
description: '注意：この記事にセクションを追加します： /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; ***また、この領域にテキストモードの概要記事の下書きを作成します )'
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '1032'
ht-degree: 0%

---

# テキストモードを使用したフィルターの編集

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">NOTE: add a section in this article: /Content/Reports and Dashboards/Reports/Reporting Elements/create-customize-fitlers.html; *** Also, draft this area in the Text Mode overview article)</p>
-->

テキストモードを使用してリストまたはレポートのフィルターを編集し、標準インターフェイスで使用できないフィールドにアクセスして、より複雑なフィルターを作成できます。

フィルターを作成する際のその他のテキストモードの例については、この記事の「カスタムフィルターのサンプル」の節も参照してください。 [カスタム表示、フィルター、グループ化のサンプル：記事のインデックス](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートのレポート要素を編集します</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限が設定されているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>レポートに対する権限を管理して、レポートのフィルターを編集します</p> <p>フィルターを編集するための権限を管理します</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

レポートまたはリストでテキストモードの使用を開始する前に、必ずWorkfrontのテキストモード構文に関する十分な知識を持っておく必要があります。

詳しくは、以下を参照してください。

* [テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [テキストモードの構文の概要](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [カスタム表示、フィルター、グループ化のサンプル：記事のインデックス](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## フィルターでのテキストの編集モード

テキストモードを使用したフィルターの編集は、レポートとリストで同じです。 レポートから、またはリストからのフィルターへのアクセスは異なります。

>[!TIP]
>
>標準モードでできるだけ多くのフィルターを作成し、そのフィルターをテキストモードに変換して編集することをお勧めします。

フィルターの作成について詳しくは、 [フィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

レポートの作成について詳しくは、 [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 次のいずれかの操作を行います。

   1. レポートからフィルターにアクセスするには、レポートに移動して、 **レポートのアクション** > **編集** > **フィルター** タブをクリックします。
   1. リストからフィルターにアクセスするには、リストに移動し、 **フィルター** ドロップダウンメニューから、変更するフィルターの上にマウスを移動し、 **編集** アイコン ![](assets/edit-icon.png).

      フィルタービルダーが開きます。

1. クリック **フィルタールールを追加する** フィルターの条件の追加を開始するには、「 **テキストモードに切り替え** をクリックします。
1. テキストモードを使用してフィルターステートメントを追加します。 各 filter 文には、次の行と追加情報を含めることができます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td><b>行/情報をフィルター</b></td> 
      <td><b>例</b></td> 
     </tr> 
     <tr> 
      <td> <p>フィールド名と、Workfrontデータベースに表示される値と等しい値。</p> <p>この行は必須です。</p> <p> データベースでのオブジェクトおよびフィールドの表示の詳細については、 <a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API エクスプローラ</a>.</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>ステータスが「処理中」のタスクをフィルターするには、次の行を使用します。</p> <p><code>status=INP</code> </p> <p><b>ヒント</b>

   ステータスをフィルターする場合、名前ではなく、3 文字のコードを使用する必要があります。</p> </td>
   </tr> 
     <tr> 
      <td> <p>フィールド名修飾子および修飾子が等しいもの。 これは、フィルタリングに使用するフィールドが満たす必要がある条件を示します。</p> <p>この行は必須です。</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p>フィルターするタスクのステータスが「処理中」に等しい必要があることを示すには、上記以外の行も使用します。</p> <p><code>status_Mod=in</code> </p> <p>モディファイヤが範囲の場合は、モディファイヤを示す線が 2 つあります。</p> 
       <div> <span class="autonumber"><span><b>例 </b></span></span> 
        <p>これは、進行中のタスクを検索し、現在の月内に完了予定日が設定され、特定の GUID を持つユーザーに割り当てられるテキストモードフィルターです。</p> 
        <p><code>assignedToID=580a55a4000701f4b2d7dee1e7a9d427</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>plannedCompletionDate=$$TODAYbm</code> </p> 
        <p><code>plannedCompletionDate_Mod=between</code> </p> 
        <p><code>plannedCompletionDate_Range=$$TODAYem</code> </p> 
        <p>テキストモードでのフィルター修飾子の完全なリストについては、この記事を参照してください。 <a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">フィルターおよび条件修飾子</a>.</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>文演算子。 デフォルトでは、各フィルター文は、「AND」演算子で結び付けられます。 これは、テキストモードインターフェイスには表示されません。 また、2 つのステートメントの間に「OR」演算子を追加して、2 つの条件の一方または他方を満たすオブジェクトをフィルタリングすることを示すこともできます。</p> <p>フィルター演算子は、複数の文を持つフィルターに対してのみ必要です。</p> <p>ヒント：   
        <ul> 
         <li> <p>「OR」の場合は大文字と小文字が区別され、常に大文字にする必要があります。</p> </li> 
         <li> <p>演算子を AND から OR に変更すると、リスト項目の数が増える場合があります。</p> </li> 
        </ul> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div> <span class="autonumber"><span><b>例 </b></span></span> 
        <p>ステータスが「処理中」、または「予定完了日」が「今日」のタスクをフィルタするには、次の手順に従います。 </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>OR:1:plannedCompletionDate=$$TODAY</code> </p> 
        <p><code>OR:1:plannedCompletionDate_Mod=eq</code> </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>ワイルドカードを使用すると、フィルターの情報を一般化し、現在の時刻やログインしているユーザーを参照できます。</p> <p>ワイルドカードはオプションです。</p> <p>ヒント：   <p>可能な限りワイルドカードを使用して、フィルターをより動的にし、各ユーザーや類似の時間枠で同じフィルターを重複させないことをお勧めします。</p> <p>ワイルドカードのフィルタの詳細については、「 <a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">ワイルドカードフィルター変数</a>.</p> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;wildcard&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>例</b></span></span> 
        <p>現在ログインしているユーザーに割り当てられているタスクをフィルタするには、次の手順に従います。</p> 
        <p><code>assignedToID=$$USER.ID</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「OR」演算子で結び付けられたフィルター文を追加するには、次の手順を実行します。

   1. 新しいコード行を追加し、OR と入力します。:1: フィルタに使用するオブジェクトまたは属性と、その比較対象の値が続きます。 「新規」以外のステータスのタスクを参照するには、次の行を使用します。

      ```
      OR:1:status=NEW
      ```

   1. 2 行目を追加し、 OR と入力します。:1: オブジェクト、モディファイヤ、およびモディファイヤコードが続きます。 「新規」を除くすべてのタスクステータスを参照するコード行の修飾子を定義するには、次の修飾子行を使用します。

      ```
      OR:1:status_Mod=notin
      ```

      新しい文の各行の前には「OR:`<number>`:&quot;.

      フィルターでの「OR」ステートメントの作成について詳しくは、 [テキストモードフィルターでの「OR」ステートメントの作成](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md).

<!--WRITER - reformat note below -->

>[!NOTE]
>
>同じフィルター内に複数の「OR」ステートメントを含めることができます。 新しい「OR」ステートメントを作成するたびに、「OR:」の後の数値が増加します。
>
ステータスが「処理中」、ログインユーザーに割り当てられているタスク、または今日予定完了日を持っているタスクをフィルタするには、次の手順に従います。
>
`status=INP`
>
`status_Mod=in`
>
`OR:1:assignedToID=$$USER.ID`
>
`OR:1:assignedToID_Mod=in`
>
`OR:2:plannedCompletionDate=$$TODAY`
>
`OR:2:plannedCompletionDate_Mod=eq`

1. クリック **完了** 変更を保存し、レポートまたはフィルターの編集を続ける場合。
1. クリック **保存して閉じる** レポートを保存するか、 **フィルターを保存** をクリックして、リストにフィルターを保存します。


