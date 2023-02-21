---
content-type: reference
product-area: workfront-integrations
keywords: ネイティブ、標準
navigation-topic: workfront-integrations-navigation-topic
title: Adobe Workfront統合方法
description: 統合可能な [!DNL Adobe Workfront] サードパーティのアプリケーションを使用する場合。 これらの統合は、のユーティリティを拡張できます [!DNL Workfront] 組織のニーズに合わせて調整します。 特定のタスクで最も役立つ統合に応じて、これらの統合のいずれかまたはすべてを使用できます。
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: bf13a7c9-eab3-4ae3-a060-8a422236122d
source-git-commit: 925e8f9d57d65fcb44068274800450d9db5c9d34
workflow-type: tm+mt
source-wordcount: '941'
ht-degree: 0%

---

# Adobe Workfront統合方法

統合可能な [!DNL Adobe Workfront] サードパーティのアプリケーションを使用する場合。 これらの統合は、のユーティリティを拡張できます [!DNL Workfront] 組織のニーズに合わせて調整します。 特定のタスクで最も役立つ統合に応じて、これらの統合のいずれかまたはすべてを使用できます。

## 組み込み統合

Workfrontは、Workfrontから直接、またはそのアプリケーション用のWorkfrontアドインをインストールして別のアプリケーションから設定できる様々な統合を提供します。 これらの組み込み統合では、多くの一般的な使用例のシナリオをカバーし、エンドユーザー向けのユーザーエクスペリエンスの拡張と接続に焦点を当てています。

Workfrontの組み込み統合は、主に個人の生産性とコラボレーションに焦点を当てています。 これらの統合により、個々のユーザーのワークフローでの中断が減り、統合アプリケーションを離れることなく、Workfront通知を受け取り、情報にアクセスし、Workfrontの作業項目に基づいて作業をおこなうことができます。

組み込み統合のメリットには、次のものがあります。

