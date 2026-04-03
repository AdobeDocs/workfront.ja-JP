---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 表示：担当業務を持つプロジェクトユーザーのリスト
description: このビューをプロジェクトリストまたはレポートに適用して、プロジェクトに関連付けられているユーザーのリストと、プロジェクトで実行する担当業務のリストを表示できます。
author: Courtney
feature: Reports and Dashboards
exl-id: a3f59f69-7f39-4814-bd2f-7734d620081e
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '335'
ht-degree: 78%

---

# 表示：担当業務を持つプロジェクトユーザーのリスト

<!--Audited: 11/2024-->

このビューをプロジェクトリストまたはレポートに適用して、プロジェクトに関連付けられているユーザーのリストと、プロジェクトで実行する担当業務のリストを表示できます。

このレポートの情報は、プロジェクトのユーザーエリアにも表示されます。

>[!TIP]
>
>ユーザーの担当業務がリストされていないが、ユーザープロファイルで担当業務に関連付けられていることがわかっている場合は、ユーザーがタスクやイシューに割り当てられていても、そのタスクやイシューの担当業務に関連付けられていない、またはレポートにリストされているユーザーがタスクやイシューの担当者ではなく、プロジェクトの他の役割を実行している可能性があります（所有者やスポンサーなど）。

![project_with_user_and_role_information_report.png](assets/project-with-user-and-role-information-report-350x100.png)

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
   <p>ビューを変更するコントリビューターまたはリクエスト </p>
   <p>レポートを修正する標準または計画</p>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルター、表示、グループ化へのアクセス権を編集して、表示を変更できるようにします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。


+++


## 担当業務を持つプロジェクトユーザーのリストを表示する

1. プロジェクトのリストに移動します。
1. **表示**&#x200B;ドロップダウンメニューから、**新規表示**&#x200B;を選択します。
1. **列プレビュー**&#x200B;領域で、1列を除くすべての列を削除します。
1. 残りの列のヘッダーをクリックし、**テキストモードに切り替え**/**テキストモードを編集**&#x200B;をクリックします。
1. 「**テキストモードを編集**」ボックスにあるテキストを削除し、次のコードに置き換えます。

   ```
   column.0.link.valueformat=val
   column.0.linkedname=direct
   column.0.listsort=string(name)
   column.0.namekey=name.abbr
   column.0.querysort=name
   column.0.section=0
   column.0.shortview=false
   column.0.stretch=100
   column.0.valuefield=name
   column.0.valueformat=HTML
   column.0.width=200
   column.1.displayname=Project Users
   column.1.listdelimiter=<br>
   column.1.listmethod=nested(projectUsers).lists
   column.1.textmode=true
   column.1.type=iterate
   column.1.valueexpression={user}.{name}
   column.1.valueformat=HTML
   column.2.displayname=Project Roles
   column.2.listdelimiter=<br>
   column.2.listmethod=nested(projectUserRoles).lists
   column.2.textmode=true
   column.2.type=iterate
   column.2.valueexpression={role}.{name}
   column.2.valueformat=HTML
   ```

1. **完了** / **ビューを保存**&#x200B;をクリックします。
