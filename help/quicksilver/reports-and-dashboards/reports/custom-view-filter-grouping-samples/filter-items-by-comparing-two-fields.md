---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: フィルター：2 つのフィールドを比較して、リスト内の項目を除外する
description: 2 つのフィールドを比較することで、リストから項目をフィルタリングできます。例えば、タスクの実際の完了日が予定完了日よりも後のタスクのみを表示できます。
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '233'
ht-degree: 78%

---

# フィルター：2 つのフィールドを比較して、リスト内の項目を除外する

<!--Audited: 10/2024-->

2 つのフィールドを比較することで、リストから項目をフィルタリングできます。例えば、タスクの実際の完了日が予定完了日よりも後のタスクのみを表示できます。

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

## 2 つのフィールドの比較による項目のフィルタリング

1. タスクのリストに移動します。
1. **フィルター** ドロップダウンメニューから、**新しいフィルター**&#x200B;を選択します。

1. **タスク :Actual完了日** > **より大きい日** > **日付を選択**&#x200B;するためのフィルターを追加します。

   >[!TIP]
   >
   >選択したフィールドに使用するフィルター修飾子を選択します（使用可能な場合）。

1. **テキストモード**&#x200B;をクリックします。
1. 表示される領域に、次のコードを追加します。

   ```
   actualCompletionDate=FIELD:plannedCompletionDate
   actualCompletionDate_Mod=gt
   ```

1. **適用** / **新規として保存**&#x200B;をクリックします。
