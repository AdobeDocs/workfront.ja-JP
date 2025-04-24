---
title: Adobe App Builderを使用したWorkfrontのカスタムアプリケーションの作成
description: Adobe App Builderを活用したWorkfront UI 拡張機能を使用すると、お客様およびパートナーはカスタマイズされたユーザーエクスペリエンスを作成できます。
author: Courtney
feature: Digital Content and Documents
hide: true
hidefromtoc: true
source-git-commit: 7c82dc70c5fde69c905b74f28a0ff9add663dbd9
workflow-type: tm+mt
source-wordcount: '1705'
ht-degree: 0%

---


# Adobe App Builderを使用したWorkfrontのカスタムアプリケーションの作成

Adobe App Builderを活用したWorkfront UI 拡張機能を使用すると、お客様およびパートナーはカスタマイズされたユーザーエクスペリエンスを作成できます。 これらのツールは、効率を高め、シームレスでつながりのあるエクスペリエンスを提供し、ユーザー満足度を大幅に向上させ、企業が独自のビジョンを実現するのに役立ちます。

例えば、Workfront UI Extensions がない場合、プロジェクト管理者はWorkfrontと、時間を記録する別の時間追跡システムを切り替える必要が生じる場合があります。 UI 拡張機能を使用すると、時間の追跡をWorkfront エクスペリエンスに直接統合し、ワークフローを合理化して時間を節約できます。 さらに、カスタムコンポーネントを追加すると、メタデータのタグ付けやコンテンツのプレビューなどの機能により、使いやすさを向上させ、繰り返しのタスクを自動化し、コンテンツ管理を強化することができます。 Adobe App Builderは、拡張性と堅牢な IMS （Identity Management）を提供し、あらゆる規模で安全で効率的なカスタマイズを保証します。

Workfront UI 拡張機能には、次のような主な利点があります。

* 正確なカスタマイズ：標準的なソフトウェアインターフェイスでは、すべてのビジネス要件を満たすことができないことが多くあります。 UI 拡張機能を使用すると、開発者は、デフォルトのユーザーインターフェイスを変更および拡張して、特定のビジネスニーズに対応できます。
* システム統合：UI 拡張により、他のシステムとの統合が容易になり、シームレスなワークフローとデータの一貫性が確保されます。
* スケーラビリティ：企業の成長に合わせて、システムを完全に見直すことなく、UI 拡張機能を開発して新しい機能を追加できます。
* 開発時間の短縮：事前定義済みの拡張ポイントとツールにより、カスタム機能の実装に必要な時間と労力が大幅に削減されます。
* ユーザーによる導入の強化：ユーザーエクスペリエンスが最適化されると、ソフトウェアの導入を大幅に促進できます。 ユーザーの好みに合わせて設計されたカスタム UI 要素により、採用率と全体的な満足度を高めることができます。
* Workfront UI 拡張機能を利用すると、効率性、統合性、ユーザー満足度を高めるために、カスタマイズされたユーザーエクスペリエンスを作成できます。

Adobe App Builderでアプリケーションが作成されたら、Workfront管理者は、レイアウトテンプレートを使用して、そのアプリケーションをWorkfrontのメインメニューと左側のナビゲーションパネルに追加できます。 レイアウトテンプレートを使用しているユーザーがアプリケーションをクリックすると、アプリケーションを個別に開かなくても、Workfrontに埋め込まれたアプリケーションが表示されます。

ここでは、App Builderにアクセスし、テンプレートを使用してアプリケーションを作成する方法を説明します。

レイアウトテンプレートにカスタムアプリケーションを追加する方法については、[ レイアウトテンプレートを使用してメインメニューをカスタマイズする ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md) および [ レイアウトテンプレートを使用して左側のパネルをカスタマイズする ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md) を参照してください。

## 前提条件

以下が必要です。

* IMS が有効なWorkfront アカウント
* ノード v18 および npm を持つ開発マシン

## Adobe App Builderへのアクセス

