---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion で練習用統合シナリオを作成
description: この記事では、Adobe Workfront Fusion で統合シナリオを作成する方法について説明します。統合シナリオは、別々のアプリを接続し、様々なアプリケーションを通じてデータを流すことができます。
author: Becky
feature: Workfront Fusion
exl-id: 643bb1d5-d7bc-402b-8ed1-9ca9a30e4560
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: ht
source-wordcount: '2142'
ht-degree: 100%

---

# Adobe Workfront Fusion で練習用統合シナリオを作成

この記事では、Adobe Workfront Fusion で統合シナリオを作成する方法について説明します。統合シナリオは、別々のアプリを接続し、様々なアプリケーションを通じてデータを流すことができます。

統合シナリオを作成するには、組織が [!DNL Workfront Fusion for Work Automation and Integration] ライセンスを保有している必要があります。

Workfront のみを使用した自動処理シナリオの作成について詳しくは、[Adobe Workfront Fusion での練習用自動処理シナリオの作成](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md)を参照してください。

Workfront Fusion ライセンスについて詳しくは、[Adobe Workfront Fusion ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

>[!NOTE]
>
>組織で、Google シートへのアクセスが許可されていない場合があります。その場合、この統合を設定することはできませんが、この記事で示す情報は、統合シナリオの機能の一般的な例として参照できます。

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
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select]または[!UICONTROL Prime]の [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入してください。[!DNL Workfront Fusion] は [!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入してください。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 練習シナリオを作成

[!DNL Adobe Workfront Fusion] の役割は、プロセスを自動処理することで、ユーザーが同じタスクを何度も繰り返すのではなく、新しいタスクに集中できるようにすることです。これは、アプリ内やサービス内、およびそれらの間でアクションをリンクし、データを自動的に転送および変換するシナリオを作成することで機能します。作成するシナリオは、アプリまたはサービス内のデータを監視し、そのデータを処理して必要な結果を提供します。

シナリオは、アプリ内でのデータの変換方法や、アプリと web サービスの間でのデータの転送方法を示す、一連のモジュールで構成されます。

シナリオの作成方法を説明し、ベストプラクティスを強化しながら [!DNL Workfront Fusion] の使用方法を学べるように、この記事ではプロセスの手順を順を追って説明します。[!DNL Google Sheets] スプレッドシートの各行に対する新規レコードを [!DNL Workfront] に作成するシナリオを作成していきます。

![](assets/finished-scenario-1-350x180.png)

>[!TIP]
>
>このようなシナリオは、[!DNL Workfront] でプロジェクトを使用しながら作業する必要のあるプロジェクトをリストしているスプレッドシートがある場合に便利です。このシナリオでは、スプレッドシートで新しい行を「監視」し、それぞれの新しい行に対して [!DNL Workfront] に新しいプロジェクトを追加できます。

シナリオの作成は、いくつかの主なタスクで構成されています。

## アプリを選択し、シナリオに名前を付ける

1. こちらの[スプレッドシート](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/Fusion+Practice+Scenario+Sample+Sheet.xlsx)をダウンロードし、この演習全体で使用するために [!DNL Google Drive] にアップロードします。

   または

   使用している次のようなシンプルな [!DNL Google Sheets] スプレッドシートを作成または探します。

   ![](assets/spreadsheet-headers-350x55.png)

1. [!DNL Workfront Fusion] アカウントにログインします。
1. 左側のパネルで&#x200B;**[!UICONTROL シナリオ]** ![](assets/scenarios-icon.png) をクリックします。

   >[!NOTE]
   >
   >左側のナビゲーションパネルまたはアイコンが表示されない場合は、メニュー ![メニュー](assets/main-menu-icon-left-nav.png) アイコンをクリックします。

   表示された灰色の[!UICONTROL フォルダー]パネルでは、シナリオをフォルダーに整理できます。

   右側のメインエリアの上部で、作成した&#x200B;**[!UICONTROL すべて]**&#x200B;のシナリオ、**[!UICONTROL アクティブなシナリオ]**&#x200B;と&#x200B;**[!UICONTROL 非アクティブなシナリオ]**、**[!UICONTROL コンセプト]**（[!DNL Workfront Fusion] がアクティブまたは非アクティブに分類するには、さらに作業が必要なシナリオ）を確認できます。

<!--
   ![](assets/scenarios-left-panel-350x215.png)
-->

1. [!UICONTROL フォルダー]パネルで、**[!UICONTROL フォルダーを追加]**&#x200B;アイコン ![](assets/add-folder-icon.png) をクリックし、「Practice scenarios」など、最初のフォルダーの名前を入力します。

1. フォルダーを開いて、ページの右上隅にある「**[!UICONTROL 新しいシナリオを作成]**」をクリックします。

   表示されるランディングページでは、作成するシナリオで使用するアプリをプリロードできます。

1. この演習では、**[!UICONTROL Google Sheets]** アプリを検索して選択します。
1. 右上隅にある「**[!UICONTROL 続行]**」をクリックします。

   シナリオエディターが表示されます。中央に空のモジュールと、プリロードした [!DNL Google Sheets] アプリがあり、いくつかのオプションが下部のツールバーにあります。

<!--
   ![](assets/scenario-editor-350x235.png)
-->

新しいシナリオの作成を開始する場合は、まずシナリオの名前を作成するのがよいでしょう。

1. 左上隅の「**[!UICONTROL 新しいシナリオ]**」プレースホルダー名を選択し、「Practice scenario 1」などの名前を入力します。
1. 続けて、以下の[最初のモジュールを追加して設定](#add-and-configure-the-first-module)を行います。

## 最初のモジュールを追加して設定

クエスチョンマーク付きの空のモジュールは、追加する必要があるトリガーモジュールを表します。このモジュールは、実行されるたびにシナリオを開始します。空のモジュールの時計アイコンは、スケジュール設定済みモジュールであることを示します。

![](assets/empty-module.png)

このモジュールには、シナリオで監視するデータが格納されます。

1. 空のモジュールをクリックして、モジュールを選択するアプリを選択します。

   事前にプリロードしたアプリが、空のモジュールの横に表示されます。[!UICONTROL 検索]ボックスを使用して、モジュールを持つ他のアプリを追加できます。

   ![](assets/pre-loaded-apps-350x139.png)

1. クリック **[!DNL Google Sheets]**.

   リストが変わり、トリガーモジュールとして使用できるすべての [!DNL Google Sheets] モジュールが表示されます。

1. トリガーモジュールの「**[!UICONTROL レコードを監視]**」をクリックします。

   次に、Google アカウントへの認証済み接続を確立する必要があります。シナリオに追加するモジュールはすべて、アプリとの接続を確立する必要があります。

1. **[!DNL Google Sheets]** ボックスの「**[!UICONTROL 接続]**」で「**[!UICONTROL 追加]**」をクリックし、「Olivia&#39;s Google account」など、接続の名前を入力したら、「**[!UICONTROL 続行]**」をクリックします。
1. 表示されるウィンドウで接続を認証します。

   接続を認証するプロセスは、アプリ間で少し異なる場合があります。アプリへのログインが必要になる場合があります。通常は、「**[!UICONTROL 許可]**」ボタンをクリックする必要があります。ヘルプが必要な場合は、[アプリまたはサービスへの  [!DNL Adobe Workfront Fusion]  の接続について](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md)を参照してください。

## 最初のモジュールを設定

[!DNL Workfront Fusion] を [!DNL Google Sheets] アカウントに接続したら、アクセスが可能で、最初のモジュールで処理するデータがある [!DNL Google Sheets] スプレッドシートを指定します。

1. 「**[!UICONTROL スプレッドシート]**」ボックスをクリックし、表示されるリストから **[!UICONTROL Workfront Fusion practice scenario] #1** スプレッドシートを選択します。

   このスプレッドシートには 2 つのシート（タブ）が含まれているので、必要なデータが含まれているシートを指定する必要があります。

1. **[!UICONTROL シート]**&#x200B;ドロップダウンリストで、「**[!UICONTROL プロジェクト]**」を選択します。

   スプレッドシートにはヘッダーが含まれており、モジュールにはヘッダーを使って処理するデータを識別させます。

   ![](assets/spreadsheet-headers-350x55.png)

1. 「**[!UICONTROL テーブルにヘッダーが含まれる]**」は「**[!UICONTROL はい]**」を選択したままにします。

1. 「**[!UICONTROL ヘッダーがある行]**」ボックスで含める行の範囲を指定できますが、この演習ではデフォルトの「A1:Z1」のままにしておきます。
1. 「**[!UICONTROL 制限]**」ボックスに「1」と入力します。

   これで、シナリオを実行するたびに、モジュールはスプレッドシートの 1 行のみを処理します。これは、シナリオの作成中にテストの実行を簡略化する場合に役立ちます。

1. 「**[!UICONTROL OK]**」をクリックします。

   「**[!UICONTROL 開始場所を選択]**」ボックスによって、モジュールの処理を開始するスプレッドシート内の場所を指定するよう求められます。

1. 「**[!UICONTROL 手動で選択]**」をクリックし、表示されるリストの先頭のオプションを選択して、「**[!UICONTROL OK]**」をクリックします。
1. モジュールを右クリックし、「**[!UICONTROL 名前を変更]**」をクリックして、モジュールで実行する処理を説明する名前（「プロジェクトリストを監視」など）を入力したら、「**[!UICONTROL OK]**」をクリックします。

   名前はモジュールのすぐ下に表示されます。その下の [!DNL Workfront Fusion] には、モジュールで実行されるアクションのタイプに関する簡単な説明が含まれます。

   ![](assets/module-renamed-350x388.png)

1. 続けて、[2 つ目のモジュールを追加して設定](#add-and-configure-the-second-module)を行います。

## 2 つ目のモジュールを追加して設定

1. モジュールの右側の部分円をクリックして、「**[!UICONTROL 別のモジュールを追加]**」を選択します。

   この 2 番目のモジュールは [!DNL Workfront] モジュールにする必要がありますが、[!DNL Workfront] アプリのプリロードは行いませんでした。

1. [!DNL Workfront] アプリを検索するには、「[!DNL Workfront]」と入力を開始し、表示されたらアプリをクリックします。
1. 表示された [!DNL Workfront] モジュールのリストで、「**[!UICONTROL レコードを作成]**」をクリックします。

1. 先ほどの Google Sheets アプリの場合と同様に、[!DNL Workfront] ボックスで「**[!UICONTROL 追加]**」をクリックして、Workfront Fusion と Workfront 間の接続を追加します。

   次に、スプレッドシートのデータを使用して何を行うかを指定します。

1. スプレッドシートの行を使用して [!DNL Workfront] にプロジェクトを作成するため、「**[!UICONTROL レコードタイプ]**」をクリックして&#x200B;**[!UICONTROL プロジェクト]**&#x200B;を選択します。

   >[!TIP]
   >
   >「[!UICONTROL プロジェクト]」という単語を入力し始めると、リスト内に&#x200B;**[!UICONTROL プロジェクト]**&#x200B;が表示されます。

   ボックスが展開されて、使用可能なすべての [!DNL Workfront] プロジェクトフィールドが表示されます。ここに最初のモジュールで見つけた情報を入力できます。

   「**[!UICONTROL 名前]**」フィールドを使用します。このモジュールでは、対応する [!UICONTROL Google Sheets] 行のテキストを使用して、[!DNL Workfront] の各プロジェクトに名前を付けます。

1. 検索して「**[!UICONTROL 名前]**」フィールドをクリックします。

   >[!TIP]
   >
   >**Cmd+F**（[!DNL Mac] OS）または **Ctrl + F**（[!DNL Windows] OS）を使用すると、フィールドをすばやく特定できます。

   これにより、「**[!UICONTROL 名前]**」フィールドで使用できる変数のリストが開き、Workfront で作成された各プロジェクトの名前を定義できます。

   ![](assets/list-of-available-variables-350x261.png)

   リストの上部付近にある変数は、スプレッドシートの列ヘッダーに対応しています。

   ![](assets/spreadsheet-headers-marked-350x55.png)

   ![](assets/list-of-available-variables-marked-350x320.png)

1. 「**[!UICONTROL My Project Name (A)]**」変数をクリックして「**[!UICONTROL 名前]**」フィールドに追加します。

   これで、このシナリオの最初のデータがマッピングされました。

   スプレッドシートから [!DNL Workfront] にもう 1 つのデータ、各プロジェクトの開始日をマッピングしましょう。

1. 検索して「**[!UICONTROL 予定開始日]**」フィールドをクリックしてから「**[!UICONTROL Planned Begin Date (E)]**」変数をクリックすると、スプレッドシートのその列からデータが取り込まれます。

1. 「**[!UICONTROL OK]**」をクリックします。

   これで、動作するシナリオが作成されました。

1. 2 つ目のモジュールに「Workfront プロジェクトの作成」などの名前を付け、[シナリオのテスト](#test-the-scenario)に移ります。

## シナリオのテスト

シナリオをアクティベートする前にテストすることが重要です。少なくとも 1 回実行して結果を確認します。これは、シナリオにおけるデータの流れを理解し、エラーを見つけるのに役立ちます。

スプレッドシートの 1 行を処理して、Workfront にプロジェクトを作成することにしました。シナリオを実行すると、そのようになります。

1. シナリオエディターの左下にある「**[!UICONTROL 1 回実行]**」をクリックします。
1. シナリオの実行が終了したら、 [!DNL Google Sheets] モジュールの上のバブルをクリックします。

   ![](assets/click-bubble.png)

   表示されるボックスで、モジュールが処理したデータのバンドルに関する情報（最初に行のスプレッドシートから取り出した実際のデータなど）を確認できます。

   ![](assets/execution-inspector-g-sheets-350x637.png)

1.  [!DNL Workfront] モジュールの上にある実行インスペクターのバブルをクリックすると、情報の入力と出力（[!DNL Workfront] で作成されたプロジェクトの ID）を確認できます。

   ![](assets/execution-inspector-wf-350x384.png)

   シナリオ実行情報の読み取り方法について詳しくは、次の記事を参照してください。

   * 一般情報については、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md) でのシナリオ実行フローを参照してください。
   * 処理されたバンドルについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md) でのシナリオの実行、サイクル、フェーズを参照してください。

1. [!DNL Workfront] に移動して「soho downtown loft」を検索し、このシナリオで作成されたプロジェクトを確認します。これは、スプレッドシートの最後の行でした。
1. [!DNL Workfront Fusion] で、左下付近ににある&#x200B;**[!UICONTROL 保存]**&#x200B;アイコン ![](assets/save-icon.png) をクリックして、シナリオの進捗を保存します。

   >[!IMPORTANT]
   >
   >シナリオを改良、テストするたびに保存するようにしてください。

## シナリオを確定させて再度テストします

スプレッドシート内の他のすべての行のプロジェクトを作成する場合も、シナリオを設定する必要があります。

1. Google Sheet 用に作成した「**[!UICONTROL 行の監視]**」モジュールをクリックします。
1. 「**[!UICONTROL 制限]**」を 100 に変更します。

   スプレッドシートの行数よりも大きい数を指定すると、シナリオですべての行を確実に取り込むことができます。

1. 「**[!UICONTROL 行の監視]**」モジュールを右クリックし、「**[!UICONTROL 開始する場所を選択]**」、「**[!UICONTROL すべて]**」、「**[!UICONTROL OK]**」の順にクリックします。

1. 「**[!UICONTROL 1 回実行]**」をクリックし、実行インスペクターのバブルを確認します。

   [!DNL Google] Sheets の&#x200B;**[!UICONTROL 行の監視]**&#x200B;モジュールが 1 回だけ実行され、すべての行を読み取ります。その後、Workfront の&#x200B;**[!UICONTROL レコードの作成]**&#x200B;モジュールが 20 回実行され、スプレッドシートの残りの 20 行ごとにプロジェクトを作成します。

1. [!DNL Workfront] モジュールの実行インスペクターのバブルをクリックすると、20 個の操作がすべて表示されます。いずれかの操作をクリックすると、作成したプロジェクトに関する情報が表示されます。
1. 左下付近にある&#x200B;**[!UICONTROL 保存]**&#x200B;アイコン ![](assets/save-icon.png)をクリックします。
1. [!DNL Workfront] に移動して、シナリオで作成されたプロジェクトを確認します。

>[!TIP]
>
>各モジュールに関するメモを追加する方法として、任意ではあるものの便利な方法をお勧めします。
>
>1. [!DNL Workfront] モジュールを右クリックして、「**[!UICONTROL メモを追加]**」をクリックします。
>1. 表示されるメモに、モジュールの概要を入力します。
>
>    何度もモジュールを開いて内容を確認する必要がないので便利です。「スプレッドシートからマッピングされた名前、予定開始日、優先度を持つプロジェクトを作成」などと入力できます。
>
>    [!UICONTROL Google Sheets] モジュールの場合は、「追加した新しい行 / プロジェクトのプロジェクトリストの監視」などと入力できます。
>
>    1 つのモジュールに複数のノートを追加できます。
>
>1. **[!UICONTROL メモ]**&#x200B;エリアを閉じます。
>
>    シナリオにメモを追加すると、シナリオエディターの下部の&#x200B;**[!UICONTROL メモ]**&#x200B;アイコン![](assets/notes-icon-w-dot.png)にオレンジ色の点が表示されます。
>
>1. **[!UICONTROL メモ]**&#x200B;アイコン![](assets/notes-icon-w-dot.png)をクリックして、メモを表示します。
>



## シナリオをアクティベート

これが実際のデータに使用するシナリオの場合は、アクティベートするのは最後です。シナリオをアクティベートすると、デフォルトでは 15 分ごとに実行されます。これは、実行するタイミングと頻度を定義することで変更できます。

シナリオのアクティベートについて詳しくは、[Adobe Workfront Fusion でのシナリオのアクティベートまたはディアクティベート](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md)を参照してください。

スケジュールについて詳しくは、[Adobe Workfront Fusion でのシナリオのスケジュール](../../workfront-fusion/scenarios/schedule-a-scenario.md)を参照してください。
