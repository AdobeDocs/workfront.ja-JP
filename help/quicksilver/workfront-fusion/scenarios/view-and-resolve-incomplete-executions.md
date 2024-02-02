---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: ' [!DNL Adobe Workfront Fusion] で未完了の実行を表示し解決する'
description: 「[!UICONTROL 未完了の実行]」フォルダーには、エラーが原因で正常に終了されなかったシナリオの実行が保存されます。保存された未完了の実行は、手動または自動で解決できます。
author: Becky
feature: Workfront Fusion
exl-id: 60fcda91-b725-4ada-a42c-5c05720d68c2
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '626'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] で未完了の実行を表示し解決する

「[!UICONTROL 未完了の実行]」フォルダーには、エラーが原因で正常に終了されなかったシナリオの実行が保存されます。保存された未完了の実行は、手動または自動で解決できます。

>[!NOTE]
>
>デフォルトでは、未完了の実行の保存は無効になっています。有効にするには、シナリオの詳細設定で「[!UICONTROL 未完了の実行の保存を許可]」オプションを有効にします。
>
>シナリオ設定について詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md) のシナリオ設定パネルを参照してください。

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
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]、[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織が [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は [!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明されている機能を使用するには、組織が [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについては、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 未完了の実行を表示

モジュールの処理中にエラーが発生した場合、新しい未完了の実行が「未完了の実行」フォルダーに追加されます。未完了の実行にはそれぞれ、シナリオのブループリントと、失敗したモジュールにマッピングできるすべてのバンドルが含まれます。未完了の実行のリストを開くには、シナリオの詳細ページで「[!UICONTROL 未完了の実行]」タブをクリックします。

![](assets/incomplete-executions-tab-350x102.png)

詳しくは、[未完了の実行になるエラー](#errors-resulting-into-incomplete-executions)を参照してください。

>[!NOTE]
>
>組織ごとの未解決の未完了の実行フォルダーに対する現在のサイズ制限は 500 MB です。組織がこの制限を超えると、次のエラーが表示される場合があります。
>
>`"There is NOT ENOUGH SPACE to add a bundle to the IEQ. The reason is: Too many incomplete executions."`
>
>詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md) のシナリオ設定パネルの[データ損失を有効にする](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable)を参照してください。

## 未完了の実行を解決

新しい未完了の実行が保存された場合、次のように解決できます。

1. 「**[!UICONTROL 未完了の実行]**」タブをクリックします。
1. 解決したい未完了の実行を見つけ、「**[!UICONTROL 詳細]**」をクリックします。


   未完了の実行を解決しようとする前に、すべてのモジュールの操作のログを確認したい場合は、「[!UICONTROL 履歴]」フォルダーから未完了の実行を解決できます。

1. 「**[!UICONTROL 履歴]**」タブをクリックします。
1. シナリオの失敗した実行ログを見つけ、「**[!UICONTROL 詳細]**」をクリックします。
1. モジュールのログを開くと、モジュールのすべての操作が表示されます。
1. 失敗した操作を見つけ、「**[!UICONTROL 解決]**」をクリックします。

   ![](assets/resolve-btn-350x188.png)

## 未完了の実行に関連するオプション

[!UICONTROL シナリオ設定]パネルの次のオプションは、未完了の実行を保存するかどうかと、その方法を決定します。

* 未完了の実行の保存を許可
* 順次処理
* データ損失を有効にする

これらのオプションについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-settings-panel.md) のシナリオ設定パネルを参照してください。

## 未完了の実行になるエラー

未完了の実行が保存される原因となるエラーには、いくつかのカテゴリがあります。次のものが含まれます。

* 不完全なデータや誤ったデータから発生する検証エラー。主に、モジュールを通過するすべてのデータを正常に処理するために予期される項目が欠落していることが原因です。
* 最終的な宛先が使用できなかったことから発生するエラー。一時的または長期的な接続障害（メールまたはリモート FTP サーバーへの接続中など）が原因です。

シナリオの最初のモジュールでエラーが発生した場合、実行は直ちに停止し、未完了の実行は保存されません。

他のモジュールでエラーが発生し、エラーハンドラールートが添付されていない場合は、次のいずれかが発生します。

* エラータイプが `ConnectionError`、`RateLimitError`、`OutOfSpaceError`、または `ModuleTimeoutError` の場合、自動再試行付きの未完了の実行レコードが保存されます。
* エラータイプが `DataError`、`InvalidConfigurationError`、`InvalidAccessTokenError`、`UnexpectedError`、`MaxFileSizeExceededError`、または `MaxResultsExceededError` の場合、自動再試行なしの未完了の実行レコードが保存されます。
* エラータイプが上記以外の場合、実行は失敗します。
