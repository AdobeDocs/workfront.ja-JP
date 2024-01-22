---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion でのシナリオのスケジュール
description: デフォルトでは、1 つのシナリオは 15 分ごとに実行されます。 有効化されたシナリオを実行するタイミングと頻度を定義することで、これを変更できます。
author: Becky
feature: Workfront Fusion
exl-id: bce89abe-ec37-4705-a88f-de62c8b27f49
source-git-commit: f5549be5951a2648d6a77d25bebbd4141f18d36c
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 0%

---

# でのシナリオのスケジュール設定 [!DNL Adobe Workfront Fusion]

デフォルトでは、1 つのシナリオは 15 分ごとに実行されます。 有効化されたシナリオを実行するタイミングと頻度を定義することで、これを変更できます。 統合シナリオは、5 分ごとに実行するようにスケジュールできます。

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">   
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
  <td>
   <p>現在のライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来のライセンス要件： [!UICONTROL [!DNL Workfront Fusion] [!UICONTROL] の [!UICONTROL] [!DNL Workfront Fusion] 自動化 (WA)</p>
   </td>    </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件： [!UICONTROL Select] または [!UICONTROL Prime] がある場合 [!DNL Adobe Workfront] プラン（組織で購入する必要がある） [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。 [!DNL Workfront Fusion] は、[!UICONTROL Ultimate] に含まれています [!DNL Workfront] プラン</p>
   <p>または</p>
   <p>従来の製品要件：組織は購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## シナリオのスケジュール設定

1. シナリオの詳細ページの右上隅で、 **[!UICONTROL オプション]** > **[!UICONTROL スケジュール]**

   または

   次をクリック： **[!UICONTROL スケジュール]** アイコン（時計）を使用して、シナリオのトリガーモジュールを表示します。

1. 次のフィールドに情報を入力します。

   <table style="table-layout:auto">   
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL シナリオを実行 ]</td> 
      <td> <p>シナリオを実行する頻度を選択し、間隔を選択します。</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL 一定の間隔で ]</strong> </p> <p>実行間隔（分）を入力します。 デフォルト値は 15 分です。</p> </li> 
        <li> <p><strong>[!UICONTROL 1 回 ]</strong> </p> <p>シナリオを実行する日時を入力します。 形式を使用 <code>MM/DD/YYYY h:mm A</code>. 例： <code>06/25/2019 11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL 毎日 ]</strong> </p> <p>シナリオを実行する時間を入力します。 形式を使用 <code>h:mm A</code>. 例： <code>11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL 曜日 ]</strong> </p> <p>日：シナリオを実行する曜日を選択します。 1 つ以上の日を選択できます。</p> <p>時間：選択した日にシナリオを実行する時間を入力します。 形式を使用 <code>h:mm A</code>. 例： <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL 月の日数 ]</strong> </p> <p>日数：シナリオを実行する日数を選択します。 1 つ以上の日を選択できます。</p> <p>時間：選択した日にシナリオを実行する時間を入力します。 形式を使用 <code>h:mm A</code>. 例： <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL 指定日 ]</strong> </p> <p>月：シナリオを実行する月を選択します。 1 つ以上の月を選択できます。</p> <p>日数：シナリオを実行する日数を選択します。 1 つ以上の日を選択できます。</p> <p>時間：選択した日にシナリオを実行する時間を入力します。 形式を使用 <code>h:mm A</code>. 例： <code>11:00 PM</code></p> </li> 
       </ul> <p>注意：シナリオをその日に実行するには、日付が存在する必要があります。 例えば、月の 31 日のみにスケジュールされているシナリオは、2 月、4 月、6 月、9 月、11 月には実行されません。これらの月には 31 日が含まれていないからです。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 詳細スケジュール設定 ]</td> 
      <td>シナリオを実行する期間を指定できます。 時間帯、平日、月を指定できます。 間隔ごとに、 <strong>[!UICONTROL 追加 ]</strong> 「[!UICONTROL シナリオを実行 ]」フィールドの説明に従って、フィールドに入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 開始 ]</td> 
      <td>シナリオを実行する日時を入力します。 形式を使用 <code>MM/DD/YYYY h:mm A</code>. 例： <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 終了 ]</td> 
      <td>シナリオを実行する前の日時を入力します。 形式を使用 <code>MM/DD/YYYY h:mm A</code>. 例： <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **[!UICONTROL OK]** スケジュール設定を保存し、シナリオに戻ります。
