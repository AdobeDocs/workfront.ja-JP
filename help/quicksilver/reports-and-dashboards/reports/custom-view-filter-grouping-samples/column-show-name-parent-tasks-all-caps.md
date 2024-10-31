---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「表示：親タスクの名前をすべて大文字で表示」
description: この列をタスクビューに追加すると、親タスクの名前をすべて大文字で表示できます。
author: Nolan
feature: Reports and Dashboards
exl-id: bb489920-6b17-4689-b432-b0c28bcb5d10
source-git-commit: a7cdee912e5047f1c8ef224aff6a41eaa3633df6
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 69%

---

# ビュー：親タスクの名前をすべて大文字で表示

<!--Audited: 10/2024-->

この列をタスクビューに追加すると、親タスクの名前をすべて大文字で表示できます。

![](assets/column-task-with-all-caps-parent-350x112.png)

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> 
    <p>新規：</p>
   <ul><li><p>フィルターを変更するコントリビューター </p></li>
   <li><p>レポートを変更する場合は Standard</p></li> </ul>

<p>現在：</p>
   <ul><li><p>フィルターを変更する場合は「要求」 </p></li>
   <li><p>レポートを変更するためのプラン</p></li> </ul></td> 
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

*詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## 親タスクの名前をすべて大文字で表示する

タスクビューでこの列を作成するには、以下のように行います。

1. タスクのリストに移動します。
1. 「**表示**」ドロップダウンメニューからビューを選択し、「**編集**」アイコンをクリックします ![](assets/edit-icon.png)
または\
   **ビュー**&#x200B;ドロップダウンメニューから、**新規ビュー**&#x200B;を選択します。

1. **列プレビュー** 領域で、リスト内のタスク名を示す列のヘッダーをクリックします。
1. 「**テキストモードに切り替え**」をクリックしてから、「**テキストモードを編集**」をクリックします。
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
