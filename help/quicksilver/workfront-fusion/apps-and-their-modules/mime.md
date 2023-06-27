---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: MIME モジュール
description: MIME タイプは、Adobe Workfront Fusion で使用できます。 多目的インターネットメール拡張 (MIME) タイプは、ソフトウェアがインターネットで共有される様々なタイプのデータを識別できるラベルです。 Web サーバーおよびブラウザーは、MIME タイプを使用して、ファイルに対して何を実行するかを決定します。 例えば、MIME タイプが text/html のファイルは、MIME タイプが image/jpeg のファイルとは異なる方法でブラウザーで処理されます。 MIME タイプは、オペレーティングシステムとハードウェアに関係なく機能します。
author: Becky
feature: Workfront Fusion
exl-id: ebbf6ad0-a1d0-47f8-849f-7bba1e0763d3
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 0%

---

# [!UICONTROL MIME] モジュール

MIME タイプは、Adobe Workfront Fusion で使用できます。 多目的インターネットメール拡張 (MIME) タイプは、ソフトウェアがインターネットで共有される様々なタイプのデータを識別できるラベルです。 Web サーバーおよびブラウザーは、MIME タイプを使用して、ファイルに対して何を実行するかを決定します。 例えば、MIME タイプがのファイル `text/html` は、MIME タイプがのファイルとは異なる方法でブラウザーで処理されます `image/jpeg`. MIME タイプは、オペレーティングシステムとハードウェアに関係なく機能します。

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
   <td>
   <p>現在のライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] [!UICONTROL] の [!UICONTROL] [!DNL Workfront Fusion] 自動化 (WA)</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] がある場合 [!DNL Adobe Workfront] プラン（組織で購入する必要がある） [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。 [!DNL Workfront Fusion] は、[!UICONTROL Ultimate] に含まれています [!DNL Workfront] プラン</p>
   <p>または</p>
   <p>従来の製品要件：組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL MIME] モジュールとそのフィールド

### [!UICONTROL MIME タイプの取得]

この変換サービスモジュールは、指定された名前、パス、または拡張子に関連付けられた MIME タイプを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル ]</td> 
   <td> <p>MIME タイプを決定するファイルを入力またはマッピングします。 </p> <p>次を使用してファイルを入力できます。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL ファイルパス ]</strong> </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例： </b></span></span>/file/image.jpeg</p> </li> 
     <li><strong>[!UICONTROL ファイル名 ]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例： </b></span></span>image.jpeg</p> </li> 
     <li><strong>[!UICONTROL ファイル拡張子 ]</strong>  <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例： </b></span></span>jpeg</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL ファイル拡張子を取得する]

この変換サービスモジュールは、指定された MIME タイプの元のファイル拡張子を返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL MIME type]</td> 
   <td> <p>ファイル拡張子を決定する MIME タイプを入力またはマッピングします。 </p> </td> 
  </tr> 
 </tbody> 
</table>
