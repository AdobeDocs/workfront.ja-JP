---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: グループ化：タスク リストのプロジェクト スポンサー
description: このタスクグループ化によって、プロジェクトスポンサー別にタスクをグループ化できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 2d8f85ea-492e-4b08-82f5-726170acc7d5
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '191'
ht-degree: 69%

---

# グループ化：タスクリストのプロジェクトスポンサー

<!--Audited: 11/2024-->

このタスクグループ化によって、プロジェクトスポンサー別にタスクをグループ化できます。

![ プロジェクトスポンサーによるグループ化 ](assets/grouping--project-sponsor-for-a-task-350x189.png)

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

## タスクリストのプロジェクトスポンサー別のグループ化


このグループ化を適用するには、次の操作を行います。

1. タスクのリストに移動します。
1. **グループ化**&#x200B;ドロップダウンメニューで「**新規グループ化**」を選択します。

1. 「**テキスト モードに切り替える**」をクリックします。
1. 表示される領域のテキストを削除し、以下のコードに置き換えます。

   ```
   group.0.name=Project Sponsor
   group.0.valuefield=project:sponsor:name
   group.0.valueformat=string
   ```

1. 「**完了**」をクリックします。
1. グループ化名を更新し、「**グループ化を保存**」をクリックします。

