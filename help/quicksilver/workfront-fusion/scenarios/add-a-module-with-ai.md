---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: AI を使用したシナリオセグメントの生成
description: Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。 この記事は廃止されましたが、この機能を説明する新しい記事へのリンクが含まれています。
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 899641a0-a104-4be9-b423-34a32e985b53
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 1%

---

# AI を使用したシナリオセグメントの生成

>[!IMPORTANT]
>
>Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。
>
>この記事の情報は、次の記事に記載されています。
>
>* [AI を使用したシナリオセグメントの生成 ](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/add-a-module-with-ai.html)
>
>ブックマークを更新してください。
>
>この記事は現在更新されておらず、近い将来に削除されます。

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

   AI アシスタント パネルが開きます。
1. ボックスにテキストプロンプトを入力します。

   プロンプトのヒントについては、この記事の [ テキストプロンプトの作成のヒント ](#tips-for-creating-text-prompts) を参照してください。

   AI アシスタントは、モジュールまたはモジュールのセットを生成します。
1. （条件付き）必要に応じて、アプリケーションの API トークンをモジュールに追加します。
1. モジュールを調べ、適切なアプリケーションとアクションに設定されていることを確認します。
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
>
>* `Generate an image in Adobe Firefly and upload it to Dropbox`
>
>    この例には複数のアプリケーションが含まれているので、正しくありません

テキストプロンプトを作成する場合は、次の点に注意してください。

* 直接的でシンプルな言語を使用します。
* モジュールを確認およびテストします。 期待どおりに実行されない場合は、プロンプトを調整して再試行してください。
