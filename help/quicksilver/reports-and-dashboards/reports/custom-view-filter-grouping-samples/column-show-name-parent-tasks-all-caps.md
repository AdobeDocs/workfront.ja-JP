---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: ビュー：親タスクの名前をすべての大文字で表示
description: この列をタスクビューに追加すると、親タスクの名前をすべて大文字で表示できます。
author: Courtney
feature: Reports and Dashboards
exl-id: bb489920-6b17-4689-b432-b0c28bcb5d10
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 69%

---

# ビュー：親タスクの名前をすべて大文字で表示

<!--Audited: 10/2024-->

この列をタスクビューに追加すると、親タスクの名前をすべて大文字で表示できます。

![すべての大文字の親タスクを含む列](assets/column-task-with-all-caps-parent-350x112.png)

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>コントリビューターまたはフィルターを変更するリクエスト </p>
   <p>レポートを修正する標準または計画</p>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルターを変更する場合は、フィルター、ビュー、グループ化への編集アクセス権</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 親タスクの名前をすべて大文字で表示する

タスクビューでこの列を作成するには、以下のように行います。

1. タスクのリストに移動します。
1. **表示** ドロップダウンメニューからビューを選択し、**編集** アイコン ![編集アイコン &#x200B;](assets/edit-icon.png)をクリックします。
または\
   **ビュー**&#x200B;ドロップダウンメニューから、**新規ビュー**&#x200B;を選択します。

1. **列プレビュー**&#x200B;領域で、リストにタスク名を表示する列のヘッダーをクリックします。
1. 「**テキストモードに切り替え**」をクリックし、「**テキストモードを編集**」をクリックします。
1. 「**テキストモード**」ボックスにあるテキストを削除し、次のコードに置き換えます。

   ```
   linkedname=direct
   namekey=name
   querysort=name
   styledef.case.0.comparison.icon=false
   styledef.case.0.comparison.leftmethod=numberOfChildren
   styledef.case.0.comparison.lefttext=numberOfChildren
   styledef.case.0.comparison.operator=gt
   styledef.case.0.comparison.operatortype=int
   styledef.case.0.comparison.righttext=0
   styledef.case.0.comparison.trueproperty.0.name=fontstyle
   styledef.case.0.comparison.trueproperty.0.value=bold
   valueexpression=IF({numberOfChildren}>"0",UPPER({name}),{name})
   valueformat=HTML
   ```

1. 「**完了**」をクリックし、「**ビューを保存**」をクリックします。
