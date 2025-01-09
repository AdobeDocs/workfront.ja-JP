---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: ダッシュボードからの外部ページを削除
description: 不要になった外部ページは、ダッシュボードから削除できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 9e400b8a-bbb8-4d1f-b419-d4a4518c0b2e
source-git-commit: a9abbeaa9abd0e905c60000a218eddb85d0389b9
workflow-type: tm+mt
source-wordcount: '239'
ht-degree: 90%

---

# ダッシュボードからの外部ページを削除

<!-- Audited: 1/2025 -->

不要になった外部ページは、ダッシュボードから削除できます。

ただし、外部ページを Adobe Workfront で作成した後に削除することはできません。外部ページの削除は、API を使用してのみ可能です。Workfront API について詳しくは、[API の基本](../../../wf-api/general/api-basics.md)を参照してください。外部ページの作成について詳しくは、[外部 web ページをダッシュボードに埋め込む](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン</strong></td> 
   <td> 
      <p>新規：</p>
         <ul>
         <li><p>標準</p></li>
         </ul>
      <p>現在：</p>
         <ul>
         <li><p>プラン</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>ダッシュボードに対する権限の管理</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ダッシュボードからの外部ページを削除

1. 削除する外部ページが含まれているダッシュボードに移動します。

1. 「**ダッシュボードの操作**」をクリックしたあと、「**編集**」をクリックします。

   ![](assets/unshimmed-edit-dashboard.png)

1. 画面の右側で、削除する外部ページを見つけて、**削除**&#x200B;アイコン ![](assets/delete.png) をクリックします。

   ![](assets/delete-external-page-icon-inside-dashboard-nwe-350x284.png)

1. 左下隅にある「**保存して閉じる**」をクリックします。

   これにより、選択したダッシュボードから外部ページが削除されます。外部ページは Workfront に残り、レポートからアクセスできます。詳しくは、[外部 web ページをダッシュボードに埋め込む](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)の記事のレポートで外部ページを表示するの節を参照してください。
