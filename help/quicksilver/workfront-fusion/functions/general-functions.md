---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion の一般的な機能
description: Adobe Workfront Fusion マッピングパネルでは、次の一般的な関数を使用できます。
author: Becky
feature: Workfront Fusion
exl-id: 74bfda4e-5690-4b8c-ac58-20cf261f188d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '299'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] の一般的な機能

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンスは必要ありません。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランの場合、この記事で説明する機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明する機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## [!UICONTROL GET（オブジェクトまたは配列パス）]

オブジェクトまたは配列の値のパスを返します。ネストされたオブジェクトにアクセスするには、ドット表記を使用します。配列内の最初の項目はインデックス 1 です。

>[!INFO]
>
>**例：**
>
>* `get( array ; 1 + 1 )`
>* `get( array ; 5.raw_name )`
>* `get( object ; raw_name )`
>* `get( object ; raw_name.sub_raw_name )`

## [!UICONTROL IF（式；値 1；値 2）]

式が true に評価される場合は、`value1` を返します。それ以外の場合は `value2` を返します。

>[!INFO]
>
>**例：**
>
>* `if( 1 = 1 ; A ; B )`
>
>    戻り値 A
>
>* `if( = 2 ; A ; B )`
>
>   戻り値 B

## [!UICONTROL ifempty (value1; value2)]

この値が空でない場合は、`value1` を返します。それ以外の場合は、`value2` を返します。

>[!INFO]
>
>**例：**
>
>* `ifempty(` `A` `;` `B` )
>
>   戻り値 A
>
>* `ifempty(` `unknown` `;` `B` )
>
>   戻り値 B
>
>* `ifempty(` `""` `;` `B` )
>
>   戻り値 B

## [!UICONTROL switch (expression; value1; result1; [value2; result2; ...]; [else])]

1 つの値（式と呼ばれます）を値のリストに対して評価し、最初に一致した値に対応する結果を返します。

>[!INFO]
>
>**例：**
>
>* `switch( B ; A ; 1 ; B ; 2 ; C ; 3 )`
>
>   戻り値 2
>
>* `switch( C ; A ; 1 ; B ; 2 ; C ; 3 )`
>
>   戻り値 3
>
>* `switch( X ; A ; 1 ; B ; 2 ; C ; 3 ; 4 )`
>
>  戻り値 4

## [!UICONTROL omit(object; key1; [key2; ...])]

オブジェクトのキーを省略し、残りのキーを返します。

>[!INFO]
>
>**例：**
>
>`omit(` ユーザー `;` パスワード `)`
>
>ユーザーの情報（パスワードを除く）のコレクションを返します。

## [!UICONTROL pick(オブジェクト; キー1; [キー2; ...])]

オブジェクトから指定されたキーのみを選択します。

>[!INFO]
>
>**例：**
>
>`pick(` ユーザー `;` パスワード `;` メール `)`
>
>ユーザーのパスワードとメールアドレスのみのコレクションを返します。
