---
title: Workspace階層の作成
description: 作業領域管理者は、Adobe Workfront Planning のレコード・タイプ間に複数の作業領域階層を作成できます。 ワークスペースでレコードタイプを接続し、階層を作成すると、レコードタイプが相互に接続され、1 つのレコードタイプが親として指定され、最大 6 つの他のレコードタイプが子として設定されます。
hide: true
hidefromtoc: true
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: 6aba4316228a320cf33e419249a64b3cf56e8f39
workflow-type: tm+mt
source-wordcount: '662'
ht-degree: 5%

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


ワークスペース内でレコードタイプを接続したら、それらの接続を整理する階層を作成できます。 階層は、レコード・タイプを親子関係に整理し、最大 4 つのレベルのオブジェクト・タイプを含めることができます。

2 つのレコードタイプ間の接続がまだ存在しない場合は、階層を設定するときに作成できます。 定義が完了すると、ワークスペース内の関連するレコードタイプ間で階層の構造化パスが確立されます。

階層では、ヘッダーに表示されるレコードタイプおよびレコード <!--ensure this is the case: does the breadcrumb show for both the RT and the record??--> のパンくずリストが生成されます。 これにより、ワークフローの任意のステージで、階層内の自分の位置を把握できます。

階層とパンくずリストに関する一般的な情報については、[&#x200B; 階層とパンくずリストの概要 &#x200B;](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md) を参照してください。

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

## ワークスペース階層の作成

{#step1-to-planning}

1. ワークスペースカードをクリックします。
1. ワークスペース名の右側にある **その他** メニュー ![&#x200B; その他のメニュー &#x200B;](assets/more-menu.png) をクリックし、**設定** をクリックします。
**階層** セクションは、デフォルトで開きます。
1. **階層** ページの右上隅にある **新規階層** をクリックします。
1. **オブジェクトを追加** をクリックし、ドロップダウンメニューからオブジェクトを選択します。 これが階層内の最初の親オブジェクトになります。
最初の親は、Planning レコード タイプのみです。 Workfront プロジェクトは、階層内の他のオブジェクトタイプの親として選択できません。
1. 「**オブジェクトを追加**」をクリックして、階層の最初の子である 2 番目のオブジェクトを追加し、ドロップダウンメニューで別のオブジェクトを選択します。
   ![&#x200B; フィールドが選択されていない新しい階層ボックス &#x200B;](assets/new-hierarchy-modal-without-connecte-fielf-selected.png)
1. **接続されたフィールドを選択**&rbrack; をクリックして、2 つのオブジェクトを接続するフィールドを指定します。
1. （条件付き） 2 つのオブジェクトタイプ間に接続されたフィールドが存在する場合は、リストから選択します。 それ以外の場合は、「**新しい接続を追加**」をクリックします。

   >[!WARNING]
   >
   >接続されたフィールドを作成したときに **リンクされたレコードタイプに対応するフィールドを作成** が選択されなかった場合は、続行する前にまずフィールドを編集する必要があります。

1. （条件付き）新しい接続を追加する場合、次の操作を行います。

   1. 接続したフィールドの名前を「**名前**」ボックスに追加します。
   1. 次の接続タイプから選択します。

      * **多対多**
      * **1 対多**
      * **多対 1**
      * **1 対 1**
   1. 次のいずれかのタイプのレコード外観を選択します。

      * **名前と画像**
      * **名前**
      * **画像**
詳しくは、[&#x200B; レコードタイプの接続 &#x200B;](/help/quicksilver/planning/architecture/connect-record-types.md) を参照してください。
   1. 「**保存**」をクリックします。
1. （オプション）上記の手順に従って、最大 4 つのオブジェクトタイプを階層に追加し続けます。 最初にすべてのオブジェクトタイプを追加してから、それらの間に接続フィールドを追加できます。
1. （オプション） **削除** アイコン ![&#x200B; 削除アイコン &#x200B;](assets/minus-icon.png) をクリックして、接続を削除します。
1. **保存** をクリックして、階層を保存します。

   >[!TIP]
   >
   >接続されているフィールドがまだない場合は、「**保存**」ボタンはグレー表示になります。

   次のことが発生します。

   * 階層がワークスペースの **階層** セクションに追加されます。
   * レコードのページに移動すると、接続フィールドに入力されるレコードに、パンくずリストのすべての接続が表示されます。
1. （オプション）階層の上にマウスポインターを置いて、「**詳細**」メニューをクリックし、次のいずれかをクリックします。

   * **編集**：変更を加えることができる **階層を編集** ボックスが開きます。
   * **削除**：階層が完全に削除されます。 削除された階層は復元できません。 接続フィールドは削除されません。





