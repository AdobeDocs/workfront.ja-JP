---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: で関数を使用して項目をマッピングする [!DNL Adobe Workfront Fusion]
description: 項目をマッピングする場合、関数を使用して単純式や複雑な数式を作成できます。
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# で関数を使用して項目をマッピングする [!DNL Adobe Workfront Fusion]

項目をマッピングする場合、関数を使用して単純式や複雑な数式を作成できます。

で使用できる関数 [!DNL Adobe Workfront Fusion] は、Excel の関数や一部のプログラミング言語の関数に似ています。 一般的なロジック、数学、テキスト、日付、配列を評価します。 条件付きロジックと項目値の変換（テキストの大文字への変換、テキストの切り抜き、日付の別の形式への変換など）を実行できます。 詳しくは、 [Adobe Workfront Fusion で、モジュール間の情報のマッピング](../../workfront-fusion/mapping/map-information-between-modules.md).

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
   <td>
   <p>現在のライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>
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

## フィールドに関数を挿入

フィールドをクリックすると、 [!UICONTROL マッピング] パネルが表示されます。 マッピングパネルには、次のようなタブがあります。

![](assets/functions-toolbar-350x189.png)

最初のタブ ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) （パネルを開く際に表示）他のモジュールからマッピングできる項目を表示します。

その他のタブには、次のような関数が含まれます。

* **一般的な関数** ![](assets/toolbar-icon-general-function.png)  — 詳しくは、 [の一般的な機能 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) を参照してください。

* **数学関数** ![](assets/toolbar-icon-math-functions.png)  — 詳しくは、 [の数学関数 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) を参照してください。

* **テキスト関数とバイナリ関数** ![](assets/toolbar-icon-text&binary-functions.png)  — 詳しくは、 [の文字列関数 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) を参照してください。

* **日時** ![](assets/toolbar-icon-date&time-functions.png)  — 詳しくは、 [の日付および時間関数 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) 詳しくは、以下の記事を参照してください。

   * [の日付と時刻の書式設定のトークン [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [での日時解析用トークン [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **配列操作用の関数** ![](assets/toolbar-icon-functions-for-arrays.png)  — 詳しくは、 [の配列関数 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) を参照してください。

フィールドに関数を挿入するには：

1. 関数名をクリックします。

   または

   関数をフィールドにドラッグします。

>[!INFO]
>
>**例：** 一部のデータタイプでは、ユーザーが特定の文字数を超えて入力できないようにします。 サブ文字列関数を使用して、値を特定の文字数に制限できます。
>
>この例では、サブ文字列関数は、プロジェクト名を 50 文字に制限します。
>
>![](assets/example-meet-length-restriction-350x184.png)

## ネスト関数

関数を相互にネストすることができます。

## 用途 [!DNL Google Sheets] 関数

If [!DNL Workfront Fusion] 使用したい関数が含まれていないが、が特集している [!DNL Google Sheets]を使用するには、次の手順に従います。

1. In [!DNL Google Sheets]」をクリックし、新しい空のスプレッドシートを作成します。
1. In [!DNL Workfront Fusion]、シナリオを開きます。
1. を **[!DNL Google Sheets]** >**[!UICONTROL セルの更新]** モジュールをシナリオに追加します。

   モジュールの追加手順については、 [シナリオへのモジュールの追加](../../workfront-fusion/scenarios/create-a-scenario.md#add) 記事内 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. モジュールの設定：

   1. で新しく作成したスプレッドシートを選択します。 **[!UICONTROL スプレッドシート]** フィールドに入力します。
   1. 次を含む数式を挿入します： [!DNL Google Sheets] 関数を **[!UICONTROL 値]** フィールドに入力します。

      通常どおり、先行モジュールの出力を使用できます。

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. を **[!UICONTROL Google Sheets] >[!UICONTROL セルを取得]** モジュールを使用して、計算結果を取得します。
1. 手順 4 で使用したのと同じセル ID を使用して、モジュールを設定します。

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
