---
title: ワークスペースの編集
description: 名前の変更など、既存のワークスペースの情報を編集できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 374b6d9c-69a9-4a73-8708-51c14a78c7c9
source-git-commit: 5c7b60ac5b78bd065ffc270588ec72ab3eb2f41d
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 53%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# ワークスペースの編集

{{planning-important-intro}}

Adobe Workfront Planning では、ワークスペースは、チームが作業を計画する一元的な場所です。

ワークスペースは、チームが使用するレコードタイプのコレクションで、チームの作業ライフサイクルを表します。Adobe Workfront Planning では、ワークスペースを完全にカスタマイズできます。

ワークスペースの作成については、[ワークスペースの作成](/help/quicksilver/planning/architecture/create-workspaces.md)を参照してください。

ワークスペースに加えたすべての変更は、そのワークスペースに対して少なくとも表示権限を持つすべてのユーザーに表示されます。

## アクセス要件

+++ 展開すると、Workfront Planning のアクセス要件が表示されます。

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
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront 契約</p></td>
   <td>
<p>Workfront Planning の早期アクセス段階に登録されている必要があります </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td>
   <td>
   <p>新規：標準</p>
   <p>現在：プラン</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベルの設定</p></td>
   <td> <p>Workfront Planning に対するアクセスレベルのコントロールはありません</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する管理権限 </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Planning エリアをレイアウトテンプレートに追加する必要があります。詳しくは、<a href="/help/quicksilver/planning/access/access-overview.md">アクセス権の概要</a>を参照してください。 </p>  
</td>
  </tr>

</tbody>
</table>

アクセス要件については、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ワークスペースの編集

{{step1-to-planning}}

1. ワークスペースカードをクリックして、ワークスペースを開きます。
1. 新しいワークスペースのヘッダーでワークスペースの名前内をクリックして名前を変更し、**Enter** キーを押します。
1. ヘッダーのワークスペース名の右 ![](assets/more-menu.png) にある **その他** メニューをクリックし、**編集** をクリックします。

   ![](assets/edit-workspace-box.png)

   「**ワークスペースを編集** ボックスで次の情報を更新します。

   * ワークスペースの名前を追加します。<!--did they add a label for this field?-->
   * **説明**：ワークスペースに関する情報を追加します。
   * ワークスペースに関連付けるアイコンを選択します。

1. 「**保存**」をクリックして「ワークスペースを編集」ボックスを閉じ、変更を適用します。

1. （オプション）新しいワークスペースセクションを追加するには、次のいずれかの操作を行います。

   * ワークスペースの下部にある「**セクションを追加**」をクリックします。
   * セクションの名前にポインタを合わせ、**その他**&#x200B;メニュー ![](assets/more-menu.png) をクリックし、「**上にセクションを追加**」または「**下にセクションを追加**」をクリックします。

1. （オプション）セクションの場所を変更するには、次のいずれかの操作を行います。

   * セクションの名前にポインタを合わせ、**つかむ** アイコン ![](assets/grab-icon.png) をクリックし、適切な場所にドラッグ＆ドロップします。
   * セクションの名前にポインタを合わせ、**その他**&#x200B;メニュー ![](assets/more-menu.png) をクリックし、「**上に移動**」または「**下に移動**」をクリックします。セクションは、ワークスペース内で上下に移動します。

1. （オプション）ワークスペースセクションを削除するには、次の手順を実行します。

   1. セクションの名前にポインタを合わせ、**その他**&#x200B;メニュー ![](assets/more-menu.png) をクリックし、「**削除**」をクリックします。<!--add screen shot when UI is final?-->
   1. 新しいセクションを選択し、すべてのレコードタイプをそのセクションに移動して、「**削除**」をクリックします。<!--check the button name; logged a bug to change it to "Delete" from "Delete section".-->

      すべてのレコードタイプが選択セクションに移動され、セクションが削除されます。

1. （オプション）「**レコードタイプを追加**」をクリックして、ワークスペースにレコードタイプを追加します。

   詳しくは、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

1. （オプション）レコードタイプカードにポインタを合わせ、右上隅にある **詳細** メニュー ![](assets/more-menu.png) ージをクリックしてから、**編集** をクリックして、レコードタイプの外観を変更します。

   詳しくは、[ レコードタイプの編集 ](/help/quicksilver/planning/architecture/edit-record-types.md) を参照してください。

1. （オプション）レコードタイプのカードにポインタを合わせ、右上隅にある **詳細** メニュー ![](assets/more-menu.png) ージをクリックしてから、**削除** をクリックしてレコードタイプを削除します。

   詳しくは、[ レコードタイプの削除 ](/help/quicksilver/planning/architecture/delete-record-types.md) を参照してください。

1. （オプション）レコードタイプカードをクリックしてドラッグし、新しい場所にドロップします。 レコードタイプは、ワークスペースセクション間でドラッグ&amp;ドロップできます。

   ![](assets/drag-and-drop-record-types-in-a-workspace.png)

1. （任意）他のユーザーとワークスペースを共有するには、ワークスペースの右上隅にある「**共有**」をクリックします。

   詳しくは、[ワークスペースの共有](/help/quicksilver/planning/access/share-workspaces.md)を参照してください。
