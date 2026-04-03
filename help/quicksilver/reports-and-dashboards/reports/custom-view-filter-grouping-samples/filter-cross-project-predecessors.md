---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: フィルター：不完全なプロジェクト間の先行タスクを表示する
description: このタスクフィルターは、不完全なプロジェクト間の先行タスクを返します。
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: 7ee2432c-1d82-454e-a73a-f1f6b6a5c10d
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '199'
ht-degree: 53%

---

# フィルター：不完全なプロジェクト間の先行タスクを表示する

<!--Audited: 10/2024-->

このタスクフィルターは、不完全なプロジェクト間の先行タスクを返します。

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

## プロジェクト間の先行タスクのフィルタリング

このフィルターを適用するには、次の手順に従います。

1. タスクのリストまたはタスクレポートに移動します。
1. **フィルター** ドロップダウンメニューから、**新しいフィルター**&#x200B;を選択します。

1. （条件付き）リストからフィルターにアクセスした場合は&#x200B;**テキストモード**&#x200B;をクリックし、レポートからフィルターにアクセスした場合は&#x200B;**テキストモードに切り替え**&#x200B;をクリックします。
1. 新しい領域に、次のコードを貼り付けます。
   <pre>predecessorsMM:projectID=FIELD:projectID<br>predecessorsMM:projectID_Mod=ne<br>percentComplete=100<br>percentComplete_Mod=ne</pre>

1. （条件付き）レポートからフィルターにアクセスした場合は&#x200B;**フィルターを保存**&#x200B;をクリックし、タスクリストからフィルターにアクセスした場合は&#x200B;**適用**&#x200B;をクリックし、次に&#x200B;**新しいフィルターとして保存**&#x200B;をクリックします。
