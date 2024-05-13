---
product-area: documents
navigation-topic: approvals
title: Workfront ドキュメントの詳細内の AppBuilder
description: AppBuilder はドキュメントの詳細内でインストールできます
author: Courtney
feature: Work Management, Digital Content and Documents
hide: true
hidefromtoc: true
recommendations: noDisplay, noCatalog
exl-id: 74e0a85b-a8aa-4e39-9c2e-0f09957ebafa
source-git-commit: 21ef9365561fca2301223ae79f6371f3c94c7313
workflow-type: tm+mt
source-wordcount: '1334'
ht-degree: 0%

---

# Workfront ドキュメントの詳細内の AppBuilder

AppBuilder は、「ドキュメントの詳細」内でインストールできます。

## 前提条件

以下が必要です。

* IMS が有効なWorkfront アカウント
* ノード v18 および npm を持つ開発マシン

## Admin Console への開発者の追加

>[!IMPORTANT]
>
>次の手順のすべてに適切な IMS 組織を選択していることを確認します。 複数の組織に属している場合は、間違った組織を選択する可能性があります。 通常は右上隅にリストされている適切な組織の下で作業していることを確認します。


1. 次のいずれかに移動します。

* ステージ： [https://stage.adminconsole.adobe.com/](https://stage.adminconsole.adobe.com/)
* 実稼動： [https://adminconsole.adobe.com/](https://adminconsole.adobe.com/)

1. 「ユーザー」セクションで、 **開発者** > **開発者を追加**.

   ![](assets/manage-users-admin-console.png)

   >[!NOTE]
   >
   >開発者を管理するオプションが表示されない場合、開発アクセスを許可する製品はありません。 Workfrontは開発者アクセスを提供しませんが、AEMは提供します。 表示されない場合は、開発者向けアプリのリストにWorkfrontを含める方法を見つける必要があります。

1. ユーザーのメールアドレスを追加します。 Admin Console 内から既に追加されている既存のユーザーを検索する必要があります。

1. 開発者プロファイルに必要な製品を追加し、 **保存**.

![](assets/add-developer.png)

## AppBuilder へのアクセスの取得

組織は、アカウントマネージャーと協力して AppBuilder を購入する必要があります。 POC に対してこれを行う必要がなかったので、正確なプロセスは理解されていません。

AppBuilder の統合をテストする場合は、IMS 組織に次の場所で無料体験版をリクエストできます。
[https://developer.adobe.com/app-builder/trial/#](https://developer.adobe.com/app-builder/trial/#)

30 日間の無料トライアルであっても、その後は実際にトライアルを無効にできないという印象を持っています。

AppBuilder が正しく設定されている場合は、新しいプロジェクトの作成の一部として「テンプレートからプロジェクトを作成」が表示されます（次の節で説明します）。

## 開発コンソールでの新しいプロジェクトの作成

1. クリック **テンプレートからプロジェクトを作成**.

   >[!IMPORTANT]
   >
   >このオプションが表示されない場合は、Admin Console の設定が誤っており、app Builder カタログにアクセスできません。 このオプションは、AppBuilder にアクセスできる場合にのみ表示されます。

   ![](assets/create-from-template.png)

1. を選択 **App Builder**.

1. を入力 **プロジェクトタイトル** および **アプリ名**. どちらもデフォルト値がありますが、値をカスタマイズすると、後で必要なプロジェクトを特定しやすくなります。

   >[!NOTE]
   >
   >この手順でワークスペースを追加するオプションがあります。 開発者向けにワークスペースを作成してはどうかと提案されました。 これにより、開発者の作業に合わせて、シークレットとデプロイメントを相互に分離することができます。 ワークスペースには、使用する開発者の名前を付ける必要があります。 AIO CLI には、ワークスペースを切り替えるためのオプションがあります。これについては後ほど説明します。


1. 移動 **ランタイムを含める** を選択しました。 理由は分からないわ、本当に、でも変えないで！

1. 「**保存**」をクリックします。

## AdobeI/O （aio） CLI

Adobeには、App Builder アプリケーションの作成に役立つオープンソース CLI が用意されています。 ドキュメントは次の場所にあります。 [https://github.com/adobe/aio-cli](https://github.com/adobe/aio-cli) app Builder のAdobe手順と同様に [https://developer.adobe.com/app-builder/docs/getting_started/first_app/](https://developer.adobe.com/app-builder/docs/getting_started/first_app/).

1. インストール
   1. ツールをインストールするには、（最初にノード v18 を使用していることを確認して）次を実行します。 `npm install -g @adobe/aio-cli `.

1. ターミナルでの認証
   1. ターミナルを起動し、次のコマンドを使用して AIO にログインします。 `aio login`.

1. アプリケーションの初期化
   1. 以下を実行して、アプリの設定を開始します。 `aio app init example-app`.

1. 設定の選択
   1. 表示されたオプションから組織とプロジェクトを選択します。\
      ![](assets/select-org.png)
      ![](assets/select-project.png)

1. テンプレートの選択と設定
   1. 使用可能なすべてのテンプレートを参照し、 **@adobe/aem-cf-editor-ui-ext-tpl** プロジェクトのテンプレート。
      ![](assets/search-template.png)
      ![](assets/select-template.png)

1. 拡張機能の定義
   1. 拡張機能に名前を付けます。
   1. 拡張機能の機能の説明的な概要を提供します。
   1. 開始する初期バージョン番号を選択します。
   1. を選択して完了を確認 **完了しました**.
      ![](assets/define-extension.png)

1. プロジェクトフォルダーに移動します
   1. src フォルダーへのアクセス
   1. フォルダーの名前を変更する `aem-cf-editor-1` 対象： `workfront-doc-details-1`.

1. 設定ファイルの変更
   1. app.config.yaml を開きます
   1. ラインを次から更新 `aem/cf-editor/1` 対象： `workfront/doc-details/1`.
   1. インクルードパスを次から調整 `src/aem-cf-editor-1/ext.config.yaml` 対象： `src/workfront-doc-details-1/ext.config.yaml`.

1. 拡張機能登録コンポーネントの編集
   1. 開く `src/workfront-doc-details-1/web-src/src/components/ExtensionRegistration.js`.
   1. 「メソッド」セクションで、関数を追加します `secondaryNav` 非同期関数を含む `getButtons`.
   1. `getButtons` は、次の構造を持つオブジェクトを受け取る必要があります。

      ```
          {
          docId: "String",  // Document ID
          docvId: "String", // Document version ID
          sharedContext: {
              hostname: "String",
              protocol: "String",
              auth: {
              imsOrgID: "String",    // Customer's IMS Org ID
              imsToken: "String",    // User's IMS token
              imsClientId: "String"
              }
          }
          }
      ```

1. この関数は、ナビゲーションに表示されるボタンオブジェクトの配列を返します。

   ```
       methods: {
       secondaryNav: {
           async getButtons({docId, docvId, sharedContext}) {
           return [
               { label: 'Registration', url: '/index.html' },
               { label: 'Review', url: '/index.html#review' }
           ];
           }
       }
       }
   ```

1. アプリケーションルーティングの設定
   1. App.js ファイルを開き、新しく開発された機能が含まれるようにルートを設定します。 デフォルトビューおよびレビューページなどの追加ビューのルートを設定する必要があります。 これらのルートを定義する方法を次に示します。

      ```
          <Route index element={<ExtensionRegistration />} />
          <Route exact path="index.html" element={<ExtensionRegistration />} />
          <Route exact path="review" element={<Review />} />
      ```

1. ドキュメントの詳細へのアクセス
   1. 提供された関数の実装 `document.getDocumentDetails` アプリケーション内で重要なドキュメント詳細を取得します。 この関数は、を含むオブジェクトを取得します。 `docId` および `docvId`、と `sharedContext` を含むオブジェクト `hostname`, `protocol`、および認証の詳細です。 アプリケーションがこのデータを適切に処理していることを確認します。

1. データ取得をコンポーネントに統合する
   1. 新しいコンポーネントをアプリケーションの components フォルダーに追加します。 このコンポーネント内で、Workfrontへの接続を確立し、ホストアプリケーションと確立された接続を使用してドキュメント情報と認証データを取得します。 これを処理するためにコンポーネントを構築する方法の例を次に示します。

      ```
          import { useEffect, useState } from 'react';
          import { attach } from "@adobe/uix-guest";
          import { extensionId } from "./Constants";
      
          function Review() {
              const [conn, setConn] = useState();
      
              useEffect(() => {
              const iife = async () => {
                  // "attach" the guest application to the host. This creates a "tunnel" from the host app that allows data to be passed to the iframe running this app.
                  const connection = await attach({
                  id: extensionId,
                  });
                  setConn(connection);
              };
      
              iife();
              }, []);
      
              useEffect(() => {
                  if (conn) {
                      // Using the connection created above, grab the document details from the host tunnel.
                      conn?.host?.document?.getDocumentDetails().then(setDocDetails);
                      // Pull the auth tokens from the sharedContext (see host app for details)
                      setAuth(conn?.sharedContext?.get("auth"));
                      setHostname(conn?.sharedContext?.get("hostname"));
                      setProtocol(conn?.sharedContext?.get("protocol"));
                  }
              }, [conn]);
      
          return (<>Text</>);
          }
      
          export default Review;
      ```

## 既存の AIO プロジェクトの設定

1. 設定ファイルを更新
   1. 開く `app.config.yaml`.
   1. からの参照を更新して、設定を変更します。 `aem/cf-editor/1` 対象： `workfront/doc-details/1`. この調整により、ファイル パスが現在のプロジェクト構造に位置合わせされます。

1. 拡張機能登録コンポーネントの変更
   1. という名前のファイルを探して開きます。 `ExtensionRegistration.js`.
   1. 「メソッド」セクションで、関数を追加します `secondaryNav` 非同期関数を含む `getButtons`.
   1. `getButtons` は、次の構造を持つオブジェクトを受け取る必要があります。

      ```
          {
          docId: "String",  // Document ID
          docvId: "String", // Document version ID
          sharedContext: {
              hostname: "String",
              protocol: "String",
              auth: {
              imsOrgID: "String",    // Customer's IMS Org ID
              imsToken: "String",    // User's IMS token
              imsClientId: "String"
              }
          }
          }
      ```

1. この関数は、ナビゲーションに表示されるボタンオブジェクトの配列を返します。

   ```
       methods: {
       secondaryNav: {
           async getButtons({docId, docvId, sharedContext}) {
           return [
               { label: 'Registration', url: '/index.html' },
               { label: 'Review', url: '/index.html#review' }
           ];
           }
       }
       }
   ```

1. アプリケーションルーティングの設定
   1. を開きます `App.js`新しく開発された機能が含まれるようにルートをファイル化し、設定します。 デフォルトビューおよびレビューページなどの追加ビューのルートを設定する必要があります。 これらのルートを定義する方法を次に示します。

      ```
          <Route index element={<ExtensionRegistration />} />
          <Route exact path="index.html" element={<ExtensionRegistration />} />
          <Route exact path="review" element={<Review />} />
      ```

1. ドキュメントの詳細へのアクセス
   1. 提供された関数の実装 `document.getDocumentDetails` アプリケーション内で重要なドキュメント詳細を取得します。 この関数は、を含むオブジェクトを取得します。 `docId` および `docvId`、と `sharedContext` を含むオブジェクト `hostname`, `protocol`、および認証の詳細です。 アプリケーションがこのデータを適切に処理していることを確認します。

1. データ取得をコンポーネントに統合する
   1. 新しいコンポーネントをアプリケーションの components フォルダーに追加します。 このコンポーネント内で、Workfrontへの接続を確立し、ホストアプリケーションと確立された接続を使用してドキュメント情報と認証データを取得します。 これを処理するためにコンポーネントを構築する方法の例を次に示します。

      ```
          import { useEffect, useState } from 'react';
          import { attach } from "@adobe/uix-guest";
          import { extensionId } from "./Constants";
      
          function Review() {
              const [conn, setConn] = useState();
      
              useEffect(() => {
              const iife = async () => {
                  // "attach" the guest application to the host. This creates a "tunnel" from the host app that allows data to be passed to the iframe running this app.
                  const connection = await attach({
                  id: extensionId,
                  });
                  setConn(connection);
              };
      
              iife();
              }, []);
      
              useEffect(() => {
                  if (conn) {
                      // Using the connection created above, grab the document details from the host tunnel.
                      conn?.host?.document?.getDocumentDetails().then(setDocDetails);
                      // Pull the auth tokens from the sharedContext (see host app for details)
                      setAuth(conn?.sharedContext?.get("auth"));
                      setHostname(conn?.sharedContext?.get("hostname"));
                      setProtocol(conn?.sharedContext?.get("protocol"));
                  }
              }, [conn]);
      
          return (<>Text</>);
          }
      
          export default Review;
      ```

## アプリの公開

>[!IMPORTANT]
>
>次の手順ごとに適切な IMS 組織が選択されていることを確認します。

Workfrontにゲストアプリケーションを読み込むには、アプリケーションを実稼動ワークスペースにプッシュし、承認を得るために送信する必要があります。

1. アプリケーションを実稼動ワークスペースにデプロイします
   1. `aio app use -w Production `
   1. `aio app deploy `

1. に移動します。 [https://developer-stage.adobe.com/](https://developer-stage.adobe.com/) または [https://developer.adobe.com/](https://developer.adobe.com/).
   1. クリック **コンソール** 右上隅

1. AppBuilder アプリケーションの作成に使用したプロジェクトを見つけます。

1. 実稼動ワークスペースを選択します。
   ![](assets/find-application.png)

1. 非公開レビュー用にアプリを送信します（アプリ交換マーケットプレイスに公開していないという警告が表示されます。問題ありません）。

1. フォーム（タイトル、説明、アイコン、レビュー担当者へのメモ）に入力します。
   ![](assets/submission-details.png)

>[!IMPORTANT]
>
>送信が完了すると、組織のシステム管理者が送信を承認する必要があります。

## 送信を承認

1. システム管理者として、に移動します。 [https://stage.exchange.adobe.com/](https://stage.exchange.adobe.com/) または [https://exchange.adobe.com/](https://exchange.adobe.com/).

1. クリック **管理** > **Experience Cloudアプリケーション**. 送信されたアプリと、承認/拒否するオプションが表示されます。
承認されると、公開済みのアプリケーション拡張機能がWorkfront環境に自動的に読み込まれます。

   ![](assets/approve-submission.png)

## その他のヘルプ

Adobeには、AppBuilder 用のアプリの構築を開始し、デプロイする方法に関する優れたドキュメントがあります。

次に、役立つリンクを示します。

* [https://developer.adobe.com/app-builder/docs/getting_started/first_app/#4-bootstrapping-new-app-using-the-cli](https://developer.adobe.com/app-builder/docs/getting_started/first_app/#4-bootstrapping-new-app-using-the-cli)

* [https://developer.adobe.com/uix/docs/guides/publication/](https://developer.adobe.com/uix/docs/guides/publication/)

* [https://developer.adobe.com/uix/docs/services/aem-cf-console-admin/extension-development/](https://developer.adobe.com/uix/docs/services/aem-cf-console-admin/extension-development/)

## ローカル開発

Workfront用の App Builder アプリケーションを開発する際に、アプリを公開せずにWorkfront内でテストする必要が生じる場合があります。 幸いなことに、私たちにはこれに対する解決策があります。

App Builder アプリ内で、次を開始できます `aio app run` （ローカル開発）。 これにより、URL （通常は次のもの）が提供されます `https://localhost:9080`. または、以下を実行できます。 `aio app deploy` 静的Adobeドメインを取得する。 今後の使用のために、これらの URL をメモしておいてください。

次に、ブラウザーで、開発する特定のドキュメントの詳細ページに移動します。 開発者ツールを開き、workfront.comまたはworkfront.adobe.comのローカルストレージにアクセスします。 ここでは、エントリを追加する必要があります。 使用方法 `appBuilderDocDetailsOverride` をキー、を値として前述の App Builder URL。

ページを再読み込みすると、App Builder アプリケーションのボタンが表示されます。 これらのボタンをクリックすると、アプリの動作を表示できます。