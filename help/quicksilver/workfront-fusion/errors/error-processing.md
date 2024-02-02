---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: ' [!DNL Adobe Workfront Fusion] でのエラー処理'
description: シナリオ実行中にエラーが発生する場合があります。この問題は通常、サービスへの接続に失敗したためにサービスが使用できない場合や、検証に失敗した場合に発生します。この記事では、発生する可能性のある一般的なエラーについて説明します。
author: Becky
feature: Workfront Fusion
exl-id: 468d7460-3853-4016-bff9-b9d3b87198ed
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: ht
source-wordcount: '1238'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] でのエラー処理

シナリオ実行中にエラーが発生する場合があります。この問題は通常、サービスへの接続に失敗したためにサービスが使用できない場合や、検証に失敗した場合に発生します。この記事では、発生する可能性のある一般的なエラーについて説明します。

[!DNL Adobe Workfront Fusion] は、いくつかの基本的なエラータイプを区別します。発生したエラーのタイプに応じて、反応が異なります。

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion]ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を、組織で購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 接続エラー

`ConnectionError`

接続エラーは、最も一般的なエラーの 1 つであり、様々な理由（過負荷、メンテナンス、停止など）によりサードパーティのサービスが利用できなくなることによって発生します。このエラーのデフォルトの処理方法は、発生したモジュールによって異なります。

* 最初のモジュールでエラーが発生した場合、シナリオの実行は警告メッセージとともに終了します。[!DNL Workfront Fusion] その後、時間間隔を増やしながら、シナリオを繰り返し再実行します（以下で説明します）。すべての試行が失敗した場合、[!DNL Workfront Fusion] がシナリオを非アクティブ化します。
* 最初のモジュール以外で接続エラーが発生した場合、後続の手順は、シナリオの詳細設定の「[不完全な実行の保存を許可](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow)」オプションによって異なります。

   * このオプションが有効な場合、シナリオの実行は[!UICONTROL 不完全な実行]フォルダーに移動され、このフォルダーで [!DNL Workfront Fusion] は、時間間隔を増やしながら、シナリオを繰り返し再実行しようとします。すべての試行が失敗した場合、不完全な実行フォルダーに実行が残り、ユーザーが手動で解決するのを待ちます。

     不完全な実行に関して詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) での不完全な実行の表示と解決を参照してください。
   * このオプションが無効になっている場合、シナリオの実行はエラーで終了し、ロールバックフェーズに移ります。その後、[!DNL Workfront Fusion] は時間間隔を増やしながら、繰り返しシナリオを再実行しようとします。すべての試行が失敗した場合、[!DNL Workfront Fusion] はシナリオを非アクティブ化します。

### 時間間隔の増加

エラー発生の際に試行の時間間隔を乗算的に増加させるアルゴリズムは、指数バックオフとして知られています。時間間隔を増加させるには、次のように設定します。

1. 10 分
1. 1 時間
1. 3 時間
1. 12 時間
1. 24 時間

[!DNL Workfront Fusion] で時間間隔を増加させる主な理由は、頻繁に実行されるシナリオが繰り返し失敗して、操作を消費するのを防ぐためです。

>[!INFO]
>
>**例：**
>
>シナリオには、[!DNL Google Sheets] トリガーの[!UICONTROL 行を監視]が含まれています。[!DNL Workfront Fusion] が起動したとき、[!DNL Google Sheets] はメンテナンスのため 30 分間使用できません。そのため、新しい行を取得できません。シナリオは停止し、10 分後に再試行します。[!DNL Google Sheets] がまだ使用できないため、[!DNL Workfront Fusion] は新しい行に関する情報をまだ取得できません。次回のシナリオの実行は、1 時間後にスケジュールされます。[!DNL Google Sheets] はこの時点で再び使用可能になり、シナリオは正常に実行されます。

## データエラー

`DataError`

項目が誤ってマッピングされ、[!DNL Workfront Fusion] サイドまたは使用されているサードパーティのサービスサイドで実行される検証を渡せない場合に、データエラーが生成されます。

このエラーが発生した場合、モジュールが失敗した位置までのシナリオが不完全な実行フォルダーに移動され、このフォルダーでイシューのトラブルシューティングを行えます。ただし、シナリオは停止せず、スケジュールに従って実行を続けます。データエラーが表示されたときにシナリオの実行を停止するには、シナリオ設定パネルの「順番に処理」オプションを有効にします。

シナリオ設定で「[!UICONTROL 不完全な実行の保存を許可]」オプションを有効にしていない場合、シナリオの実行はエラーで終了し、ロールバックが実行されます。

マッピングについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でのあるモジュールから別のモジュールへの情報のマッピングを参照してください。

