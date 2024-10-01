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
source-git-commit: 67e1d158b09ca339d25473ebedf8851155b2c1c0
workflow-type: tm+mt
source-wordcount: '408'
ht-degree: 3%

---

# AI を使用したシナリオセグメントの生成

<!--DO NOT DELETE - linked through CSH-->

>[!IMPORTANT]
>
>この機能はBetaで使用できるので、一部のWorkfront ユーザーのみが使用できます。

AI を使用すると、シナリオの一部で必要な作業を説明するテキストプロンプトを入力できます。 Fusion は、シナリオで使用できるこれらのアクションを実行するモジュールを生成します。

AI から生成されるものと同様に、生成されたモジュールを再確認およびテストして、意図したとおりに実行されていることを確認することをお勧めします。

## 現在サポートされている AI モジュールアプリケーション

Fusion AI は、現在、次のアプリケーションに接続するモジュールを生成できます。

* Adobe Firefly
* Azure OpenAI
* Microsoft グラフ
* Adobe Workfrontの計画
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

## モジュールの生成

1. モジュールの追加を開始し、アプリケーションのリストから **AI を使用して生成** を選択します。

   または

   シナリオエディターページの下部付近にある「AI で生成 ![ アイコン ](assets/generate-with-ai-icon-beta.png)AI で生成）をクリックします。

   その AI アシスタント パネルが開きます。
1. ボックスにテキストプロンプトを入力します。

   プロンプトのヒントについては、この記事の [ テキストプロンプトの作成のヒント ](#tips-for-creating-text-prompts) を参照してください。

   モジュールまたはモジュールのセットが生成されます。
1. （条件付き）必要に応じて、アプリケーションの API トークンをモジュールに追加します。
1. モジュールを調べ、適切なアプリケーションとアクションに合わせて設定されていることを確認します。
1. （条件付き）生成されたシナリオセクションがシナリオに添付されていない場合は、適切な場所にドラッグします。

モジュールのテストを実施し、モジュールが意図したとおりに動作していることを確認することをお勧めします。

## テキストプロンプトの作成に関するヒント

テキストプロンプトには、少なくとも次の情報を含める必要があります。

* 接続先のアプリケーション
* 実行する 1 つ以上のアクション

>[!IMPORTANT]
>
>一度に複数のモジュールを生成できますが、一度に生成できるモジュールは 1 つのアプリケーションのみです。

>[!INFO]
>
>**例**:
>
>* `Delete the records 'xyz-123', 'xyz-456', 'xyz-789' from Adobe Workfront Planning`
>これには、アプリケーション `Workfront Planning` とアクション `delete records` が含まれます。 このプロンプトは、削除されるレコードごとに 1 つずつ、3 つのモジュールを作成します。
>* `Change campaign summary of the record 'xyz-123' from Adobe Workfront Planning`
>これには、アプリケーション `Workfront Planning` とアクション `change campaign summary` が含まれます。
>* `Get all field details in the record type with ID 'test-record' from Adobe Workfront Planning`
>これには、アプリケーション `Workfront Planning` とアクション `get field details` が含まれます。
>
>次の例は正しくありません。
>* `Generate an image in Adobe Firefly and upload it to Dropbox`
>
>    この例には複数のアプリケーションが含まれているので、正しくありません

テキストプロンプトを作成する場合は、次の点に注意してください。

* 直接的でシンプルな言語を使用します。
* モジュールを確認およびテストします。 期待どおりに実行されない場合は、プロンプトを調整して再試行してください。
