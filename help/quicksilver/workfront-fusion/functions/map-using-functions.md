---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: ' [!DNL Adobe Workfront Fusion] の関数を使用して項目をマッピング'
description: 項目をマッピングする場合、関数を使用して単純な数式や複雑な数式を作成できます。
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '532'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] の関数を使用して項目をマッピング

項目をマッピングする場合、関数を使用して単純な数式や複雑な数式を作成できます。

[!DNL Adobe Workfront Fusion] で使用できる関数は、Excel の関数や一部のプログラミング言語の関数に似ています。一般的なロジック、数学、テキスト、日付および配列を評価します。条件付きロジックと項目値の変換（テキストの大文字への変換、テキストの切り抜き、日付の別の形式への変換など）を実行できます。詳しくは、[Adobe Workfront Fusion でのモジュール間の情報のマッピング](../../workfront-fusion/mapping/map-information-between-modules.md)を参照してください。

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンスは必要ありません。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select]または[!UICONTROL Prime]の [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入してください。[!DNL Workfront Fusion] は [!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入してください。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## フィールドに関数を挿入

フィールドをクリックすると、[!UICONTROL マッピング]パネルが表示されます。マッピングパネルには、次のようなタブがあります。

![](assets/functions-toolbar-350x189.png)

（パネルを開く際に表示される）最初のタブ ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) は、他のモジュールからマッピングできる項目を表示します。

その他のタブには、次のような関数が含まれます。

* **一般的な関数** ![](assets/toolbar-icon-general-function.png) - 詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) の一般的な機能を参照してください。

* **数式** ![](assets/toolbar-icon-math-functions.png) - 詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) の数式を参照してください。

* **テキスト関数とバイナリ関数** ![](assets/toolbar-icon-text&binary-functions.png) - 詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) の文字列関数を参照してください。

* **日付と時間** ![](assets/toolbar-icon-date&time-functions.png) - 詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) の日付と時間の関数および次の記事を参照してください。

   * [ [!DNL Adobe Workfront Fusion] の日付と時刻の形式設定のトークン](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [ [!DNL Adobe Workfront Fusion] の日付と時間の解析用トークン](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **配列操作の関数** ![](assets/toolbar-icon-functions-for-arrays.png) - 詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) の配列関数を参照してください。

フィールドに関数を挿入するには、次の手順に従います。

1. 関数名をクリックします。

   または

   関数をフィールドにドラッグします。

>[!INFO]
>
>**例：**&#x200B;一部のデータタイプでは、ユーザーが一定の文字数以上を入力できないよう設定されています。サブ文字列関数を使用して、値を特定の文字数に制限できます。
>
>この例では、サブ文字列関数は、プロジェクト名を 50 文字に制限します。
>
>![](assets/example-meet-length-restriction-350x184.png)

## 関数のネスト

関数を相互にネストすることができます。

## [!DNL Google Sheets] 関数の使用

[!DNL Workfront Fusion] に使用する関数が含まれおらず、[!DNL Google Sheets] にある場合は、次の手順を実行すると使用できます。

1. [!DNL Google Sheets] で、新しい空のスプレッドシートを作成します。
1. [!DNL Workfront Fusion] で、シナリオを開きます。
1. **[!DNL Google Sheets]**／**[!UICONTROL セルを更新]**&#x200B;モジュールをシナリオに追加します。

   モジュールを追加する手順については、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) でのシナリオの作成の記事の[シナリオへのモジュールの追加](../../workfront-fusion/scenarios/create-a-scenario.md#add)を参照してください。

1. モジュールを設定します。

   1. 「**[!UICONTROL スプレッドシート]**」フィールドで新しく作成したスプレッドシートを選択します。
   1. [!DNL Google Sheets] 関数を含む数式を「**[!UICONTROL 値]**」フィールドに挿入します。

      通常どおり、先行モジュールの出力を使用できます。

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. **[!UICONTROL Google Sheets]／[!UICONTROL セルを取得]**&#x200B;モジュールを挿入して、計算結果を取得します。
1. 手順 4 で使用した同じセル ID を使用して、モジュールを設定します。

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
