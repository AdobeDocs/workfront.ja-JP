---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 「レポートの実行時のエラーメッセージ：'現在ログインしていません。''
description: この記事の手順を実行するには、次のアクセス権が必要です — EDIT ME.
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 4%

---

# レポート実行時のエラーメッセージ：「現在ログインしていません。」

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
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 問題

レポートを実行したり、ダッシュボードに表示したりすると、次のエラーが返されます。\
*もう一度試してください。現在ログインしていません。*

結果はレポートに表示されません。

## 原因

現在、このレポートは非アクティブなユーザーとして実行されるように設定されています。

## 解決策

レポート設定を変更するには、レポートに対する管理権限が必要です。\
レポートを調整して結果を確認するには：

1. レポートに移動します。
1. クリック **レポートのアクション** > **編集** > **レポート設定**.

1. アクティブなユーザーの名前を **このレポートを実行する際のアクセス権は次のとおりです。** フィールドに入力します。\
   または\
   を **このレポートを実行する際のアクセス権は次のとおりです。** フィールドが空白です。

1. クリック **完了**.
1. クリック **保存して閉じる**.\
   このレポートの実行時にエラーが再び表示されることはありません。
