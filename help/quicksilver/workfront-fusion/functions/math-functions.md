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
source-git-commit: c325e16ba0cde4cd48fc3e40358a9ea9ed310659
workflow-type: tm+mt
source-wordcount: '306'
ht-degree: 91%

---

# [!DNL Adobe Workfront Fusion] の数式

<!--Audited: 4/2024-->

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td>  
   <td> <p>任意</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td>  
   <td> <p>新規：[!UICONTROL Standard]</p><p>または</p><p>現在：[!UICONTROL Work] 以上</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td>  
   <td> 
   <p>現在：[!DNL Workfront Fusion] ライセンスは必要ありません。</p> 
   <p>または</p> 
   <p>レガシー：任意 </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">製品</td>  
   <td> 
   <p>新規：</p> <ul><li>[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Workfront] プラン：組織は [!DNL Adobe Workfront Fusion] を購入する必要があります。</li><li>[!UICONTROL Ultimate] [!DNL Workfront] プラン：[!DNL Workfront Fusion] が含まれています。</li></ul> 
   <p>または</p> 
   <p>現在：[!DNL Adobe Workfront Fusion] を購入する必要があります。</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

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

## [!UICONTROL max ([値の配列])、max (値1;値2; ...)]

指定された配列内の最大の数値、または個別に入力された数値の中で最大の数値を返します。

## [!UICONTROL min ([値の配列])、min (value1; value2;...)]

指定された配列内の最小の数値、または個別に入力された数値の中で最小の数値を返します。

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

## [!UICONTROL parseNumber (数値; 小数点区切り文字)]

数値を含む文字列を解析し、数値を返します。例えば、parseNumber (1 756,456;,) のように指定します。

## [!UICONTROL formatNumber (数値; 小数点以下桁数; [小数点区切り文字]; [三桁ごとの区切り文字])]

要求された形式で数値を返します。デフォルトでは、小数点はカンマ（,）で、三桁ごとの区切り文字はピリオド（.）です。

>[!INFO]
>
>**例：**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>戻り値 123.456.789,000
