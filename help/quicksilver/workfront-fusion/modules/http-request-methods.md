---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]
description: モジュールで API 呼び出しを設定する場合は、HTTP リクエストメソッドのフィールドに入力する必要があります。
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '354'
ht-degree: 0%

---

# の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]

モジュールで API 呼び出しを設定する場合は、HTTP リクエストメソッドのフィールドに入力する必要があります。

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## HTTP メソッド

次のいずれかの HTTP メソッドを使用します。

* **[!UICONTROL GET]**:パラメーターに基づいて Web サーバーからデータを取得します。 [!UICONTROL GET] 指定されたリソースの表現を要求し、 [!UICONTROL 200 OK] 成功した場合は、リクエストされたコンテンツを含む応答メッセージ。
* **[!UICONTROL POST]**:パラメーターに基づいて Web サーバーにデータを送信します。 [!UICONTROL POST] リクエストには、ファイルのアップロードなどのアクションが含まれます。 複数 [!UICONTROL POST]結果が 1 つの [!UICONTROL POST]したがって、意図せずに複数の [!UICONTROL POST]s.次の場合、 [!UICONTROL POST] が成功した場合、 [!UICONTROL 200 OK] 応答メッセージ。
* **[!UICONTROL PUT]**:パラメーターに基づいて Web サーバー内の場所にデータを送信します。 [!UICONTROL PUT] リクエストには、ファイルのアップロードなどのアクションが含まれます。 の違いは、 [!UICONTROL PUT] および [!UICONTROL POST] は、PUTがべき等であること、つまり単一の成功の結果であることを意味します [!UICONTROL PUT] は、同じ [!UICONTROL PUT]s.PUTが成功した場合は、200 件の応答メッセージ（通常は 201 または 204）が返されます。
* **[!UICONTROL PATCH]**:（一部の API 呼び出しモジュールでは使用できません）パラメーターに基づいて、Web サーバー上のリソースに部分的な変更を適用します。 [!UICONTROL PATCH] はべき等ではなく、複数の [!UICONTROL PATCH]思いもよらない結果を招くかもしれない。 次の場合、 [!UICONTROL PATCH] が成功した場合は、200 件の応答メッセージ（通常は 204）が返されます。
* **[!UICONTROL DELETE]**:パラメーター（リソースが存在する場合）に基づいて、指定したリソースを Web サーバーから削除します。 次の場合、 [!UICONTROL DELETE] が成功した場合は、200 OK の応答メッセージが表示されます。