UI 拡張機能を作成するには、Adobe Developer ConsoleのAdobe App Builderにアクセスできる必要があります。

その他の手順については、[Adobe Developer サイト ](https://developer.adobe.com/uix/docs/guides/get-access/) を参照してください。

### Adobe Admin Consoleへの開発者の追加

>[!IMPORTANT]
>
>次の手順のすべてに適切な IMS 組織を選択していることを確認します。 複数の組織に属している場合は、間違った組織を選択する可能性があります。 通常は右上隅にリストされている適切な組織の下で作業していることを確認します。

1. 実稼動に移動します。https://adminconsole.adobe.com/

1. 「**ユーザー**」セクションで、**開発者**/**開発者を追加** をクリックします。

   ![admin console でのユーザーの追加 ](assets/manage-users-admin-console.png)

   >[!NOTE]
   >
   >開発者を管理するオプションが表示されない場合、開発者がアクセスできる製品はありません。

1. ユーザーのメールアドレスを追加します。 Admin Console 内から既に追加されている既存のユーザーを検索する必要があります。

1. 開発者プロファイルに必要な製品を追加して、「**保存**」をクリックします。\
   ![ 開発者を追加 ](assets/add-developer.png)

### App Builderへのアクセスの取得

組織がApp Builderを購入するには、担当のアカウントマネージャーと協力する必要があります。

AppBuilder の統合をテストするには、IMS 組織の無料体験版を次の場所でリクエストします。https://developer.adobe.com/app-builder/trial/#

AppBuilder が正しく設定されている場合は、新しいプロジェクトの作成の一部として、テンプレートからプロジェクトを作成が表示されます。

## Adobe Developer Consoleで新規プロジェクトを作成します

UI 拡張機能を構築するには、Adobe Developer Consoleを使用する必要があります。

その他の手順については、[Adobe Developer サイト ](https://developer.adobe.com/uix/docs/guides/creating-project-in-dev-console/) を参照してください。

1. Adobe IDを使用してAdobe Developer Consoleにログインします。

1. アカウント、およびプロファイルまたは組織を選択します。

1. クイックスタート領域で **テンプレートからプロジェクトを作成** をクリックするか、**新規プロジェクトを作成/テンプレートからプロジェクト** をクリックします。

   >[!IMPORTANT]
   >
   >テンプレートからプロジェクトを作成するオプションが表示されない場合は、Admin Console の設定が誤っており、app Builder カタログにアクセスできません。 このオプションは、AppBuilder にアクセスできる場合にのみ表示されます。

   ![ テンプレートから作成 ](assets/create-from-template.png)

1. 「**App Builder**」を選択します。

1. **プロジェクトタイトル** および **アプリ名** を入力します。 どちらもデフォルト値がありますが、値をカスタマイズすると、後で必要なプロジェクトを識別しやすくなります。

1. **ランタイムを含む** が選択されたままにします。

1. **保存**&#x200B;をクリックします。

## Adobe IO （aio） CLI の使用

Adobeには、App Builder アプリケーションの作成に使用できるオープンソース CLI が用意されています。

その他の手順については、GitHub とAdobe Developer サイトを参照してください。

* https://github.com/adobe/aio-cli
* https://developer.adobe.com/app-builder/docs/getting_started/first_app/

1. ツールをインストールするには、（最初にノード v18 を使用していることを確認して） `npm install -g @adobe/aio-cli` を実行します。
1. ターミナルを起動し、次のコマンドで AIO にログインします：`aio login`。 正しい IMS 組織へのログインで問題が発生した場合は、`aio login -f` 試行して強制的にログインプロンプトを表示させます。 `aio where` を使用して、正しい IMS 組織にログインしている組織を確認します。 詳細については、`aio config` を使用してください。
1. 次を実行してアプリの設定を開始 `aio app init example-app` ます。「example-app」をアプリ名に置き換えてください。 アプリ名が不明な場合は、コマンド `aio console project list` を使用してアプリ名のリストを確認できます。
1. 提供されたオプションから組織とプロジェクトを選択します。
   ![ コマンドの結果 ](assets/1-command-result.png)
   ![ プロジェクトの選択 ](assets/2-select-a-project.png)

1. 使用可能なすべてのテンプレートを参照し、プロジェクトの **@adobe/workfront-ui-ext-tpl** を選択します。
   ![ テンプレートを選択 ](assets/3-choose-template.png)
1. を選択し、Adobe Developer Consoleで作成したプロジェクト名を入力します。
   ![ プロジェクト名を選択および入力 ](assets/4-select-and-enter-project-name.png)

1. アプリケーションのプロンプトに答えます。

   * 拡張機能に名前を付けます。
   * 拡張機能の機能の説明的な概要を提供します。
   * 開始する初期バージョン番号を選択します。
   * 「次に何をしますか？」というメッセージが表示されたときに「メインメニュー項目にカスタムボタンを追加する」を選択した場合、テンプレートによってプライマリナビゲーションボタンのコードが作成されます。

   ![ 「完了」を選択 ](assets/5-select-done.png)

1. 「完了」を選択して完了を確認します。 テンプレートからのコード生成が進行中です。
   ![ 生成中 ](assets/6-generation-in-process.png)
1. アプリの初期化が完了したことを示すメッセージが表示されるまで待ちます。 その後、プロジェクトを IDE で開き（VSCode をお勧めします）、src フォルダーにアクセスできます。

   プロジェクト内のフォルダーおよびファイルについて詳しくは、[Adobe開発者向けサイト ](https://developer.adobe.com/app-builder/docs/getting_started/first_app/#5-anatomy-of-an-appbuilder-application) を参照してください。

## VSCode での拡張機能の構築

Workfrontのメインメニューまたはセカンダリナビゲーション（左パネル）を使用したナビゲーションを有効にするには、App.js ファイル設定が必要です。

Workfront レイアウトテンプレートで拡張機能を表示するには、ExtensionRegistration.js ファイル設定が必要です。

次の例は、UI 拡張機能を使用して、Workfrontのメインメニューとオブジェクトの左側のパネルにカスタムアプリケーションを追加する方法を示しています。

### ExtensionRegistration.js の設定

Workfrontのメインメニューでカスタムアプリケーションを許可するには：

1. ExtensionRegistration.js に移動します。

ExtensionRegistration 関数に、次のコードが表示されます。 このコードは、テンプレートによって作成されました。 このコードを追加して、追加のメニュー項目を作成できます。 ID と URL を必ず置き換えてください。

    ```
    mainMenu: {
    
    getItems （） {
    
    return [
    
    {
    
    id: &#39;main-menu-label&#39;,
    
    url: &#39;/index.html#/main-menu-label&#39;,
    
    label: &#39;Main menu label&#39;,
    
    icon: icon1,
    
    },
    
    ];
    
    },
    
    }
    ```

1. 次のコードスニペットを追加します。
   ![ コードスニペット ](assets/7-extension-registration-step1-from-sam.png)
この例では、メイン メニュー項目を示します。 ID、ラベル、アイコン、URL を、アプリケーションに適した名前に更新する必要があります。 複数の項目を追加する場合は、ID が一意であることを確認します。

1. 作業内容を保存します。

### Workfrontの左側のパネルナビゲーションでのカスタムアプリケーションの許可

Workfrontの左側のパネルナビゲーションでカスタムアプリケーションを許可するには：

1. ExtensionRegistration.js に移動します。
1. ExtensionRegistration 関数に、次のコードスニペットを追加します。

   ```
   secondaryNav: {  
   
   TASK: {  
   
       getItems() {       return [         {           id: "TASK", 
   
   label: "My TASK",           icon: metricsIcon,           url: "/myTask",  
   
           },  
   
       ];  
   
       },  
   
   },  
   
   },  
   ```

   ![ 拡張機能の登録 ](assets/8-extension-registration-file-step2.png)

   * 次の例は、My Task という左側のパネルのナビゲーション項目を示しています。 ID、ラベル、アイコン、URL を、アプリケーションに適した名前に更新する必要があります。

   * 次の使用例は、プロジェクト オブジェクトの種類の左側のパネルのナビゲーション項目を示します。 これらの項目は、Workfrontでサポートされているオブジェクトごとに個別に作成する必要があります。 使用できるオブジェクトは、プロジェクト、タスク、イシュー、ポートフォリオ、プログラムです。

1. 作業内容を保存します。

### App.js の設定

1. App.js に移動します。

1. テンプレートは、メインメニューオプションのルートになります。 ルートは、URL パスと、これらのパス用にレンダリングされるコンポーネントとのマッピングを定義します。 ルートを追加するには、次のコードスニペットを使用して、正確なパスと要素を自分のものに置き換えてください。

   ```
       <Route 
   
               exact path="custom-application" 
   
               element={<Customapplication />} 
   
           /> 
   ```

   ![ コードの例 ](assets/9-app-file-step-1-from-sam.png)
1. 作業内容を保存します。

アプリケーションの開発と実行について詳しくは、[Adobe開発者向けサイト ](https://developer.adobe.com/app-builder/docs/getting_started/first_app/#6developing-the-application) を参照してください。

## 共有コンテキスト

共有コンテキストは、Workfrontから UI 拡張機能にデータを共有するために使用されます。 共有コンテキストを通じて利用可能なデータは、ユーザーデータとアプリケーションコンテキストを含む。


### ユーザー

Workfrontの UI 拡張機能は、ユーザーデータを共有します。 共有コンテキストを通じて使用可能なユーザーオブジェクトには、Workfront ユーザー ID とユーザーのメールアドレスが含まれます。

`user = (conn?.sharedContext?.get("user")); // {ID: '1', email: 'test@aaa.com'} userID = user.ID userEmail = user.email `

### アプリケーションコンテキスト

セカンダリのナビゲーション拡張機能ポイントを使用してカスタムアプリケーションを追加する場合、カスタムアプリケーションでプロジェクト ID やドキュメント ID などのコンテキストデータを使用するのが一般的です。 これらのデータの場合、共有コンテキストには、オブジェクトコードとオブジェクト ID が含まれます。

次に、ドキュメントのアプリケーションコンテキストを取得する例を示します。

`context = conn?.sharedContext; // Using the connection created above, grab the document details from the host tunnel. // conn?.host?.document?.getDocumentDetails().then(setDocDetails); `

## Workfrontでのアプリのテスト

App Builder アプリケーションをWorkfront用に開発する際に、アプリを公開せずにWorkfront内でテストする必要が生じる場合があります。

App Builder アプリ内で、ローカル開発の `aio app run` を開始できます。 これにより、URL （通常は `https://localhost:9080`）が提供されます。 または、`aio app deploy` を実行して静的Adobe ドメインを取得することもできます。 今後の使用のために、これらの URL をメモしておいてください。

次に、ブラウザーで開発対象の特定のページに移動します。 開発者ツールを開き、workfront.comまたはworkfront.adobe.comのローカルストレージにアクセスします。 ここでは、エントリを追加する必要があります。 キーとして `extensionOverride` を使用し、値として以前にメモした App Builder URL を使用します。

設定が正しく完了した場合、Workfrontでレイアウトテンプレートページをリロードすると、App Builder アプリケーションのボタンが表示されます。 オブジェクトのメインメニューと左側のパネルにアプリのボタンを追加し、それらの領域に正しく表示されることを確認します。

Adobe開発者向けサイトで、AEMの例を使用した追加手順を参照できます。https://developer.adobe.com/uix/docs/guides/preview-extension-locally/

## 申請の公開と送信の承認

アプリを公開して承認するには、[Adobe開発者サイト ](https://developer.adobe.com/uix/docs/guides/publication/) の手順に従ってください。