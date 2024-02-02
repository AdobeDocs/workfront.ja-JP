---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion の基本用語
description: Adobe Workfront Fusion を使用するには、Adobe Workfront ライセンスに加えて、Adobe Workfront Fusion ライセンスが必要です。
author: Becky
feature: Workfront Fusion
exl-id: 2169dc2e-2135-47e0-a615-3de12cd120a9
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: ht
source-wordcount: '830'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] の基本用語

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] には、[!UICONTROL Adobe Workfront] ライセンスに加えて [!DNL Adobe Workfront Fusion] ライセンスが必要です。


<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>アクション</p> </td> 
   <td>選択したアプリやサービスに対して、バンドルの読み取りまたは書き込みを行うことができるモジュール。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Aggregator]</p> </td> 
   <td> <p>複数のバンドル（複数のデータ配列）を 1 つのバンドルに結合するモジュールのタイプ。詳しくは、<a href="../../workfront-fusion/modules/aggregator-module.md" class="MCXref xref">[!UICONTROL Adobe Workfront Fusion] の [!UICONTROL Aggregator] モジュール</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API キー</td> 
   <td>ソフトウェアの API を呼び出すユーザー、開発者またはプログラムを識別する一意のコードで、認証に使用されます。[!DNL Adobe Workfront Fusion] モジュールは API を接続して動作するため、API キーが必要になる場合があります。API キーは、API キーを必要とするアプリによって配布されます。例えば、[!DNL ActiveCampaign] の API キーが必要な場合は、[!DNL ActiveCampaign] アカウントを介してリクエストします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アプリまたはサービス</td> 
   <td> <p>最も一般的にはソフトウェアアプリケーションです。</p> <p>またアプリは、イテレーターやアグリゲーターなどのデータを操作する特別な関数である場合もあります。 </p> <p>サービスは、web API、web ページ、様々なタイプのサーバー（FTP、SMTP、IMAP）などを含むバンドルのソースです。 </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アプリコネクタ</td> 
   <td>別のシステムに接続するアプリ。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>バンドル</p> </td> 
   <td> <p>バンドルは、モジュールが返す、または受け取る基本単位です。バンドルは複数の項目で構成されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>シナリオにアプリまたはサービスを追加する場合、選択したデータを取得または送信するために、まず [!DNL Workfront Fusion] とアプリまたはサービスの間に接続を作成する必要があります。詳しくは、<a href="../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md" class="MCXref xref">アプリまたはサービスへの [!DNL Adobe Workfront Fusion] の接続について</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>サイクル</p> </td> 
   <td> <p>サイクルとは、シナリオ実行の 2 つのフェーズ、すなわちオペレーションとコミットを指します。このシナリオは、1 つ以上のサイクルで構成されます。詳しくは、<a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのシナリオの実行、サイクルおよびフェーズを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>データ保存</p> </td> 
   <td> <p>シナリオからデータを保存するツール、または個々のシナリオ間や、シナリオの実行間でデータを転送するツール。詳しくは、<a href="../../workfront-fusion/modules/data-stores.md" class="MCXref xref">[!UICONTROL Adobe Workfront Fusion] のデータ保存</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>データ転送</p> </td> 
   <td> <p>シナリオを介して転送されたデータの量。詳しくは、<a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">[!UICONTROL Adobe Workfront Fusion] のシナリオの詳細</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>フィルター</p> </td> 
   <td> <p>2 つのモジュール間で適用可能な追加機能。フィルターを使用すると、特定の基準を満たすバンドルのみを操作できます。様々なフィルターを適用できます。詳しくは、<a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">[!UICONTROL Adobe Workfront Fusion] のシナリオへのフィルターの追加</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ID</p> </td> 
   <td> <p>バンドルを一意に識別するために使用される名前。ID は通常、特定のサービスから更新または削除されるバンドルを区別するのに使用されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>項目</p> </td> 
   <td> <p>バンドルの一部。バンドルは複数の項目で構成できます。項目には、テキスト、数値、ブール値（はい／いいえ）、日付、時刻、バッファー（バイナリデータ）、コレクション、選択メニュー、配列、検証など、様々なタイプがあります。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Iterator]</p> </td> 
   <td> <p>1 つのデータのバンドル（データの配列）を取得し、別々のバンドルに分割できるモジュールのタイプ。詳しくは、<a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> の [!UICONTROL Iterator] モジュールを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>モジュール</p> </td> 
   <td> <p>関連するアプリまたはサービス内で、レコードの作成などの機能を実行するシナリオ内の 1 つの手順。</p> <p>それぞれのアプリやサービスには、リクエストへの応答方法を定義する様々なモジュールがあります。</p> <p>モジュールには、アクション、トリガー、イテレーターおよびアグリゲーターの 4 つのタイプがあります。</p> <p> <img src="assets/module.jpg"> </p> <p>詳しくは、<a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">モジュールのタイプ</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>操作</p> </td> 
   <td> <p>モジュールによって実行されるタスク。</p><p>詳しくは、<a href="../../workfront-fusion/get-started/operations-in-workfront-fusion.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> での操作を参照してください。</p>
  </tr> 
  <tr> 
   <td role="rowheader">公開鍵と秘密鍵</td> 
   <td>公開鍵と秘密鍵は、データの暗号化と復号化に使用されます。公開鍵は配布でき、公開鍵を持つすべてのユーザーがデータを暗号化できますが、復号化できるのは秘密鍵のみです。同様に、同様に、秘密鍵を持つユーザーは、公開鍵を持つ誰もが復号化できるデータを暗号化できます。秘密鍵による暗号化は、データが秘密鍵の所有者から送信されたことを保証し、データのソースの検証として機能します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Router]</p> </td> 
   <td>データを複製したり、シナリオに新しいルートを追加したりできるので、データを再ルーティングし、異なるデータグループを別々に処理できます。詳しくは、<a href="../../workfront-fusion/modules/router-module.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> の [!UICONTROL Router] モジュールを参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>シナリオ</p> </td> 
   <td> <p>ユーザーが作成した一連の自動化された手順で、それぞれがモジュールによって表され、実行されます。シナリオの目的は、データの移動と操作です。</p> <p> <img src="assets/scenario-350x178.jpg" style="width: 350;height: 178;"> </p> <p> 詳しくは、<a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">[!UICONTROL Adobe Workfront Fusio] でのシナリオの作成</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>トランザクション</p> </td> 
   <td> <p>[!DNL Workfront Fusion] トランザクション処理を使用してシナリオのライフサイクルをキャプチャします。トランザクションは、データが 1 つの一貫性のある状態から別の一貫性のある状態に変換される間のいくつかのフェーズから構成されます。初期化、操作（読み取りまたは書き込み）、コミット／ロールバック、最終化の 4 つのフェーズがあります。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>トリガー</p> </td> 
   <td> <p>前回のシナリオ実行以降に追加または更新されたバンドルを取得できるモジュール。ポーリングとインスタント（Webhook）の 2 つのタイプのトリガーがあります。詳しくは、<a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> のインスタントトリガー（Webhook）を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Webhook</p> </td> 
   <td> <p>新しいバンドルが使用可能になった直後にシナリオを実行できる特別なタイプのトリガー。詳しくは、<a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">[!UICONTROL Adobe Workfront Fusion] のインスタントトリガー（Webhook）</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>
