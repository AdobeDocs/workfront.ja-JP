---
content-type: tips-tricks-troubleshooting
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: レポートの実行時に「現在ログインしていません」というエラーメッセージが表示される。
description: 「現在ログインしていません」というエラーメッセージについて説明します。
author: Courtney
feature: Reports and Dashboards
exl-id: fda4630a-2590-46f4-94ff-499a485367ee
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Vg-z-oXY25if70i5l2GBZad4iBj6hNRhu9LHE-6kCU8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 215
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
*もう一度試してください。 現在ログインしていません。*

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
