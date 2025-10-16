---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: フィルター：個人タスク
description: このタスクフィルターは、ユーザーに送信されたアドホックな作業要求、またはユーザーがホームエリアで追加した To Do アイテムを返します。 個人のタスクはプロジェクトに接続されていませんが、必要に応じてプロジェクトに移動できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 204cfae1-7c57-4223-9e00-ac94e1e2ba3a
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 17%

---

# フィルター：個人用タスク

<!--Audited: 10/2024-->

このタスクフィルターは、ユーザーに送信されたアドホックな作業要求、またはユーザーがホーム領域の To Do ウィジェットに追加した To Do アイテムを返します。

アドホックな作業要求および To Do アイテムは、個人のタスクとしてAdobe Workfrontに保存されます。

個人のタスクはプロジェクトに接続されていませんが、必要に応じてプロジェクトに移動できます。 詳しくは、[&#x200B; 個人タスクの作成 &#x200B;](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md) を参照してください。

![&#x200B; 個人タスクレポート &#x200B;](assets/personal-tasks-report.png)

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

## 個人タスクのフィルター

このフィルターを作成するには：

1. タスクの一覧またはタスク報告書に移動します。
1. **フィルター** ドロップダウンメニューから、「**新しいフィルター**」をクリックします。
1. （条件付き）レポートからフィルターにアクセスする場合は **フィルタールールを追加** をクリックし、リストからフィルターにアクセスする場合は最初のフィールドでフィルター条件の選択を開始します。
1. （条件付き）次のフィルター条件を選択します。

   * リストフィルターから：**タスク**/**個人**&#x200B;**True**
   * レポートフィルターから：**タスク**/**個人**/**次と等しい（大文字と小文字を区別）**/**True**。
1. フィルターを保存します。

   リストには、どのプロジェクトにも含まれていない個人用タスクのみが表示されます。
