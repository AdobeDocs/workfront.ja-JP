---
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: connections-annd-webhooks
title: ' [!DNL Adobe Workfront Fusion]  への接続を作成する - 基本的な手順'
description: 多数の [!DNL Adobe Workfront Fusion] コネクタでは、接続を作成するときにカスタム設定は必要ありません。この記事では、デフォルトの接続作成プロセスについて説明します。
author: Becky
feature: Workfront Fusion
exl-id: 6576a515-a1a1-4613-8d04-3c9d36bb1ed9
source-git-commit: 7d5f7c21fe38d43fb5601c81b8a31cc80587848f
workflow-type: tm+mt
source-wordcount: '355'
ht-degree: 74%

---

# [!DNL Adobe Workfront Fusion] への接続を作成する - 基本的な手順

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront]を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 接続の作成

[!DNL Workfront Fusion] モジュール内で接続を作成するには、以下を実行します。

1. [!UICONTROL 接続]ボックスの横にある&#x200B;**[!UICONTROL 追加]**&#x200B;をクリックして、**[!UICONTROL 接続の作成]**&#x200B;パネルを開きます。
1. （オプション）デフォルトの&#x200B;**[!UICONTROL 接続名]**&#x200B;を変更
1. （条件付き）アプリで ID、キー、[!UICONTROL シークレット] などの詳細な接続設定が必要な場合は、その情報を入力します。

   この種の情報を入力できるフィールドを表示するには、**[!UICONTROL 詳細設定を表示]**&#x200B;をクリックする必要がある場合があります。

1. 「**[!UICONTROL 続行]**」をクリックします。
1. 表示されるログインウィンドウで、アプリにログインするための資格情報を入力します（まだ入力していない場合）。
1. （条件付き）「**[!UICONTROL 許可]**」ボタンが表示された場合、コネクタが実行できるアクションを調べてから、ボタンをクリックしてアプリを [!DNL Workfront Fusion] に接続します。

   >[!NOTE]
   >
   >一部のMicrosoft アプリは、同じ接続を使用し、これは個々のユーザー権限に関連付けられています。 そのため、接続を作成すると、権限同意画面に、現在のアプリケーションに必要な新しい権限に加え、このユーザーの接続に以前に付与された権限が表示されます。
   >
   >例えば、ユーザーが Excel コネクタを使用して「テーブルの読み取り」権限を付与され、Outlook コネクタにメールを読み取るための接続を作成した場合、権限の同意画面には、既に付与されている「テーブルの読み取り」権限と、新しく必要な「メールの書き込み」権限の両方が表示されます。