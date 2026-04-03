---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Personal Tasks'
description: このタスクフィルターは、ユーザーに送信されたアドホック作業リクエスト、またはユーザーがホームエリアに追加したTo Do アイテムを返します。 個人タスクはプロジェクトに関連付けられていませんが、必要に応じてプロジェクトに移動できます。
author: Courtney
feature: Reports and Dashboards
exl-id: 204cfae1-7c57-4223-9e00-ac94e1e2ba3a
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 23%

---

# フィルター：個人用タスク

<!--Audited: 10/2024-->

このタスクフィルターは、ユーザーに送信されたアドホック作業リクエスト、またはユーザーがホームエリアのTo-Do ウィジェットに追加したTo-Do アイテムを返します。

アドホック作業リクエストとToDo アイテムは、Adobe Workfrontに個人タスクとして保存されます。

個人タスクはプロジェクトに関連付けられていませんが、必要に応じてプロジェクトに移動できます。 詳しくは、[個人用タスクの作成](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md)を参照してください。

![個人タスクレポート ](assets/personal-tasks-report.png)

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

## 個人タスクのフィルタリング

このフィルターを作成するには：

1. タスクのリストまたはタスクレポートに移動します。
1. **フィルター** ドロップダウンメニューから、**新規フィルター**&#x200B;をクリックします。
1. （条件付き）リストからフィルターにアクセスする場合は、**フィルター規則**&#x200B;をクリックするか、最初のフィールドでフィルター条件の選択を開始します。
1. （条件付き）次のフィルタリング条件を選択します。

   * リスト フィルターから：**タスク** > **個人** **はtrue**
   * レポートフィルターから：**タスク** > **個人** > **等しい（大文字と小文字を区別）** > **True**。
1. フィルターを保存します。

   このリストには、どのプロジェクトにもない個人タスクのみが表示されます。
