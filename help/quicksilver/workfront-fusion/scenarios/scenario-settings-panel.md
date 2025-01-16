---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion のシナリオ設定パネル
description: Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。 この記事は廃止されましたが、この機能を説明する新しい記事へのリンクが含まれています。
author: Becky
feature: Workfront Fusion
exl-id: 64a7a39a-f450-4eba-b4db-f31dd22aefdc
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '1266'
ht-degree: 80%

---

# [!DNL Adobe Workfront Fusion] のシナリオ設定パネル

>[!IMPORTANT]
>
>Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。
>
>この記事の情報は、次の記事に記載されています。
>
>* [ シナリオ設定を指定 ](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/configure-scenario-settings/configure-scenario-settings.html)
>
>ブックマークを更新してください。
>
>この記事は現在更新されておらず、近い将来に削除されます。

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件は不要。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]、[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront]を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## シナリオ設定を開く

1. シナリオエディターを開きます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-editor.md) のシナリオエディターを参照してください。
1. ページの左下隅付近にある歯車アイコンをクリックします。

   ![](assets/scenario-settings-350x221.png)

   表示される[!UICONTROL シナリオ設定]パネルで、シナリオの様々な詳細設定ができます。

## [!UICONTROL 不完全な実行の保存を許可]

このオプションでは、シナリオの実行中にエラーが発生した場合の [!DNL Adobe Workfront Fusion] での処理方法を指定します。このオプションを有効にすると、シナリオは一時停止され、「[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md) での不完全な実行を表示して解決」に移行します。これにより、問題を修正し、シナリオが停止した場所から続行できます。このオプションを無効にした場合、シナリオの実行が停止し、ロールバックフェーズが開始します。

## [!UICONTROL 順番に処理]

このオプションは、すべての実行を順番に実行します。主に Webhook と不完全な実行に関連しています。

順次処理が有効な場合、シナリオの並列実行は無効になります。

### Instant Webhook

Webhook トリガーが `instant` として設定され、「順次処理」が有効になっている場合、すべてのインスタント Webhook ペイロードはキューに入り、届いた順に処理されます。 これは、外部システムからのイベントを正確な順序で処理する場合に役立ちます。

>[!NOTE]
>
>次のペイロードが開始される前に各ペイロードが処理されるので、自動処理の遅延が発生します。

### 不完全な実行

「不完全な実行」も有効になっている場合、シナリオの実行中にエラーが発生すると、シナリオは一時停止します。 次のいずれかの処理が行われます。

* 「順次処理」オプションが **有効** になっている場合、Workfront Fusion は、すべての不完全な実行が解決されるまで既存のシーケンスの処理を停止します。
* 「順次処理」オプションが **無効** の場合、シナリオはスケジュールに従って引き続き実行され、不完全な実行は繰り返し再試行されます。

不完全な実行について詳しくは、[Adobe Workfront Fusion での不完全な実行の表示と解決](/help/quicksilver/workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)を参照してください。

<!--

This option determines how [!DNL Workfront Fusion] proceeds if an error occurs and the execution of a scenario is moved to the [View and resolve incomplete executions in [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md). If the [!UICONTROL Sequential processing] option is enabled, Workfront Fusion stops processing the task sequence altogether until all incomplete executions are resolved. If the [!UICONTROL Sequential processing] option is disabled, the scenario continues to run according to its schedule, accompanied by repeated attempts to rerun the incomplete executions.-->

>[!NOTE]
>
>順番に処理を行うと、シナリオの実行に遅延が生じる場合があります。インスタントシナリオがトリガーされた時、またはスケジュールされたシナリオが実行される時に、キューにまだ未完了の実行がある場合、そのシナリオは、キュー内の前の実行が全て完了してから実行されます。
>
>シナリオのユースケースで順番に処理することが必要ない場合は、順番処理のオプションを無効にすることをお勧めします。

詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md) でのシナリオのスケジュールを参照してください。

## データは機密情報

シナリオを実行すると、シナリオ内のモジュールでどのデータが処理されたかに関する情報をデフォルトで表示できます。この情報を保存しない場合は、「[!UICONTROL データは機密情報]」オプションを有効にします。

情報の表示について詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md) でのシナリオ実行フローを参照してください。

>[!IMPORTANT]
>
>このオプションを有効にすると、シナリオの実行中に発生する可能性のあるエラーを解決するのが困難になる場合があります。

## データ損失を有効にする

このオプションは、[!DNL Workfront Fusion] が「[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-and-resolve-incomplete-executions.md)での不完全な実行を表示して解決」のキューにバンドルを保存できなかった場合（空き領域が不足している場合など）に、データの損失を有効にすることと関係します。このオプションを有効にすると、シナリオの実行全体で中断が発生しないように、データが失われます。これは、最も優先度が高いものが継続して実行され、入力時の誤りのあるデータがそれほど重要でないシナリオで役立ちます。

