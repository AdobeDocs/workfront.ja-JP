---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: フィルター：不完全なプロジェクト間の先行タスクの表示
description: このタスクフィルターは、不完全なプロジェクト間の先行タスクを返します。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7ee2432c-1d82-454e-a73a-f1f6b6a5c10d
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '213'
ht-degree: 52%

---

# フィルター：不完全なプロジェクト間の先行タスクを表示する

<!--Audited: 10/2024-->

このタスクフィルターは、不完全なプロジェクト間の先行タスクを返します。

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

## プロジェクト間の先行タスクのフィルタリング

このフィルターを適用するには、次の手順に従います。

1. タスクの一覧またはタスク報告書に移動します。
1. **フィルター** ドロップダウンメニューから「**新しいフィルター**」を選択します。

1. （条件付き）リストからフィルターにアクセスした場合は **テキストモード** をクリックし、レポートからフィルターにアクセスした場合は **テキストモードに切り替え** をクリックします。
1. 新しい領域に、次のコードを貼り付けます。
   <pre>predecessorsMM:projectID=FIELD:projectID<br>predecessorsMM:projectID_Mod=ne<br>percentComplete=100<br>percentComplete_Mod=ne</pre>

1. （条件付き）レポートからフィルターにアクセスした場合は **[ フィルターの保存 ]**、タスク リストからフィルターにアクセスした場合は **[ 適用 ]**、**[ 新規として保存** をクリックします。
