---
title: レコードの共有
description: 他のユーザーとレコードを共有して、共同作業を強化できます。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 45%

---


<!--should this move to the Access folder when we have sharing for ALL the objects???-->

<!--take out preview and production references at release-->

# レコードの共有

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>  -->

{{planning-important-intro}}

他のユーザーと共同作業する場合は、他のユーザーとレコードを共有できます。

次の方法で Adobe Workfront Planning レコードを共有できます。

* ページが開いている場合に、レコードページのリンクをブラウザーからコピーします。

* レコードタイプのテーブルビューのレコードを表示する際に、レコードのページへのリンクをコピーします。

* ワークスペースとレコードタイプを共有すると、ワークスペース内のすべてのレコードを他のユーザーと共有できます。

  詳しくは、次の記事を参照してください。

   * [ワークスペースの共有](/help/quicksilver/planning/access/share-workspaces.md)

   * [レコードタイプの共有](/help/quicksilver/planning/access/share-record-types.md)

この記事では、レコードタイプのテーブルビューからレコードのページへのリンクをコピーする方法について説明します。

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
<p>任意のWorkfrontと任意の Planning パッケージ</p> <p>任意のワークフローおよび任意の計画パッケージ</p>
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>投稿者以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>  <p>ワークスペースに対する表示以上の権限と、リンクを使用してレコードを共有するためのレコードタイプ</p>
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> ライト ライセンスまたはコントリビュータ ライセンスを持つユーザには、Planning を含むレイアウト テンプレートを割り当てる必要があります。
   <p>標準ユーザーとシステム管理者は、デフォルトで Planning 領域を有効にします。</p></div></li></ul>
</td>
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
   <td><p> Contributor or higher license </p>
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
   <td>  <p>View or higher permissions to a workspace and record typeto share   a record using a link </p>
   <p>Manage permissions to a workspace and record type to share the records in the workspace </p>
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>  </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table> -->


## レコードタイプのテーブルビューからレコードリンクの共有

{{step1-to-planning}}

最後にアクセスしたワークスペースが開きます。

1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。

1. （条件付き）テーブルの右上隅にある&#x200B;**ビュー**&#x200B;のドロップダウンメニューから、テーブルビューを選択します。最後にアクセスしたときにタイムラインビューでレコードタイプを表示した場合を除き、これがデフォルトのビューになります。

   選択したレコードタイプに関連付けられているレコードが、テーブルビューに表示されます。

1. レコード行を右クリックします。

   または

   レコードの名前にポインタを合わせ、「**その他**」メニュー ![&#x200B; その他メニュー &#x200B;](assets/more-menu.png) をクリックしてから、「**リンクをコピー**」をクリックします。

   ![&#x200B; レコード行のコンテキストメニュー &#x200B;](assets/contextual-menu-for-record-row.png)

   リンクがクリップボードにコピーされます。

1. メールまたはチャットウィンドウにリンクを貼り付けて、他のユーザーと共有します。ユーザーがリンクを受け取ると、レコードページが開きます。

   >[!TIP]
   >
   >レコードページのフィールドは、そのレコードのテーブルビューで使用できるフィールドと同じです。


   <!--add there when it will be available: if they have access to this record-->

## ワークスペースを共有することで、ワークスペース内のすべてのレコードを共有します。

ワークスペースを他のユーザーと共有する場合は、ワークスペース内のすべてのレコードを共有できます。

レコードタイプとレコードは、ワークスペースから同じ権限を継承します。

ワークスペースに対する管理権限を持つユーザーのみが、そのワークスペースを他のユーザーと共有できます。

詳しくは、[ワークスペースの共有](/help/quicksilver/planning/access/share-workspaces.md)を参照してください。

## レコードタイプを共有することで、レコードタイプ内のすべてのレコードを共有する

レコードはレコードタイプから権限を継承します。

デフォルトでは、レコードタイプはワークスペースから権限を継承します。

ただし、次のいずれかの操作を行うことができます。

* レコードタイプのワークスペースから継承された権限を無効にします。 これにより、レコードに対するより高い権限が削除されますが、ワークスペース、レコードタイプおよびレコードに対する表示権限は保持されます。
* ワークスペースに対する権限を持っていない場合でも、レコードタイプに対する権限をユーザーに手動で付与します。 これにより、ワークスペースに対する表示権限が自動的に付与されます。 これにより、レコードに対する権限がユーザーに付与されます。

ワークスペースに対する管理権限を持つユーザーのみが、そのレコードタイプとレコードを他のユーザーと共有できます。

詳しくは、[&#x200B; レコードタイプの共有 &#x200B;](/help/quicksilver/planning/access/share-record-types.md) を参照してください。