その他、シナリオを実行する際に、モジュールで許容される最大サイズを超えるファイルが見つかることがあります。この場合、[!DNL Workfront Fusion] は「[!UICONTROL データ損失を有効にする]」オプションの設定に従って処理し、警告メッセージを表示します。

最大ファイルサイズについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/about-mapping-files.md) でのファイルのマッピングについてを参照してください。

警告について詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) でのエラー処理を参照してください。

## [!UICONTROL 自動コミット]

[!UICONTROL 自動コミット]設定はトランザクションに適用され、シナリオの処理方法を定義するものです。「自動コミット」オプションがオンの場合、各モジュールのコミットフェーズは、操作フェーズが完了した直後に開始します。「自動コミット」オプションを無効にした場合、すべてのモジュールに対して操作が実行されるまでコミットは行われません（これはデフォルトのモードです）。

トランザクションについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md) でのシナリオの実行、サイクル、フェーズを参照してください。

## サイクルの最大数

サードパーティのサービスへの接続が中断されるのを防ぎ、1 回のシナリオ実行内にすべてのレコードが確実に処理されるようにする場合は、より多くのサイクルを設定すると便利です。

* ポーリングトリガーで始まるシナリオの場合、この設定で、シナリオの実行中に許可されるサイクルの最大数を定義します。

  ポーリングトリガーについて詳しくは、[モジュールのタイプ](../../workfront-fusion/modules/module-types.md)の[ポーリングトリガー](../../workfront-fusion/modules/module-types.md#polling)を参照してください。

* シナリオがインスタントトリガーで開始する場合、設定は無視され、1 回のシナリオの実行中にすべての保留中のイベントが処理されます（1 サイクルにつき 1 つのイベント）。

  インスタントトリガーについて詳しくは、[モジュールのタイプ](../../workfront-fusion/modules/module-types.md)の[インスタントトリガー](../../workfront-fusion/modules/module-types.md#instant)を参照してください。

* シナリオが（インスタントまたはポーリング）トリガーで始まらない場合は、指定された最大サイクル数が常に実行されます。

>[!INFO]
>
>**例：**[!DNL Workfront]／[!UICONTROL レコードを監視]で、発生した新しいイシューを監視し、[!DNL Workfront]／[!UICONTROL オブジェクトを変換]で、新しいリクエストをプロジェクトに変換し、適切なテンプレートを割り当てます。
>
>![](assets/scenario-settings-ex-1-350x157.png)
>
>[!UICONTROL より多くのサイクル]設定は、シナリオの実行をスケジュールする場合にのみ適用されます。「[!UICONTROL 1 回実行]」ボタンを使用する場合、サイクル設定を考慮します。
>
>### サイクルの最大数は 1 に設定されています（デフォルト）
>
>![](assets/max-number-cycles-1-350x201.png)
>
>[!UICONTROL 2}Workfront] >[!UICONTROL  レコードを監視 ] モジュールの { 返されるファイルの最大数 ] が `10` に設定されています。[!UICONTROL 
>100 件のリクエストが [!DNL Workfront] に送信され、「[!UICONTROL 制限]」フィールドが 10 に設定されている場合、1 回のシナリオ実行後に 90 件のファイルが未処理のまま残ります。次の 10 個のファイルは、スケジュールされた次のシナリオの実行で処理されます。
>
>### サイクルの最大数を 10 に設定
>
>[!UICONTROL Dropbox] [!UICONTROL ファイル監視]モジュールの[!UICONTROL 返されるファイルの最大数]は `10` に設定されています。
>
>100 個のファイルが Dropbox フォルダーに追加され、「[!UICONTROL 返されるファイルの最大数]」オプションが 10 に設定されている場合、最初のサイクルで 10 個のファイルが処理され、2 番目のサイクルで次の 10 個のファイルが処理され、3 番目のサイクルでは次の 10 ファイルが処理され、というように、すべてのファイルが処理されるまで続きます。
>
>すべてのファイルは、1 回のシナリオ実行の間に処理されます。
>
>シナリオの詳細には、既に実行されたサイクルが表示されます。
>
>![](assets/scenario-detail-350x207.png)
>
>このページについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-detail.md) にあるシナリオの詳細を参照してください。

## 連続エラー数

シナリオの実行が非アクティブ化されるまでの連続実行試行の最大回数を定義します（[!UICONTROL DataError]、[!UICONTROL DuplicateDataError]、および [!UICONTROL ConnectionError] を除く）。

エラーについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/errors/error-processing.md) でのエラー処理を参照してください。

>[!NOTE]
>
>シナリオがインスタントトリガーで始まる場合、設定が無視され、最初のエラーが発生するとシナリオは直ちに非アクティブ化されます。
