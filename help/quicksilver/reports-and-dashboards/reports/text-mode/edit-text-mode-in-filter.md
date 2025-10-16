---
product-area: reporting
navigation-topic: text-mode-reporting
title: テキストモードを使用したフィルターの編集
description: テキストモードを使用してリストまたはレポートのフィルターを編集し、標準インターフェースで使用できないフィールドにアクセスして、より複雑なフィルターを作成できます。
author: Nolan
feature: Reports and Dashboards
exl-id: bfd1d49f-72cd-466d-8b35-8ae9848646be
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '1044'
ht-degree: 84%

---

# テキストモードを使用したフィルターの編集

<!-- Audited: 1/2025 -->

テキストモードを使用してリストまたはレポートのフィルターを編集し、標準インターフェースで使用できないフィールドにアクセスして、より複雑なフィルターを作成できます。

フィルター作成時のその他のテキストモード例については、[カスタムビュー、フィルターおよびグループ化の例：記事インデックス](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)の記事にある[カスタムフィルターの例](../custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md#samples-of-custom-filters)の節も参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
     <p>標準</p>
     <p>プラン</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>フィルター、ビュー、グループ化の編集アクセス権</p> <p>レポートのレポート要素を編集するための、レポート、ダッシュボード、カレンダーへの編集アクセス権</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートの権限を管理してレポートのフィルターを編集</p> <p>フィルターを編集する権限を管理</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

レポートまたはリストでのテキストモードの使用を開始する前に、必ず Workfront のテキストモード構文を熟知してください。

詳しくは、以下を参照してください。

* [テキストモードの概要](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md)
* [テキストモード構文の概要](../../../reports-and-dashboards/reports/text-mode/text-mode-syntax-overview.md)
* [カスタムビュー、フィルター、グループ化の例：記事インデックス](../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/custom-view-filter-grouping-samples.md)

## フィルターでのテキストモード編集

テキストモードを使用したフィルターの編集は、レポートとリストで同じです。レポートから、またはリストからのフィルターへのアクセスは異なります。

>[!TIP]
>
>標準モードでできるだけ多くのフィルターを作成し、そのフィルターをテキストモードに変換して編集することをお勧めします。

フィルターの作成について詳しくは、[フィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)を参照してください。

レポートの作成について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。

1. 次のいずれかの操作を行います。

   リストからフィルターにアクセスするには、リストに移動して **フィルター** アイコンをクリックし、変更する **フィルター** サイドパネルのフィルターにカーソルを置いて **編集** アイコン ![&#x200B; 編集アイコン &#x200B;](assets/edit-icon.png) をクリックします。 **フィルター** サイドパネルに選択したフィルターが表示されるか、従来のフィルタービルダーが開きます。

   または

   レポートからフィルターにアクセスするには、レポートに移動して、**レポートアクション**/**編集**/「**フィルター**」タブをクリックします。

1. 次のいずれかの操作を行います。

   リストの **フィルター** サイドパネルを使用している場合は、「**テキストモード**」をクリックします。

   または

   従来のフィルタービルダーまたはレポートを使用している場合は、「**フィルタールールを追加**」をクリックして、フィルターの条件の追加を開始します。 次に、ビルダーの右側にある **テキストモードに切り替える** 次に **テキストモードを編集** をクリックします。

1. テキストモードを使用してフィルターステートメントを追加します。各フィルターステートメントには、次の行と追加情報を含めることができます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td><b>行／情報のフィルター</b></td> 
      <td><b>例</b></td> 
     </tr> 
     <tr> 
      <td> <p>フィールド名および Workfront データベースに表示されるものと等しい値。</p> <p>この行は必須です。</p> <p> データベースでのオブジェクトおよびフィールドの表示について詳しくは、<a href="../../../wf-api/general/api-explorer.md" class="MCXref xref">API エクスプローラー</a>を参照してください。</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;=&lt;value&gt;</code> </p> <p>ステータスが処理中のタスクをフィルタリングするには、次の行を使用します。</p> <p><code>status=INP</code> </p> <p><b>ヒント</b>

   ステータスをフィルタリングする場合、名前ではなく、3 文字のコードを使用する必要があります。</p> </td>
   </tr> 
     <tr> 
      <td> <p>フィールド名修飾子およびその修飾子に相当するもの。これは、フィルタリングに使用するフィールドが満たす必要がある条件を示します。</p> <p>この行は必須です。</p> </td> 
      <td> <p><code>&lt;field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p>フィルタリング対象タスクのステータスが「処理中」である必要があると示すには、上記に加えて、次の行も使用します。</p> <p><code>status_Mod=in</code> </p> <p>修飾子が範囲の場合、修飾子を示す 2 行があります。</p> 
       <div> <span class="autonumber"><span><b>例 </b></span></span> 
        <p>処理中のタスクを検索し、現在の月内に予定完了日が設定され、特定の GUID を持つユーザーに割り当てられるテキストモードフィルターです。</p> 
        <p><code>assignedToID=580a55a4000701f4b2d7dee1e7a9d427</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>plannedCompletionDate=$$TODAYbm</code> </p> 
        <p><code>plannedCompletionDate_Mod=between</code> </p> 
        <p><code>plannedCompletionDate_Range=$$TODAYem</code> </p> 
        <p>テキストモードでのフィルター修飾子の完全なリストについては、<a href="../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md" class="MCXref xref">フィルターと条件修飾子</a>の記事を参照してください。</p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>ステートメント演算子。デフォルトでは、それぞれのフィルターステートメントは、「AND」演算子で結び付けられます。これは、テキストモードインターフェイスには表示されません。また、2 つのステートメントの間に「OR」演算子を追加して、2 つの条件の一方または他方を満たすオブジェクトをフィルタリングすることを示すこともできます。</p> <p>フィルター演算子は、複数のステートメントを持つフィルターに対してのみ必要です。</p> <p>ヒント：   
        <ul> 
         <li> <p>「OR」の場合は大文字と小文字が区別され、常に大文字にする必要があります。</p> </li> 
         <li> <p>演算子を AND から OR に変更すると、リスト項目の数が増える場合があります。</p> </li> 
        </ul> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;=&lt;value&gt;</code> </p> <p><code>OR:1:&lt;second field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div> <span class="autonumber"><span><b>例</b></span></span> 
        <p>ステータスが処理中のタスク、または予定完了日が今日のタスクをフィルタするには、以下のものを使用します。 </p> 
        <p><code>status=INP</code> </p> 
        <p><code>status_Mod=in</code> </p> 
        <p><code>OR:1:plannedCompletionDate=$$TODAY</code> </p> 
        <p><code>OR:1:plannedCompletionDate_Mod=eq</code> </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td> <p>ワイルドカードは、フィルターの情報を一般化し、現在の時刻やログインしているユーザーを参照できるようにします。</p> <p>ワイルドカードはオプションです。</p> <p>ヒント：   <p>可能な限りワイルドカードを使用して、フィルターをより動的にし、各ユーザーや類似の時間枠で同じフィルターを重複させないようにすることをお勧めします。</p> <p>ワイルドカードのフィルタリングについて詳しくは、<a href="../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md" class="MCXref xref">ワイルドカードフィルター変数の概要</a>を参照してください。</p> </p> </td> 
      <td> <p><code>&lt;first field name in camel case&gt;=&lt;wildcard&gt;</code> </p> <p><code>&lt;first field name in camel case&gt;_Mod=&lt;modifier value&gt;</code> </p> 
       <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>例</b></span></span> 
        <p>現在ログインしているユーザーに割り当てられているタスクをフィルタリングするには、以下のものを使用します。</p> 
        <p><code>assignedToID=$$USER.ID</code> </p> 
        <p><code>assignedToID_Mod=in</code> </p> 
       </div> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「OR」演算子で接続されたフィルターステートメントを追加するには、以下のように行います。

   1. 新しいコード行を追加し、OR:1: と入力します。続けて、フィルタリングするオブジェクトまたは属性と、それを比較する値を入力します。新規以外のステータスのタスクを参照するには、次の行を使用します。

      `OR:1:status=NEW`

   1. 2 行目を追加し、OR:1:と入力します。オブジェクト、修飾子、修飾子コードが続きます。新規を除くすべてのタスクステータスを参照するコード行の修飾子を定義するには、次の修飾子行を使用します。

      `OR:1:status_Mod=notin`

      新しいステートメントの各行の前には「OR:`<number>`:」が付いています。

      フィルターでの「OR」ステートメントの作成について詳しくは、[テキストモードフィルターで「OR」ステートメントを作成](../../../reports-and-dashboards/reports/text-mode/create-or-statements-in-filters-text-mode.md)を参照してください。

      >[!NOTE]
      >
      >同じフィルター内に複数の「OR」ステートメントを含めることができます。新しい「OR」ステートメントを作成するたびに、「OR:」の後の数値が増加します。
      >
      >ステータスが「処理中」のタスク、ログインしているユーザーに割り当てられているタスク、または予定完了日が今日のタスクをフィルタリングするには、以下を使用します。
      >
      >`status=INP`
      >`status_Mod=in`
      >`OR:1:assignedToID=$$USER.ID`
      >`OR:1:assignedToID_Mod=in`
      >`OR:2:plannedCompletionDate=$$TODAY`
      >`OR:2:plannedCompletionDate_Mod=eq`

1. **適用** または **完了** をクリックして、テキストモードの変更を保存し、レポートまたはフィルターの編集を続行します。
1. 「**保存して閉じる**」をクリックしてレポートを保存するか、「**フィルターを保存**」をクリックして、リストにフィルターを保存します。


