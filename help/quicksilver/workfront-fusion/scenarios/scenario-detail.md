---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: ' [!DNL Adobe Workfront Fusion] のシナリオの詳細'
description: ' [!DNL Adobe Workfront Fusion] のシナリオの詳細'
author: Becky
feature: Workfront Fusion
exl-id: 1d8a3492-d609-43c8-a486-a401a597f160
source-git-commit: ae57c38149bf6db3bbbb471fad8f3567b7d712a7
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 90%

---

# [!DNL Adobe Workfront Fusion] のシナリオの詳細

シナリオの詳細ページは、特定のシナリオのホームページです。ページに表示されているシナリオの特定の情報へのアクセスを提供します。

また、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md) のシナリオエディターにアクセスを提供して、シナリオを編集できます。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p><p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation] </p><p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>   </td> 
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

[!DNL Adobe Workfront Fusion] ライセンスについては、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## [!UICONTROL シナリオの詳細]ページを開きます。

1. 左パネルの「**[!UICONTROL シナリオ]**」タブをクリックし、詳細が必要なシナリオをクリックします。

   または

   [ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md) のシナリオエディターでシナリオを使用している場合は、ウィンドウの左上隅付近にある左向き矢印 ![](assets/exit-editing-arrow.png) をクリックします。

1. 表示されるページで、次の表に示す要素をレビューできます。

   ![](assets/scenario-detail-350x207.png)

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Modules diagram] </td> 
      <td>このタブには、シナリオが視覚的に表示されます。図はシナリオエディターで表示されるものと同じです。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL History]（タブ） </td> 
      <td> <p>このタブを開いて、シナリオの編集を含むシナリオの履歴を表示します。 </p> <p>「[!UICONTROL History]」タブには、各実行のシナリオ実行履歴も提供されます。これには次の情報が含まれます。</p> 
       <ul> 
        <li>各実行のステータス（成功またはエラー）</li> 
        <li>実行時間</li> 
        <li>操作の数</li> 
        <li>データ転送のサイズ</li> 
        <li>詳細情報へのリンク</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Incomplete executions]</td> 
      <td> <p>このタブには、シナリオの実行が不完全な場合に関する情報が提供されます。不完全な実行ごとに、次の情報が含まれます。</p> 
       <ul> 
        <li>作成日</li> 
        <li>データ転送のサイズ</li> 
        <li>再試行</li> 
        <li>解決済み</li> 
        <li>試行回数</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Activate scenario]（「オン／オフ」ボタン）</td> 
      <td>シナリオを作成したら、スケジュールに従って実行するために、アクティブ化する必要があります。右上隅近くの「オン／オフ」ボタンをクリックすると、シナリオをアクティブ化または非アクティブ化できます。オンにすると、シナリオはスケジュールに従って実行されます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Edit]</td> 
      <td>右上隅のこのボタンをクリックして、シナリオエディターを開き、シナリオを操作できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Options]</td> 
      <td> <p>このメニューを使用すると、シナリオエディターを開かなくても追加のオプションを使用できます。改善点には、以下のものが含まれます。</p> 
       <ul> 
        <li>[!UICONTROL Scheduling]</li> 
        <li>[!UICONTROL Rename]</li> 
        <li>[!UICONTROL Clone]</li> 
        <li>[!UICONTROL Delete]</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Currently running]</td> 
      <td>このエリアには、現在実行中の実行に関連する情報が表示されます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL History]（エリア）</p> <p> </p> </td> 
      <td> <p>このエリアには、シナリオの最後の実行に関連する情報が表示されます。実行ごとに、次の情報が表示されます。</p> 
       <ul> 
        <li>実行日</li> 
        <li>ステータス（成功または失敗）</li> 
        <li>実行時間</li> 
        <li>データ転送のサイズ</li> 
        <li>詳細情報へのリンク</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Stats]</p>  </td> 
      <td>このグラフでは、シナリオの実行中に使用されたデータ転送と操作の量を [!UICONTROL line] で表示できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 処理バナー ]</p>  </td> 
      <td>シナリオが最近実行された場合は、次の内容のバナーが表示される場合があります。<p><code>Data is still being processed. Only partial scenario history will show until processing is complete.</code></p>これは、実行の詳細がストレージに書き込まれる間に表示されます。 処理は、シナリオの実行直後に実行されます。 そして数分以内に持続する 実行の処理中に、シナリオの実行の詳細が表示されない場合があります。</td> 
     </tr> 
    </tbody> 
   </table>
