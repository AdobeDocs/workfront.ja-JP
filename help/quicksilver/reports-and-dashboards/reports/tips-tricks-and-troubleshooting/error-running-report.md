---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 「レポート実行時のエラーメッセージ：「現在ログインしていません」」。
description: 「現在ログインしていません」というエラーメッセージについて説明します。
author: Nolan
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
source-git-commit: bcafa607da733b89747f6b448dd295d9b906d060
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 95%

---

# レポート実行時のエラーメッセージ：「現在ログインしていません」。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン、作業</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスの編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 問題

レポートを実行したり、ダッシュボードに表示したりすると、次のエラーが返されます。\
*もう一度試してください。現在ログインしていません。*

結果はレポートに表示されません。

## 原因

現在、このレポートは非アクティブなユーザーとして実行されるように設定されています。

## ソリューション

レポート設定を変更できるようにするには、レポートに対する管理権限が必要です。\
レポートを調整して結果を確認するには、以下の手順に従います。

1. レポートに移動します。
1. **報告書アクション**／**編集**／**報告書設定**&#x200B;をクリックします。

1. アクティブなユーザーの名前を「**次のアクセス権でこのレポートを実行する：**」フィールドに指定します。\
   または\
   「**次のアクセス権でこのレポートを実行する：**」フィールドは空白のままにします。

1. 「**完了**」をクリックします。
1. 「**保存して閉じる**」をクリックします。\
   このレポートの実行時にエラーが再び表示されることはありません。
