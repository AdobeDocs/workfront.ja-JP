---
title: レポートキャンバスでのレポートのエクスポート
description: レポートキャンバスでのレポートのエクスポート
hidefromtoc: true
hide: true
source-git-commit: 350d64577bac677bb0cc9bcb804c32b0301bc5d4
workflow-type: tm+mt
source-wordcount: '181'
ht-degree: 2%

---

# レポートキャンバスでのレポートのエクスポート

必要に応じて、レポート全体（または特定のブロック）をファイルフォーマットにエクスポートできます。 書き出し先は次のとおりです。

* PDF（現在無効）
* CSV
* PNG
* XLSX

## 前提条件

開始する前に、レポートキャンバスベータ版に登録する必要があります。 詳しくは、 [レポートキャンバスベータ版：概要](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/reporting-canvas-beta-overview.md).

## レポートのエクスポート

1. エクスポートするレポートに移動します。
1. レポートのヘッダーで、 **その他** アイコン ![](assets/more-icon-27x15.png)をクリックし、 **書き出し**&#x200B;をクリックし、作成するファイル形式を選択します。

   >[!NOTE]
   >
   >書き出したファイルに関しては、次の点を考慮してください。
   >
   >   * 複数のテーブルを含むレポートを XLSX 形式で書き出す場合、書き出されたファイルには、テーブルごとに別々のシートが含まれます。
   >   * 複数のテーブルを含むレポートを CSV 形式でエクスポートする場合、エクスポート結果は、各テーブルに対して個別のファイルを含む zip 形式のフォルダになります。
   >   * グループ化された行を含むテーブルを CSV 形式で書き出す場合、CSV ファイルにはすべての行が含まれますが、グループには表示されません。
   >   

<!-- 1. (Conditional) If you selected **PDF**, configure the fields below to format the exported file, then click **Download PDF**.

   >[!TIP]
   >
   >The PDF preview in the right pane updates as you configure each field.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Document size</td> 
      <td> <p>Select a size for the exported file from the drop-down menu.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Orientation</td> 
      <td> <p>Select either <strong>Portrait</strong> or <strong>Landscape</strong>.</p> </td> 
     </tr>
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">Scaling options</td> 
       <td> <p>Select the scaling option for the exported file:</p> 
        <ul> 
         <li> <p><strong>Normal</strong> (default option)</p> </li> 
         <li> <p><strong>Fit to width</strong> </p> </li> 
         <li> <p><strong>Fit to height</strong> </p> </li> 
        </ul> </td> 
      </tr>
     <tr> 
      <td role="rowheader">Heading settings</td> 
      <td> <p>Select all the content you want to display in the header.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Footer settings</td> 
      <td> <p>Select all the content you want to display in the footer.</p> <p>If you select <strong>Footer message</strong>, type the <strong>Footer text</strong> that you want to display in the footer. You can type up to 255 characters.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Watermark</td> 
      <td> <p>If you select <strong>Include watermark</strong>:</p> 
       <ul> 
        <li>Type the <strong>Watermark text</strong> that you want to display. You can type up to 20 characters.</li> 
        <li>Slide or enter the <strong>Opacity</strong> percentage that you want for the text.</li> 
        <li>Enter the degree of <strong>Rotation</strong> that you want for the text.</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

   The exported PDF file is named in the following format: REPORT_TITLE_YYYY-MM-DDTHH_MM_SS. -->
