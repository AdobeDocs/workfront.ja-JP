---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: のデータ構造 [!DNL Adobe Workfront Fusion]
description: データ構造は、Adobe Workfront Fusion に転送されるデータの形式について詳しく説明したドキュメントです。 このドキュメントに基づいて、シナリオエディターはどのモジュールがどの種類のデータを返すか、または受け取るかを判断できます。 データ構造ドキュメントは、JSON、XML、CSV などのデータ形式のシリアル化や解析に最も一般的に使用されます。
author: Becky
feature: Workfront Fusion
exl-id: 35a7e906-7ca2-433d-87a9-bbb01babffb0
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# のデータ構造 [!DNL Adobe Workfront Fusion]

データ構造とは、転送先のデータの形式を詳細に記述したドキュメントです [!DNL Adobe Workfront Fusion]. このドキュメントに基づいて、シナリオエディターはどのモジュールがどの種類のデータを返すか、または受け取るかを判断できます。 データ構造ドキュメントは、JSON、XML、CSV などのデータ形式のシリアル化や解析に最も一般的に使用されます。

データ構造を作成するには、 [!UICONTROL 新しいデータ構造の作成] ボタン [!UICONTROL データ構造の概要] 」セクションまたはデータ構造の指定が必要なモジュールの設定で使用できます。

サポートされるデータタイプについては、 [[!UICONTROL モジュールのタイプ]](../../workfront-fusion/modules/module-types.md) 記事。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## データ構造ジェネレーター

データ構造を作成する必要がない場合もあります。 組み込みのジェネレーターのテンプレートを使用すると、作業を容易にすることができます。 ジェネレーターは、データサンプルを指定することで、入力したデータサンプルに基づいてデータ構造を自動的に作成します。 作成したデータ構造は手動で変更できます。

![](assets/data-structure-generator-350x341.jpg)
