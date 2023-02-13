---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Web サービスから Webhook を受け取る
description: Web サービスが現在アプリとして [!DNL Adobe Workfront Fusion]Web フックの送信をサポートしていますが、カスタム Webhook モジュールをインスタントトリガーとして使用して、サービスをシナリオに追加できます。
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '258'
ht-degree: 0%

---

# Web サービスから Webhook を受け取る

Web サービスが現在アプリとして [!DNL Adobe Workfront Fusion]Web フックの送信をサポートしていますが、カスタム Webhook モジュールをインスタントトリガーとして使用して、サービスをシナリオに追加できます。

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## ウェブフックを受け取る

1. を **[!UICONTROL ウェブフック] >[!UICONTROL カスタムウェブフック]** モジュールをシナリオに追加します。
1. クリック **[!UICONTROL 追加]**, type **[!UICONTROL ウェブフック名]** 表示されるボックスで、 **[!UICONTROL 保存]**.

1. クリック **[!UICONTROL アドレスをクリップボードにコピー]**&#x200B;を選択し、「 **[!UICONTROL OK]**.

1. Web サービスにログインし、次の操作を行います。

   1. 内 [!UICONTROL 設定] web サービス用の領域で、webhook を作成します。
   1. 手順 3 でクリップボードにコピーしたアドレスを貼り付けます。
   1. Webhook をトリガーするイベントを選択します。

1. 内 [!DNL Workfront Fusion] シナリオの場合は、イベントをトリガーする 1 つ以上のイベントを指定します [!UICONTROL カスタムウェブフック] モジュール。
1. シナリオを実行します。

   イベントが発生した場合、 [!UICONTROL カスタムウェブフック] モジュールトリガーとシナリオが実行されます。
