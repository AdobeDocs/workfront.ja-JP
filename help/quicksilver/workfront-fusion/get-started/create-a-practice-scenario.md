---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Adobe Workfront Fusion でのプラクティス統合シナリオの作成
description: この記事では、Adobe Workfront Fusion で統合シナリオを作成する方法について説明します。 統合シナリオは、別々のアプリを接続し、異なるアプリケーションを通じてデータを送信できます。
author: Becky
feature: Workfront Fusion
exl-id: 643bb1d5-d7bc-402b-8ed1-9ca9a30e4560
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '2076'
ht-degree: 0%

---

# Adobe Workfront Fusion でのプラクティス統合シナリオの作成

この記事では、Adobe Workfront Fusion で統合シナリオを作成する方法について説明します。 統合シナリオは、別々のアプリを接続し、異なるアプリケーションを通じてデータを送信できます。

統合シナリオを作成するには、組織が [!DNL Workfront Fusion for Work Automation and Integration] ライセンス。

Workfrontのみの自動化シナリオの作成手順については、 [Adobe Workfront Fusion での自動化プラクティスシナリオの作成](../../workfront-fusion/get-started/create-a-practice-automation-scenario.md)

Workfront Fusion ライセンスの詳細については、 [Adobe Workfront Fusion ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

>[!NOTE]
>
>お客様の組織では、Googleシートへのアクセスが許可されていません。 その場合、この統合を設定することはできませんが、ここで示す情報は、統合シナリオの一般的な機能例として使用できます。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## プラクティスシナリオの作成

の役割 [!DNL Adobe Workfront Fusion] は、同じタスクを何度も繰り返す代わりに、新しいタスクに集中できるように、プロセスを自動化するためのものです。 アプリやサービス内でアクションをリンクして、データを自動的に転送および変換するシナリオを作成できます。 アプリまたはサービスのデータを監視し、そのデータを処理して目的の結果を提供するシナリオです。

シナリオは、アプリ内でのデータの変換方法や、アプリと Web サービスの間での転送方法を示す一連のモジュールで構成されます。

シナリオの作成方法を説明し、使用方法を学ぶ際にベストプラクティスを強化するには [!DNL Workfront Fusion]この記事では、プロセスの手順を順を追って説明します。 新しいレコードを作成するシナリオを次の場所に作成します。 [!DNL Workfront] 行ごとに [!DNL Google Sheets] スプレッドシート。

![](assets/finished-scenario-1-350x180.png)

>[!TIP]
>
>このようなシナリオは、でプロジェクトを使用する際に作業する必要のあるスプレッドシートリストプロジェクトがある場合に役立ちます。 [!DNL Workfront]. このシナリオでは、スプレッドシートで新しい行を「監視」し、に新しいプロジェクトを追加できます。 [!DNL Workfront] それぞれに対して

シナリオの作成は、主なタスクで構成されます。

## アプリを選択し、シナリオに名前を付けます

1. これをダウンロード [スプレッドシート](https://cdn.experience.workfront.com/Documentation/Workfront+Fusion/Fusion+Practice+Scenario+Sample+Sheet.xlsx)」、「 [!DNL Google Drive] この演習全体で使用します。

   または

   独自のシンプルなを作成または検索 [!DNL Google Sheets] スプレッドシートは次のようになります。

   ![](assets/spreadsheet-headers-350x55.png)

1. ログイン [!DNL Workfront Fusion] アカウント
1. クリック **[!UICONTROL シナリオ]** ![](assets/scenarios-icon.png) をクリックします。

   表示される左側のパネルで、シナリオをフォルダーに整理できます。

   右側のメイン領域の上部に、 **[!UICONTROL すべて]** 作成したシナリオ、 **[!UICONTROL アクティブなシナリオ]** および **[!UICONTROL 非アクティブなシナリオ]**、および **[!UICONTROL 概念]**（以前にさらに作業が必要なシナリオ） [!DNL Workfront Fusion] は、それらをアクティブまたは非アクティブに分類できます。

   ![](assets/scenarios-left-panel-350x215.png)

1. 左側のパネルで、 **[!UICONTROL フォルダーを追加]** アイコン ![](assets/add-folder-icon.png)次に、最初のフォルダーに「Practice scenarios」などの名前を入力します。

1. フォルダーを開いて、「 **[!UICONTROL 新しいシナリオの作成]** をクリックします。

   表示されるランディングページでは、作成するシナリオで使用するアプリをプリロードできます。

1. この演習では、「 」を検索し、「 」を選択します。 **[!UICONTROL Google Sheets]** アプリを使用します。
1. クリック **[!UICONTROL 続行]** をクリックします。

   シナリオエディターが表示され、中央に空のモジュールが表示されます。 [!DNL Google Sheets] アプリケーションがプリロードされ、一部のオプションが下部のツールバーに表示されます。

   ![](assets/scenario-editor-350x235.png)

   新しいシナリオの作成を開始する場合は、まずシナリオの名前を作成することをお勧めします。

1. を選択します。 **[!UICONTROL 新しいシナリオ]** プレースホルダー名を左上隅に入力し、「Practice scenario 1」などの名前を入力します。
1. 続行 [最初のモジュールを追加して設定します](#add-and-configure-the-first-module) 下

## 最初のモジュールを追加して設定します

疑問符付きの空のモジュールは、追加する必要のあるトリガーモジュールを表します。 このモジュールは、シナリオが実行されるたびに起動します。 空のモジュールの時計アイコンは、がスケジュール済みモジュールであることを示します。

![](assets/empty-module.png)

このモジュールには、シナリオで監視するデータが含まれます。

1. 空のモジュールをクリックして、モジュールを選択するアプリを選択します。

   事前に読み込んだアプリが、空のモジュールの横に表示されます。 を使用して、モジュールを持つ他のアプリを追加できます。 [!UICONTROL 検索] ボックス

   ![](assets/pre-loaded-apps-350x139.png)

1. クリック **[!DNL Google Sheets]**.

   リストがすべての [!DNL Google Sheets] モジュールモジュールとして使用できるトリガー。

1. トリガー **[!UICONTROL レコードを監視]**.

   次に、Googleアカウントへの認証済み接続を確立する必要があります。 シナリオに追加するモジュールはすべて、アプリに接続する必要があります。

1. 内 **[!DNL Google Sheets]** ボックス、下 **[!UICONTROL 接続]**&#x200B;をクリックし、 **[!UICONTROL 追加]**&#x200B;次に、「Olivia&#39;s Google account」など、接続の名前を入力し、 **[!UICONTROL 続行]**.
1. 表示されるウィンドウで接続を認証します。

   接続を認証するプロセスは、アプリ間で少し異なる場合があります。 デスクトップアプリケーションへのログインが必要になる場合があります。 通常、 **[!UICONTROL 許可]** 」ボタンをクリックします。 ヘルプが必要な場合は、 [接続について [!DNL Adobe Workfront Fusion] アプリまたはサービスに](../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md).

## 最初のモジュールの設定

接続後 [!DNL Workfront Fusion] を [!DNL Google Sheets] アカウントを使用する場合は、 [!DNL Google Sheets] にアクセスできるスプレッドシートと、最初のモジュールで処理するデータ。

1. 次をクリック： **[!UICONTROL スプレッドシート]** 」ボックスで、 **[!UICONTROL Workfront Fusion プラクティスのシナリオ] #1** スプレッドシートが表示されます。

   このスプレッドシートには 2 つのシート（タブ）が含まれているので、必要なデータが含まれているシートを指定する必要があります。

1. 内 **[!UICONTROL シート]** ドロップダウンリストで、「 **[!UICONTROL プロジェクト]**.

   スプレッドシートにはヘッダーが含まれており、モジュールでそれらを使用して処理するデータを識別します。

   ![](assets/spreadsheet-headers-350x55.png)

1. 終了 **[!UICONTROL はい]** 次の項目で選択： **[!UICONTROL テーブルにヘッダーが含まれています]**.

1. 内 **[!UICONTROL ヘッダー付きの行]** ボックスで、含める行の範囲を指定できますが、この演習ではデフォルトの A1:Z1 をそのままにしておきます。
1. 内 **[!UICONTROL 制限]** 「 」ボックスに「 1 」と入力します。

   これにより、シナリオを実行するたびに、モジュールはスプレッドシートの 1 行のみを処理します。 これは、シナリオの作成中にテストの実行を簡略化する場合に役立ちます。

1. クリック **[!UICONTROL OK]**.

   この **[!UICONTROL 開始場所を選択]** 」ボックスに、モジュールの処理を開始するスプレッドシート内の場所を指定するよう求められます。

1. クリック **[!UICONTROL 手動で選択]**」をクリックし、表示されるリストの上部のオプションを選択して、 **[!UICONTROL OK]**.
1. モジュールを右クリックし、 **[!UICONTROL 名前を変更]**&#x200B;次に、モジュールで実行する操作を説明する名前（例：「プロジェクトリストを見る」）を入力し、 **[!UICONTROL OK]**.

   名前はモジュールのすぐ下に表示されます。 その下に [!DNL Workfront Fusion] には、モジュールで実行されるアクションのタイプに関する簡単な説明が含まれます。

   ![](assets/module-renamed-350x388.png)

1. 続行 [2 番目のモジュールの追加と設定](#add-and-configure-the-second-module).

## 2 番目のモジュールの追加と設定

1. モジュールの右側の部分円をクリックして、 **[!UICONTROL 別のモジュールを追加]**.

   この 2 番目のモジュールは、 [!DNL Workfront] モジュールに対して、 [!DNL Workfront] アプリを使用します。

1. 次を検索： [!DNL Workfront] app，入力を開始する&quot;[!DNL Workfront]」と表示されたら、アプリをクリックします。
1. リスト内の [!DNL Workfront] 表示されたモジュールで、 **[!UICONTROL レコードを作成]**.

1. Google Sheets アプリの場合と同様に、「 **[!UICONTROL 追加]** 内 [!DNL Workfront] ボックスを使用して、Workfront Fusion とWorkfrontの間の接続を追加します。

   次に、スプレッドシートのデータを使用して何を行うかを指定します。

1. クリック **[!UICONTROL レコードタイプ]**&#x200B;を選択し、「 **[!UICONTROL プロジェクト]** でプロジェクトを作成するので [!DNL Workfront] スプレッドシートの行を使用します。

   >[!TIP]
   >
   >以下を見つけることができます。 **[!UICONTROL プロジェクト]** 」という単語を[!UICONTROL プロジェクト].&quot;

   ボックスが展開し、使用可能なすべての [!DNL Workfront] 最初のモジュールで見つかった情報を配置できるプロジェクトフィールド。

   使用する **[!UICONTROL 名前]** フィールド：このモジュールで、内の各プロジェクトに名前を付けます [!DNL Workfront] 対応する [!UICONTROL Google Sheets] 行

1. を検索して、 **[!UICONTROL 名前]** フィールドに入力します。

   >[!TIP]
   >
   >以下を使用できます。 **Cmd+F** ([!DNL Mac] (OS) または **Ctrl + F**([!DNL Windows] OS) を使用して、すばやくフィールドを検索できます。

   これにより、 **[!UICONTROL 名前]** 「 」フィールドを使用して、Workfrontで作成する各プロジェクトの名前を定義します。

   ![](assets/list-of-available-variables-350x261.png)

   リストの上部付近にある変数は、スプレッドシートの列ヘッダーに対応しています。

   ![](assets/spreadsheet-headers-marked-350x55.png)

   ![](assets/list-of-available-variables-marked-350x320.png)

1. 変数をクリックします。 **[!UICONTROL マイプロジェクト名 (A)]** を **[!UICONTROL 名前]** フィールドに入力します。

   このシナリオの最初のデータをマッピングしました。

   スプレッドシートからにデータをもう 1 つマッピングしましょう。 [!DNL Workfront]:各プロジェクトの開始日。

1. を検索して、 **[!UICONTROL 計画開始日]** フィールドに値を入力し、 **[!UICONTROL 計画開始日 (E)]** 変数を使用して、スプレッドシートのその列からデータを取り込みます。

1. クリック **[!UICONTROL OK]**.

   これで、動作するシナリオが作成されました。

1. 2 つ目のモジュールに「Workfrontプロジェクトの作成」などの名前を付け、次に [シナリオのテスト](#test-the-scenario).

## シナリオのテスト

シナリオをアクティブ化する前に、少なくとも 1 回実行し、結果を表示して、シナリオをテストすることが重要です。 これは、データがシナリオをどのように流れているかを理解し、エラーを見つけるのに役立ちます。

スプレッドシートの 1 行を処理して、Workfrontにプロジェクトを作成することを選択しました。 シナリオを実行すると、そのようになります。

1. クリック **[!UICONTROL 1 回実行]** をクリックします。
1. シナリオの実行が終了したら、 [!DNL Google Sheets] モジュール。

   ![](assets/click-bubble.png)

   表示されるボックスに、モジュールが処理したデータのバンドルに関する情報（最初に行のスプレッドシートから取り出した実際のデータなど）を表示できます。

   ![](assets/execution-inspector-g-sheets-350x637.png)

1. 実行インスペクターのバブルを [!DNL Workfront] モジュールを使用して、情報の入力と出力 ( 現在は [!DNL Workfront]

   ![](assets/execution-inspector-wf-350x384.png)

   シナリオ実行情報の読み取り方法について詳しくは、次の記事を参照してください。

   * 一般情報については、 [のシナリオ実行フロー [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).
   * 処理されたバンドルについて詳しくは、 [のシナリオの実行、サイクル、フェーズ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md).

1. に移動します。 [!DNL Workfront] 「soho downtown loft」を探して、このシナリオが作成したプロジェクトを確認します。 これは、スプレッドシートの最後の行です。
1. In [!DNL Workfront Fusion]をクリックし、 **[!UICONTROL 保存]** ![](assets/save-icon.png) 左下隅付近に表示され、シナリオの進行状況を保存できます。

   >[!IMPORTANT]
   >
   >シナリオの作成時に頻繁に保存し、テストします。

## シナリオを最終決定し、再度テストします

スプレッドシート内の他のすべての行のプロジェクトを作成するには、シナリオを設定する必要があります。

1. 次をクリック： **[!UICONTROL 監視行]** Google Sheet 用に作成したモジュール。
1. を **[!UICONTROL 制限]** を 100 に設定します。

   行数よりも大きい数を指定すると、シナリオはすべての行を確実に取り込むことができます。

1. を右クリックします。 **[!UICONTROL 監視行]** モジュール、クリック **[!UICONTROL 開始場所を選択]**&#x200B;をクリックし、 **[!UICONTROL すべて]**&#x200B;を選択し、「 **[!UICONTROL OK]**.

1. クリック **[!UICONTROL 1 回実行]** そして、実行検査官の泡が何を示しているか見てみましょう。

   この [!DNL Google] シート **[!UICONTROL 監視行]** モジュールは 1 回だけ実行され、すべての行を読み取ります。 その後、Workfront **[!UICONTROL レコードを作成]** モジュールは 20 回実行され、スプレッドシートの残りの 20 行ごとにプロジェクトを作成します。

1. 実行インスペクターのバブルをクリックします。 [!DNL Workfront] モジュールで 20 個の操作をすべて表示し、いずれかの操作をクリックして、作成したプロジェクトに関する情報を表示します。
1. クリック **[!UICONTROL 保存]** ![](assets/save-icon.png) 左下隅付近に
1. に移動します。 [!DNL Workfront] ：シナリオが作成したプロジェクトを表示します。

>[!TIP]
>
>各モジュールに関するメモを追加する方法としては、オプションですが便利な方法を推奨します。
>
>1. を右クリックします。 [!DNL Workfront] モジュール、次に **[!UICONTROL メモを追加]**.
>1. 表示されるメモに、モジュールの概要を入力します。

>
>   モジュールを開いて何が起きているかを絶えず確認する必要がないので、これは便利です。 「スプレッドシートからマッピングされた名前、計画開始日、優先度を持つプロジェクトを作成します」などの値を入力できます。
>
>   の [!UICONTROL Google Sheets] モジュールの場合は、「プロジェクトリストを監視して新しい行/プロジェクトを追加」などの値を入力できます。
>
>   1 つのモジュールに複数のメモを追加できます。
>
>1. を閉じる **[!UICONTROL メモ]** 領域
>
>   シナリオにメモを追加すると、オレンジ色の点が **[!UICONTROL メモ]** アイコン ![](assets/notes-icon-w-dot.png) をクリックします。
>
>1. 次をクリック： **[!UICONTROL メモ]** アイコン ![](assets/notes-icon-w-dot.png) をクリックしてメモを表示します。

>




## シナリオを有効化

これが実際のデータに使用するシナリオの場合は、最後にアクティブ化します。 シナリオをアクティブ化すると、デフォルトでは、15 分ごとに実行されます。 これは、実行するタイミングと頻度を定義することで変更できます。

シナリオの有効化について詳しくは、 [Adobe Workfront Fusion でのシナリオのアクティブ化または非アクティブ化](../../workfront-fusion/scenarios/activate-or-inactivate-scenario.md).

スケジュールについて詳しくは、 [Adobe Workfront Fusion でのシナリオのスケジュール](../../workfront-fusion/scenarios/schedule-a-scenario.md).
