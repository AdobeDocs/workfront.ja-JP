---
title: フィールドを削除
description: Adobe Workfront Planning では、関係なくなったカスタムフィールドを削除できます。
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
author: Alina
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 33%

---



# フィールドの削除

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

Adobe Workfront Planning では、カスタムフィールドを作成して、レコードに関する情報を格納できます。

Workfront Planning でのカスタムフィールドの作成について詳しくは、[フィールドの作成](/help/quicksilver/planning/fields/create-fields.md)を参照してください。

関係がなくなった Workfront Planning フィールドは削除できます。

## アクセス要件

+++ 展開して、この記事の機能のアクセス要件を表示します。 

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
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<ul> 
<li><p>任意のWorkfrontと任意の Planning パッケージ</p></li>
または
<li><p>任意のワークフローおよび任意の計画パッケージ</p></li></ul>

<p><span class="preview">グローバルレコードタイプからフィールドを削除する手順は次のとおりです。</span></p>
<ul><li><p><span class="preview">任意のWorkfront パッケージと Planning Plus パッケージ</span></p></li>
または
<li><p><span class="preview">あらゆるワークフローおよび Planning PrimeおよびUltimate パッケージ</span></p></li></ul>

<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースに対する権限の管理</p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++   

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
   <td><p> Standard </p>
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
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> -->

## Workfront Planning フィールドの削除に関する考慮事項：

* レコードタイプのテーブルビューでのみフィールドを削除できます。
* レコードの主フィールドは削除できません。
* フィールドに格納されている情報はすべて削除され、復元できません。
* 接続したレコードフィールドを削除すると、接続したすべてのルックアップフィールドも接続元のレコードタイプから削除されます。 接続先のレコードタイプの接続済みレコードフィールドも、接続先のレコードから削除されます。

  例えば、キャンペーンを製品と呼ばれる別のレコードタイプに接続し、キャンペーンから「製品の接続」フィールドと「製品のステータス」ルックアップフィールドを削除すると、次の項目が削除されます。

   * キャンペーンの「接続済み製品」フィールド
   * キャンペーンの「製品ステータス」ルックアップフィールド
   * 製品の「キャンペーンに接続」フィールド

  詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

* <span class="preview"> セカンダリワークスペースに追加されたグローバルレコードのフィールドは、セカンダリワークスペースから削除できません。</span>

## フィールドを削除

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. レコード フィールドを削除するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプが表示されます。

1. レコードタイプのカードをクリックします。

1. （条件付き）選択していない場合は、レコードタイプページで **テーブル表示** のタブをクリックします。

   そのレコードタイプに関連付けられている既存のすべてのレコードが、テーブルビューの行に表示されます。

1. 削除するフィールドを列ヘッダーで見つけてその上にポインタを合わせ、フィールド名の後の下向き矢印をクリックします。

   ![&#x200B; テーブルヘッダーのフィールド名の後の矢印メニューがハイライト表示されている &#x200B;](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. 「**削除**」をクリックします。<!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. 「**削除**」をクリックして確定します。

   削除したフィールドは復元できません。

   削除したフィールドのタイプに応じて、次のようになります。

   * 選択したレコードに属するフィールドを削除すると、そのフィールドは削除され、どのレコードにも関連付けられなくなります。 このフィールドが他のレコードの参照フィールドとして追加されると、これらのフィールドも削除されます。
   * 接続フィールドを削除すると、選択したレコードからそのフィールドが削除されます。 また、対応する接続フィールドも元のレコードから削除されます。
   * 接続されたレコードから追加されたルックアップ フィールドを削除すると、選択したレコードの種類からフィールドが削除されますが、元のレコードの種類には残ります。
   * <span class="preview"> プライマリワークスペースのグローバルレコードタイプからフィールドを削除すると、そのレコードタイプが追加されたすべてのワークスペースから削除されます。 グローバルレコードタイプのフィールドをセカンダリワークスペースから削除することはできません。</span>
