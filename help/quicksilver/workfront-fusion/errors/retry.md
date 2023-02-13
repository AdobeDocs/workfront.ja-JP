---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: での再試行エラー処理 [!DNL Adobe Workfront Fusion]
description: 場合によっては、失敗の理由が時間の経過と共に渡る可能性がある場合に、障害が発生したモジュールを数回再実行すると便利です。
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '639'
ht-degree: 0%

---

# での再試行エラー処理 [!DNL Adobe Workfront Fusion]

場合によっては、失敗の理由が時間の経過と共に渡る可能性がある場合に、失敗したモジュールを再実行すると便利です。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p><p>[!UICONTROL [!DNL Workfront Fusion] 自動化 (WA)</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## の [!UICONTROL 再試行] エラー処理指令

[!UICONTROL Adobe Workfront Fusion] は現在、 [!UICONTROL 再試行] エラー処理ディレクティブですが、機能を模倣するために 2 つの回避策を使用できます。 詳しくは、 [Adobe Workfront Fusion でのエラー処理用ディレクティブ](../../workfront-fusion/errors/directives-for-error-handling.md).

### 以下を使用： [!UICONTROL 改行] 指令

1. シナリオ設定パネルで、 **[!UICONTROL 不完全な実行の保存を許可]** オプション。

   詳しくは、 [のシナリオ設定パネル [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

1. モジュールにエラーハンドラルートをアタッチします。詳しくは、 [でのエラー処理 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md).
1. リンク [!UICONTROL 改行] ディレクティブをエラーハンドラールートに追加し、設定します。

   詳しくは、 [でのエラー処理用のディレクティブ [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

   ![](assets/break-directive-350x241.png)

#### 欠点

* 再試行間隔の最小値は 1 分です。
* モジュールが複数のバンドルを処理していて、バンドルの処理が失敗した場合、部分的な実行（エラーが発生したバンドルのみ）は不完全な実行フォルダーに移動され、 [!UICONTROL 改行] ディレクティブ設定。 ただし、現在の実行は続き、モジュールは後続のバンドルを引き続き処理します。 「[!UICONTROL 順次処理]」オプションが [!UICONTROL シナリオ設定] :「実行が不完全です」フォルダーに保存されている実行が正常に解決されるまで、シナリオが再実行されないようにします。

実行が不完全な場合について詳しくは、 [での不完全な実行の表示と解決 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### 以下を使用： [!UICONTROL リピーター] モジュール

1. 使用する **[!UICONTROL リピーター]** モジュールとその設定 [!UICONTROL 繰り返し] フィールドに最大試行回数を入力します。
1. 問題が発生する可能性のあるモジュールを **[!UICONTROL リピーター]** モジュール。
1. このモジュールにエラーハンドラールートをアタッチします ( [でのエラー処理 [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md)) をクリックします。
1. リンク **[!UICONTROL ツール] > [!UICONTROL スリープ]** モジュールをエラーハンドラルートに追加し、その **[!UICONTROL 遅延]** フィールドに、試行間の秒数を入力します。

1. リンク **[!UICONTROL 無視]** 指令が **[!UICONTROL ツール] > [!UICONTROL スリープ]** モジュール ( [Adobe Workfront Fusion でのエラー処理用ディレクティブ](../../workfront-fusion/errors/directives-for-error-handling.md)) をクリックします。

1. リンク **[!UICONTROL ツール] > [!UICONTROL 変数を設定]** モジュールに追加し、モジュールの結果をという名前の変数に格納するように設定します。例： `Result`.

1. リンク **[!UICONTROL 配列の集約]** モジュールの後 **[!UICONTROL ツール] > [!UICONTROL 変数を設定]** を選択し、 **[!DNL Repeater]** モジュールを選択します。

1. リンク **[!UICONTROL ツール] > [!UICONTROL 変数を取得]** モジュールを **[!UICONTROL 配列の集約]** モジュールを作成し、 `Result` 変数を使用します。

1. を **[!UICONTROL ツール] > [!UICONTROL 変数を取得]** 間のモジュール **[!UICONTROL リピーター]** モジュールと、問題が発生する可能性のあるモジュールを参照し、それを設定して、 `Result` 変数を使用します。

1. この間にフィルターを挿入 **[!UICONTROL ツール] > [!UICONTROL 変数を取得]** モジュールと、潜在的に失敗するモジュールは、 `Result` 変数が存在しません。

>[!INFO]
>
>**例：** 以下に、 [!UICONTROL HTTP] >[!UICONTROL リクエストを実行] モジュールは、問題が発生する可能性があるモジュールを表します。
>
>![](assets/http-make-request-350x116.png)
>
>モジュールの失敗の可能性の結果が複雑すぎて、単純な変数に格納できない場合は、データストアを使用して結果を保存または取得できます。 データストアには、1 つのレコードのみが含まれます。 レコードのキーは、例えば、 `Result`.
>
>データストアの詳細については、 [のデータストア [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

#### ドローバック

この回避策は、少し複雑すぎるように見える場合があり、操作の面でもより厳しくなります。
