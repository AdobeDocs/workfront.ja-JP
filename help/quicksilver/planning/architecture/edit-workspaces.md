---
title: ワークスペースを編集
description: 名前の変更など、既存のワークスペースの情報を編集できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 374b6d9c-69a9-4a73-8708-51c14a78c7c9
source-git-commit: e25f6ac3fb4ffc114d59bf5cceecfe718ae914ec
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 30%

---


# ワークスペースの編集

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

Adobe Workfront Planning では、ワークスペースは、チームが作業を計画する一元的な場所です。

ワークスペースは、チームが使用するレコードタイプのコレクションで、チームの作業ライフサイクルを表します。Adobe Workfront Planning では、ワークスペースを完全にカスタマイズできます。

ワークスペースの作成については、[ワークスペースの作成](/help/quicksilver/planning/architecture/create-workspaces.md)を参照してください。

ワークスペースに加えたすべての変更は、そのワークスペースに対して少なくとも表示権限を持つすべてのユーザーに表示されます。

## アクセス要件

+++ 展開すると、アクセス要件が表示されます。

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
   <td>  <p>ワークスペースに対する管理権限 </p>   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> <p>実稼動環境では、システム管理者を含むすべてのユーザーを、Planning を含むレイアウト・テンプレートに割り当てる必要があります。</p>
<p><span class="preview">プレビュー環境では、標準ユーザーとシステム管理者は、デフォルトで計画を有効にしています。</span></p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


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
