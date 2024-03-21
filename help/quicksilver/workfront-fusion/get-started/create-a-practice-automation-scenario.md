---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: ' [!DNL Adobe Workfront Fusion] での練習用自動処理シナリオの作成'
description: この記事では、Adobe Workfront Fusion で自動処理シナリオを作成する方法について説明します。自動処理シナリオは、データの操作や変換を含む Workfront プロセスを自動化します。この例では、プロジェクトを検索し、そのプロジェクトに関連付けられたすべてのタスクを返すシナリオを作成するプロセスを、順を追って説明します。
author: Becky
feature: Workfront Fusion
exl-id: f6a6eb28-9b0b-48ea-af11-f55009a01178
source-git-commit: 3d53042b9321c8712b9aaeea686989add5b9e35e
workflow-type: tm+mt
source-wordcount: '1847'
ht-degree: 99%

---

# [!DNL Adobe Workfront Fusion] での練習用自動処理シナリオの作成

この記事では、Adobe Workfront Fusion で自動処理シナリオを作成する方法について説明します。自動処理シナリオは、データの操作や変換を含む Workfront プロセスを自動化します。この例では、プロジェクトを検索し、そのプロジェクトに関連付けられたすべてのタスクを返すシナリオを作成するプロセスを、順を追って説明します。

個別のアプリを接続する統合シナリオの作成手順について詳しくは、[Adobe Workfront Fusion での練習用統合シナリオの作成](../../workfront-fusion/get-started/create-a-practice-scenario.md)を参照してください。

