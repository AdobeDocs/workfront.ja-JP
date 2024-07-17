---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: AI を使用したモジュールの生成
description: テキストプロンプトを入力して、プロンプトに設定された HTTP モジュールを作成できます。
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 899641a0-a104-4be9-b423-34a32e985b53
source-git-commit: 0a01acd56b3ea10d1cccc31a21e434da55b1ec13
workflow-type: tm+mt
source-wordcount: '347'
ht-degree: 5%

---

# AI を使用したモジュールの生成

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>この機能は開発の初期段階にあるので、Workfrontの内部ユーザーのみが使用できます。

AI を使用すると、モジュールで必要な作業を説明するテキストプロンプトを入力できます。 次に、Fusion は、目的の API の正しいエンドポイントに接続する HTTP モジュールを生成します。

AI から生成されるものと同様に、生成されたモジュールを再確認およびテストして、意図したとおりに実行されていることを確認することをお勧めします。

## 現在サポートされている AI モジュールアプリケーション

Fusion AI は、現在、次のアプリケーションに接続するモジュールを生成できます。

* Adobe Firefly
* Azure OpenAI
* Microsoft グラフ
* Adobe マエストロ
* Adobe Analytics
* Adobe PDF サービス
* Adobe Marketo
* Adobe フレーム.io
* Dropbox
* NetSuite
* Google カレンダー
* Atlassian Jira
* GitLab
* Spotify
* Bitbucket
* OpenAI
* Slack

## モジュールを生成

1. モジュールを追加し、アプリケーションのリストから **AI を使用して生成** を選択します。

   または

   シナリオエディターの空白領域を右クリックし、「**AI を使用して生成**」を選択します。
1. ボックスにテキストプロンプトを入力します。

   プロンプトのヒントについては、この記事の [ テキストプロンプトの作成のヒント ](#tips-for-creating-text-prompts) を参照してください。
1. アプリケーションの API トークンをモジュールに追加します。
1. モジュールを調べ、適切なアプリケーションとアクションに合わせて設定されているように表示されることを確認します。
1. （条件付き）モジュールがシナリオに添付されていない場合は、適切な場所にドラッグします。

モジュールをテストし、生成されたモジュールが意図したとおりに実行されていることを確認することをお勧めします。

## テキストプロンプトの作成に関するヒント

テキストプロンプトには、少なくとも次の情報を含める必要があります。

* 接続先のアプリケーション
* 実行するアクション

>[!INFO]
>
>**例**:
>
>* `Retrieve a list of my calendars from Google Calendar`
>
>   これには、アプリケーション `Google Calendar` とアクション `Retrieve a list of my calendars` が含まれます。
>
>* `Retrieve popular songs from Spotify`
>
>   これには、アプリケーション `Spotify` とアクション `Retrieve popular songs` が含まれます。

テキストプロンプトを作成する場合は、次の点に注意してください。

* Fusion モジュールごとに 1 つのアクションが実行されるので、テキストプロンプトでは、1 つの特定のアクションを記述する必要があります。
* 直接的でシンプルな言語を使用します。
* モジュールを確認およびテストします。 期待どおりに実行されない場合は、プロンプトを調整して再試行してください。
