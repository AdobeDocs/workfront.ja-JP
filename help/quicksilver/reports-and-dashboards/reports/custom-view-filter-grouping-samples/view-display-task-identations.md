---
content-type: reference
product-area: reporting;projects;portfolios;programs
navigation-topic: custom-view-filter-and-grouping-samples
title: 表示：タスク リスト内のタスク インデントを表示します
description: このタスクビューでは、タスク名列にコードを追加して、プロジェクトの作業分割構造に従ってインデントされたタスクを表示できます。
author: Nolan
feature: Reports and Dashboards
exl-id: f7f43e1e-db32-48b8-9a23-ff9fa6195386
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '241'
ht-degree: 63%

---

# ビュー：タスクリストでのタスクのインデントの表示

<!--Audited: 11/2024-->

このタスクビューでは、タスク名列にコードを追加して、プロジェクトの作業分割構造に従ってインデントされたタスクを表示できます。

![&#x200B; タスクのインデントの表示 &#x200B;](assets/view-text-mode-indentation-task-list-350x171.png)

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

## タスクリストの列にタスクのインデントを表示する

1. タスクのリストに移動します。
1. **表示**&#x200B;ドロップダウンメニューで、「**新規ビュー**」をクリックします。

1. **列を追加** をクリックし、「この列に表示 **フィールドに「タスク名」と入力し始め、リストに表示されたら選択します。**

1. 新しい列から、**テキストモードに切り替え** > **テキストモードを編集** をクリックします。
1. `valuefield=` 行にあるテキストを削除し、次のコードに置き換えます。

   ```
   displayname=Task hierarchy
   valueexpression=IF({indent}<1,{name},IF({indent}<2,CONCAT(' - ',{name}),IF({indent}<3,CONCAT(' - - ',{name}),IF({indent}<4,CONCAT(' - - - ',{name}),CONCAT(' - - - - ',{name})))))
   ```

1. 「**完了**」をクリックし、「**ビューを保存** をクリックします。
1. （オプション）ビュー名を更新し、「**ビューを保存**」をクリックします。
