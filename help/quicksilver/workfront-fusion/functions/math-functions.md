---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion の数学関数
description: Adobe Workfront Fusion マッピングパネルでは、次の数学関数を使用できます。
author: Becky
feature: Workfront Fusion
exl-id: 8a3c7a89-62b5-45e9-b857-8beedd0e5af4
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '332'
ht-degree: 2%

---

# の数学関数 [!DNL Adobe Workfront Fusion]

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

## [!UICONTROL 平均 ([値の配列]) average(value1; [value2], ...)]

特定の配列の数値の平均値、または個々に入力された数値の平均値を返します。

## [!UICONTROL ceil （数値）]

指定された数値以上の最小の整数を返します。

>[!INFO]
>
>**例:**
>
>* `ceil(` `1.2` `)`
>
>   戻り値 2
>
>* `ceil(` `4` `)`
>
>   戻り値 4

## [!UICONTROL floor （数値）]

指定された数値以下の最大の整数を返します。

>[!INFO]
>
>**例:**
>
>* `floor(` `1.2` `)`
>
>   戻り値 1
>
>* `floor(` `1.9` `)`
>
>   戻り値 1
>
>* `floor(` `4` `)`
>
>   戻り値 4

## [!UICONTROL formatNumber ( 数値；decimalPOINTS; [decimalSeparator]; [thoundsSeparator])]

リクエストされた形式の数値を返します。 デフォルトでは、小数点はコンマ (,) で、千単位区切り文字はピリオド (.) です。

>[!INFO]
>
>**例:**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>戻り値 123.456.789,000

## [!UICONTROL 最大 ([値の配列]), max(value1;value2;...)]

指定した配列の最大の数値または個々に入力された数値の中で最大の数値を返します。

## [!UICONTROL 分 ([値の配列]), min(value1;value2;...)]

指定した配列の最小の数値または個々に入力された数値の中で最小の数値を返します。

## [!UICONTROL parseNumber ( 数値；小数点 )]

数値で文字列を解析し、その数値を返します。 例えば、parseNumber(1 756,456;,) のように指定します。

## [!UICONTROL round (number)]

数値を最も近い整数に丸めます。

>[!INFO]
>
>**例:**
>
>* `round(` `1.2` `)`
>
>   戻り値 1
>
>* `round(` `1.5` `)`
>
>   戻り値 2
>
>* `round(` `1.7` `)`
>
>   戻り値 2
> 
>* `round(` `2` `)`
>
>   戻り値 2

## [!UICONTROL sum ([値の配列]), sum(value1;value2;...)]

指定した配列の値の合計または個々に入力された数値の合計を返します。
