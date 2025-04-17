---
title: 数式フィールドの概要
description: Adobe Workfront Planning では、関数と既存のフィールドを使用して新しいカスタム値を計算する数式フィールドを作成できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 5027d611-916e-492d-9a44-841bdde11c94
source-git-commit: 5a4ceb3bd7a5f121312d26775b6cf91604585775
workflow-type: tm+mt
source-wordcount: '710'
ht-degree: 50%

---

# 数式フィールドの概要

<!--when we release permissions to RECORDS and we release referring lookup fields in a formula field, update considerations to say that lookup fields from linked records depends on the permissions to the record; if they have no permissions to view a linked record, they won't be able to use that records's lookup fields in a formula-->

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

既存のフィールドを参照し、式タイプのフィールドで接続することで、Adobe Workfront Planning でカスタムフィールドを作成できます。

数式フィールドは、レコードタイプの他のフィールドの既存の値と、既存の値の計算方法を示す関数を使用して、新しい値を生成します。

詳しくは、「フィールドの作成 [ の「式」の節を参照してくだ ](/help/quicksilver/planning/fields/create-fields.md) い。

## アクセス要件

+++ 展開してアクセス要件を表示します…

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> 製品</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfrontの計画<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td> 
<p>次のいずれかのWorkfront プラン：</p> 
<ul><li>選択</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning は、従来のWorkfront プランでは使用できません</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning パッケージ*</p></td> 
   <td> 
<p>任意 </p> 
<p>各Workfront Planning プランに含まれる内容について詳しくは、Workfront担当営業または販売店にお問い合わせください。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>組織のWorkfront インスタンスは、Workfront Planning のすべての機能にアクセスできるように、Adobe Unified Experience にオンボーディングされる必要があります。</p> 
<p>詳しくは、<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront の Adobe Unified Experience</a> を参照してください。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td><p> 標準</p>
   <p>Workfront Planning は、従来のWorkfront ライセンスでは使用できません</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペース <span class="preview"> およびレコードタイプ </span></a> に対する権限の管理 </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> <p>Workfront の管理者を含むすべてのユーザーには、メインメニューの Planning エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--

OLD:
<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license*</p></td>
   <td>
   <p>New: Standard</p>
   <p>Current: Plan</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access controls for Workfornt planining</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>Manage permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>

 </tbody>
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->

## 数式フィールドに関する考慮事項

* 式フィールドは、同じレコードタイプに属するフィールドを参照します。
* 他のレコードタイプのフィールドを参照できるのは、式フィールドを作成するレコードタイプに別のレコードタイプを接続する場合のみです。
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

## サポートされる数式

Adobe Workfront Planning の数式フィールドは、Workfrontの計算フィールドの式のほとんどをサポートしています。

>[!NOTE]
>
>次のWorkfront式は、Workfront Planning 式フィールドではサポートされていません：
>
>* SORTASCARRAY
>* SORTDESCARRAY
>* ADDHOUR
>* SWITCH
>* 形式


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