不完全な実行について詳しくは、[Adobe Workfront Fusion での不完全な実行の表示と解決](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)を参照してください。

シナリオ設定パネルについて詳しくは、[Adobe Workfront Fusion のシナリオ設定パネル](../../workfront-fusion/scenarios/scenario-settings-panel.md)を参照してください。

スケジュールについて詳しくは、[Adobe Workfront Fusion でのシナリオのスケジュール](../../workfront-fusion/scenarios/schedule-a-scenario.md)を参照してください。

## 重複データエラー

`DuplicateDataError`

重複するデータを許可しないサービスに対して、[!DNL Workfront Fusion] が同じバンドルを 2 回挿入しようとすると、重複データエラーが生成されます。このエラーが発生した場合、[!DNL Workfront Fusion] はデータエラーの場合と同じ方法で処理します。

## 無効なアクセストークンエラー

`InvalidAccessTokenError`

サードパーティのサービスで登録されているアカウントに [!DNL Workfront Fusion] がアクセスできない場合に、無効なアクセストークンエラーが生成されます。このエラーが発生するのは通常、特定のサービスの管理において [!DNL Workfront Fusion] のアクセス権が取り消されたが、関連するシナリオがスケジュールに従って実行を続けている場合です。

このエラーが発生すると、シナリオの実行は直ちに停止します。エラーが発生したモジュール以降の残りのシナリオは、不完全な実行フォルダーに移動されます。

不完全な実行について詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) での不完全な実行の表示と解決を参照してください。

## レート制限エラー

`RateLimitError`

特定のサービスによって設定された制限を超えると、レート制限エラーが生成されます。このエラーが発生した場合、[!DNL Workfront Fusion] は接続エラーの場合と同じ方法で処理します。

詳しくは、[接続エラー](#connection-error)を参照してください。

## 不完全なデータエラー

`IncompleteDataError`

不完全なデータエラーは、トリガーでのみ発生します。トリガーが特定のサービスから必要なデータをダウンロードできなかった場合に、このエラーが生成されます。

シナリオが `IncompleteDataError` で終了した場合、それ以降の動作は「[!UICONTROL 連続エラーの最大数]」の設定によって変わります。

詳しくは、[Adobe Workfront Fusion のシナリオ設定パネル](../../workfront-fusion/scenarios/scenario-settings-panel.md)の記事にある[連続エラーの数](../../workfront-fusion/scenarios/scenario-settings-panel.md#number)を参照してください。

>[!INFO]
>
>**例：**
>
>シナリオには、ドキュメントを監視するように設定された、[!DNL Workfront] トリガーの[!UICONTROL レコードを監視]が含まれています。このシナリオは、長時間のビデオなどの大きなドキュメントのアップロード中に実行されます。[!UICONTROL Workfront Fusion] は、Workfront へのアップロードが続いている間にビデオをダウンロードしようとするため、シナリオは `IncompleteDataError` で終了します。

## 実行時エラー

`RuntimeError`

シナリオの実行中に（上記以外の）他のエラーが発生した場合は、`RunTimeError` としてレポートされます。

シナリオが `RuntimeError` で終了した場合、それ以降の動作は「[!UICONTROL 連続エラーの最大数]」の設定によって変わります。詳しくは、[Adobe Workfront Fusion のシナリオ設定パネル](../../workfront-fusion/scenarios/scenario-settings-panel.md)の記事にある[連続エラーの数](../../workfront-fusion/scenarios/scenario-settings-panel.md#number)を参照してください。

>[!NOTE]
>
>シナリオがインスタントトリガーで始まる場合、[!UICONTROL 連続エラーの最大数]の設定が無視され、最初のエラーが発生するとシナリオは直ちに非アクティブ化されます。詳しくは、[モジュールの種類](../../workfront-fusion/modules/module-types.md)の記事にある[インスタントトリガー](../../workfront-fusion/modules/module-types.md#instant)を参照してください。

## 不整合エラー

`InconsistencyError`

コミットまたはロールバックフェーズ中に上記のエラーが発生した場合、シナリオが不整合エラーで終了します。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md) でのシナリオの実行、サイクル、フェーズを参照してください。

このエラーがシナリオに表示された場合、シナリオの実行は直ちに停止します。

## 警告

シナリオの実行中に、問題を知らせる警告が表示される場合があります。しかし、シナリオの成功を妨げるものではありません。

例えば、最大許容ファイルサイズを超え、[!UICONTROL データ損失を有効にする]オプションが無効になっている場合、警告が表示されることがあります。詳しくは、[Adobe Workfront Fusion のシナリオ設定パネル](../../workfront-fusion/scenarios/scenario-settings-panel.md)の記事にある[データ損失を有効にする](../../workfront-fusion/scenarios/scenario-settings-panel.md#enable)を参照してください。
