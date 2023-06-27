---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: での不完全な実行の表示と解決 [!DNL Adobe Workfront Fusion]
description: この [!UICONTROL 実行が不完全です] フォルダーには、エラーが原因で正常にファイナライズされなかったシナリオの実行が格納されます。 保存された不完全な実行は、手動または自動で解決できます。
author: Becky
feature: Workfront Fusion
exl-id: 60fcda91-b725-4ada-a42c-5c05720d68c2
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '626'
ht-degree: 5%

---

# での不完全な実行の表示と解決 [!DNL Adobe Workfront Fusion]

この [!UICONTROL 実行が不完全です] フォルダーには、エラーが原因で正常にファイナライズされなかったシナリオの実行が格納されます。 保存された不完全な実行は、手動または自動で解決できます。

>[!NOTE]
>
>デフォルトでは、実行が不完全な場合、保存は無効になります。 有効にするには、 [!UICONTROL 不完全な実行の保存を許可] 」オプションを使用します。
>
>シナリオ設定の詳細については、 [のシナリオ設定パネル [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

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
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] [!UICONTROL] の [!UICONTROL] [!DNL Workfront Fusion] 自動化 (WA)</p>
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

## 実行が不完全であることを表示

モジュールの処理中にエラーが発生した場合、未完了の新しい実行が「未完了の実行」フォルダーに追加されます。 各不完全な実行には、シナリオのブループリントと、失敗したモジュールにマッピングできるすべてのバンドルが含まれます。 不完全な実行のリストを開くには、 [!UICONTROL 実行が不完全です] タブをクリックします。

![](assets/incomplete-executions-tab-350x102.png)

詳しくは、 [実行が不完全になるエラー](#errors-resulting-into-incomplete-executions).

>[!NOTE]
>
>組織ごとの未解決の不完全な実行フォルダーの現在のサイズ制限は 500 MB です。 組織がこの制限を超えると、次のエラーが発生する場合があります。
>
>`"There is NOT ENOUGH SPACE to add a bundle to the IEQ. The reason is: Too many incomplete executions."`
>
>詳しくは、 [データ損失を有効にする](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) in [のシナリオ設定パネル [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## 不完全な実行の解決

新しい不完全な実行が保存された場合、次のように解決できます。

1. 次をクリック： **[!UICONTROL 実行が不完全です]** タブをクリックします。
1. 解決したい不完全な実行を見つけ、 **[!UICONTROL 詳細]**.


   不完全な実行を解決する前に、すべてのモジュールの操作のログを確認したい場合は、 [!UICONTROL 履歴] フォルダー：

1. 次をクリック： **[!UICONTROL 履歴]** タブをクリックします。
1. シナリオの失敗した実行ログを探し、 **[!UICONTROL 詳細]**.
1. モジュールのログを開き、モジュールのすべての操作が表示されます。
1. 失敗した操作を見つけ、 **[!UICONTROL 解決]**:

   ![](assets/resolve-btn-350x188.png)

## 実行が不完全なことに関連するオプション

次のオプション ( [!UICONTROL シナリオ設定] パネルは、不完全な実行が保存されるかどうかと、その方法を決定します。

* 不完全な実行の保存を許可
* 順次処理
* データ損失を有効にする

これらのオプションについて詳しくは、 [のシナリオ設定パネル [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md).

## 実行が不完全になるエラー

エラーには、不完全な実行の保存につながるいくつかのカテゴリがあります。 次のものが含まれます。

* 不完全または誤ったデータに起因する検証エラー。主に、モジュールを経由するすべてのデータを正しく処理するために予期される項目が見つからないことが原因です。
* 一時的または長期的な接続障害（電子メールまたはリモート FTP サーバーへの接続中など）が原因で、最終的な宛先が使用できなかったことから発生するエラー。

シナリオの最初のモジュールでエラーが発生した場合、実行は直ちに停止し、不完全な実行は保存されません。

他のモジュールでエラーが発生し、エラーハンドラールートがアタッチされていない場合は、次のいずれかが発生します。

* エラータイプが `ConnectionError`, `RateLimitError`, `OutOfSpaceError` または `ModuleTimeoutError`に設定されている場合、自動再試行を含む不完全な実行レコードが保存されます。
* エラータイプが `DataError`, `InvalidConfigurationError`, `InvalidAccessTokenError`, `UnexpectedError`, `MaxFileSizeExceededError`または `MaxResultsExceededError`を指定した場合、自動再試行のない不完全な実行レコードが保存されます。
* エラータイプが上記以外の場合、実行は失敗します。
