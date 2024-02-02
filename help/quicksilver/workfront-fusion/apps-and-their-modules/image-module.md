---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: 画像モジュール
description: Adobe Workfront Fusion 画像モジュールを使用すると、特定の画像に関する情報（サイズ、タイプなど）を取得し、画像を別のファイル形式に変換し、画像のサイズを直接変更できます。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 89efa9d5-00c9-4bb5-97b3-2b2f9d73721d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '908'
ht-degree: 100%

---

# 画像モジュール

[!DNL Adobe Workfront Fusion] [!UICONTROL 画像]モジュールを使用すると、特定の画像に関する情報（サイズ、タイプなど）を取得し、画像を別のファイル形式に変換し、画像のサイズを直接変更できます。

## アクセス要件

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion]ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]、[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront]プランをご利用の場合、この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明する機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## [!UICONTROL 画像]モジュールとそのフィールド

このモジュールを設定する際には、次のフィールドが表示されます。モジュール内の太字のタイトルは、必須フィールドを示します。

* [[!UICONTROL サイズ変更]](#resize)
* [[!UICONTROL 形式の変換]](#convert-a-format)
* [[!UICONTROL メタデータの抽出]](#extract-metadata)

### [!UICONTROL サイズ変更]

この変換モジュールは、指定した条件に従って画像の高さと幅を変更します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>変換する画像のソースを選択します。前のモジュールから出力を選択するか、データファイルとファイル名をマッピングできます。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data]</td> 
   <td>変換するファイルをマッピングします。このフィールドは、[!UICONTROL Source file] フィールドで [!UICONTROL Map] を選択した場合に使用できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>変換ファイルの名前を入力します。このフィールドは、[!UICONTROL Source file] フィールドで [!UICONTROL Map] を選択した場合に使用できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL I want to]</td> 
   <td>高さと幅の比率を維持するか、寸法を指定した高さと幅に変更するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL According to]</td> 
   <td> <p>モジュールが画像の新しいサイズを決定する方法を選択します。このフィールドは、目的のフィールドで高さと幅の比率の維持を選択した場合に表示されます。このフィールドでの選択に基づいて、他のフィールドが表示されます。</p> 
    <ul> 
     <li> <p>[!UICONTROL Maximum width]</p> <p>画像を指定した幅に縮小します。高さは自動的に計算されます。</p> </li> 
     <li> <p>[!UICONTROL Maximum height]</p> <p>画像を指定した高さに縮小します。幅は自動的に計算されます。</p> </li> 
     <li> <p>[!UICONTROL Maximum height or width]</p> <p>画像の高さと幅が指定した値を超えないように画像を縮小します。このオプションでは高さと幅の比率が維持されるので、寸法のどちらかが指定より小さくなる場合があります。例えば、高さと幅の両方を 40 と指定した場合、400x300 の画像は 40x30 に縮小されます。</p> </li> 
     <li> <p>[!UICONTROL Minimum width]</p> <p>画像を指定した幅に拡大します。高さは自動的に計算されます。</p> </li> 
     <li> <p>[!UICONTROL Minimum height]</p> <p>画像を指定した高さに拡大します。幅は自動的に計算されます。</p> </li> 
     <li> <p>[!UICONTROL Minimum height or width]</p> <p>高さと幅が指定した値以上になるように画像を拡大します。このオプションでは高さと幅の比率が維持されるので、寸法のどちらかが指定より大きくなる場合があります。例えば、高さと幅の両方を 300 と指定した場合、40x30 の画像は 400x300 に拡大されます。</p> </li> 
     <li> <p>[!UICONTROL Percent]</p> <p>指定した値に基づいて、画像サイズをパーセンテージで変更します。 </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Width]</td> 
   <td>サイズ変更した画像の希望の幅をピクセル単位で入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Height]</td> 
   <td>サイズ変更した画像の希望の高さをピクセル単位で入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 形式の変換]

この変換モジュールは、画像ファイルの形式を変更します。このモジュールは、以下の形式と互換性があります。

* PNG
* JPG
* GIF
* BMP

ソースファイルと出力の両方が、これらのいずれかの形式である必要があります。例えば、[!UICONTROL 画像]／[!UICONTROL 形式を変換]するモジュールは、PNG ファイルを BMP ファイルに、または BMP を JPG に変換できます。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>変換する画像のソースを選択します。前のモジュールから出力を選択するか、データファイルとファイル名をマッピングできます。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data]</td> 
   <td>変換するファイルをマッピングします。このフィールドは、[!UICONTROL Source file] フィールドで [!UICONTROL Map] を選択した場合に使用できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>変換ファイルの名前を入力します。このフィールドは、[!UICONTROL Source file] フィールドで [!UICONTROL Map] を選択した場合に使用できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Output format]</td> 
   <td>モジュールでソースファイルを変換する形式を選択します。 </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL メタデータの抽出]

この変換モジュールは、モジュールに関する基本情報を返します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>変換する画像のソースを選択します。前のモジュールから出力を選択するか、データファイルとファイル名をマッピングできます。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data]</td> 
   <td>変換するファイルをマッピングします。このフィールドは、[!UICONTROL Source file] フィールドで「マップ」を選択した場合に使用できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>変換ファイルの名前を入力します。このフィールドは、[!UICONTROL Source file] フィールドで「マップ」を選択した場合に使用できます。</td> 
  </tr> 
 </tbody> 
</table>

## 考えられる問題

### エラーによりアクションが終了しました

エラーでアクションが終了する場合は、次の 3 つの場合があります。

* 受信したデータが JPG、GIF、PNG、BMP の形式ではありません
* 画像の寸法を変更する際に、幅や高さの上限を超えました。画像サイズは、幅 3840 ピクセルと高さ 2160 ピクセルを超えないようにする必要があります
* 画像のサイズまたは形式を変更する際に、画像の最大許容サイズを超えました。
