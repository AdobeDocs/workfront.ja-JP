---
navigation-topic: get-started-with-workfront
title: 「優先順位」ワークリスト列のカスタマイズ
description: 作業方法をサポートするために、「優先順位」でワークリストの列をカスタマイズできます。
author: Courtney
feature: Get Started with Workfront
recommendations: noDisplay, noCatalog
exl-id: e4232fbe-1b5c-4614-8613-3b0e25ffee46
TQID: https://experienceleague.adobe.com/YIqeZbiTZH00yXJ6LnQrpEZuHvW4Y5QZVkYU3OquWqE
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 37be1f25fa54f3efd4113478496e95db3c8bce1c
workflow-type: tm+mt
source-wordcount: 437
ht-degree: 14%

---

# 「優先順位」ワークリスト列のカスタマイズ

{{preview-fast-release-general}}

<!--I think this article can point to the Enhanced lists article for managing the view-->

<!--
<span class="preview">The information highlighted on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->


作業方法をサポートするために、「優先順位」でワークリストの列をカスタマイズできます。

「優先度」には、割り当てられた作業項目が表示されます。 チームに割り当てられた作業項目を表示できません。

<!--
>[!NOTE]
>
>You cannot add custom data to columns at this time.
-->

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront パッケージ</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン</strong></td> 
   <td> 
   <p>レビュアー以上</p>
   <p>明るいまたはそれ以上</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>更新先のオブジェクトに対する表示または編集アクセス権</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>オブジェクトに対する表示アクセス権</p></td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 「優先順位」ワークリスト列のカスタマイズ

### 列を有効または無効にする

{{step1-to-priorities}}

1. 画面の左側にある&#x200B;**列**&#x200B;をクリックします。

   <span class="preview"> プレビュー環境のサンプル画像：</span>
   ![列](assets/columns-new-060226.png)

   実稼動環境のサンプル画像：
   ![列](assets/columns-new.png)

1. 切り替えスイッチを使用して、ワークリストの列を表示または非表示にします。

### 列の並べ替え

{{step1-to-priorities}}

1. 画面の左側にある&#x200B;**列**&#x200B;をクリックします。
1. **ドラッグ** アイコンをクリックし、列を目的の場所に移動します。移動列は、ワークリスト内で自動的に更新されます。
   ![列を並べ替え](assets/reorder-columns-new.png)

>[!NOTE]
>
>「名前」列は固定されており、移動できません。

<div class="preview">

### 列マネージャーを使用した列の追加と削除

{{step1-to-priorities}}

1. リストの右上隅にある「+」アイコンをクリックして、**列マネージャー** ボックスを開きます。
1. 列を追加または削除してから、**保存**&#x200B;をクリックします。

   >[!NOTE]
   >
   >リスト表示に追加できるのは、既存のフィールドのみです。 タスクとイシューのネイティブフィールドとカスタムフィールドの両方を列として追加できます。

列マネージャーについて詳しくは、記事[拡張リストを使用](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)の「[列マネージャー](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#add-and-remove-columns-with-the-column-manager)で列を追加および削除する」を参照してください。

</div>

### 優先順位リストの行の高さを変更する

{{step1-to-priorities}}

1. **行の高さ** アイコンをクリックします。

   これにより、行の垂直方向の長さが更新されます。 次のオプションから選択します。

   * 低い
   * 標準： これはデフォルトの選択肢です。
   * 中
   * 高い

   リストはすぐに更新されます。

<div class="preview">

## 優先順位リストのビューの管理

ビューでは、プリセット設定を使用して、リスト内の列、フィルター、グループ化を定義します。

デフォルトのビューが優先順位リストに割り当てられます。 また、独自のビューを作成して共有することもできます。

{{step1-to-priorities}}

1. リストの左上隅にあるドロップダウンビューメニューを展開して別のビューを選択するか、**新しいビュー**&#x200B;をクリックして別のビューを作成します。
1. ビューに含める列、フィルター、グループを更新します。

   ビューの変更は自動的に保存されます。 このビューを次回に適用しても、列とフィルターの設定は設定した方法のまま維持されます。

ビューについて詳しくは、記事[強化リストを使用](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)の記事[強化リスト要素の更新](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md#update-enhanced-list-elements)を参照してください。

</div>
