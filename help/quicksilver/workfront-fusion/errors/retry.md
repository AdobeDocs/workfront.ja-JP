---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: ' [!DNL Adobe Workfront Fusion] でエラー処理を再試行します'
description: 失敗の原因が時間の経過とともに解消される可能性がある場合は、失敗したモジュールを数回再実行すると便利です。
author: Becky
feature: Workfront Fusion
exl-id: 1058905c-6c95-4a8c-8956-e1606f1486d9
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: ht
source-wordcount: '683'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] でエラー処理を再試行します

失敗の原因が時間の経過とともに解消される可能性がある場合は、失敗したモジュールを再実行すると便利です。

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件はありません。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランがある場合、この記事で説明する機能を使用するには、組織は [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明する機能を使用するには、組織は [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] のライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  のライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## [!UICONTROL 再試行]エラー処理ディレクティブの回避策

[!UICONTROL Adobe Workfront Fusion] は現在、[!UICONTROL 再試行]エラー処理ディレクティブを提供していませんが、その機能を模倣するために 2 つの回避策を採用できます。詳しくは、[Adobe Workfront Fusion でのエラー処理のディレクティブ](../../workfront-fusion/errors/directives-for-error-handling.md)を参照してください。

### [!UICONTROL 一時停止]ディレクティブを使用

1. シナリオ設定パネルで、「**[!UICONTROL 未完了の実行の保存を許可]**」オプションを有効にします。

   詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md)のシナリオ設定パネルを参照してください。

1. [[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-handling.md) でのエラー処理の説明に従って、エラーハンドラールートをモジュールにアタッチします。
1. [!UICONTROL 一時停止]ディレクティブをエラーハンドラールートにリンクし、構成します。

   詳しくは、[[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md) でのエラー処理のディレクティブを参照してください。

   ![](assets/break-directive-350x241.png)

#### 欠点

* 最小再試行間隔は 1 分です。
* モジュールが複数のバンドルを処理していて、バンドルの処理が失敗した場合、部分的な実行（エラーの原因となったバンドルのみ）が未完了の実行フォルダーに移動され、[!UICONTROL 一時停止]ディレクティブの設定に従って再試行がスケジュールされます。ただし、現在の実行は続行され、モジュールは後続のバンドルの処理を続行します。[!UICONTROL シナリオ設定]で「[!UICONTROL 順次処理]」オプションを有効にすると、未完了の実行フォルダーに保存されている実行が正常に解決されるまでシナリオが再実行されないようにすることができます。

  未完了の実行について詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) での未完了の実行の表示と解決を参照してください。

### [!UICONTROL リピーター]モジュールを使用する

1. **[!UICONTROL リピーター]**&#x200B;モジュールを使用し、その&#x200B;**[!UICONTROL 繰り返し]**&#x200B;フィールドを最大試行回数に設定します。
1. 障害が発生する可能性があるモジュールを&#x200B;**[!UICONTROL リピーター]**&#x200B;モジュールにリンクします。
1. エラーハンドラールートをこのモジュールにアタッチします（[ [!DNL Adobe Workfront Fusio]n](../../workfront-fusion/errors/error-handling.md) のエラー処理を参照）。
1. **[!UICONTROL ツール]／[!UICONTROL スリープ]**&#x200B;モジュールをエラーハンドラールートにリンクし、その **[!UICONTROL 遅延]**&#x200B;フィールドを試行間の秒数に設定します。

1. **[!UICONTROL 無視]**&#x200B;ディレクティブを&#x200B;**[!UICONTROL ツール]／[!UICONTROL スリープ]**&#x200B;モジュールの後にリンクします（[Adobe Workfront Fusion でのエラー処理のディレクティブ](../../workfront-fusion/errors/directives-for-error-handling.md)を参照）

1. **[!UICONTROL ツール]／[!UICONTROL 変数設定]**&#x200B;モジュールを失敗する可能性のあるモジュールの後にリンクし、モジュールの結果を `Result` などの名前の変数に保存するように構成します。

1. **[!UICONTROL ツール]／[!UICONTROL 変数の設定]**&#x200B;に移動してからに「**[!UICONTROL 配列アグリゲータ]**」モジュールをリンクし、ソースモジュールフィールドで&#x200B;**[!DNL Repeater]**&#x200B;モジュールを選択します。

1. **[!UICONTROL ツール]／[!UICONTROL 変数の取得]**&#x200B;モジュールを「**[!UICONTROL 配列アグリゲーター]**」モジュールにリンクし、`Result` 変数の値を取得するように構成します。

1. **[!UICONTROL ツール]／[!UICONTROL 変数の取得]**&#x200B;モジュールを&#x200B;**[!UICONTROL リピーター]**&#x200B;モジュールと障害が発生する可能性のあるモジュールの間に挿入し、`Result` の値を取得するように構成します。

1. `Result` 変数が存在しない場合にのみ続行するには、この&#x200B;**[!UICONTROL ツール]／[!UICONTROL 変数の取得]**&#x200B;モジュールと失敗する可能性があるモジュールの間にフィルターを挿入します。

>[!INFO]
>
>**例：** 以下は、[!UICONTROL HTTP]／[!UICONTROL リクエストを作成]モジュールが失敗する可能性のあるモジュールを表すサンプルシナリオです。
>
>![](assets/http-make-request-350x116.png)
>
>失敗する可能性があるモジュールの結果が複雑すぎて単純な変数に格納できない場合は、データストアを使用して結果を格納/取得できます。データストアにはレコードが 1 つだけ含まれます。レコードのキーは、例えば `Result` などです。
>
>データストアについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md) のデータストアを参照してください。

#### 欠点

この回避策は少し複雑すぎるように見えるかもしれませんし、操作の面でも要求がより厳しくなっています。
