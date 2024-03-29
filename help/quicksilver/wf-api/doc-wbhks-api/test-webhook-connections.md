---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: Webhook 接続のテスト
description: Webhook 接続のテスト
author: Becky
feature: Workfront API
role: Developer
exl-id: 7452ebfc-7c72-4fea-99ac-7f76b12404b8
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '806'
ht-degree: 100%

---


# Webhook 接続のテスト

ドキュメント webhook 実装が正しく動作することを確認するには、このセクションで手動テストを実行します。これらの手順は、Adobe Workfront web インターフェイスを介して、webhook 実装のエンドポイントを間接的にヒットします。

## 前提条件

テストを実行するには、次の前提条件が必要です。

* 高度文書管理（ADM）が有効になっている Workfront アカウント

* システム管理者権限を持つ、このアカウントの Workfront ユーザー 1 名

* Workfront にアクセス可能な HTTP エンドポイントを備えた Document Webhook インスタンス

またこれらのテストでは、Document Webhook インスタンスが登録されていることも前提としています。（インスタンスは、Workfront のセットアップ／ドキュメント／カスタム統合で登録できます。）

**テスト 1：ユーザー向けの Document Webhook サービスをプロビジョニングする**

OAuth ベースの web フックプロバイダーの認証 URL とトークンエンドポイント URL をテストします。

1. Workfront で、上部のナビゲーションバーにある「ドキュメント」リンクをクリックして、ドキュメントのメインページに移動します。
1. ドキュメントを追加ドロップダウンをクリックし、サービスを追加で Document Webhook サービスを選択します。
1. （OAuth サービスのみ）前のステップを完了すると、サービスの OAuth2 認証ページがポップアップウィンドウに読み込まれます。（メモ：最初にサービスにログインするよう求められる場合があります）。認証ページで、「信頼」ボタンまたは「許可」ボタンをクリックして、ユーザーのアカウントに Workfront へのアクセス権を付与します。
1. サービスがドキュメントの追加ドロップダウンに追加されたことを確認します。初めに表示されない場合は、ブラウザーを更新してみてください。

**テスト 2：ドキュメントを Workfront Tests 次のエンドポイントにリンクする：/files、/metadata**

1. Workfront で、上部のナビゲーションバーにある「ドキュメント」リンクをクリックして、ドキュメントのメインページに移動します。
1. 「ドキュメントを追加」でドキュメント web フックサービスを選択します。
1. モーダルでフォルダー構造内を移動します。
1. フォルダー構造内を移動できることを確認します。
1. ドキュメントを選択して Workfront にリンクします。

**テスト 3：コンテンツ管理システム内のドキュメントに移動**

/metadata エンドポイント（特に viewLink）をテストします。

1. Workfront にドキュメントをリンクします。
1. そのドキュメントを選択し、「開く」リンクをクリックします。
1. ドキュメントが新しいタブで開くことを確認します。

**テスト 4：コンテンツ管理システム内のドキュメントに移動する（ログインを使用）**

/metadata エンドポイント（特に viewLink）をテストします。

1. コンテンツ管理システムからログアウトしていることを確認します。
1. Workfront にドキュメントをリンクします。
1. そのドキュメントを選択し、「開く」リンクをクリックします。
1. コンテンツ管理システムのログイン画面が新しいタブに読み込まれることを確認します。
1. ログインして、ドキュメントに移動したことを確認します。

**テスト 5：コンテンツ管理システムからドキュメントをダウンロードする**

次のエンドポイント（特に downloadLink）をテストします：/metadata

1. Workfront にドキュメントをリンクします。
1. そのドキュメントを選択し、「ダウンロード」リンクをクリックします。
1. ダウンロードが開始されることを確認します。

**テスト 6：コンテンツを検索する**

/search エンドポイントをテストします。

1. Workfront で、上部のナビゲーションバーにある「ドキュメント」リンクをクリックして、ドキュメントのメインページに移動します。
1. 「ドキュメントを追加」でドキュメント web フックサービスを選択します。
1. モーダルで検索を実行します。
1. 検索結果が正しいことを確認します。

**テスト 7：Workfront からコンテンツ管理システムにドキュメントを送信する**

/files、/uploadInit および /upload エンドポイントをテストします。

1. Workfront で、上部のナビゲーションバーにある「ドキュメント」リンクをクリックして、ドキュメントのメインページに移動します。
1. お使いのコンピューターから Workfront にドキュメントをアップロードします。
1. ドキュメントの詳細ページに移動します。
1. ドキュメント アクションドロップダウンから、「送信先」でドキュメント web フックサービスを選択します。
1. 目的の宛先フォルダーに移動し、「保存」ボタンをクリックします。
1. ドキュメントがコンテンツ管理システム内の正しい場所にアップロードされていることを確認します。

**テスト 8：Workfront でサムネールを表示する**

/thumbnail エンドポイントをテストします。

1. Workfront にドキュメントをリンクします。
1. リストでドキュメントを選択します。
1. サムネールが右側のパネルに表示されることを確認します。

**テスト 9：コンテンツのバイト数を取得する**

/download エンドポイントをテストします。

1. Workfront にドキュメントをリンクします。
1. ドキュメントの詳細ページに移動します。
1. ドキュメント アクション／送信先／Workfront を選択して、ドキュメントを Workfront に送信します。この結果、Workfront に新しいドキュメントバージョンが作成されます。
1. 「ダウンロード」リンクをクリックして、このドキュメントを Workfront からダウンロードします。

**テスト 10：アクセストークンを更新する（OAuth2 Webhook プロバイダーのみ）**

トークンエンドポイント URL のエンドポイントをテストします。

1. ドキュメント web フックサービスをユーザーにプロビジョニングします。
1. 次のいずれかの方法で、ユーザーのアクセストークンを無効にします。1）タイムアウトまで待機する、2）外部システムで手動で無効にする。
1. Workfront でアクセストークンを更新します。それには、例えば、Workfront にドキュメントをリンクします。ドキュメントに移動してリンクできれば、アクセストークンが正常に更新されたことがわかります。

>[!NOTE]
>
>現在、リンクされたドキュメントには送信先を使用できません。この機能は Workfront に追加される予定です。/download エンドポイントをテストするには、Postman などの REST クライアントを使用して、手動でエンドポイントにヒットさせます。または、デジタルプルーフを生成して、/download エンドポイントをテストすることもできます。デジタルプルーフを有効にするには、Workfront 管理者にお問い合わせください。
