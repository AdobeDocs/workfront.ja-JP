---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 表示：列にタスクの後続タスクのリストを追加
description: タスクビューに列を追加して、後続タスクのリストを表示できます。後続タスクの列には、後続タスクの番号と名前が含まれます。
author: Nolan
feature: Reports and Dashboards
exl-id: 45e9cb13-99c7-4401-962e-2aea5e5258c0
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 64%

---

# ビュー：後続タスクのリストを列に追加

<!--Audited: 11/2024-->

タスクビューに列を追加して、後続タスクのリストを表示できます。**後続タスク**&#x200B;の列には、後続の番号と名前が含まれます。

![task_view_with_a_list_of_successors_.png](assets/task-view-with-a-list-of-successors--350x118.png)

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
   <p>フィルターの変更者または変更依頼 </p>
   <p>レポートを変更するための標準またはプラン</p>
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


## 後続タスクのリストを列に追加

この列をタスクビューに追加するには、次の手順に従います。

1. タスクリストに移動します。
1. **ビュー** ドロップダウンメニューを展開し、「**新規ビュー**」をクリックします。
1. 「**列を追加**」をクリックします。
1. **テキストモードに切り替え** をクリックしてから、**テキストモードを編集** をクリックします。
1. 「**テキストモードを編集**」ボックスのすべてのテキストを削除し、次のコードに置き換えます。

   ```
   displayname=Task Successors
   listdelimiter=
   listmethod=nested(successors).lists
   textmode=true
   type=iterate
   valueexpression=CONCAT({successor}.{taskNumber},' - ',{successor}.{name})
   valueformat=HTML
   ```

1. 「**完了**」をクリックし、「**ビューを保存** をクリックします。
