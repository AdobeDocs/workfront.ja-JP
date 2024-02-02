---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Markdown モジュール
description: ' [!DNL Adobe Workfront Fusion]  シナリオでは、Markdown モジュールを使用して、Markdown をHTMLに、HTMLを Markdown に変換できます。'
author: Becky
feature: Workfront Fusion
exl-id: 9e810302-4897-494a-9b50-667d87ce9cb7
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '285'
ht-degree: 100%

---

# [!UICONTROL Markdown] モジュール

[!DNL Adobe Workfront Fusion] シナリオでは、[!UICONTROL Markdown] モジュールを使用して、Markdown を HTMLに、HTMLを Markdown に変換できます。

シナリオの作成手順が必要な場合は、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) でのシナリオの作成を参照してください。

モジュールについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md) のモジュールを参照してください。

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンスは必要ありません。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランがある場合、この記事で説明する機能を使用するには [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>レガシー製品要件：この記事で説明する機能を使用するには、組織で [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。</p>
   </td> 
  </tr>
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## [!UICONTROL Markdown から HTML に]

このモジュールは、Markdown を HTML に変換します。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Markdown]</td> 
   <td> <p>Markdown 形式のプレーンテキストを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL GitHub Flavored Markdown] </td> 
   <td> <p>GitHub Flavored Markdown を HTML に変換する場合は、このオプションを有効にします。</p> <p>詳しくは、[!DNL ]Markdown のチートシート[!DNL GitHub]ドキュメントを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sanitize]</td> 
   <td>オプションを選択して、テキストから HTML タグを取り除くか、HTML をエスケープ処理するかを指定します。</td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL HTML から Markdown に]

このモジュールは、HTML コードを Markdown に変換します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Markdown]</td> 
   <td> <p>Markdown に変換する HTML コードを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL GitHub Flavored Markdown] </td> 
   <td> <p>このオプションを有効にして、HTML を [!DNL GitHub Flavored Markdown] に変換します。</p> <p>詳しくは、[!DNL GitHub] ドキュメントの Markdown のチートシートを参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>
