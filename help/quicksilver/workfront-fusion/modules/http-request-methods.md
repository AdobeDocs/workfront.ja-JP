---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: ' [!DNL Adobe Workfront Fusion] での HTTP リクエストメソッド'
description: モジュールで API 呼び出しを設定する場合は、HTTP リクエストメソッドのフィールドに入力する必要があります。
author: Becky
feature: Workfront Fusion
exl-id: 20b3c0f4-4a4c-4ba0-8570-ac39573ef1c0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '402'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion]での HTTP リクエストメソッド

モジュールで API 呼び出しを設定する場合は、HTTP リクエストメソッドのフィールドに入力する必要があります。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件はありません。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランがある場合、この記事で説明する機能を使用するには、組織は [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明する機能を使用するには、組織は [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] のライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  のライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## HTTP メソッド

次のいずれかの HTTP メソッドを使用します。

* **[!UICONTROL GET]**：パラメーターに基づいて web サーバーからデータを取得します。[!UICONTROL GET] は、指定されたリソースの表現をリクエストし、成功した場合は、リクエストされたコンテンツを含む [!UICONTROL 200 OK] 応答メッセージを受け取ります。
* **[!UICONTROL POST]**：パラメーターに基づいて web サーバーにデータを送信します。[!UICONTROL POST] リクエストには、ファイルのアップロードなどのアクションが含まれます。複数の [!UICONTROL POST] の結果は単一の [!UICONTROL POST] とは異なる可能性があるため、意図せずに複数の [!UICONTROL POST] を送信しないように注意してください。[!UICONTROL POST] が成功すると、[!UICONTROL 200 OK] 応答メッセージを受け取ります。
* **[!UICONTROL PUT]**：パラメーターに基づいて web サーバー内の場所にデータを送信します。[!UICONTROL PUT] リクエストには、ファイルのアップロードなどのアクションが含まれます。[!UICONTROL PUT] と [!UICONTROL POST] の違いは、PUT がべき等であることです。つまり、1 回の [!UICONTROL PUT] の成功の結果は複数回の同一の [!UICONTROL PUT] の結果は同じになります。PUT が成功すると、200 応答メッセージ（通常は 201 または 204）を受け取ります。
* **[!UICONTROL PATCH]**：（一部の API 呼び出しモジュールでは使用不可）パラメーターに基づいて web サーバー上のリソースに部分的な変更を適用します。[!UICONTROL PATCH] はべき等ではなく、複数の [!UICONTROL PATCH] の結果は意図しない影響をもたらす可能性があります。[!UICONTROL PATCH] が成功した場合は、200 応答メッセージ（通常は 204）を受け取ります。
* **[!UICONTROL DELETE]**：パラメーター（リソースが存在する場合）に基づいて、指定したリソースを web サーバーから削除します。[!UICONTROL DELETE] が成功した場合は、200 OK メッセージを受け取ります。
