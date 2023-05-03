---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: でのエラー処理用のディレクティブ [!DNL Adobe Workfront Fusion]
description: この記事では、 [!DNL Adobe Workfront Fusion] シナリオ。
author: Becky
feature: Workfront Fusion
exl-id: dcf4f7e3-78d8-4eb4-9483-8a1c18b0e436
source-git-commit: f4e43d34068c987755559573b4ecd618ff710686
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 14%

---

# でのエラー処理用のディレクティブ [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## エラー処理用のディレクティブ

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>ロールバック</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>シナリオの実行は直ちに停止し、 <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref">ロールバック</a> フェーズは、すべてのモジュールで開始され、すべてのモジュールを初期状態に戻そうとします。 後続のモジュールは処理されません。</p> <p>いくつかのエラータイプがある場合、シナリオは、シナリオ設定で指定された連続するエラーの数の後で無効化されます。 詳しくは、 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref">連続エラー数</a>.</p> <p>シナリオの実行ステータスは「エラー」とマークされます。</p> <p>注意：これは、モジュールと <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">[!UICONTROL 不完全な実行の保存を許可 ]</a> [!UICONTROL シナリオ設定 ] の設定がオンになっていません。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>コミット</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>シナリオの実行は直ちに停止し、すべてのモジュールでコミットフェーズが開始します。 後続のモジュールは処理されません。</p> <p>未処理のバンドルはすべて無視されます。</p> <p>シナリオの実行ステータスは「成功」とマークされます。コミットフェーズの詳細については、 <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref">コミット</a> 記事内 <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Adobe Workfront Fusion のシナリオの実行、サイクル、フェーズ</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>再開</p> <p> <img src="assets/resume.png"> </p> </td> 
   <td> <p>エラーが発生したモジュールに代替出力が指定され、提供されます。</p> <p>以降のモジュールが処理されます。</p> <p>シナリオの実行ステータスは「成功」とマークされます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>無視</p> <p> <img src="assets/ignore.png"> </p> </td> 
   <td> <p>エラーは無視され、後続のモジュールは処理されません。</p> <p>未処理のバンドルがある場合、シナリオの実行は通常どおり続行されます。</p> <p>シナリオの実行ステータスは「成功」とマークされます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>一時停止</p> <p> <img src="assets/break.png"> </p> </td> 
   <td> <p>シナリオの実行状態は、不完全な実行のキューに保存されます。このキューでは、エラーを手動で解決できます。 詳しくは、 <a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref">Adobe Workfront Fusion での不完全な実行の表示と解決</a>. </p> <p>しかし、いくつかの例外があります。 詳しくは、 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">不完全な実行の保存を許可</a> 記事内 <a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Adobe Workfront Fusion のシナリオ設定パネル</a>.</p> <p>後続のモジュールは処理されません。</p> <p>未処理のバンドルがある場合、シナリオの実行は通常どおり続行されます。</p> <p>[!UICONTROL 自動実行を完了 ] オプションが無効になっている場合、シナリオの実行ステータスは「警告」とマークされます。</p> <p>詳しくは、 <a href="#break" class="MCXref xref">[!UICONTROL 分割 ]</a> 詳しくは、以下の節を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>再試行</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>場合によっては、失敗の理由が時間の経過と共に渡る可能性がある場合に、障害が発生したモジュールを数回再実行すると便利です。</p> <p>現在、Workfront Fusion では Retry ディレクティブは提供されていませんが、機能を模倣するために、いくつかの回避策を使用できます。 詳しくは、 <a href="../../workfront-fusion/errors/retry.md" class="MCXref xref">Adobe Workfront Fusion での再試行エラー処理</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* 現在、エラー処理ディレクティブは、エラー処理ルート以外では使用できません。
   >
   >   詳しくは、 [エラーハンドラールート](../../workfront-fusion/errors/error-handling.md#error) 記事内 [Adobe Workfront Fusion でのエラー処理](../../workfront-fusion/errors/error-handling.md).
>* [!DNL Workfront Fusion] では、現在、条件付きで簡単にエラーを生成（スロー）できる Throw モジュールは提供していませんが、機能を模した回避策を使用できます。
   >
   >   詳しくは、 [スローの回避策](../../workfront-fusion/errors/throw.md#workaround-for-throw) 記事内 [Adobe Workfront Fusion でのエラー処理のスロー](../../workfront-fusion/errors/throw.md).


## 一時停止 {#break}

エラーが [!DNL Break] ディレクティブの場合、レコードは不完全な実行フォルダーに作成されます。 このレコードには、シナリオの実行の状態と共に、前のモジュールのデータが格納されます。 レコードは、エラーが発生したモジュールを参照し、モジュールが受け取ったデータに関する情報を入力として含みます。 エラーの原因となるデータのバンドルごとに、別のレコードが作成されます。

詳しくは、 [Adobe Workfront Fusion での不完全な実行の表示と解決](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md).

### Break ディレクティブによって発生したエラーを解決する

シナリオを更新し（必要に応じて）1 回実行することで、手動でエラーを解決できます。

また、シナリオを再実行することで、不完全な実行を自動的に処理するようにシナリオを設定することもできます。 不完全な実行を処理するようにモジュールを設定するには：

1. Break モジュール内で、 [!UICONTROL **自動的に実行を完了**] オプション。
1. 内 **試行回数** フィールドに値を入力するか、モジュールが実行を再試行する最大試行回数を入力またはマップします

   この数は 1 ～ 100 の範囲で指定する必要があります。
1. 内 **試行間の間隔** フィールドに値を入力するか、再試行の間隔（分）をマップします。

このオプションを有効にすると、エラーが発生した場合、不完全な実行が ( [!UICONTROL 試行間の間隔] 」フィールド ) を含め、元の入力データで実行されます。 この処理は、エラーなしでモジュールの実行が完了するか、指定された試行回数に達するまで繰り返されます。

>[!NOTE]
>
>最初の再試行が失敗した場合、再試行間の間隔は、それ以外の試行のたびに急激に増加します。


「自動的に実行を完了」がオンになっている場合、ブレークエラーハンドラーの自動再試行が問題を自動的に処理するので、シナリオの実行は「成功」とマークされます。 この場合、ユーザーは、実行の失敗に関する電子メールを受け取りません。

「自動実行を完了」がオフの場合、実行は「警告」とマークされます。

実行が「不完全な実行」の下に保存されている場合は例外があり、一部のエラータイプでは、シナリオの実行の自動再試行はできません。

詳しくは、 [不完全な実行の保存を許可](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow) 記事内 [Adobe Workfront Fusion のシナリオ設定パネル](../../workfront-fusion/scenarios/scenario-settings-panel.md).

詳しくは、 [Adobe Workfront Fusion での高度なエラー処理](../../workfront-fusion/errors/advanced-error-handling.md).
