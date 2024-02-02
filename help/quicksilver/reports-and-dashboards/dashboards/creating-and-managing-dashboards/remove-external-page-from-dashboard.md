---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: ダッシュボードからの外部ページを削除
description: 不要になった外部ページは、ダッシュボードから削除できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 9e400b8a-bbb8-4d1f-b419-d4a4518c0b2e
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: ht
source-wordcount: '299'
ht-degree: 100%

---

# ダッシュボードからの外部ページを削除

不要になった外部ページは、ダッシュボードから削除できます。

ただし、外部ページを Adobe Workfront で作成した後に削除することはできません。外部ページの削除は、API を使用してのみ可能です。Workfront API について詳しくは、[API の基本](../../../wf-api/general/api-basics.md)を参照してください。外部ページの作成について詳しくは、[外部 web ページをダッシュボードに埋め込む](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront ライセンス*</strong></td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>ダッシュボードに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## ダッシュボードからの外部ページを削除

1. **メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、「**ダッシュボード**」をクリックします。
1. 外部ページを削除するダッシュボードを選択し、**編集** ![](assets/edit-icon.png) をクリックします。

   ![編集アイコンを選択します。](assets/nwe-editdashboard2021-350x188.png)

1. 画面の右側で、削除する外部ページを見つけて、**削除**&#x200B;アイコン ![](assets/delete.png) をクリックします。

   ![](assets/delete-external-page-icon-inside-dashboard-nwe-350x284.png)

1. 左下隅にある「**保存して閉じる**」をクリックします。

   これにより、選択したダッシュボードから外部ページが削除されます。外部ページは Workfront に残り、レポートからアクセスできます。詳しくは、[外部 web ページをダッシュボードに埋め込む](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)の記事のレポートで外部ページを表示するの節を参照してください。
