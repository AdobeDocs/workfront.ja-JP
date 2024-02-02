---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: Web サービスから web フックを受け取る
description: Web サービスが現在  [!DNL Adobe Workfront Fusion] にアプリとして実装されていないが、web フックの送信をサポートしている場合は、カスタム web フックモジュールをインスタントトリガーとして使用して、サービスをシナリオに追加できます。
author: Becky
feature: Workfront Fusion
exl-id: f1a67dbf-c245-4936-9dcc-3fdbfc6ee3b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '306'
ht-degree: 100%

---

# Web サービスから web フックを受け取る

Web サービスが現在 [!DNL Adobe Workfront Fusion] にアプリとして実装されていないが、web フックの送信をサポートしている場合は、カスタム web フックモジュールをインスタントトリガーとして使用して、サービスをシナリオに追加できます。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
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

## Web フックを受信

1. **[!UICONTROL Web フック]／[!UICONTROL カスタム web フック]**&#x200B;モジュールをシナリオに追加します。
1. 「**[!UICONTROL 追加]**」をクリックし、表示されるボックスに **[!UICONTROL web フック名]**&#x200B;を入力してから、「**[!UICONTROL 保存]**」をクリックします。

1. **[!UICONTROL アドレスをクリップボードにコピー]**、次に「**[!UICONTROL OK]**」をクリックします。

1. Web サービスにログインし、以下の操作を行います。

   1. Web サービス用の[!UICONTROL 設定]エリアで、web フックを作成します。
   1. 手順 3 でクリップボードにコピーしたアドレスをペーストします。
   1. Web フックをトリガーするイベントを選択します。

1. [!DNL Workfront Fusion] シナリオで、[!UICONTROL カスタム web フック]モジュールをトリガーする 1 つ以上のイベントを指定します。
1. シナリオを実行します。

   イベントが発生した場合、[!UICONTROL カスタム web フック]モジュールがトリガーして、シナリオが実行されます。
