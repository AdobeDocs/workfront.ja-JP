---
content-type: tips-tricks-troubleshooting
product-previous: workfront-proof
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-workfront-proof-tech-corner
title: トラブルシューティング — [!DNL Workfront Proof] 校閲者
description: 配達確認のコンテンツが読み込まれず、空の校正ビューアのみが表示される場合は、何かがこのアクションをローカルでブロックしている可能性が高くなります。 以下の考えられる解決策を試してみてください。
author: Courtney
feature: Workfront Proof, Digital Content and Documents
exl-id: ce463565-d21e-4dbc-8de8-78bcbf16fb2c
source-git-commit: 20fcf4dd07c1058559533501f7e297d78c43a70b
workflow-type: tm+mt
source-wordcount: '1075'
ht-degree: 0%

---

# トラブルシューティング — [!DNL Workfront Proof] 校閲者

>[!IMPORTANT]
>
>この記事では、スタンドアロン製品の機能について説明します [!DNL Workfront Proof]. 内部での検証に関する情報 [!DNL Adobe Workfront]を参照してください。 [校正](../../../review-and-approve-work/proofing/proofing.md).

配達確認のコンテンツが読み込まれず、空の校正ビューアのみが表示される場合は、何かがこのアクションをローカルでブロックしている可能性が高くなります。 以下の考えられる解決策を試してみてください。

## ブラウザーと [!DNL Flash Player] バージョンは最新です

すべての開発者は、常にアプリケーションに取り組み、製品の新機能や修正を定期的にリリースしています。 これは、ユーザーエクスペリエンスを向上させ、セキュリティレベルを維持するために、最新バージョンのみを使用することをお勧めします。 これは、アプリケーション間の競合を回避するのにも役立ちます。

<!--
### [!DNL Flash Player] Plugin Version

