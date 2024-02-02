---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion の数式
description: 次の数式は、Adobe Workfront Fusion マッピングパネルで使用できます。
author: Becky
feature: Workfront Fusion
exl-id: 8a3c7a89-62b5-45e9-b857-8beedd0e5af4
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '332'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] の数式

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

## [!UICONTROL average ([値の配列]）average (1;[値2], ...)]

特定の配列内の数値の平均値、または個別に入力された数値の平均値を返します。

## [!UICONTROL ceil (数値)]

指定された数値以上の最小の整数を返します。

>[!INFO]
>
>**例：**
>
>* `ceil(` `1.2` `)`
>
>   戻り値 2
>
>* `ceil(` `4` `)`
>
>   戻り値 4

## [!UICONTROL floor (数値)]

指定された数値以下の最大の整数を返します。

>[!INFO]
>
>**例：**
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

## [!UICONTROL formatNumber (数値; 小数点以下桁数; [小数点区切り文字]; [三桁ごとの区切り文字])]

要求された形式で数値を返します。デフォルトでは、小数点はカンマ（,）で、三桁ごとの区切り文字はピリオド（.）です。

>[!INFO]
>
>**例：**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>戻り値 123.456.789,000

## [!UICONTROL max ([値の配列])、max (値1;値2; ...)]

指定された配列内の最大の数値、または個別に入力された数値の中で最大の数値を返します。

## [!UICONTROL min ([値の配列])、min (value1; value2;...)]

指定された配列内の最小の数値、または個別に入力された数値の中で最小の数値を返します。

## [!UICONTROL parseNumber (数値; 小数点区切り文字)]

数値を含む文字列を解析し、数値を返します。例えば、parseNumber (1 756,456;,) のように指定します。

## [!UICONTROL round (数値)]

数値を最も近い整数に丸めます。

>[!INFO]
>
>**例：**
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

## [!UICONTROL sum ([値の配列])、sum (値 1; 値 2; ...)]

指定された配列内の値の合計、または個別に入力された数値の合計を返します。
