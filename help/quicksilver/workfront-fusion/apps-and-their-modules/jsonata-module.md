---
title: JSONata モジュール
description: Adobe Workfront Fusion JSONata コネクタは、Adobe Workfront Fusion がデータコンテンツをさらに操作できるように、データを JSON 形式で処理するモジュールを提供します。
author: Becky
feature: Workfront Fusion
source-git-commit: b7a6ecd9089c3a5517c56b849b860d57a900dade
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 37%

---

# [!UICONTROL JSONata] モジュール

[!DNL Adobe Workfront Fusion] [!UICONTROL JSONata] コネクタを使用すると、JSON オブジェクトをクエリできます。 このモジュールには接続は必要ありません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]、[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] の [!DNL Adobe Workfront] プランがある場合、この記事に記載されている機能を使用するには、組織で [!DNL Adobe Workfront Fusion] の購入 [!DNL Adobe Workfront] 必要です。 [!DNL Workfront Fusion] は、[!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront]を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

+++

## JSONata モジュールとそのフィールド

### 評価

このアクションモジュールは JSON オブジェクトをクエリし、配列を返します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expression]</td> 
   <td>JSON オブジェクトの評価に使用する式を入力します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data] </td> 
   <td> 評価する JSON オブジェクトを入力します。  </td> 
  </tr> 
  </tbody>
  </table>

>[!BEGINSHADEBOX]

**例**:

目的は、次の JSON オブジェクトから名前の配列を返すことです。

```JSON
{
  "people": [
    { "name": "Alice", "age": 30 },
    { "name": "Bob", "age": 25 },
    { "name": "Charlie", "age": 35 }
  ]
}
```

1. 「式」フィールドに「`people.name`」と入力します。
1. データフィールドに、JSON オブジェクトを入力します。

モジュールは、JSON オブジェクトから取得した名前の配列を返します。

>[!ENDSHADEBOX]
