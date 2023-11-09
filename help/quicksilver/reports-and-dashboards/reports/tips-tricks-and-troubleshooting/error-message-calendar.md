---
content-type: tips-tricks-troubleshooting
product-area: reporting;calendars
navigation-topic: tips-tricks-and-troubleshooting-reports
title: "カレンダーのエラーメッセージ： 'このカレンダーには、非アクティブなユーザーの表示権限があります'。"
description: 「このカレンダーには、非アクティブなユーザーの表示権限があります」というエラーメッセージについて説明します。
author: Lisa
feature: Reports and Dashboards
exl-id: ba1e25f2-4960-47f7-ac7d-6f6b0f59cfe2
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '308'
ht-degree: 6%

---

# カレンダーに関するエラーメッセージ：「このカレンダーには、非アクティブなユーザーの表示権限があります」

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>プラン、作業</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限が設定されているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>カレンダーに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 問題

自分と共有されているカレンダーにアクセスすると、次のエラーが表示されます。 

*このカレンダーには、非アクティブ化されたユーザーの表示権限が含まれています。管理者にカレンダーの権限を修正してもらってください。*

## 原因

このカレンダーを作成したユーザー（元の所有者）は、非アクティブ化されたユーザーです。 

## 解決策

これは、次の方法で解決できます。

1. 元のカレンダーをコピーします。 カレンダーをコピーすると、そのカレンダーの所有者になります。 コピーしたカレンダーには、元のカレンダーのすべての情報が表示されます。\
   カレンダーのコピーの詳細については、「 [カレンダーレポートのコピー](../../../reports-and-dashboards/reports/calendars/copy-a-calendar-report.md).

1. コピーしたカレンダーを元のカレンダーと同じユーザーと共有します。 新しいカレンダーには、すべてのユーザーに同じ情報が表示されます。
1. （オプションおよび条件付き）元のカレンダーを管理する権限を持っている場合、カレンダーの共有領域から、そのカレンダーを共有している他のすべてのユーザーを削除します。 これにより、誤ったカレンダーを表示しようとするユーザーの混乱を解消できます。
