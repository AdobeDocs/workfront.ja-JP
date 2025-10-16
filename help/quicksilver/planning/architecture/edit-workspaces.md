---
title: ワークスペースを編集
description: 名前の変更など、既存のワークスペースの情報を編集できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 374b6d9c-69a9-4a73-8708-51c14a78c7c9
source-git-commit: 8546311acf722c0f4d47d4663b02ff701416894a
workflow-type: tm+mt
source-wordcount: '645'
ht-degree: 27%

---


# ワークスペースの編集

<!--<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Adobe Workfront Planning では、ワークスペースは、チームが作業を計画する一元的な場所です。

ワークスペースは、チームが使用するレコードタイプのコレクションで、チームの作業ライフサイクルを表します。Adobe Workfront Planning では、ワークスペースを完全にカスタマイズできます。

ワークスペースの作成については、[ワークスペースの作成](/help/quicksilver/planning/architecture/create-workspaces.md)を参照してください。

ワークスペースに加えたすべての変更は、そのワークスペースに対して少なくとも表示権限を持つすべてのユーザーに表示されます。

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
<p>または</p>
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
   <td>  <p>Manage permissions to the workspace </p>   </td> 
  </tr> 
</tbody> 
</table> -->


## ワークスペースの編集

{{step1-to-planning}}

1. （条件付き）Workfront管理者の場合は、「**自分が参加しているワークスペース** **」をクリックして作成したワークスペースにアクセスしたり、「その他のワークスペース** をクリックして自分と共有されている他のワークスペースにアクセスしたりします。

<!--***********Replace the steps from the next below till the "Update the following information in the Edit workspace box:" (but keep this last step)*******-->

1. （任意）「**すべて表示**」をクリックして、追加のワークスペースを表示します。 **すべてを表示** リンクは、ワークスペースカードが 3 行を超える場合にのみ表示されます。
1. （任意） ClicK **表示を減らす** を使用して、画面に表示するワークスペースの数を制限します。
1. ワークスペースを編集するには、次のいずれかの操作を行います。

   * ワークスペースカードにポインタを合わせ、カードの右上隅にある **その他** メニュー ![ その他のメニュー ](assets/more-menu.png) をクリックします
または
   * ワークスペースカードをクリックしてワークスペースを開き、ワークスペース名の右側にある **その他** メニュー ![ その他のメニュー ](assets/more-menu.png) をクリックします。
1. 「**編集**」をクリックします。

   **ワークスペースを編集** ボックスが表示されます。

   ![ ワークスペースを編集ボックス ](assets/edit-workspace-box.png)

1. 「**ワークスペースを編集** ボックスで次の情報を更新します。

   * ワークスペースの名前を追加します。<!--did they add a label for this field?-->
   * **説明**：ワークスペースに関する情報を追加します。
   * ワークスペースに関連付けるアイコンを選択します。

1. 「**保存**」をクリックして「ワークスペースを編集」ボックスを閉じ、変更を適用します。

1. （オプション）新しいワークスペースセクションを追加するには、次のいずれかの操作を行います。

   * ワークスペースの下部にある「**セクションを追加**」をクリックします。
   * セクション名にポインタを合わせて、「**詳細**」メニュー ![ 詳細メニュー ](assets/more-menu.png) をクリックし、「**上にセクションを追加**」または「**下にセクションを追加**」をクリックします。

1. （オプション）セクションの場所を変更するには、次のいずれかの操作を行います。

   * セクション名にカーソルを合わせて **グラブ** アイコン ![ グラブアイコン ](assets/grab-icon.png) をクリックし、適切な場所にドラッグ&amp;ドロップします。
   * セクションの名前にポインタを合わせて、**その他** メニュー ![ その他のメニュー ](assets/more-menu.png) をクリックし、**上へ移動** または **下へ移動** をクリックします。 セクションは、ワークスペース内で上下に移動します。

1. （オプション）ワークスペースセクションを削除するには、次の手順を実行します。

   1. セクションの名前にポインタを合わせて、**その他** メニュー ![[ その他 ] メニュー ](assets/more-menu.png) をクリックしてから、**削除** をクリックしてください。<!--add screen shot when UI is final?-->
   1. 新しいセクションを選択し、すべてのレコードタイプをそのセクションに移動して、「**削除**」をクリックします。<!--check the button name; logged a bug to change it to "Delete" from "Delete section".-->

      すべてのレコードタイプが選択セクションに移動され、セクションが削除されます。

1. （オプション）「**レコードタイプを追加**」をクリックして、ワークスペースにレコードタイプを追加します。

   詳しくは、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

1. （オプション）レコードタイプのカードにポインタを合わせ、右上隅にある **その他** メニュー ![ その他のメニュー ](assets/more-menu.png) をクリックしてから、**編集** をクリックして、レコードタイプの外観を変更します。

   詳しくは、[ レコードタイプの編集 ](/help/quicksilver/planning/architecture/edit-record-types.md) を参照してください。

1. （オプション）レコードタイプのカードにポインタを合わせ、右上隅にある **詳細** メニュー ![ 詳細メニュー ](assets/more-menu.png) をクリックしてから、**削除** をクリックしてレコードタイプを削除します。

   詳しくは、[ レコードタイプの削除 ](/help/quicksilver/planning/architecture/delete-record-types.md) を参照してください。

1. （オプション）レコードタイプカードをクリックしてドラッグし、新しい場所にドロップします。 レコードタイプは、ワークスペースセクション間でドラッグ&amp;ドロップできます。

   ![ レコードタイプのワークスペースへのドラッグ&amp;ドロップ ](assets/drag-and-drop-record-types-in-a-workspace.png)

1. （任意）他のユーザーとワークスペースを共有するには、ワークスペースの右上隅にある「**共有**」をクリックします。

   詳しくは、[ワークスペースの共有](/help/quicksilver/planning/access/share-workspaces.md)を参照してください。
