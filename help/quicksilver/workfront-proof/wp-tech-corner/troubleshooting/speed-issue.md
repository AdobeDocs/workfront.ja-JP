---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: での問題を迅速に解決 [!DNL Workfront Proof]
description: このヘルプページは、を使用する際に発生する可能性のある速度の問題を判断するのに役立ちます。 [!DNL Workfront Proof] は、ISP または [!DNL Workfront Proof]のコンテンツ配信ネットワーク。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: 42e999a6-5b27-482d-a7cf-b8030272da32
source-git-commit: 41ab1312d2ccb8b8271bc851a35e31e9ff18c16b
workflow-type: tm+mt
source-wordcount: '723'
ht-degree: 0%

---

# での問題を迅速に解決 [!DNL Workfront Proof]

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

このヘルプページは、を使用する際に発生する可能性のある速度の問題を判断するのに役立ちます。 [!DNL Workfront Proof] は、ISP または [!DNL Workfront Proof]のコンテンツ配信ネットワーク。

速度の問題は、通常、ローカル ISP 接続またはローカルインターネットアクセスの設定（例えば、プロキシサーバーが使用されている場合）に起因します。 [!DNL Workfront Proof].

ただし、接続速度を確認するためにいくつかの手順を実行します。これにより、発生している問題の根本原因を特定できます。 これらの手順はすべてトラブルシューティングプロセスでも同様に重要です。問題の最も正確な診断を行うために、リストに表示されているすべての手順に関する情報を収集するように時間をかけておくことをお勧めします。

すべての詳細を収集したら、担当の IT 部門に相談して、現地の問題を特定することをお勧めします。 この件に関してさらにサポートが必要な場合は、 [サポートチーム](https://support.workfront.com/hc/en-us/requests/new).

## システムのどの部分が低速かを確認します。

を使用する場合、 [!DNL Workfront Proof]の場合は、ダッシュボードを使用して、例えば、フォルダーのコンテンツやユーザーの管理や [!DNL Workfront Proof] ビューア：配達確認のレビューの実行、コメントの確認など。

速度の問題をトラブルシューティングする最初の手順は、システムの正確な部分を特定することです。 レポートの作成時 [!DNL Workfront Proof] 遅い場合は、必ず次の内容を記述してください。

* 他の Web ページで速度が低下していますか。
* 問題がダッシュボードで発生しているか、または [!DNL Workfront Proof] 閲覧者？
* システムのどの部分が遅いか。 ( 例：新しい配達確認の処理、 [!DNL Workfront Proof] 閲覧者 )

## traceroute テストと ping テストの実行

パフォーマンスの問題が発生した場合は、 traceroute コマンドを実行して接続を検証することが重要です。 これをおこなうには、システム (Mac/Linux のターミナル ) でコマンドプロンプトを開き、次の手順を実行します。

1. 次のいずれかを入力し、トレーサーアウトが完了するのを待ちます。

   * Windows の場合： **tracert app.proofhq.com**
   * Mac/Linux: **traceroute app.proofhq.com**

1. （Windows のみ）種類 **ping app.proofhq.com**.
1. ping が完了したら、コマンドプロンプトで右クリックし、[ すべて ] を選択します。
1. 結果をコピーして、E メールの返信に貼り付けます。
結果をサポートチームに送信する前に、traceroute と ping を必ず完了させてください。

## Speedtest.net を使用した接続速度のテスト

1. クリック [ここ](http://www.speedtest.net/) をクリックして、Speedtest.net にアクセスします。
1. Speedtest ナレッジベースの手順に従って、インターネット接続の速度をテストします。
1. 結果をコピーして、サポートチームのメールに貼り付けます。

## ブラウザーコンソールで「ネットワーク」タブを確認する

最新のブラウザーで利用可能な Web コンソールは、ネットワークの待ち時間に関する有用な情報を収集します。これは、発生している速度の問題の根本原因を特定するのに役立ちます。

Web ページの読み込み時間を確認するには：

1. ブラウザーのコンソールと「ネットワーク」タブを開きます。
1. ページを再度読み込みます。
1. スクリーンショットを撮るか、結果のスクリーンキャストを記録します。
1. 結果をサポートチームと共有します。

スクリーンショットにすべてのデータが表示されていることを確認してください。スクリーンショットを取る場合はコンソールウィンドウを展開し、スクリーンキャスト内で下にスクロールします。

ブラウザーでコンソールを開く方法がわからない場合は、次の記録済みの手順を参照してください。

* [クロム](http://screencast.com/t/AgQU6JQQ)
* [Safari](http://screencast.com/t/f31GqQYm0w)
* [Firefox](http://screencast.com/t/Xg7SscmAi)
* [Edge](http://www.screencast.com/t/epSwBiaD)
* [Internet Explorer 以降](http://screencast.com/t/x5Q3eHczbc)

詳しい手順については、ブラウザーのドキュメントを参照してください。

## 別のネットワークとコンピューターで接続を確認してください

別のデバイスやネットワークを使用して、接続速度に同じ問題が発生したかどうかを確認することは、トラブルシューティングプロセスの重要な手順です。 別のマシンやモバイルデバイスに切り替えて、別のネットワーク（モバイルデータなど）を使用してみてください。

様々な組み合わせでの接続の比較：同じネットワーク上の別のマシンを使用し、別のネットワーク上の同じマシンを使用し、別のマシンとネットワークの両方を使用して、結果をサポートチームと共有します。
