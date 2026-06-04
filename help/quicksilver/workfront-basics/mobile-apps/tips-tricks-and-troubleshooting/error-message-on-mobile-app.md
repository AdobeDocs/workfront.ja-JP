---
content-type: tips-tricks-troubleshooting
product-previous: mobile
navigation-topic: tips-tricks-and-troubleshooting-mobile-apps
title: ' [!DNL Adobe Workfront]  モバイルアプリのエラーメッセージ：「お使いのアカウントはAPIが有効になっていません。」'
description: ' [!DNL Adobe Workfront]  モバイルアプリのエラーメッセージ：「お使いのアカウントはAPIが有効になっていません。」'
author: Lisa
feature: Get Started with Workfront
exl-id: 120e56f4-9fd5-4c41-890e-981937714db0
TQID: https://experienceleague.adobe.com/t-ANxgXpzPBSM8cGUipyAIczqSEUJGXTthbaVP5dh2E
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 161
ht-degree: 68%

---

# [!DNL Adobe Workfront] モバイルアプリエラーメッセージ：「[!UICONTROL お使いのアカウントは API が有効になっていません。]」

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] プラン*</strong></td> 
   <td> <p> 任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] ライセンス</strong></td> 
   <td> <p>プラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>[!UICONTROL System administrator] </p> </td> 
  </tr> 
 </tbody> 
</table>

## 問題

[!DNL Adobe Workfront] モバイルアプリにログインしようとすると、次のエラーが表示されます：*[!UICONTROL お使いのアカウントは API が有効になっていません。 システム管理者に知らせて、設定してもらってください。 お手数をおかけします。]*

## 原因

[!DNL Workfront] 管理者は、お使いの [!DNL Workfront] 環境にモバイルデバイスからアクセスできるようにしていません。

## ソリューション

1. [!DNL Workfront] web アプリケーションに [!DNL Workfront] 管理者としてログインします。
1. **[!UICONTROL 設定]**&#x200B;エリアに移動します。
1. **[!UICONTROL システム]**&#x200B;メニューを開き、「**[!UICONTROL 環境設定]**」をクリックします。

1. 「**[!UICONTROL セキュリティ]**」セクションで、「**[!UICONTROL ユーザーが[!DNL Workfront]のモバイルアプリケーション]**」オプションを選択して有効にします。

1. 「**[!UICONTROL 保存]**」をクリックします。\
   システム内のすべてのユーザーが、モバイルアプリから[!DNL Workfront]にアクセスできるようになりました。
