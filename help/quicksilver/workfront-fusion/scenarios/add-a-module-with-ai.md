---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: AI を使用したモジュールの生成
description: テキストプロンプトを入力して、プロンプトに設定する HTTP モジュールを作成できます。
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
source-git-commit: cb2dba1c74f1d33be0bb21a7e1cdd176a3577bb2
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 2%

---

# AI を使用したモジュールの生成

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>この機能はまだ開発の初期段階なので、Workfrontの内部ユーザーのみが利用できます。

AI を使用して、モジュールが必要なことを説明するテキストプロンプトを入力できます。 次に、目的の API の正しいエンドポイントに接続する HTTP モジュールが生成されます。

AI から生成されたものと同様に、生成されたモジュールを再度確認し、テストして、意図したとおりに実行されていることを確認することをお勧めします。

## 現在サポートされている AI モジュールアプリケーション

現在、Fusion AI は、次のアプリケーションに接続するモジュールを生成できます。

* Adobe Firefly
* Azure OpenAI
* Microsoft Graph
* Adobeマエストロ
* Adobe Analytics
* Adobe PDF サービス
* AdobeMarketo
* AdobeFrame.io
* Dropbox
* NetSuite
* Google カレンダー
* アトラシアジラ
* GitLab
* Spotify
* Bitbucket
* OpenAI
* Slack

## モジュールの生成

1. モジュールを追加し、「 」を選択します。 **AI で生成** を選択します。

   または

   シナリオエディターの空白の領域を右クリックし、「 」を選択します。 **AI で生成**.
1. ボックスにテキストプロンプトを入力します。

   プロンプトのヒントについては、を参照してください。 [テキストプロンプトの作成に関するヒント](#tips-for-creating-text-prompts) 」を参照してください。
1. アプリケーションの API トークンをモジュールに追加します。
1. モジュールをチェックして、適切なアプリケーションおよびアクションに対して設定されているように見えるかを確認します。
1. （条件付き）モジュールがシナリオに付属していない場合は、そのモジュールを適切な位置にドラッグします。

モジュールをテストして、生成されたモジュールが意図したとおりに実行されていることを確認することをお勧めします。

## テキストプロンプトの作成に関するヒント

少なくとも次の情報を入力する必要があります。

* 接続先のアプリケーション
* 実行するアクション

>[!INFO]
>
>**例**:
>
>* `Retrieve a list of my calendars from Google Calendar`
>
>   これにはアプリケーションが含まれます `Google Calendar` とアクション `Retrieve a list of my calendars`.
>
>* `Retrieve popular songs from Spotify`
>
>   これにはアプリケーションが含まれます `Spotify` とアクション `Retrieve popular songs`.

テキストプロンプトを作成する際は、次の点に注意してください。

* 各 Fusion モジュールは 1 つのアクションを実行するので、テキストプロンプトには 1 つのアクションを示す必要があります。
* 直接的でシンプルな言語を使用します。
* モジュールを確認し、テストします。 期待どおりに動作しない場合は、プロンプトを調整して、もう一度試してください。



