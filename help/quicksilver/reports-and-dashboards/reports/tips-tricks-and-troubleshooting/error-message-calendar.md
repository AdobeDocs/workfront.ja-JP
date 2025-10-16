---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: カレンダーのエラーメッセージ：「このカレンダーには、非アクティブ化されたユーザーの表示権限があります」
description: エラーメッセージ「このカレンダーにはアクティブ化を解除したユーザーの表示権限があります」について説明します。
author: Lisa
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 89%

---

# カレンダーのエラーメッセージ：「このカレンダーには、非アクティブなユーザーの表示権限があります」

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
     <p>ワークまたはそれ以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>カレンダーに対する権限を管理</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 問題

自分と共有されているカレンダーにアクセスすると、以下のエラーが表示されます。

*このカレンダーにはアクティブ化を解除したユーザーの表示権限があります。管理者にカレンダー権限の修正を依頼してください。*

## 原因

このカレンダーを作成したユーザー（元の所有者）は、非アクティブ化されているユーザーです。 

## ソリューション

これは、以下の手順で解決できます。

1. 元のカレンダーをコピーします。カレンダーをコピーすると、そのカレンダーの所有者になります。コピーしたカレンダーには、元のカレンダーのすべての情報が表示されます。\
   カレンダーのコピーについて詳しくは、[カレンダーレポートのコピー](../../../reports-and-dashboards/reports/calendars/copy-a-calendar-report.md)を参照してください。

1. コピーしたカレンダーを元のカレンダーと同じユーザーと共有します。新しいカレンダーには、すべてのユーザーに同じ情報が表示されます。
1. （オプションおよび条件付き）元のカレンダーを管理する権限がある場合、カレンダーの共有エリアから、そのカレンダーを共有している他のすべてのユーザーを削除します。これにより、誤ったカレンダーを表示しようとするユーザーの混乱を解消できます。