* これらの組み込み統合の多くは、追加費用なしで利用できます。 （追加購入が必要な場合もあります）。
* 組み込み統合は、例えば [!DNL Slack], [!DNL Google Drive]または [!DNL Adobe] 製品 ( [!DNL Adobe Creative Cloud] または [!DNL Adobe Experience Manager] アセット。 これらのアプリを既に使用している場合、統合はユーザーの既存のワークフローにスムーズに進みます。
* 統合 [!DNL Workfront] 頻繁に使用するアプリケーションを使用すると、ユーザー間での採用が増加する可能性があります。

>[!INFO]
>
>**例:**
>
>を使用 [!DNL Workfront for Microsoft Teams integration]、で通知を受け取ることができます。 [!DNL Microsoft Teams] について [!DNL Workfront] 作業項目。 離れずに [!DNL Microsoft Teams]を使用すると、作業項目の承認、コメントの追加、ステータスの変更などのアクションを実行できます。 作業項目に加えた変更 [!DNL Microsoft Teams] は、次のように反映されます。 [!DNL Workfront] 同様に。

現在使用可能な組み込み統合のリストなど、組み込み統合について詳しくは、 [[!DNL Adobe Workfront] 組み込み統合の概要](../workfront-integrations-and-apps/built-in-integrations-non-admin.md).

## カスタム OAuth2 アプリケーション

Adobe [!DNL Workfront] 管理者は、のインスタンス用に OAuth2 アプリケーションを作成できます [!DNL Workfront]（他のアプリケーションがにアクセスできるようにする） [!DNL Workfront]. その後、ユーザーは他のアプリケーションに対し、そのアプリケーションへのアクセス権を付与できます [!DNL Workfront] データ。 この方法で、Workfrontを、独自の社内アプリケーションを含む、任意のアプリケーションと統合できます。

>[!NOTE]
>
>OAuth2 のコンテキストでは、「アプリの作成」は、アプリとWorkfrontなどのサーバーとの間に、この種のアクセスリンクを作成するプロセスを指します。

を作成する利点 [!UICONTROL OAuth2] アプリケーションには、次のものが含まれます。

* ユーザーは、これらの統合を [!DNL Workfront]（組み込み統合と似ています）
* の設定または使用 [!UICONTROL OAuth2] アプリケーションは、知識など、追加の技術知識を必要としません。 [!DNL Workfront] API
* お客様の組織では、 [!DNL Workfront] 組み込みアプリケーション。 このソフトウェアは、引き続き [!DNL Workfront] を使用して [!UICONTROL OAuth2] アプリケーション（ソフトウェアが組織独自のものであっても）。

詳しくは、 [Workfront統合用の OAuth2 アプリケーションの作成](../administration-and-setup/configure-integrations/create-oauth-application.md).

## [!DNL Workfront] API

[!DNL Workfront] は、Workfrontのエクスペリエンスを拡張および強化できるパブリック API（アプリケーションプログラミングインターフェイス）を提供します。 の目標 [!DNL Workfront] API は、 [!DNL Workfront] HTTP 経由で動作する REST-ful アーキテクチャを導入することで、 この [!DNL Workfront] API には技術的な知識が必要ですが、データの取得、作成、変更をおこなうための非常に強力なツールです。 API 呼び出しをカスタマイズして、非常に具体的な機能を実行できます。

さらに、 [!DNL Workfront] は、イベント購読 API を提供します。 アクションが [!DNL Workfront] イベントサブスクリプションでサポートされるオブジェクトの場合は、 [!DNL Workfront] をクリックして、目的のエンドポイントに応答を送信します。 つまり、サードパーティアプリケーションは、 [!DNL Workfront] 操作 [!DNL Workfront] API が発生した直後に発生します。

を使用する利点 [!DNL Workfront] API には、次のものが含まれます。

* 以下を使用して、 [!DNL Workfront] 公開 API を提供する他のほとんどの Web サービスまたはアプリに接続するための API。 したがって、 [!DNL Workfront] を、使用するほとんどすべての web サービスまたはアプリと共に使用します。
* この [!DNL Workfront] API の柔軟性は、お客様のビジネス独自のソフトウェアにも及びます。 を使用して、 [!DNL Workfront] 独自のソフトウェア内からのデータ。
* API はソフトウェアにとってよく使用されるので、社内の開発者は API に詳しいと考えられます。 [!DNL Workfront] は、最も一般的なタイプの API である REST-ful API を使用しているので、開発者がすばやく習得しやすくなっています。

>[!INFO]
>
>**例:**
>
>次の API 呼び出しは、指定された ID を持つタスクの更新ストリームにコメントを配置します。
>
>
```
>https://`<your domain>`.workfront.com/attask/api-internal/note?noteText=<text of comment>&noteObjCode=TASK&objID=<task ID>&apiKey=<your API key>
>```

詳しくは、 [!DNL Workfront] API（を参照） [API の基本](../wf-api/general/api-basics.md).

イベントの購読について詳しくは、 [イベント購読 API](../wf-api/general/event-subs-api.md).

## [!DNL Adobe Workfront Fusion]

[!DNL Workfront Fusion] では、ワークフローを自動化できます。 を使用 [!DNL Workfront Fusion for Work Automation and Integration] ライセンスを使用すると、複数のアプリや web サービスにわたってこれらの自動化を作成し、アプリが連携してタスクを実行するシナリオを作成できます。 シナリオとは、モジュールを使用して構築されたタスクまたはワークフローを視覚的に表現したものです。モジュールは、「ドキュメントのダウンロード」や「プロジェクトの作成」など、個別のタスクです。 モジュールを連結してワークフローを定義し、ワークフロー条件が満たされた場合に、トリガーを自動的に実行します。

の利点 [!DNL Workfront Fusion] 次のものが含まれます。

* [!DNL Workfront Fusion] では、API ほど技術的な知識は必要ありません。これは、視覚的なインターフェイスがワークフローの理解と設定に役立つからです。 つまり、開発チーム以外の個人が使用できるので、組織の時間とコストを節約できます。
* 次以降 [!DNL Workfront Fusion] は API を通じて動作し、ほとんどのアプリや Web サービスにアクセスできます。 多くのアプリには API 呼び出しをおこなうモジュールがあります。また、HTTP、SOAP、JSON モジュールを使用して、専用の [!DNL Workfront Fusion] コネクタ。

>[!INFO]
>
>**例:**
>
>以下 [!DNL Workfront] モジュール [!DNL Workfront Fusion] は、選択したプロジェクトにコメントを追加するように設定されています。 モジュールを実行すると、Workfrontのプロジェクトの更新ストリームにコメントが表示されます。
>
>![](assets/fusion-example-comment-350x416.png)

詳しくは、 [!DNL Workfront Fusion]を参照してください。 [[!DNL Adobe Workfront Fusion]](../workfront-fusion/workfront-fusion-2.md).
