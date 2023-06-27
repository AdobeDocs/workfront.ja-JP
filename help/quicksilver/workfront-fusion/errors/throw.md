---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: Adobe Workfront Fusion でのエラー処理のスロー
description: 場合によっては、シナリオの実行を強制的に停止し、ロールバックまたはコミットフェーズを実行するか、ルートの処理を停止し、必要に応じてAdobe Workfront Fusion で未完了の実行を表示のキューに格納します。
author: Becky
feature: Workfront Fusion
exl-id: 6258bd4d-31a0-4fbb-b1b4-8e9a5a9dbe36
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 0%

---

# でのエラー処理をスロー [!DNL Adobe Workfront Fusion]

場合によっては、シナリオの実行を強制的に停止し、その後に [ロールバック](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback) または [コミット](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit) ルートの処理を停止するか、（オプションで）不完全な実行のキューに格納するかを選択します。

現在、エラー処理ディレクティブは、 [エラーハンドラールート](../../workfront-fusion/errors/error-handling.md#error) および [!DNL Adobe Workfront Fusion] では、条件付きで簡単にエラーを生成（スロー）できるモジュールは提供されません。

実行が不完全な場合について詳しくは、 [Adobe Workfront Fusion での不完全な実行の表示と解決](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

エラー処理ディレクティブについて詳しくは、 [でのエラー処理用のディレクティブ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/directives-for-error-handling.md).

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

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion licenses]](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## スローの回避策

条件付きでエラーをスローするには、モジュールを設定して、オプションで、その処理中に意図的にエラーが発生するようにします。 1 つの可能性は、 [!UICONTROL JSON] > [!UICONTROL JSON を解析] モジュール ( [JSON モジュール](../../workfront-fusion/apps-and-their-modules/json-modules.md)) の代わりに、オプションでエラーをスローするように設定されます（この場合、BundleValidationError）。

次に、エラー処理ディレクティブの 1 つを次のエラー処理ルートにアタッチできます。

* シナリオの実行を強制的に停止し、ロールバック・フェーズを実行します。 [!UICONTROL ロールバック]
* シナリオの実行を強制的に停止し、コミットフェーズを実行します。 [!UICONTROL コミット]
* ルートの処理を停止します。 [!UICONTROL 無視]
* ルートの処理を停止し、不完全な実行のキューフォルダーに保存します。 [!UICONTROL 改行]

次の例は、 [!DNL Rollback] ディレクティブ：

![](assets/rollback-directive-350x175.png)
