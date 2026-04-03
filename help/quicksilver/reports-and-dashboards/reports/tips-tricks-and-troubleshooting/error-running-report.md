---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: レポートの実行時に「現在ログインしていません」というエラーメッセージが表示される。
description: 「現在ログインしていません」というエラーメッセージについて説明します。
author: Courtney
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '215'
ht-degree: 94%

---

# レポート実行時のエラーメッセージ：「現在ログインしていません」。

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
     <p>Work またはそれ以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


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
