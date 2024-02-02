---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: errors
title: ' [!DNL Adobe Workfront Fusion] でのエラー処理のディレクティブ'
description: この記事では、 [!DNL Adobe Workfront Fusion] シナリオでのエラー処理に使用できるディレクティブについて説明します。
author: Becky
feature: Workfront Fusion
exl-id: dcf4f7e3-78d8-4eb4-9483-8a1c18b0e436
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: ht
source-wordcount: '953'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] でのエラー処理のディレクティブ

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

## エラー処理のディレクティブ

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>ロールバック</p> <p> <img src="assets/rollback.png"> </p> </td> 
   <td> <p>シナリオの実行は直ちに停止され、すべてのモジュールを初期状態に戻すために、すべてのモジュールに対して<a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#rollback" class="MCXref xref">ロールバック</a>フェーズが開始されます。後続のモジュールは処理されません。</p> <p>いくつかのエラータイプを除き、シナリオ設定で指定された連続エラー回数を超過すると、シナリオは非アクティブ化されます。詳しくは、<a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#number" class="MCXref xref">連続エラー回数</a>を参照してください。</p> <p>シナリオの実行ステータスは「エラー」とマークされます。</p> <p>メモ：これは、エラーハンドラールートがモジュールにアタッチされておらず、[!UICONTROL Scenario settings] の「<a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">[!UICONTROL Allow storing incomplete executions]</a>」設定がオンになっていない場合のデフォルトの動作です。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>コミット</p> <p> <img src="assets/commit.png"> </p> </td> 
   <td> <p>シナリオの実行は直ちに停止され、すべてのモジュールでコミットフェーズが開始されます。後続のモジュールは処理されません。</p> <p>未処理のバンドルはすべて無視されます。</p> <p>シナリオの実行ステータスは「成功」とマークされます。コミットフェーズについては、<a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Adobe Workfront Fusion のシナリオの実行、サイクル、フェーズ</a>の記事の<a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md#commit" class="MCXref xref">コミット</a>を参照してください。</p> </td> 
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
   <td> <p>シナリオの実行状態は、不完全な実行のキューに保存されます。このキューでは、エラーを手動で解決できます。 詳しくは、<a href="../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md" class="MCXref xref">Adobe Workfront Fusion での不完全な実行の表示と解決</a>を参照してください。 </p> <p>ただし、いくつかの例外があります。詳しくは、<a href="../../workfront-fusion/scenarios/scenario-settings-panel.md" class="MCXref xref">Adobe Workfront Fusion のシナリオ設定パネル</a>の記事で<a href="../../workfront-fusion/scenarios/scenario-settings-panel.md#allow" class="MCXref xref">不完全な実行の保存の許可</a>を参照してください。</p> <p>後続のモジュールは処理されません。</p> <p>未処理のバンドルがある場合、シナリオの実行は通常どおり続行されます。</p> <p>「[!UICONTROL Automatically complete execution]」オプションが無効になっている場合、シナリオの実行ステータスは「警告」とマークされます。</p> <p>詳しくは、以下の<a href="#break" class="MCXref xref">[!UICONTROL Break]</a>の節を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>再試行</p> <p> <img src="assets/retry.png"> </p> </td> 
   <td> <p>場合によっては、時間の経過とともに失敗の理由が消える可能性がある場合、失敗したモジュールを数回再実行すると便利な場合があります。</p> <p>現在、Workfront Fusion では Retry ディレクティブは提供されていませんが、機能を模倣するために、いくつかの回避策を使用できます。詳しくは、<a href="../../workfront-fusion/errors/retry.md" class="MCXref xref">Adobe Workfront Fusion での再試行エラー処理</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* 現在、エラー処理ディレクティブは、エラー処理ルート以外では使用できません。
>
>   詳しくは、[Adobe Workfront Fusion でのエラー処理](../../workfront-fusion/errors/error-handling.md)の記事の[エラーハンドラールート](../../workfront-fusion/errors/error-handling.md#error)を参照してください。
>* [!DNL Workfront Fusion] では、現在、条件付きで簡単にエラーを生成（スロー）できる Throw モジュールは提供していませんが、機能を模した回避策を使用できます。
>
>   詳しくは、[Adobe Workfront Fusion でのエラー処理のスロー](../../workfront-fusion/errors/throw.md)の記事の[スローの回避策](../../workfront-fusion/errors/throw.md#workaround-for-throw)を参照してください。

## 一時停止 {#break}

エラーが [!DNL Break] ディレクティブによって処理されると、未完了の実行フォルダーにレコードが作成されます。このレコードには、シナリオの実行の状態と共に、前のモジュールのデータが格納されます。レコードは、エラーが発生したモジュールを参照し、モジュールが受け取ったデータに関する情報を入力として含みます。エラーの原因となるデータのバンドルごとに、別々のレコードが作成されます。

詳しくは、[Adobe Workfront Fusion での未完了の実行の表示と解決](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)を参照してください。

### Break ディレクティブによって発生したエラーを解決する

シナリオを更新し（必要に応じて）1 回実行することで、手動でエラーを解決できます。

シナリオを再実行することで、未完了の実行を自動的に処理するようにシナリオを設定することもできます。未完了の実行を処理するようにモジュールを設定するには、次の手順に従います。

1. Break モジュール内で、[!UICONTROL **自動的に実行を完了する**]&#x200B;オプションを有効にします。
1. **試行回数**&#x200B;フィールドに、モジュールが実行を再試行する最大回数を入力またはマッピングします

   この数は 1 ～ 100 の範囲で指定する必要があります。
1. **試行間隔**&#x200B;フィールドに、各再試行の間隔の分数を入力またはマッピングします。

このオプションを有効にすると、エラーが発生した場合、]試行間隔[!UICONTROL フィールドで指定された時間後に未完了の実行が回収され、元の入力データで実行されます。この処理は、エラーなしでモジュールの実行が完了するか、指定された試行回数に達するまで繰り返されます。

>[!NOTE]
>
>最初の再試行が失敗した場合、再試行の間隔は再試行のたびに飛躍的に長くなります。


「自動的に実行を完了」がオンになっている場合、ブレークエラーハンドラーの自動再試行がイシューを自動的に処理するので、シナリオの実行は「成功」とマークされます。この場合、ユーザには、実行が失敗したことについてのメールは届きません。

「自動実行を完了」がオフの場合、実行は「警告」とマークされます。

実行が「未完了の実行」の下に保存されている場合は例外があり、一部のエラータイプでは、シナリオの実行の自動再試行はできません。

詳しくは、[未完了の実行の保存を許可](../../workfront-fusion/scenarios/scenario-settings-panel.md#allow)の記事内の[Adobe Workfront Fusion のシナリオ設定パネル](../../workfront-fusion/scenarios/scenario-settings-panel.md)を参照してください。

詳しくは、[Adobe Workfront Fusion での高度なエラー処理](../../workfront-fusion/errors/advanced-error-handling.md)を参照してください。