各 Workfront Fusion ライセンスで利用可能な機能について詳しくは、[Adobe Workfront Fusion ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

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
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
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

[!DNL Adobe Workfront Fusion] ライセンスについては、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 練習シナリオを作成

[!DNL Adobe Workfront Fusion] の役割は、プロセスを自動処理することにより、ユーザーが同じタスクを何度も繰り返すのではなく、新しいタスクに集中できるようにすることです。これは、アプリ内やサービス内、およびそれらの間でアクションをリンクし、データを自動的に転送および変換するシナリオを作成することで機能します。作成するシナリオは、アプリまたはサービス内のデータを監視し、そのデータを処理して必要な結果を提供します。

シナリオは、アプリ内でのデータの変換方法や、アプリと web サービスの間でのデータの転送方法を示す、一連のモジュールで構成されます。
この例では、[!DNL Workfront] プロジェクトを検索し、プロジェクト内のタスクを返すシナリオを作成するプロセスを、順を追って説明します。

![](assets/create-practice-scenario-wf-only-350x157.png)

シナリオの作成は、いくつかの主なタスクで構成されています。

## アプリを選択し、シナリオに名前を付ける

1. [!DNL Workfront Fusion] アカウントにログインします。
1. 左側のパネルで&#x200B;**[!UICONTROL シナリオ]** ![](assets/scenarios-icon.png) をクリックします。

   >[!NOTE]
   >
   >左側のナビゲーションパネルまたはアイコンが表示されない場合は、メニュー ![メニュー](assets/main-menu-icon-left-nav.png) アイコンをクリックします。

   表示された灰色の[!UICONTROL フォルダー]パネルでは、シナリオをフォルダーに整理できます。

   右側のメイン領域の上部に、作成した&#x200B;**[!UICONTROL すべて]**&#x200B;のシナリオ、**[!UICONTROL アクティブなシナリオ]**、**[!UICONTROL 非アクティブなシナリオ]**、**[!UICONTROL 概念]**&#x200B;を表示することができます。概念は、[!DNL Workfront Fusion] によりアクティブまたは非アクティブとして分類される前に、さらに作業が必要なシナリオです。

<!--
   ![](assets/scenarios-left-panel-350x215.png)
-->

1. [!UICONTROL フォルダー]パネルで、**[!UICONTROL フォルダーを追加]**&#x200B;アイコン ![](assets/add-folder-icon.png) をクリックし、「練習用シナリオ」など、最初のフォルダーの名前を入力します。

1. フォルダーを開いて、ページの右上隅にある「**[!UICONTROL 新しいシナリオを作成]**」をクリックします。

   表示されるランディングページでは、作成するシナリオで使用するアプリをプリロードできます。

1. この演習では、**[!DNL Workfront]** アプリを検索して選択します。
1. 右上隅にある「**[!UICONTROL 続行]**」をクリックします。

   シナリオエディターが表示されます。中央に空のモジュールと、プリロードした [!DNL Workfront] アプリがあり、いくつかのオプションが下部のツールバーにあります。

<!--
   ![](assets/scenario-editor-350x235.png)
-->

新しいシナリオの作成を開始する場合は、まずシナリオの名前を作成するのがよいでしょう。

1. 左上隅にある「**[!UICONTROL 新規シナリオ]**」プレースホルダー名を選択し、「練習用シナリオ 1」などの名前を入力します。
1. 続いて、以下の[最初のモジュールを追加して設定](#add-and-configure-the-first-module)を行います。

## 最初のモジュールを追加して設定

クエスチョンマーク付きの空のモジュールは、追加する必要があるトリガーモジュールを表します。このモジュールは、実行されるたびにシナリオを開始します。空のモジュールの時計アイコンは、スケジュール設定済みモジュールであることを示します。

![](assets/empty-module.png)

このモジュールには、シナリオで監視するデータが格納されます。

この例では、トリガーモジュールを使用していません。代わりに、このシナリオは検索で始まります。

1. 空のモジュールをクリックして、モジュールを選択するアプリを選択します。

   事前にプリロードしたアプリが、空のモジュールの横に表示されます。[!UICONTROL 検索]ボックスを使用して、モジュールを持つ他のアプリを追加できます。

   ![](assets/pre-loaded-app-wf-350x172.png)

1. **[!DNL Workfront]** をクリックします。

   リストが変わり、すべての [!DNL Workfront] モジュールが表示され、トリガーモジュールとして使用できます。

1. 検索モジュール「**[!UICONTROL 検索]**」をクリックします。

   次に、[!DNL Workfront] アカウントに認証接続を確立する必要があります。シナリオに追加するモジュールはすべて、アプリとの接続を確立する必要があります。

1. **[!DNL Workfront]** ボックスの「**[!UICONTROL 接続]**」の下で、「**[!UICONTROL 追加]**」をクリックし、接続の名前（「オリビアの Workfront アカウント」など）を入力して、「**[!UICONTROL 続行]**」をクリックします。
1. 表示されるウィンドウで接続を認証します。

   接続を認証するプロセスは、アプリ間で少し異なる場合があります。次のプロセスは、[!DNL Workfront] に特有ですが、このプロセスは多くのアプリに類似しています。

   1. [!DNL Workfront] ドメインを入力し、「**[!UICONTROL 続行]**」をクリックします。
   1. [!DNL Workfront] にログインします。
   1. [!DNL Workfront Fusion] がリクエストするアクセス権を確認し、「**[!UICONTROL アクセスを許可]**」をクリックします。

   ヘルプが必要な場合は、[アプリまたはサービスへの  [!DNL Adobe Workfront Fusion]  の接続について](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md)を参照してください。

## 最初のモジュールを設定

[!DNL Workfront] アカウントに [!DNL Workfront Fusion] を接続した後、アクセス権のある [!DNL Workfront] リクエストキューおよび最初のモジュールで処理するデータを指定できます。

1. [!UICONTROL レコードタイプ]ボックスで、「**[!UICONTROL プロジェクト]**」を選択します。これにより、モジュールはプロジェクトのみを検索するように設定されます。

   >[!TIP]
   >
   >「[!UICONTROL プロジェクト]」と入力すると、リストで&#x200B;**[!UICONTROL プロジェクト]**&#x200B;を検索できます。

1. **[!UICONTROL 結果セット]**&#x200B;ボックスで、「**[!UICONTROL 一致する最初のレコード]**」を選択します。これにより、モジュールは、条件を満たす最初のレコードのみを返すように設定されます。この例では、返されるレコードは 1 つだけです。
1. **[!UICONTROL 検索条件]**&#x200B;領域で、特定のプロジェクトを返すフィルターを設定します。

   1. [!UICONTROL 検索条件]の下の最初のボックスで、値を検索するフィールドを選択します。この例では、「**[!UICONTROL 名前]**」を選択します。
   1. 演算子の場合は、「[!UICONTROL 次を含む（大文字と小文字を区別しない）]」を選択します。これにより、名前全体を入力しない場合または名前に大文字と小文字を区別せずに入力した場合でも、モジュールは名前に選択した単語を含むプロジェクトを検索できます（すべて大文字など）。
   1. [!UICONTROL 検索条件]の下の最後のフィールドに、検索対象のプロジェクト名に含まれる単語やフレーズを入力します。

1. Adobe Analytics の **[!UICONTROL 出力]** 「 」リストで、モジュールから出力するフィールドを選択します。 この例では、「**[!UICONTROL ID]**」フィールドおよび「**[!UICONTROL 名前]**」フィールドを選択します。

   >[!TIP]
   >
   >**Cmd+F**（[!DNL Mac] OS）または **Ctrl+F**（[!DNL Windows] OS）を使用して、すばやくフィールドを検索できます。

1. 「**[!UICONTROL OK]**」をクリックします。

   >[!NOTE]
   >
   >（情報のみ）これはトリガーモジュールではないので、どこで開始するかは選択しません。トリガーモジュールを使用する場合、開始場所を選択できるようになりました。
   >
   >
   >詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md) でのトリガーモジュールの開始場所の選択を参照してください。

1. モジュールを右クリックし、「**[!UICONTROL 名前を変更]**」をクリックして、モジュールで実行する操作を示す名前（「プロジェクトの検索」など）を入力し、「**[!UICONTROL OK]**」をクリックします。

   名前はモジュールのすぐ下に表示されます。その下に [!DNL Workfront Fusion] には、モジュールで実行されるアクションのタイプに関する簡単な説明が含まれます。

   ![](assets/module-renamed-wf.png)

1. [2 つ目のモジュールを追加して設定](#add-and-configure-the-second-module)に進みます。

## 2 つ目のモジュールを追加して設定

1. モジュールの右側の半円をクリックして、**[!UICONTROL 別のモジュールを追加]**&#x200B;します。
1. アプリケーションのリストから [!DNL Workfront] を選択し、検索モジュール&#x200B;**[!UICONTROL 関連レコードの読み取り]**&#x200B;を選択します。
1. 前のモジュールですでに [!DNL Workfront] への接続を作成しています。ここで再度作成する必要はありませんが、このモジュールが前のモジュールと同じ接続を使用していることを確認する必要があります。\
   「**[!UICONTROL 接続]**」ボックスで、前のモジュール用に作成した接続を選択します。
1. プロジェクトに関連するレコードを読み取るには、「**[!UICONTROL レコードタイプ]**」をクリックして、「**[!UICONTROL プロジェクト]**」を選択します。

   >[!TIP]
   >
   >**[!UICONTROL プロジェクト]**&#x200B;は、「プロジェクト」という単語を入力すると、リストの中に表示されます。

1. 「**[!UICONTROL 親レコード ID]**」フィールドをクリックします。このフィールドには、タスクを返す元のプロジェクトの Workfront ID が必要です。

   このフィールドをクリックすると、「**[!UICONTROL 親レコード ID]**」フィールドで使用できる変数のリストが開き、Workfront でプロジェクトを識別できます。

   ![](assets/list-of-available-variables-wf-350x368.png)

1. 変数 **[!UICONTROL ID]** をクリックして、「**[!UICONTROL 親レコード ID]**」フィールドに追加します。これにより、最初のモジュールから返された ID が、2 番目のモジュールで作業するプロジェクトの識別子として使用されるようになり、返されたタスクは確実にそのプロジェクトに属します。
1. 「**[!UICONTROL コレクション]**」フィールドで、「**[!UICONTROL タスク]**」を選択します。これは、モジュールが、選択されたプロジェクトに関連付けられたタスクを返すことを示します。
1. 「**[!UICONTROL OK]**」をクリックします。

   これで、動作するシナリオが作成されました。

1. 2 つ目のモジュールに「プロジェクトに関連付けられたタスクを返す」などの名前を付け、次に、[シナリオのテスト](#test-the-scenario)に進みます。

## シナリオのテスト

シナリオをアクティベートする前にテストすることが重要です。少なくとも 1 回実行して結果を確認します。これは、シナリオにおけるデータの流れを理解し、エラーを見つけるのに役立ちます。

1 つのプロジェクトを返し、そのプロジェクトに関連付けられたタスクを選択しました。シナリオを実行すると、そのようになります。

1. シナリオエディターの左下隅にある「**[!UICONTROL 1 回実行]**」をクリックします。
1. シナリオの実行が終了したら、最初のモジュールの上のバブルをクリックします。

   ![](assets/click-bubble.png)

   表示されるボックスで、モジュールが返したプロジェクトから取り出された実際のデータなど、モジュールが処理したデータのバンドルに関する情報を表示できます。

   ![](assets/execution-inspector-wf-only-first-350x423.png)

1. 2 つ目のモジュールの上にある実行インスペクターのバブルをクリックすると、情報の入力と出力（プロジェクトに含まれるタスクのコレクション）を確認できます。

   ![](assets/execution-inspector-wf-only-second-350x738.png)

   シナリオ実行情報の読み取り方法について詳しくは、次の記事を参照してください。

   * 詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md) でのシナリオ実行フローを参照してください。
   * 処理されたバンドルについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md) でのシナリオの実行、サイクル、フェーズを参照してください。

1. [!DNL Workfront Fusion] で、左下隅付近ににある「**[!UICONTROL 保存]**」![](assets/save-icon.png) をクリックして、シナリオの進行状況を保存します。

   >[!IMPORTANT]
   >
   >シナリオを改良、テストするたびに保存するようにしてください。

>[!TIP]
>
>各モジュールに関するメモを追加する方法として、任意ではあるものの便利な方法をお勧めします。
>
>1. [!DNL Workfront] モジュールを右クリックして、「**[!UICONTROL メモを追加]**」をクリックします。
>1. 表示されるメモに、モジュールの概要を入力します。
>
>    1 つのモジュールに複数のノートを追加できます。
>
>1. **[!UICONTROL メモ]**&#x200B;エリアを閉じます。
>
>     シナリオにメモを追加すると、シナリオエディターの下部の&#x200B;**[!UICONTROL メモ]**&#x200B;アイコン ![](assets/notes-icon-w-dot.png) にオレンジ色の点が表示されます。
>
>1. **[!UICONTROL メモ]**&#x200B;アイコン ![](assets/notes-icon-w-dot.png) をクリックして、メモを表示します。
>



## シナリオをアクティベート

この例のシナリオにはトリガーモジュールがありません。これが実際のデータに使用するシナリオの場合は、トリガーモジュールから始まり、最後にアクティブ化します。シナリオをアクティベートすると、デフォルトでは 15 分ごとに実行されます。これは、実行するタイミングと頻度を定義することで変更できます。

シナリオのアクティブ化について詳しくは、[[!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md) でのシナリオのアクティブ化または非アクティブ化を参照してください。

スケジュールについて詳しくは、[[!UICONTROL Adobe Workfront Fusion でのシナリオのスケジュール設定]](../../workfront-fusion/scenarios/schedule-a-scenario.md)を参照してください。
