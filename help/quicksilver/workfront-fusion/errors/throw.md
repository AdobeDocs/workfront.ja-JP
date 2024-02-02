---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Adobe Workfront Fusion でのエラー処理をスロー
description: 場合によっては、Adobe Workfront Fusion でシナリオの実行を強制的に停止し、その後でロールバックまたはコミットフェーズを実行したり、ルートの処理を停止して必要に応じて不完全な実行をビューのキューに格納し、不完全な実行を解決したりすることができます。
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: ht
source-wordcount: '384'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] でのエラー処理をスロー

場合によっては、シナリオの実行を強制的に停止して、その後で[ロールバック](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback)または[コミット](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit)フェーズを実行したり、ルートの処理を停止してオプションで不完全な実行をキューに格納したりすることができます。

現在、エラー処理ディレクティブは、[エラーハンドラールート](../../workfront-fusion/errors/error-handling.md#error)以外では使用できません。また、[!DNL Adobe Workfront Fusion] では、条件付きでエラーを簡単に生成（スロー）できるモジュールは提供されていません。

不完全な実行について詳しくは、[Adobe Workfront Fusion での不完全な実行の表示と解決](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)を参照してください。

エラー処理ディレクティブについて詳しくは、[エラー処理ディレクティブ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md)を参照してください。

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランがある場合、この記事で説明する機能を使用するには [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明する機能を使用するには、組織で [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] の管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## スローの回避策

条件付きでエラーをスローするために、オプションでモジュールを設定し、実行中に意図的にエラーを発生させることができます。その方法の 1 つは、[!UICONTROL JSON]／[!UICONTROL Parse JSON] モジュール（[JSON モジュール](../../workfront-fusion/apps-and-their-modules/json-modules.md)を参照）を使用して、オプションでエラーをスローするように設定することです（この場合は BundleValidationError を使用します）。

次に、エラー処理ディレクティブの 1 つをエラー処理ルートにアタッチして、以下の操作を行います。

* シナリオの実行を強制的に停止し、ロールバックフェーズを実行します：[!UICONTROL ロールバック]
* シナリオの実行を強制的に停止し、コミットフェーズを実行します：[!UICONTROL コミット]
* ルートの処理を停止します：[!UICONTROL 無視]
* ルートの処理を停止し、不完全な実行フォルダーのキューに保存します：[!UICONTROL 一時停止]

[!DNL Rollback] ディレクティブの使用例を以下に示します。

![](assets/rollback-directive-350x175.png)
