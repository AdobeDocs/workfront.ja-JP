---
content-type: tips-tricks-troubleshooting
product-previous: mobile
navigation-topic: tips-tricks-and-troubleshooting-mobile-apps
title: 「 [!DNL Adobe Workfront] モバイルアプリ：'お使いのアカウントは API が有効になっていません。''
description: 「 [!DNL Adobe Workfront] モバイルアプリ：'お使いのアカウントは API が有効になっていません。''
author: Lisa
feature: Get Started with Workfront
exl-id: 120e56f4-9fd5-4c41-890e-981937714db0
source-git-commit: fdef22d9685d349a6f9492dec98475493ee9c048
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 2%

---

# エラーメッセージ [!DNL Adobe Workfront] モバイルアプリ：&quot;[!UICONTROL お使いのアカウントは API が有効になっていません。]&quot;

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計画</strong></td> 
   <td> <p> 任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] ライセンス</strong></td> 
   <td> <p>計画</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>[!UICONTROL システム管理者 ] </p> </td> 
  </tr> 
 </tbody> 
</table>

## 問題

にログインしようとしたとき [!DNL Adobe Workfront] モバイルアプリでは、次のエラーが発生します。 *[!UICONTROL お使いのアカウントは API が有効になっていません。 システム管理者に知らせれば、設定が完了します。 ごめんね。]*

## 原因

お使いの [!DNL Workfront] 管理者が有効化していません [!DNL Workfront] モバイルデバイスからアクセスする環境。

## 解決策

1. にログインします。 [!DNL Workfront] as a web アプリケーション [!DNL Workfront] 管理者。
1. 次に移動： **[!UICONTROL 設定]** 領域
1. を展開します。 **[!UICONTROL システム]** メニュー、次に「 **[!UICONTROL 環境設定]**.

1. 以下 **[!UICONTROL セキュリティ]** セクションで、 **[!UICONTROL 担当者に使用を許可 [!DNL Workfront]のモバイルアプリケーションおよび [!DNL Workfront Outlook] アドイン]** オプションを使用して有効にします。

1. 「**[!UICONTROL 保存]**」をクリックします。\
   システム内のすべてのユーザーがにアクセスできるようになりました [!DNL Workfront] モバイルアプリから、または [!DNL Outlook].
