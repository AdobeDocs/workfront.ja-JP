---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: でのエラー処理 [!DNL Adobe Workfront Fusion]
description: シナリオの実行中にエラーが発生する場合があります。 この問題は、通常、サービスへの接続に失敗したためにサービスが使用できない場合や、検証に失敗した場合に発生します。 この記事では、発生する可能性のある一般的なエラーについて説明します。
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '1191'
ht-degree: 0%

---

# でのエラー処理 [!DNL Adobe Workfront Fusion]

シナリオの実行中にエラーが発生する場合があります。 この問題は、通常、サービスへの接続に失敗したためにサービスが使用できない場合や、検証に失敗した場合に発生します。 この記事では、発生する可能性のある一般的なエラーについて説明します。

[!DNL Adobe Workfront Fusion] は、いくつかの基本的なエラータイプを区別します。 発生したエラーのタイプに応じて、応答は異なります。

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

## 接続エラー

`ConnectionError`

接続エラーは、様々な理由（過負荷、メンテナンス、停止など）によるサードパーティのサービスの利用不可によって発生する、最も一般的なエラーの 1 つです。 このエラーのデフォルトの処理方法は、発生したモジュールによって異なります。

* 最初のモジュールでエラーが発生した場合、シナリオの実行は警告メッセージで終了します。 [!DNL Workfront Fusion] その後、時間間隔を増やして、シナリオを繰り返し再実行します（以下で説明します）。 すべての試みが失敗した場合、 [!DNL Workfront Fusion] シナリオを非アクティブ化します。
* 最初のモジュール以外で接続エラーが発生した場合、以降の手順は [不完全な実行の保存を許可](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) オプションを使用します。

   * このオプションが有効な場合、シナリオの実行は [!UICONTROL 実行が不完全です] フォルダ [!DNL Workfront Fusion] は、時間間隔を増やして、シナリオを繰り返し再実行しようとします。 すべての試行が失敗した場合、実行は [での不完全な実行の表示と解決 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) ユーザーが手動で解決するのを待っているフォルダー。
   * このオプションを無効にした場合、シナリオの実行はエラーで終わり、ロールバックフェーズが続きます。 [!DNL Workfront Fusion] その後、時間間隔を増やして、繰り返しシナリオの再実行を試みます。 すべての試みが失敗した場合、 [!DNL Workfront Fusion] シナリオを非アクティブ化します。

### 時間間隔の増加

エラーが発生した時間間隔を乗算的に増やすアルゴリズムは、指数バックオフと呼ばれます。 増加する時間間隔は、次のように設定します。

1. 10 分
1. 1 時間
1. 3 時間
1. 12 時間
1. 24 時間

時間間隔を増やす主な理由は [!DNL Workfront Fusion] は、頻繁に実行されるシナリオが、失敗した試行を繰り返し実行したときに操作を消費するのを防ぐためです。

>[!INFO]
>
>**例:**
>
>シナリオには、 [!DNL Google Sheets] トリガー [!UICONTROL 監視行]. [!DNL Google Sheets] は、 [!DNL Workfront Fusion] はシナリオを開始するので、新しい行を取得できません。 シナリオは停止し、10 分後に再試行します。 この期間内にサービスが利用できない状態が続くため、 [!DNL Workfront Fusion] は、まだ新しい行に関する情報を取得できません。 次回のシナリオの実行は、1 時間でスケジュールされます。 [!DNL Google Sheets] はこの時間内に再び使用可能になり、シナリオは正常に実行されます。

## データエラー

`DataError`

項目が誤ってマッピングされ、 [!DNL Workfront Fusion] サイドまたはサードパーティのサービスのサイドで使用されます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

このエラーが発生した場合は、モジュールが失敗した場所までのシナリオが不完全な実行フォルダーに移動し、このフォルダーで問題のトラブルシューティングをおこなうことができます。 ただし、シナリオは停止せず、スケジュールに従って実行を続けます。 データエラーが表示されたときにシナリオの実行を停止するには、シナリオ設定パネルの「順次処理」オプションを有効にします。

を有効にしていない場合、 [!UICONTROL 不完全な実行の保存を許可] オプションを選択すると、シナリオの実行はエラーで終了し、ロールバックが実行されます。

