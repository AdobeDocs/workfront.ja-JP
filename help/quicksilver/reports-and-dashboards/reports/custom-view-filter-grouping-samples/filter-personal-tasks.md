---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: フィルター：個人タスク
description: このタスクフィルタは、ユーザーに送信された臨時の作業要求、またはユーザーがホーム領域で追加したTo Doアイテムを返します。 個人タスクはプロジェクトに接続されていませんが、必要に応じてプロジェクトに移動できます。
author: Courtney
feature: Reports and Dashboards
exl-id: 204cfae1-7c57-4223-9e00-ac94e1e2ba3a
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '291'
ht-degree: 23%

---

# フィルター：個人用タスク

<!--Audited: 10/2024-->

このタスクフィルターは、ユーザーに送信された一時的な作業要求、またはユーザーがホーム領域のTo-Doウィジェットで追加したTo-Doアイテムを返します。

臨時の作業要求とTo Doアイテムは、個人のタスクとしてAdobe Workfrontに保存されます。

個人タスクはプロジェクトに接続されていませんが、必要に応じてプロジェクトに移動できます。 詳細については、[個人用タスクの作成](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/create-personal-tasks.md)を参照してください。

![個人用タスクレポート](assets/personal-tasks-report.png)

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
   <p>フィルターの変更をコントリビューターまたはリクエスト </p>
   <p>レポートを変更するための「標準」または「プラン」</p>
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

1. タスクの一覧またはタスクレポートに移動します。
1. **フィルター**&#x200B;ドロップダウンメニューから、**新しいフィルター**&#x200B;をクリックします。
1. （条件付き）レポートからフィルタにアクセスする場合は、**フィルタルールを追加**&#x200B;をクリックします。リストからフィルタにアクセスする場合は、最初のフィールドでフィルタ条件の選択を開始します。
1. （条件付き）次のフィルタ条件を選択します。

   * リストフィルターから： **タスク** > **個人** **真実**
   * レポートフィルターから： **タスク** > **個人** > **等しい（大文字と小文字を区別）** > **真**。
1. フィルターを保存します。

   リストには、どのプロジェクトにも含まれていない個人のタスクのみが表示されます。