To check your current [!DNL Flash Player] version visit the [[!DNL Adobe] website](http://www.adobe.com/software/flash/about/).

![ProofView_2.png](assets/proofview-2-350x199.png)

If your version number differs from the one listed for your platform go to the [[!DNL Flash Player] download page](http://get.adobe.com/flashplayer/otherversions/) and get the latest version.

Please note: we do recommend using the original [!DNL Adobe] plugin, so if your browser uses a built-in solution deactivate it and install the [!DNL Adobe] solution.
-->

### ブラウザーのバージョン

最近では、ほとんどのブラウザは自動的に更新されますが、問題が発生した場合は、必要に応じて、どのバージョンを使用し、更新を実行するかを確認する価値があります。

ブラウザーで、に移動します。 [!UICONTROL メニュー] をクリックし、 [!UICONTROL について] オプション ( 場合によっては、 [!UICONTROL ヘルプ] メニュー ) を参照してください。 Adobe Analytics の [!UICONTROL について] ポップアップには、現在のブラウザのバージョンに関する情報と、更新を更新/確認するオプションが表示されます。

Chrome のを参照してください。

![ProofView_3.png](assets/proofview-3-350x206.png)

最新の [!DNL Flash Player] プラグインとブラウザーのバージョンがインストールされている場合は、配達確認を再度開いて問題が解決したかどうかを確認します。

## ローカル環境を確保 [!DNL Flash] ストレージを利用可能

アドビの [!DNL Workfront Proof] 閲覧者はFlashに基づいており、配達確認に関するデータ（コメント、配達確認タイルなど）が格納されます。 [!DNL Workfront Proof] ビューアの設定 ) を使用して、コンピューター上で [!DNL Flash Player]. 次の場合、 [!DNL Workfront Proof] ビューアが開きますが、内部にコンテンツがありません。Flashストレージがコンピューター上で使用可能であり、 [!DNL Workfront Proof] を使用することが許可されています。

ストレージが割り当てられているが、複数のページとコメントでより大きな配達確認を使用している場合は、 [!DNL Flash] 配達確認を保存して再読み込みします。

以下をご覧ください。 [配達確認の表示に関する問題 — [!DNL Flash] 共有オブジェクトの説明](../../../workfront-proof/wp-tech-corner/troubleshooting/view-proof-flash-shared-object.md) 」を参照してください。

## 問題の発生場所の特定

* 配達確認を別のブラウザーで開くか。
* 1 台のブラウザーを毎日使用していて、配達確認の表示に問題がある場合は、コンピューター上の別のブラウザーで同じ配達確認を開こうとします。 これをおこなうには、メインブラウザーの URL バーから配達確認リンクをコピーし、別のブラウザーに貼り付けます。 配達確認が正常に開いた場合は、メインのブラウザー設定、プラグインおよび拡張機能を確認します。これらは干渉している可能性があります。
* 適切なブラウザーはありませんが、現在のブラウザーでパフォーマンスの問題が発生している場合は、別のブラウザーに切り替えることをお勧めします。
* 配達確認が別のマシンで場所に表示されているか
お使いのコンピューター上のどのブラウザーでも配達確認が開かれない場合は、自分の場所の別のコンピューターや、自分の場所の外部で配達確認を開いてみてください。 これにより、問題が特定のコンピューターに起因しているか、またはローカルネットワーク内に存在するかを判断できます。
セキュリティレベルがより高い場合は、 [!DNL Workfront Proof] 次のユーザーによってブロックされている可能性があります：

   * ローカルの AV ソフトウェア
   * ネットワークセキュリティソリューション
   * DNS、ファイアウォール、またはプロキシの設定
   * これらの設定は制御できません。 様々なセキュリティソリューションを利用できます。どのセキュリティソリューションがネットワークに実装されているのか、どのセキュリティソリューションが接続をブロックしているのかは判別できません。 [!DNL Workfront Proof]. また、次の項目にも依存しません。 [!DNL Workfront Proof] 内部セキュリティ設定を決定する場合。 場所やネットワークの複数のマシンで配達確認を開く際に問題が発生した場合は、IT チームに連絡して、ネットワーク設定を確認し、承認または [!DNL Workfront Proof] 必要に応じ許可リストに加えるて、に追加します。

* 接続先： [!DNL Workfront Proof] ネットワークで許可されているか？
配達確認ビューア内に、ページのタイル（ページのフラグメント）が読み込まれます。 このコンテンツがお客様のエンドで正常に読み込まれない場合は、 [!DNL Workfront Proof] はネットワーク内でブロックされています。 *.proofhq.comのすべての接続とすべてのコンテンツが確実にに追加されるようにする必要があり許可リストに加えるます。 IT チームがこの検証に役立てる必要があります。

## プラグインを確認

ブラウザーが [!DNL Flash Player] プラグインが最新です。ネットワークがへの接続をブロックしていません。 [!DNL Workfront Proof] ブラウザーに、配達確認の表示に影響を与えている可能性があります。 最近では、ブラウザーに複数のプラグインや拡張機能が用意されており、一部のプラグインや拡張機能が他のプラグインに干渉したり、他のプラグインと競合したりしています。

ベストプラクティスは、すべての不明なアドオンを削除し、使用するアドオンと信頼するアドオンのみを保持することです。 各ブラウザーには、プラグインや拡張機能を確認、変更、削除するオプションが用意されています。 アドビの [!DNL Workfront Proof] ビューアのベース [!DNL Flash] ここでは、ビューアを読み込む際に JavaScript を使用します。そのため、これらに影響を与える可能性のあるプラグインを特に確認する必要があります。

配達確認の読み込みに干渉する特定のアドオンがある場合は、ブラウザーのコンソールで詳細を確認してみてください。

![ProofView_4.png](assets/proofview-4-350x57.png)

ほとんどの新しいブラウザーには、追加の開発者ツールがいくつか用意されており、より高度なトラブルシューティングに使用できます。

配達確認の表示で問題が発生した場合：

* ブラウザーのコンソールを開き、配達確認を再度読み込みます。
* コンソールにアラートまたはメッセージがあるかどうかを確認します。 これらの詳細は、問題の根本原因を特定するのに役立ちます。
* IT チームに結果を分析してもらう。 ローカルの問題の解決に関するアドバイスと支援を提供できるはずです。
* 結果をサポートチームに共有します。 喜んでお手伝いします。


## 混在コンテンツ設定の確認

へのすべての接続 [!DNL Workfront Proof] は HTTPS 経由です。 ただし、 [!DNL Workfront Proof] ビューアは HTTP 経由でタイルを読み込み、データはトークンで保護されます。 これにより、一部のブラウザーやセキュリティソリューションが（デフォルトで、または手動設定により）ブロックしている可能性のある混合コンテンツが作成されます。

これが、配達確認がコンピューターで開かれない理由の場合（ブラウザーのコンソールに関連するアラートが表示されます）、 [!DNL Workfront Proof] または設定を変更して、コンピューター上のパッシブ混合コンテンツを許可します。 混合コンテンツは、ブラウザー、AV ソフトウェア、ネットワーク設定などによってブロックされ、正確な原因を特定する場合は、IT チームやネットワーク管理者に問い合わせてください。 また、お使いのコンピューターで混合コンテンツを有効にする際にも役立ちます。


