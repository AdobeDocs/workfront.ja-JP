---
title: レコードの共有
description: 他のユーザーとレコードを共有して、共同作業を強化できます。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: 5a4ceb3bd7a5f121312d26775b6cf91604585775
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 50%

---


<!--should this move to the Access folder when we have sharing for ALL the objects???-->

<!--take out preview and production references at release-->

# レコードの共有

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

他のユーザーと共同作業する場合は、他のユーザーとレコードを共有できます。

次の方法で Adobe Workfront Planning レコードを共有できます。

* ページが開いている場合に、レコードページのリンクをブラウザーからコピーします。

* レコードタイプのテーブルビューのレコードを表示する際に、レコードのページへのリンクをコピーします。

* ワークスペース <span class="preview"> およびレコードタイプ </span> を共有することで、ワークスペース内のすべてのレコードを他のユーザーと共有できます。

  詳しくは、次の記事を参照してください。

   * [ワークスペースの共有](/help/quicksilver/planning/access/share-workspaces.md)

  <div class="preview">

   * [レコードタイプの共有](/help/quicksilver/planning/access/share-record-types.md)

  </div>

この記事では、レコードタイプのテーブルビューからレコードのページへのリンクをコピーする方法について説明します。

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
   <td><p> 共同作成者、ライト、または標準 </p>
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
   <td>  <p>共有するワークスペース <span class="preview"> およびレコードタイプ </span> に対する表示以上の権限   リンクを使用したレコード </p>
   <p>ワークスペース <span class="preview"> およびレコードタイプ </span> に対する権限を管理して、ワークスペース内のレコードを共有します </p>
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> <p>Workfront の管理者を含むすべてのユーザーには、メインメニューの Planning エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


<!--OLD:

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
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls for Workfront Planning</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace to share a record using a link </p>
   <p>Manage permissions to a workspace to share the workspace the record belongs to </p>
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

-->

## レコードタイプのテーブルビューからレコードリンクの共有

{{step1-to-planning}}

最後にアクセスしたワークスペースが開きます。
1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。
1. （条件付き）テーブルの右上隅にある&#x200B;**ビュー**&#x200B;のドロップダウンメニューから、テーブルビューを選択します。最後にアクセスしたときにタイムラインビューでレコードタイプを表示した場合を除き、これがデフォルトのビューになります。

   選択したレコードタイプに関連付けられているレコードが、テーブルビューに表示されます。
1. レコード行を右クリックします。

   または

   レコードの名前にポインタを合わせ、「**その他**」メニュー ![ その他メニュー ](assets/more-menu.png) をクリックしてから、「**リンクをコピー**」をクリックします。

   ![ レコード行のコンテキストメニュー ](assets/contextual-menu-for-record-row.png)

   リンクがクリップボードにコピーされます。

1. メールまたはチャットウィンドウにリンクを貼り付けて、他のユーザーと共有します。ユーザーがリンクを受け取ると、レコードページが開きます。

   >[!TIP]
   >
   >レコードページのフィールドは、そのレコードのテーブルビューで使用できるフィールドと同じです。


   <!--add there when it will be available: if they have access to this record-->

## ワークスペースを共有することで、ワークスペース内のすべてのレコードを共有します。

ワークスペースを他のユーザーと共有する場合は、ワークスペース内のすべてのレコードを共有できます。

ワークスペースに対する管理権限を持つユーザーのみが、そのワークスペースを他のユーザーと共有できます。

詳しくは、[ワークスペースの共有](/help/quicksilver/planning/access/share-workspaces.md)を参照してください。


<div class="preview">

## レコードタイプを共有することで、レコードタイプ内のすべてのレコードを共有する

実稼動環境では、レコードはワークスペースから権限を継承します。

プレビュー環境では、レコードはレコードタイプから権限を継承します。

デフォルトでは、レコードタイプはワークスペースから権限を継承します。

ただし、次のいずれかの操作を行うことができます。

* レコードタイプのワークスペースから継承された権限を無効にします。 これにより、レコードに対するより高い権限が削除されますが、ワークスペース、レコードタイプおよびレコードに対する表示権限は保持されます。
* ワークスペースに対する権限を持っていない場合でも、レコードタイプに対する権限をユーザーに手動で付与します。 これにより、ワークスペースに対する表示権限が自動的に付与されます。 これにより、レコードに対する権限がユーザーに付与されます。

ワークスペースに対する管理権限を持つユーザーのみが、そのレコードタイプとレコードを他のユーザーと共有できます。

詳しくは、[ レコードタイプの共有 ](/help/quicksilver/planning/access/share-record-types.md) を参照してください。

</div>
