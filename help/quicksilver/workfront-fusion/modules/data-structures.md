---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: ' [!DNL Adobe Workfront Fusion] のデータ構造'
description: データ構造は、Adobe Workfront Fusion に転送されるデータの形式について詳しく説明したドキュメントです。このドキュメントに基づいて、シナリオエディターはどのモジュールがどの種類のデータを返すか、または受け取るかを判断できます。データ構造ドキュメントは、JSON、XML、CSV などのデータ形式をシリアル化したり、解析したりするために一般的によく使用されます。
author: Becky
feature: Workfront Fusion
exl-id: 35a7e906-7ca2-433d-87a9-bbb01babffb0
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '341'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] のデータ構造

データ構造とは、[!DNL Adobe Workfront Fusion] に転送されているデータの形式を詳細に記述したドキュメントです。このドキュメントに基づいて、シナリオエディターはどのモジュールがどの種類のデータを返すか、または受け取るかを判断できます。データ構造ドキュメントは、JSON、XML、CSV などのデータ形式をシリアル化したり、解析したりするために一般的によく使用されます。

データ構造を作成するには、「[!UICONTROL データ構造の概要]」セクションまたはデータ構造の仕様が必要なモジュールの設定にある「[!UICONTROL データ構造を新規作成]」ボタンをクリックします。

サポートされるデータタイプについては、[[!UICONTROL モジュールのタイプ]](../../workfront-fusion/modules/module-types.md)を参照してください。

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件： [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、[!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も組織で購入する必要があります。[!DNL Workfront Fusion] は [!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明されている機能を使用するには、[!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについては、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## データ構造ジェネレーター

データ構造を作成する必要がない場合もあります。ビルトインジェネレーターのテンプレートを使用すると、作業を容易にすることができます。ジェネレーターは、データサンプルを指定することで、入力したデータサンプルに基づいてデータ構造を自動的に作成します。作成したデータ構造は手動で変更できます。

![](assets/data-structure-generator-350x341.jpg)
