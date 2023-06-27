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
workflow-type: tm+mt
source-wordcount: '299'
ht-degree: 3%

---

# の一般的な機能 [!DNL Adobe Workfront Fusion]

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
   <td>
   <p>現在のライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>
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

## [!UICONTROL get (object または array;パス )]

オブジェクトまたは配列の値のパスを返します。 ネストされたオブジェクトにアクセスするには、ドット表記を使用します。 配列の最初の項目はインデックス 1 です。

>[!INFO]
>
>**例:**
>
>* `get( array ; 1 + 1 )`
>* `get( array ; 5.raw_name )`
>* `get( object ; raw_name )`
>* `get( object ; raw_name.sub_raw_name )`

## [!UICONTROL if ( 式；value1;value2)]

を返します。 `value1` 式が true と評価される場合、それ以外の場合は、 `value2`.

>[!INFO]
>
>**例:**
>
>* `if( 1 = 1 ; A ; B )`
>
>    を返します。
>
>* `if( = 2 ; A ; B )`
>
>   戻り値 B

## [!UICONTROL ifempty ( 値 1;value2)]

を返します。 `value1` この値が空でない場合、それ以外の場合は、 `value2`.

>[!INFO]
>
>**例:**
>
>* `ifempty(` `A` `;` `B` )
>
>   を返します。
>
>* `ifempty(` `unknown` `;` `B` )
>
>   戻り値 B
>
>* `ifempty(` `""` `;` `B` )
>
>   戻り値 B

## [!UICONTROL switch (expression;value1;result1; [value2;result2;...]; [else])]

値のリストに対して、1 つの値（式と呼ばれます）を評価します。最初に一致した値に対応する結果を返します。

>[!INFO]
>
>**例:**
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

## [!UICONTROL omit(object;key1; [key2;...])]

オブジェクトの指定されたキーを省略し、残りのキーを返します。

>[!INFO]
>
>**例:**
>
>`omit(` ユーザー `;` パスワード `)`
>
>ユーザーの情報（パスワードを除く）のコレクションを返します。

## [!UICONTROL pick(object;key1; [key2;...])]

オブジェクトから指定されたキーのみを選択します。

>[!INFO]
>
>**例:**
>
>`pick(` ユーザー `;` パスワード `;` 電子メール `)`
>
>ユーザーのパスワードと電子メールアドレスのみのコレクションを返します。
