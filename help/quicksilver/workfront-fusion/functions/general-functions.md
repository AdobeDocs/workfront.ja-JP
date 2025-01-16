---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion の一般的な機能
description: Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。 この記事は廃止されましたが、この機能を説明する新しい記事へのリンクが含まれています。
author: Becky
feature: Workfront Fusion
exl-id: 74bfda4e-5690-4b8c-ac58-20cf261f188d
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '455'
ht-degree: 57%

---

# [!DNL Adobe Workfront Fusion] の一般的な機能

>[!IMPORTANT]
>
>Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。
>
>この記事の情報は、次の記事に記載されています。
>
>* [ 一般的な関数 ](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/mapping-panel/functions/general-functions.html)
>
>ブックマークを更新してください。
>
>この記事は現在更新されておらず、近い将来に削除されます。

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件は不要。</p>
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

2 つ以上の式が true と評価された場合にのみ値を返す if ステートメントを作成するには、`and` キーワードを使用します。

`if` ステートメントを組み合わせるには、`and` 演算子と `or` 演算子を使用します。

![and 演算子 ](/help/quicksilver/workfront-fusion/functions/assets/and-in-if-statement.png)

>[!INFO]
>
>**例：**
>
>* `if( 1 = 1 ; A ; B )`
>
>    戻り値 A
>
>* `if( 1 = 2 ; A ; B )`
>
>   戻り値 B
>
>* `if( 1 = 2 and 1 = 2 ; A ; B )`
>
>    戻り値 B
>   

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

（式と呼ばれる） 1 つの値を値のリストと照合して評価します。最初に一致した値に対応する結果が返されます。 `else` 値を含めるには、最終的な式または値の後に追加します。

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
>   戻り値 4
>   
>   この関数では、4 は式が適用されない場合に返される値（`else` 値）です。

## [!UICONTROL omit(object; key1; [key2; ...])]

オブジェクトのキーを省略し、残りのキーを返します。

>[!INFO]
>
>**例：**
>
>`omit(` ユーザー `;` パスワード `)`
>
>パスワードを除くユーザーの情報のコレクションを返します。

## [!UICONTROL pick(オブジェクト; キー1; [キー2; ...])]

オブジェクトから指定されたキーのみを選択します。

>[!INFO]
>
>**例：**
>
>`pick(` ユーザー `;` パスワード `;` メール `)`
>
>ユーザーのパスワードとメールアドレスのみのコレクションを返します。

## mergeCollections （collection1 ; collection2）

2 つのコレクションのキーと値のペアを組み合わせて、それらのコレクションを結合します。 両方のコレクションに同じキーが含まれている場合、2 番目のコレクションの値が最初のコレクションの値を上書きします。

