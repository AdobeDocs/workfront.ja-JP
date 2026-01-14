---
title: Workspace階層の作成
description: 作業領域管理者は、Adobe Workfront Planning のレコード・タイプ間に複数の作業領域階層を作成できます。 ワークスペースでレコードタイプを接続し、階層を作成すると、レコードタイプが相互に接続され、1 つのレコードタイプが親として指定され、他の 3 つのレコードタイプが子として設定されます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: 9a7ab1928bfd25c197fca65eddfba1bc01977ea7
workflow-type: tm+mt
source-wordcount: '894'
ht-degree: 5%

---


# ワークスペース階層の作成

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

作業領域管理者は、Adobe Workfront Planning のレコード・タイプ間に複数の作業領域階層を作成できます。

ワークスペース内でレコードタイプを接続したら、それらの接続を整理する階層を作成できます。 階層は、レコードとオブジェクトのタイプを親子関係に整理し、最大 4 つのレベルのオブジェクトのタイプを含めることができます。

2 つのレコードタイプ間の接続がまだ存在しない場合は、階層を設定するときに作成できます。 定義が完了すると、ワークスペース内の関連するレコードタイプ間で階層の構造化パスが確立されます。

階層は、ヘッダーに表示される各レコードのパンくずリストを生成します。 これにより、ワークフローの任意のステージで、階層内の自分の位置を把握できます。

階層とパンくずリストに関する一般的な情報については、[ 階層とパンくずリストの概要 ](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md) を参照してください。

## アクセス要件

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

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## ワークスペース階層の作成

1 つのワークスペースに最大 5 つの階層を作成できます。

{#step1-to-planning}

1. ワークスペースカードをクリックします。
1. ワークスペース名の右側にある **その他** メニュー ![ その他のメニュー ](assets/more-menu.png) をクリックし、**設定** をクリックします。
**階層** セクションは、デフォルトで開きます。
1. **階層** ページの右上隅にある **新規階層** をクリックします。
1. **オブジェクトを追加** をクリックし、ドロップダウンメニューからオブジェクトタイプを選択します。 これが階層内の最初のオブジェクトタイプになります。<!--logged bug to correct to "Add object type"-->

   最初のオブジェクト タイプは、Planning レコード タイプのみです。

   Workfront プロジェクトは、階層内の他のオブジェクトタイプの親として選択できません。

1. 「**オブジェクトを追加**」をクリックして、階層の最初の子である 2 番目のオブジェクトタイプを追加し、ドロップダウンメニューで別のオブジェクトタイプを選択します。
追加された各オブジェクトタイプは、以前のオブジェクトタイプの子になります。

   ![ フィールドが選択されていない新しい階層ボックス ](assets/new-hierarchy-modal-without-connecte-fielf-selected.png)

1. **接続されたフィールドを選択**] をクリックして、2 つのオブジェクトを接続するフィールドを指定します。
1. （条件付き）接続フィールドが複数ある場合は、リストから 1 つ選択します。

   または

   **新しい接続を追加** をクリックして、新しい接続フィールドを追加します。

   これにより、親として使用しているレコードタイプから接続フィールドが作成され、子として使用しているレコードタイプから接続フィールドに対応する接続フィールドが作成されます。

   Workfront プロジェクトへの接続を作成する場合、プロジェクトにフィールドは作成されません。

1. （条件付き）接続されたフィールドがない場合は、「**接続を作成**」をクリックして新しい接続を追加し、「**保存**」をクリックします。

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

      詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。

   1. 「**保存**」をクリックします。

1. （条件付き）接続されたフィールドを作成したときに **リンクされたレコードタイプの対応するフィールドを作成** が選択されなかった場合、エラーが発生し、最初に次の操作を行う必要があります。<!--check back on these steps; this is supposed to be seamless, but now you have to abandon creating a hierarchy to do this-->

   1. **新しい階層** ボックスで **キャンセル** をクリックします。
   1. ワークスペース名の左側にある戻る矢印をクリックし、親として選択するレコードタイプのカードをクリックします。
   1. 上記の手順で選択したレコードタイプのテーブル表示を開き、子として使用するオブジェクトタイプの接続フィールドに移動して、列見出しにカーソルを置いて **編集** フィールドをクリックします。
   1. 「**リンクされたレコードタイプに対応するフィールドを作成**」設定をオンにし、「**保存**」をクリックします。
   1. ワークスペースの **設定** 領域に戻って **新規階層** を再度クリックし、手順に従って階層を作成します。

1. （オプション）上記の手順に従って、最大 4 つのオブジェクトタイプを階層に追加し続けます。 最初にすべてのオブジェクトタイプを追加してから、それらの間に接続フィールドを追加できます。
1. （オプション） **削除** アイコン ![ 削除アイコン ](assets/minus-icon.png) をクリックして、接続を削除します。
1. **保存** をクリックして、階層を保存します。

   >[!TIP]
   >
   >接続されているフィールドがまだない場合は、「**保存**」ボタンはグレー表示になります。

   次のことが発生します。

   * 階層がワークスペースの **階層** セクションに追加されます。
   * レコードのページに移動すると、接続フィールドに入力されるレコードに、パンくずリストのすべての接続が表示されます。

   >[!NOTE]
   >
   >子レコードタイプから 1 つのレコードを、親レコードタイプから最大 10 個のレコードに接続できます。
   >
   >詳しくは、[ 階層とパンくずリストの概要 ](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md) を参照してください。

1. （任意）階層の上にマウスポインターを置き、「**詳細**」メニューをクリックします。

   ![ 階層の詳細メニューが展開されました ](assets/hierarchy-more-menu-expanded.png)

1. 次のいずれかをクリックします。

   * **編集**：変更を加えることができる **階層を編集** ボックスが開きます。
   * **削除**：階層が完全に削除されます。 削除された階層は復元できません。 接続フィールドは削除されません。





