---
title: Workspace階層の作成
description: 作業領域管理者は、Adobe Workfront Planning のレコード・タイプ間に複数の作業領域階層を作成できます。 ワークスペースでレコードタイプを接続し、階層を作成すると、レコードタイプが相互に接続され、1 つのレコードタイプが親として指定され、最大 6 つの他のレコードタイプが子として設定されます。
hide: true
hidefromtoc: true
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: ff9371b639e7684a94c08b8cd6293b632fac9edf
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 12%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Create Workspace Hierarchies
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---

-->

# ワークスペース階層の作成

作業領域管理者は、Adobe Workfront Planning のレコード・タイプ間に複数の作業領域階層を作成できます。

ワークスペースでレコードタイプを接続し、階層を作成すると、レコードタイプが相互に接続され、1 つのレコードタイプが親として指定され、最大 6 つの他のレコードタイプが子として設定されます。<!--asking Robert how many we can have in one hierarchy; I think 7 total but not sure-->

階層では、ヘッダーに表示されるレコードタイプおよびレコード <!--ensure this is the case: does the breadcrumb show for both the RT and the record??--> のパンくずリストが生成されます。 これにより、ワークフローの任意のステージで、階層内の自分の位置を把握できます。

階層とパンくずリストに関する一般的な情報については、[ 階層とパンくずリストの概要 ](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md) を参照してください。


## アクセス要件

<!--check the access to see if you oversimplified???-->

<!--Update the TOC for this to publish-->

+++ を展開してアクセス要件を表示し、この記事の手順を実行します。  

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
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>Standard</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースに対する権限の管理</p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## ワークスペース階層の作成
