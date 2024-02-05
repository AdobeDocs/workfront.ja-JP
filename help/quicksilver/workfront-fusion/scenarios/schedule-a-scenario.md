---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion でのシナリオのスケジュール
description: デフォルトでは、シナリオは 15 分ごとに実行されます。アクティブ化されたシナリオを実行するタイミングと頻度を定義することで、これを変更できます。
author: Becky
feature: Workfront Fusion
exl-id: bce89abe-ec37-4705-a88f-de62c8b27f49
source-git-commit: f5549be5951a2648d6a77d25bebbd4141f18d36c
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 95%

---

# [!DNL Adobe Workfront Fusion] でのシナリオのスケジュール

デフォルトでは、シナリオは 15 分ごとに実行されます。有効化されたシナリオを実行するタイミングと頻度を定義することで、これを変更できます。 統合シナリオは、5 分ごとに実行するようにスケジュールできます。

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件は不要。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]、[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
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

[!DNL Adobe Workfront Fusion] のライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  のライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## シナリオのスケジュール

1. シナリオの詳細ページの右上隅で、**[!UICONTROL オプション]**／**[!UICONTROL スケジュール]**&#x200B;をクリックします。

   または

   シナリオのトリガーモジュール上の&#x200B;**[!UICONTROL スケジュール]**&#x200B;アイコン（時計）をクリックします。

1. 次のフィールドに情報を入力します。

   <table style="table-layout:auto">   
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Run scenario]</td> 
      <td> <p>シナリオを実行する頻度を選択し、間隔を選択します。</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL At regular intervals]</strong> </p> <p>実行間隔（分）を入力します。デフォルト値は 15 分です。</p> </li> 
        <li> <p><strong>[!UICONTROL Once]</strong> </p> <p>シナリオを実行する日時を入力します。<code>MM/DD/YYYY h:mm A</code> の形式を使用します。例：<code>06/25/2019 11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Every day]</strong> </p> <p>シナリオを実行する時間を入力します。<code>h:mm A</code> の形式を使用します。例：<code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Days of the week]</strong> </p> <p>日：シナリオを実行する曜日を選択します。1 つ以上の日を選択できます。</p> <p>時間：選択した日にシナリオを実行する時間を入力します。<code>h:mm A</code> の形式を使用します。例： <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Days of the month]</strong> </p> <p>日：シナリオを実行する日付を選択します。1 つ以上の日を選択できます。</p> <p>時間：選択した日にシナリオを実行する時間を入力します。<code>h:mm A</code> の形式を使用します。例： <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Specified dates]</strong> </p> <p>月：シナリオを実行する月を選択します。1 つ以上の月を選択できます。</p> <p>日：シナリオを実行する日付を選択します。1 つ以上の日を選択できます。</p> <p>時間：選択した日にシナリオを実行する時間を入力します。<code>h:mm A</code> の形式を使用します。例： <code>11:00 PM</code></p> </li> 
       </ul> <p>メモ：シナリオを実行するには、実行の日付が存在する必要があります。例えば、31日にスケジュールされているシナリオは、2月、4月、6月、9月、11月には実行されません。これらの月には 31日がないからです。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Advanced scheduling]</td> 
      <td>シナリオを実行する特定の期間を定義できます。時間間隔、平日、月を指定できます。時間間隔ごとに、「<strong>[!UICONTROL Add]</strong>」をクリックして、「[!UICONTROL Run scenario]」フィールドの説明に従って、フィールドに入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Start]</td> 
      <td>シナリオの実行を開始する日時を入力します。<code>MM/DD/YYYY h:mm A</code> 形式を使用します。例：<code>06/25/2019 11:00 PM</code></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL End]</td> 
      <td>シナリオの実行を終了する日時を入力します。<code>MM/DD/YYYY h:mm A</code> 形式を使用します。例：<code>06/25/2019 11:00 PM</code></td> 
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL OK]**」をクリックしてスケジュール設定を保存し、シナリオに戻ります。