実行が不完全な場合について詳しくは、 [Adobe Workfront Fusion での不完全な実行の表示と解決](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

シナリオ設定パネルについて詳しくは、 [Adobe Workfront Fusion のシナリオ設定パネル](../../workfront-fusion/scenarios/scenario-settings-panel.md).

スケジュールについて詳しくは、 [Adobe Workfront Fusion でのシナリオのスケジュール](../../workfront-fusion/scenarios/schedule-a-scenario.md).

## 重複データエラー

`DuplicateDataError`

If [!DNL Workfront Fusion] 重複データを許可しないサービスに対して、同じバンドルを 2 回挿入しようとすると、重複データエラーが生成されます。 このエラーが発生した場合、 [!DNL Workfront Fusion] は、データエラーの場合と同じ方法で実行されます。

## 無効なアクセストークンエラー

`InvalidAccessTokenError`

無効なアクセストークンエラーは、 [!DNL Workfront Fusion] は、サードパーティのサービスに登録されているアカウントにアクセスできません。 これは主に、 [!DNL Workfront Fusion] 特定のサービスの管理では、関連するシナリオは、スケジュールに従って実行を続けます。

このエラーが発生すると、シナリオの実行は直ちに停止します。 エラーが発生したモジュール以降の残りのシナリオは、不完全な実行フォルダーに移動されます。

実行が不完全な場合について詳しくは、 [での不完全な実行の表示と解決 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

## レート制限エラー

`RateLimitError`

特定のサービスによって設定された制限を超えると、レート制限エラーが発生します。 このエラーが発生した場合、 [!DNL Workfront Fusion] は、接続エラーの場合と同じ方法で実行されます。 詳しくは、 [接続エラー](#connection-error).

## 不完全なデータエラー

`IncompleteDataError`

不完全なデータエラーは、エラーでのみトリガーします。 このエラーは、トリガーが特定のサービスから必要なデータをダウンロードできなかった場合に生成されます。

シナリオが `IncompleteDataError`の場合、その以降の動作は設定によって異なります [!UICONTROL 連続エラーの最大数]. 詳しくは、 [連続エラー数](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) 記事内 [Adobe Workfront Fusion のシナリオ設定パネル](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!INFO]
>
>**例：** シナリオには [!DNL Workfront] トリガー [!UICONTROL レコードを監視] ドキュメントを監視するように設定します。 このシナリオは、長いビデオなどの大きなドキュメントをアップロードする際に実行されます。 理由： [!UICONTROL Workfront Fusion] Workfrontへのアップロード中にビデオのダウンロードを試みると、シナリオは `IncompleteDataError`.

## 実行時エラー

`RuntimeError`

シナリオの実行中に他のエラー（前述の説明がない）が発生した場合は、 `RunTimeError`.

シナリオが `RuntimeError`の場合、その以降の動作は設定によって異なります [!UICONTROL 連続エラーの最大数]. 詳しくは、 [連続エラー数](../../workfront-fusion/scenarios/scenario-settings-panel.md#number) 記事内 [Adobe Workfront Fusion のシナリオ設定パネル](../../workfront-fusion/scenarios/scenario-settings-panel.md).

>[!NOTE]
>
>シナリオがインスタントトリガーで始まる場合、 [!UICONTROL 連続エラーの最大数] が無視され、最初のエラーが発生すると、シナリオは直ちに非アクティブ化されます。 詳しくは、 [インスタントトリガー](../../workfront-fusion/modules/module-types.md#instant) 記事内 [モジュールのタイプ](../../workfront-fusion/modules/module-types.md).

## 不整合エラー

`InconsistencyError`

コミットまたはロールバックフェーズ中に上記のエラーが発生した場合は、矛盾エラーでシナリオが終了します。 詳しくは、 [のシナリオの実行、サイクル、フェーズ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

このエラーがシナリオに表示された場合、シナリオの実行は直ちに停止されます。

## 警告

シナリオの実行中に、問題を知らせる警告が表示される場合があります。 ただし、シナリオが正常に完了するのを防ぐことはできません。

例えば、許可されているファイルの最大サイズを超え、 [!UICONTROL データ損失を有効にする] オプションは無効です。 詳しくは、 [データ損失を有効にする](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable) 記事内 [Adobe Workfront Fusion のシナリオ設定パネル](../../workfront-fusion/scenarios/scenario-settings-panel.md).
