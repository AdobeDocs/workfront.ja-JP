---
title: ワークスペースの編集
description: 名前の変更など、既存のワークスペースの情報を編集できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 374b6d9c-69a9-4a73-8708-51c14a78c7c9
source-git-commit: 8a4da96562b18977f56567f0fc5f72b369078432
workflow-type: tm+mt
source-wordcount: '551'
ht-degree: 55%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# ワークスペースの編集

{{planning-important-intro}}

Adobe Workfront Planning では、ワークスペースは、チームが作業を計画する一元的な場所です。

ワークスペースは、チームが使用するレコードタイプのコレクションで、チームの作業ライフサイクルを表します。Adobe Workfront Planning では、ワークスペースを完全にカスタマイズできます。

ワークスペースの作成については、[ワークスペースの作成](/help/quicksilver/planning/architecture/create-workspaces.md)を参照してください。

ワークスペースに加えたすべての変更は、そのワークスペースに対して少なくとも表示権限を持つすべてのユーザーに表示されます。

## アクセス要件

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


## ワークスペースの編集

{{step1-to-planning}}

1. ワークスペースカードをクリックして、ワークスペースを開きます。
1. 新しいワークスペースのヘッダーでワークスペースの名前内をクリックして名前を変更し、を押します **Enter**.
1. 「」をクリックします **詳細** メニュー ![](assets/more-menu.png) ヘッダーのワークスペース名の右側にある「」をクリックします。 **編集**.

   ![](assets/edit-workspace-box.png)

   次の情報を更新： **ワークスペースを編集** ボックス：

   * ワークスペースの名前を追加します。 <!--did they add a label for this field?-->
   * **説明**：ワークスペースに関する情報を追加します。
   * ワークスペースに関連付けるアイコンを選択します。

1. クリック **保存** をクリックして「ワークスペースを編集」ボックスを閉じ、変更を適用します。

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

1. （任意）レコードタイプのカードの上にマウスポインターを置き、 **詳細** メニュー ![](assets/more-menu.png) 右上隅のをクリックします。 **編集** レコードタイプの外観を変更する

   詳しくは、を参照してください [レコードタイプを編集](/help/quicksilver/planning/architecture/edit-record-types.md).

1. （任意）レコードタイプのカードの上にマウスポインターを置き、 **詳細** メニュー ![](assets/more-menu.png) 右上隅のをクリックします。 **削除** をクリックしてレコードタイプを削除します。

   詳しくは、を参照してください [レコードタイプを削除](/help/quicksilver/planning/architecture/delete-record-types.md).

1. （オプション）レコードタイプカードをクリックしてドラッグし、新しい場所にドロップします。 レコードタイプは、ワークスペースセクション間でドラッグ&amp;ドロップできます。

   ![](assets/drag-and-drop-record-types-in-a-workspace.png)

1. （任意）クリック **共有** をクリックし、他のユーザーとワークスペースを共有します。

   詳しくは、[ワークスペースの共有](/help/quicksilver/planning/access/share-workspaces.md)を参照してください。
