---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: ダッシュボードからの外部ページを削除
description: 不要になった外部ページは、ダッシュボードから削除できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 9e400b8a-bbb8-4d1f-b419-d4a4518c0b2e
source-git-commit: c8b7ad473b0c2120ef5ea52374b3501ad6f553f1
workflow-type: tm+mt
source-wordcount: '250'
ht-degree: 77%

---

# ダッシュボードからの外部ページを削除

<!-- Audited: 1/2025 -->

不要になった外部ページは、ダッシュボードから削除できます。

ただし、外部ページを Adobe Workfront で作成した後に削除することはできません。外部ページの削除は、API を使用してのみ可能です。Workfront API について詳しくは、[API の基本](../../../wf-api/general/api-basics.md)を参照してください。外部ページの作成について詳しくは、[外部 web ページをダッシュボードに埋め込む](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)を参照してください。

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
      <p>標準</p>
      <p>プラン</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボードおよびカレンダーへのアクセスを編集する</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ダッシュボードに対する権限の管理</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ダッシュボードからの外部ページを削除

1. 削除する外部ページが含まれているダッシュボードに移動します。

1. 「**ダッシュボードの操作**」をクリックしたあと、「**編集**」をクリックします。

   ![&#x200B; ダッシュボードを編集 &#x200B;](assets/unshimmed-edit-dashboard.png)

1. 画面の右側で、削除する外部ページを見つけて、「**削除**」アイコン ![&#x200B; 削除アイコン &#x200B;](assets/delete.png) をクリックします。

   ![&#x200B; ダッシュボード内の「外部ページを削除」アイコン &#x200B;](assets/delete-external-page-icon-inside-dashboard-nwe-350x284.png)

1. 左下隅にある「**保存して閉じる**」をクリックします。

   これにより、選択したダッシュボードから外部ページが削除されます。外部ページは Workfront に残り、レポートからアクセスできます。詳しくは、[外部 web ページをダッシュボードに埋め込む](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)の記事のレポートで外部ページを表示するの節を参照してください。
