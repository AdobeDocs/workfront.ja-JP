---
title: 数式フィールドの概要
description: Adobe Workfront Planning では、関数と既存のフィールドを使用して新しいカスタム値を計算する数式フィールドを作成できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '779'
ht-degree: 29%

---

# 数式フィールドの概要

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

既存のフィールドを参照し、式タイプのフィールドで接続することで、Adobe Workfront Planning でカスタムフィールドを作成できます。

数式フィールドは、レコードタイプの他のフィールドの既存の値と、既存の値の計算方法を示す関数を使用して、新しい値を生成します。

詳しくは、「フィールドの作成 [ の「式」の節を参照してくだ ](/help/quicksilver/planning/fields/create-fields.md) い。

<!--do we need these for an overview article?

## Access requirements

+++ Expand to view the access requirements for the functionality in this article. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Any Workfront and any Planning package</p>
<p>Any Workflow and any Planning package</p>
<p>For more information about what is included in each Workfront Planning package, contact your Workfront account representative. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr>  
</tbody> 
</table> 

For more information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   

-->

<!--Old:

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
 
</tbody> 
</table> -->

## 数式フィールドに関する考慮事項

* 式フィールドは、同じレコードタイプに属するフィールドを参照します。
* 他のレコードタイプのフィールドを参照できるのは、式フィールドを作成するレコードタイプに別のレコードタイプを接続する場合のみです。
* 数式内で接続されたレコードタイプまたはそのルックアップフィールドを参照できるかどうかは、接続されたレコードタイプに対する権限によって異なります。 レコードタイプを表示する権限がない場合、数式でそのフィールドを参照することはできません。
* 式フィールドを保存した後で、そのフィールド タイプを変更することはできません。
* 数式フィールドを保存した後でその計算を更新すると、同じタイプのすべてのレコードに対して、計算結果を自動的に更新できます。
* Workfront Planning インターフェイスに表示される数式で参照するフィールドを追加する必要があります。
* レコードタイプのテーブル表示またはレコードの詳細ページに表示されるフィールドのみを参照できます。
* 次のフォーマット・オプションから選択して、式の計算の値のフォーマットを定義できます：

   * テキスト
   * 数値
   * パーセント
   * 通貨
   * タグ
   * 日付

  詳しくは、「フィールドの作成 [ の「式」の節を参照してくだ ](/help/quicksilver/planning/fields/create-fields.md) い。
* 新しい数式で数式フィールドを参照できます。 式フィールドで参照されているフィールドの値が更新されると、そのフィールドまたはそのフィールドを含む式フィールドを参照している後続のすべてのフィールドは、自動的に更新されます。

* 影響を与える可能性のある式フィールドまたはフィールドを更新すると、変更の影響を知らせるアラートが表示されます。 アラートは、次の場合に表示されます。

   * 式フィールドに従属式または参照フィールドがある場合、そのフィールドを更新するとき（名前および説明の変更を除く）。 アラートには、これらの依存フィールドが一覧表示され、続行するかどうかを尋ねられます。

   * 数式または参照フィールドとして使用されているフィールドを削除したとき。 このアラートでは、従属式およびルックアップ フィールドがリスト表示され、削除を続行するかどうかを確認するメッセージが表示されます。

## 式フィールドの制限事項

* 1 つのレコードタイプに対して最大 20 個の式フィールドを追加できます。

  接続されたレコードタイプから追加された数式参照フィールドは、この制限にカウントされません。

* 数式は 50,000 文字を超えることはできません。

* 式フィールドは、次の場合に `#ERROR!` のように表示されることがあります。
   * 式で使用されているフィールドが削除されたとき。
   * 集計参照フィールドで使用されているフィールドが `#ERROR!` として表示されている場合。

     例えば、集計参照式フィールドを含む参照フィールドを表示すると、参照式フィールドの 1 つが `#ERROR!` として表示されます。
   * 選択した形式で式の値を表示できない場合。

     例えば、数式フィールドの「形式」で「数値」を選択したときに、数式で使用されているフィールドが数値以外のテキスト値のみを表示するテキストフィールドである場合、テキストを数値に解析できないので、数式の結果は `#ERROR!` と表示されます。


## サポートされる数式

Adobe Workfront Planning の数式フィールドは、Workfrontの計算フィールドの式のほとんどをサポートしています。

>[!NOTE]
>
>次のWorkfront式は、Workfront Planning 式フィールドではサポートされていません：
>
><!--* SORTASCARRAY-->
><!--* SORTDESCARRAY-->
>* ADDHOUR
>* SWITCH
>* 形式

<!--remove the ones commented out when we go live to Preview and Prod, if they truly are added to Planning-->

Workfront式の完全なリストについては、[ 計算データ式の概要 ](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md) を参照してください。

また、Workfront Planning の数式フィールドでは、以下の式をサポートしています。 次の式は、Workfrontの式ではサポートされていません。

<!--take these three out when they also come to WF and Lisa has added them to the WF expression article linked above-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>式</th> 
   <th>説明と例</th> 
  </tr> 
 </thead> 
 <tbody>

<tr> 
   <td><strong>ARRAYJOIN</strong> </td> 
   <td> <p>区切り文字で連結された文字列を返します。</p> <p>式の形式は次のとおりです。

<code>ARRAYJOIN(区切り文字,配列)</code>
</p>
   </td></tr>
    <tr> 
   <td><strong>ARRAYUNIQUE</strong> </td> 
   <td> <p>一意の値を含む配列を返します。</p> <p>式の形式は次のとおりです。

<code>ARRAYUNIQUE(配列)</code>
</p>
   </td></tr>
     <tr> 
   <td><strong>ID</strong> </td> 
   <td> <p>レコードの ID を返します。各レコードには一意の ID が割り当てられています。</p> <p>式の形式は次のとおりです。

<code>{ID}</code>
</p>
   </td></tr>
  <tr> 
   <td><strong>JSONELEMENT</strong> </td> 
   <td> <p>指定された JSONPath によって JSON からデータを返します。 JSON 内に JSONPath が存在しない場合は、空の結果が返されます。 </p> <p>式は次のようにフォーマットされます。
      <code>JSONELEMENT(JSONString, JSONPathString) </code>
   </p>
   </td></tr>
  <tr> 
   <td><strong>SETTIMEZONE</strong> </td> 
   <td> <p>日付と時刻のタイムゾーンを指定されたタイムゾーンに設定します。</p> <p>式の形式は次のとおりです。

<code>SETTIMEZONE(日付, &#39;America/Los_Angeles&#39;)</code>
</p>
   </td></tr>

<tr> 
   <td><strong>WEEKOFYEAR</strong> </td> 
   <td> <p>年の週数を返します。必要に応じて、週の開始日を指定できます (日曜日の場合は 1、月曜日の場合は 2 を使用)。省略した場合、デフォルトでは週は日曜日に開始します。</p> <p>式の形式は次のとおりです。

<code>WEEKOFYEAR(日付、2)</code>
または
<code>WEEKOFYEAR(日付)</code>
</p>
   </td></tr>

</table>
