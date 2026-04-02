---
title: ワークスペースの編集
description: 名前の変更など、既存のワークスペースの情報を編集できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 374b6d9c-69a9-4a73-8708-51c14a78c7c9
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 10d2bcf3f2d349418a8a04e96873bc5c2d3af4a1
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 25%

---


# ワークスペースの編集


<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。すべてのユーザーのプレビュー環境でのみ使用できます。 実稼動環境への毎月のリリース後、高速リリースを有効にしたお客様は、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>


{{planning-important-intro}}

Adobe Workfront Planning では、ワークスペースは、チームが作業を計画する一元的な場所です。

ワークスペースは、チームが使用するレコードタイプのコレクションで、チームの作業ライフサイクルを表します。Adobe Workfront Planning では、ワークスペースを完全にカスタマイズできます。

ワークスペースの作成については、[ワークスペースの作成](/help/quicksilver/planning/architecture/create-workspaces.md)を参照してください。

ワークスペースに加えたすべての変更は、少なくともワークスペースに対する表示権限を持っているすべてのユーザーに対して表示されます。

ワークスペースは、次の方法で編集できます。

* 手作業で。

  この記事では、ワークスペースを手動で編集する方法について説明します。

* AIを活用したPlanning Designerを使用します。 この機能は、現在、限定的なBeta プログラムでのみ使用できます。

  詳しくは、「[Adobe Workfront計画Designerの基本を学ぶ](/help/quicksilver/planning/general/planning-ai-designer.md)」を参照してください。

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
<li><p>任意のWorkfrontおよびプランニングパッケージ</p></li>
または
<li><p>任意のワークフローとプランニングパッケージ</p></li></ul>
<p>各Workfront計画パッケージに含まれる内容について詳しくは、Workfrontの担当者にお問い合わせください。 </p> 
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

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメント &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++   

<!--
Old:
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
</table>
-->

## ワークスペースの編集

{{step1-to-planning}}

1. （条件付き）Workfront管理者の場合は、次のいずれかをクリックします。

   * **作成したワークスペースにアクセスするための**&#x200B;のワークスペース
   * **自分または自分が作成したワークスペースで共有されているワークスペースにアクセスするためのワークスペース**&#x200B;すべて

1. （オプション）「**すべてを表示**」をクリックして、追加のワークスペースを表示します。 **すべてを表示** リンクは、2行以上のワークスペースカードがある場合にのみ表示されます。
1. （オプション）「**表示回数**」をクリックして、画面に表示されるワークスペースの数を制限します。
1. ワークスペースを編集するには、次のいずれかの操作を行います。

   * ワークスペースカードにカーソルを合わせ、カードの右上隅にある&#x200B;**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックします
または
   * ワークスペースページの右上隅にある&#x200B;**検索** アイコン ![検索アイコン &#x200B;](assets/search-icon.png)をクリックして、ワークスペースを名前で検索し、ワークスペースカードをクリックしてワークスペースを開き、ワークスペース名の右側にある&#x200B;**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックします。

   >[!TIP]
   >
   ><span class="preview">次のキーボードの組み合わせを使用して、任意のWorkfront Planning ページからグローバル検索ボックスを開き、ワークスペースを検索できます：</span>
   >
   >* Windows<span class="preview">の</span>CTRL+K
   >* Mac<span class="preview">⌘の</span>+K
   >
   >![&#x200B; グローバル検索ボックス &#x200B;](assets/global-search-box.png)

1. 「**編集**」をクリックします。

   「**ワークスペースを編集**」ボックスが表示されます。

   ![&#x200B; ワークスペース ボックスを編集](assets/edit-workspace-box.png)

1. 「**ワークスペースを編集**」ボックスで、次の情報を更新します。

   * ワークスペースの名前を追加します。<!--did they add a label for this field?-->
   * **説明**: ワークスペースに関する情報を追加します。
   * ワークスペースに関連付けるアイコンを選択します。

1. 「**保存**」をクリックして「ワークスペースを編集」ボックスを閉じ、変更を適用します。

1. （オプション）新しいワークスペースセクションを追加するには、次のいずれかの操作を行います。

   * ワークスペースの下部にある「**セクションを追加**」をクリックします。
   * セクション名にカーソルを合わせ、**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックし、**上のセクションを追加**&#x200B;または&#x200B;**下のセクションを追加**&#x200B;をクリックします。

1. （オプション）セクションの場所を変更するには、次のいずれかの操作を行います。

   * セクション名にカーソルを合わせて&#x200B;**グラブ** アイコン ![&#x200B; グラブアイコン &#x200B;](assets/grab-icon.png)をクリックし、右側の場所にドラッグ&amp;ドロップします。
   * セクション名にカーソルを合わせ、**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックし、**上に移動**&#x200B;または&#x200B;**下に移動**&#x200B;をクリックします。 セクションは、ワークスペース内で上下に移動します。

1. （オプション）ワークスペースセクションを削除するには、次の操作を行います。

   1. セクションの名前にカーソルを合わせ、**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックし、**削除**&#x200B;をクリックします。<!--add screen shot when UI is final?-->
   1. 新しいセクションを選択し、すべてのレコードタイプをそのセクションに移動して、「**削除**」をクリックします。<!--check the button name; logged a bug to change it to "Delete" from "Delete section".-->

      すべてのレコードタイプが選択セクションに移動され、セクションが削除されます。

1. （オプション）「**レコードタイプを追加**」をクリックして、ワークスペースにレコードタイプを追加します。

   詳しくは、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

1. （オプション）レコードタイプカードにカーソルを合わせ、右上隅の&#x200B;**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックし、**編集**&#x200B;をクリックしてレコードタイプの外観を変更します。

   詳しくは、[&#x200B; レコードタイプの編集](/help/quicksilver/planning/architecture/edit-record-types.md)を参照してください。

1. （オプション）レコードタイプカードにカーソルを合わせ、右上隅の&#x200B;**詳細** メニュー![詳細メニュー](assets/more-menu.png)をクリックし、**削除**&#x200B;をクリックしてレコードタイプを削除します。

   詳しくは、[&#x200B; レコードタイプの削除](/help/quicksilver/planning/architecture/delete-record-types.md)を参照してください。

1. （オプション）レコードタイプのカードを押しながらクリックしてドラッグし、新しい場所にドロップします。 レコードタイプをワークスペースセクションから別のセクションにドラッグ&amp;ドロップできます。

   ![&#x200B; ワークスペースにレコードタイプをドラッグ&amp;ドロップ &#x200B;](assets/drag-and-drop-record-types-in-a-workspace.png)

1. （オプション）ワークスペースの右上隅にある「**共有**」をクリックして、ワークスペースを他のユーザーと共有します。

   詳しくは、[ワークスペースの共有](/help/quicksilver/planning/access/share-workspaces.md)を参照してください。
