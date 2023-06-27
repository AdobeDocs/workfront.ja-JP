---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: 画像モジュール
description: Adobe Workfront Fusion Image モジュールを使用すると、特定の画像に関する情報（寸法、種類など）を取得し、画像を別のファイル形式に変換し、画像のサイズを直接変更することができます。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 89efa9d5-00c9-4bb5-97b3-2b2f9d73721d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 0%

---

# 画像モジュール

[!DNL Adobe Workfront Fusion] [!UICONTROL 画像] モジュールを使用すると、特定の画像に関する情報（サイズ、種類など）を取得し、画像を別のファイル形式に変換し、画像のサイズを直接変更することができます。

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

## [!UICONTROL 画像] モジュールとそのフィールド

このモジュールを設定する際には、次のフィールドが表示されます。 モジュール内の太字のタイトルは、必須フィールドを示します。

* [[!UICONTROL サイズ変更]](#resize)
* [[!UICONTROL 形式の変換]](#convert-a-format)
* [[!UICONTROL メタデータを抽出]](#extract-metadata)

### [!UICONTROL サイズ変更]

この変換サービスモジュールは、指定した条件に従って画像の高さと幅を変更します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td> <p>変換する画像のソースを選択します。 前のモジュールから出力を選択するか、データファイルとファイル名をマッピングすることができます。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL データ ]</td> 
   <td>変換するファイルをマッピングします。 このフィールドは、[!UICONTROL ソースファイル ] フィールドで [!UICONTROL Map] を選択した場合に使用できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル名 ]</td> 
   <td>変換後のファイルの名前を入力します。 このフィールドは、[!UICONTROL ソースファイル ] フィールドで [!UICONTROL Map] を選択した場合に使用できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 希望する ]</td> 
   <td>高さと幅の比率を維持するか、寸法を指定した高さと幅に変更するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 基準 ]</td> 
   <td> <p>モジュールで画像の新しいサイズを決定する方法を選択します。 このフィールドは、「目的のフィールド」で高さと幅の比率を維持することを選択した場合に表示されます。 このフィールドでの選択に基づいて、他のフィールドが表示されます。</p> 
    <ul> 
     <li> <p>[!UICONTROL 最大幅 ]</p> <p>画像を指定した幅に縮小します。 高さは自動的に計算されます。</p> </li> 
     <li> <p>[!UICONTROL 最大の高さ ]</p> <p>イメージを指定した高さに縮小します。 幅は自動的に計算されます。</p> </li> 
     <li> <p>[!UICONTROL 最大の高さまたは幅 ]</p> <p>画像の高さと幅が指定した値を超えないように画像を縮小します。 このオプションでは高さと幅の比率が維持されるので、寸法の 1 つが指定より小さくなる場合があります。 例えば、高さと幅の両方を 40 と指定した場合、400x300 の画像は 40X30 に縮小されます。</p> </li> 
     <li> <p>[!UICONTROL 最小幅 ]</p> <p>画像を指定した幅に拡大します。 高さは自動的に計算されます。</p> </li> 
     <li> <p>[!UICONTROL 最小の高さ ]</p> <p>イメージを指定した高さに拡大します。 幅は自動的に計算されます。</p> </li> 
     <li> <p>[!UICONTROL 最小の高さまたは幅 ]</p> <p>指定した値よりも大きく、高さと幅が小さくならないように画像を拡大します。 このオプションでは高さと幅の比率が維持されるので、寸法の 1 つが指定より大きくなる場合があります。 例えば、高さと幅の両方を 300 と指定した場合、40x30 の画像は 400X300 に拡大されます。</p> </li> 
     <li> <p>[!UICONTROL Percent]</p> <p>指定した値に基づいて、画像サイズをパーセンテージで変更します。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 幅 ]</td> 
   <td>サイズ変更された画像の幅をピクセル単位で入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL の高さ ]</td> 
   <td>サイズ変更された画像の高さをピクセル単位で入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 形式の変換]

この変換サービスモジュールは、画像ファイルの形式を変更します。 このモジュールは、次の形式と互換性があります。

* PNG
* JPG
* GIF
* BMP

ソースファイルと出力の両方が、次のいずれかの形式である必要があります。 例えば、 [!UICONTROL 画像] >[!UICONTROL 形式の変換] モジュールは、PNG ファイルを BMP ファイルに、または BMP をJPGに変換できます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td> <p>変換する画像のソースを選択します。 前のモジュールから出力を選択するか、データファイルとファイル名をマッピングすることができます。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL データ ]</td> 
   <td>変換するファイルをマッピングします。 このフィールドは、[!UICONTROL ソースファイル ] フィールドで [!UICONTROL Map] を選択した場合に使用できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル名 ]</td> 
   <td>変換後のファイルの名前を入力します。 このフィールドは、[!UICONTROL ソースファイル ] フィールドで [!UICONTROL Map] を選択した場合に使用できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力形式 ]</td> 
   <td>モジュールでソースファイルを変換する形式を選択します。 </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL メタデータを抽出]

この変換器モジュールは、モジュールに関する基本情報を返します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td> <p>変換する画像のソースを選択します。 前のモジュールから出力を選択するか、データファイルとファイル名をマッピングすることができます。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL データ ]</td> 
   <td>変換するファイルをマッピングします。 このフィールドは、[!UICONTROL ソースファイル ] フィールドで「マップ」を選択した場合に使用できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル名 ]</td> 
   <td>変換後のファイルの名前を入力します。 このフィールドは、[!UICONTROL ソースファイル ] フィールドで「マップ」を選択した場合に使用できます。</td> 
  </tr> 
 </tbody> 
</table>

## 考えられる問題

### エラーによりアクションが終了しました

エラーでアクションが終了する場合は、次の 3 つの場合があります。

* 受信したデータはJPG/GIF/PNG/BMP 形式ではありませんでした
* 画像のサイズを変更する際に、幅/高さの上限を超えました。 画像サイズは、幅 3840 px と高さ 2160 px を超えないようにする必要があります
* 画像のサイズまたは形式を変更する際に、画像の最大許容サイズを超えました。
