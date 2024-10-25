---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'フィルター：個人用タスク'
description: このタスクフィルターは、ユーザーに送信されたアドホックな作業要求、またはユーザーがホームエリアで追加した To Do アイテムを返します。 個人のタスクはプロジェクトに接続されていませんが、必要に応じてプロジェクトに移動できます。
author: Nolan
feature: Reports and Dashboards
source-git-commit: 1e69d715f343bfef1e5aee658a1dff12abfc61a0
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 23%

---

# フィルター：個人用タスク

<!--Audited: 10/2024-->

このタスクフィルターは、ユーザーに送信されたアドホックな作業要求、またはユーザーがホームエリアで追加した To Do アイテムを返します。

アドホックな作業要求および To Do アイテムは、個人のタスクとしてAdobe Workfrontに保存されます。

個人のタスクはプロジェクトに接続されていませんが、必要に応じてプロジェクトに移動できます。

![](assets/personal-tasks-report.png)

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

## 個人タスクのフィルター

このフィルターを作成するには：

1. タスクの一覧またはタスク報告書に移動します。
1. **フィルター** ドロップダウンメニューから、「**新しいフィルター**」をクリックします。
1. （条件付き）レポートからフィルターにアクセスする場合は **フィルタールールを追加** をクリックし、リストからフィルターにアクセスする場合は最初のフィールドでフィルター条件の選択を開始します。
1. （条件付き）次のフィルター条件を選択します。

   * リストフィルターから：**タスク**/**個人****True**
   * レポートフィルターから：**タスク**/**個人**/**次に等しい**/**True**
1. フィルターを保存します。

   リストには、どのプロジェクトにも含まれていない個人用タスクのみが表示されます。
