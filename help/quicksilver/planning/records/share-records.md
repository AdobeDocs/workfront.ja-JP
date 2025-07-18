---
title: レコードの共有
description: 他のユーザーとレコードを共有して、共同作業を強化できます。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 47%

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

+++ 展開すると、アクセス要件が表示されます。

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
<p>Workfront Planning にアクセスするには、組織のWorkfront インスタンスをAdobe Unified Experience にオンボーディングする必要があります。</p> 
<p>詳しくは、<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront の Adobe Unified Experience</a> を参照してください。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td><p> コントリビューター以上のライセンス </p>
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
   <td>  <p>ワークスペースに対する表示以上の権限と共有するレコードタイプ   リンクを使用したレコード </p>
   <p>ワークスペースに対する権限とワークスペースでレコードを共有するためのレコードタイプを管理します </p>
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

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


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

詳しくは、[ レコードタイプの共有 ](/help/quicksilver/planning/access/share-record-types.md) を参照してください。

