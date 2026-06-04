---
title: フィールドの削除
description: Adobe Workfront Planning では、関係なくなったカスタムフィールドを削除できます。
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
author: Alina
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/EusoK7-jmYJHg9nqyvvQamsfVeUy802p36EyDmLGwik
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: e147ce9d-7675-49bd-8a32-44f27d865560
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 733
ht-degree: 29%

---

# フィールドの削除

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。 すべてのユーザーのプレビュー環境でのみ使用できます。 実稼動環境への毎月のリリース後、高速リリースを有効にしたお客様は、実稼動環境でも同じ機能を利用できます。</span>

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
<li><p>任意のWorkfrontおよびプランニングパッケージ</p></li>
または
<li><p>任意のワークフローとプランニングパッケージ</p></li></ul>

<p>グローバルレコードタイプからフィールドを削除するには：</p>
<ul><li><p>任意のWorkfront パッケージとPlanning Plus パッケージ</p></li>
または
<li><p>PrimeとUltimateのあらゆるパッケージのワークフローとプランニング</p></li></ul>

<p>各Workfront計画パッケージに含まれる内容について詳しくは、Workfrontの担当者にお問い合わせください。 </p> 
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

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++   

<!--
Old:

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
</table>
-->

## Workfront Planning フィールドの削除に関する考慮事項：

* レコードタイプのテーブルビューでのみフィールドを削除できます。
* レコードの主フィールドは削除できません。
* フィールドに格納されている情報はすべて削除され、復元できません。
* 接続されたレコードフィールドを削除すると、接続されたすべてのルックアップフィールドも、接続したレコードタイプから削除されます。 接続先のレコードタイプの接続レコードフィールドも、接続先のレコードから削除されます。

  例えば、CampaignsをProductという別のレコードタイプに接続し、キャンペーンからProduct connected フィールドとProduct&#39;s Status ルックアップフィールドを削除すると、次のものが削除されます。

   * キャンペーンの「製品接続」フィールド
   * キャンペーンの「製品ステータス」ルックアップフィールド
   * 製品のキャンペーン接続フィールド

  詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

* セカンダリワークスペースに追加されたグローバルレコードから、セカンダリワークスペースからフィールドを削除することはできません。

## フィールドを削除

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-planning}}

1. 削除するレコードフィールドがあるワークスペースをクリックします。

   ワークスペースが開き、レコードタイプが表示されます。

1. レコードタイプのカードをクリックします。

1. （条件付き）まだ選択していない場合は、レコードタイプページの&#x200B;**テーブルビュー**&#x200B;のタブをクリックします。

   そのレコードタイプに関連付けられている既存のすべてのレコードが、テーブルビューの行に表示されます。

1. 削除するフィールドを列ヘッダーで見つけてその上にポインタを合わせ、フィールド名の後の下向き矢印をクリックします。

   ![ テーブルヘッダーのフィールド名の後の矢印メニューが強調表示される](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. 「**削除**」をクリックします。<!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. <span class="preview"> （条件付き）削除するフィールドがリクエストフォームの一部である場合、「**フィールドを削除**」ボックスが表示され、変更の影響を受けるフォームが示されます。 次のいずれかの操作を行います：</span>

   <div class="preview">

   * 右向きの矢印をクリックして、変更の影響を受けるフォームを表示し、フォーム名をクリックしてフォームを新しいタブで開き、フィールドをフォームに保持するか、フォームに追加の変更を加えるかを決定します。
   * 表示されているすべての領域からフィールドを削除する&#x200B;**削除**&#x200B;をクリックします。

   </div>

   削除されたフィールドは復元できません。

   削除したフィールドのタイプに応じて、次のことが行われます。

   * 選択したレコードに属するフィールドを削除すると、そのフィールドは削除され、どのレコードにも関連付けられなくなります。 このフィールドが他のレコードのルックアップフィールドとして追加された場合、それらのフィールドも削除されます。
   * 接続フィールドを削除すると、選択したレコードからフィールドが削除されます。 また、元のレコードの対応する接続フィールドも削除されます。
   * 接続されたレコードから追加されたルックアップフィールドを削除すると、そのフィールドは選択したレコードタイプから削除されますが、元のレコードタイプに残ります。
   * プライマリワークスペースのグローバルレコードタイプからフィールドを削除すると、そのレコードタイプが追加されたすべてのワークスペースからフィールドが削除されます。 セカンダリワークスペースからグローバルレコードタイプのフィールドを削除することはできません。
