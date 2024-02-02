---
content-type: reference
product-area: workfront-integrations
keywords: ネイティブ、ootb
navigation-topic: workfront-integrations-navigation-topic
title: Adobe Workfront 統合方法
description: ' [!DNL Adobe Workfront]  をサードパーティのアプリケーションと統合できます。これらの統合により、 [!DNL Workfront]  のユーティリティを拡張し、これを組織のニーズに合わせて調整できます。特定のタスクに最も役立つ統合に応じて、これらの統合のいずれかまたはすべてを使用できます。'
feature: Workfront Integrations and Apps, Workfront Fusion
exl-id: bf13a7c9-eab3-4ae3-a060-8a422236122d
source-git-commit: 328d3a8d16ace22100d86efc127874d7edd6cb6d
workflow-type: ht
source-wordcount: '946'
ht-degree: 100%

---

# Adobe Workfront 統合方法

[!DNL Adobe Workfront] をサードパーティのアプリケーションや他の [!DNL Adobe] 製品と統合できます。これらの統合により、[!DNL Workfront] のユーティリティを拡張し、これを組織のニーズに合わせて調整できます。特定のタスクに最も役立つ統合に応じて、これらの統合のいずれかまたはすべてを使用できます。

## 組み込みの統合

Workfront は、様々な統合を提供します。これは Workfront から直接設定することも、そのアプリケーション用の Workfront アドインをインストールすることで、別のアプリケーションから設定することもできます。これらの組み込み統合では、多くの一般的なユースケースのシナリオを扱い、エンドユーザー向けのユーザーエクスペリエンスの拡張と接続に焦点を当てています。

Workfront の組み込み統合は、主に個人の生産性と共同作業に焦点を当てています。 これらの統合により、個々のユーザーのワークフローでの中断が減り、統合アプリケーションを離れることなく、Workfront 通知の受信や情報へのアクセス、Workfront の作業項目に従って対処できます。

組み込み統合には次のような利点があります。

* これらの組み込み統合の多くは、追加費用なしで利用できます。 （追加購入が必要な場合もあります。）
* 組み込み統合では、[!DNL Adobe Creative Cloud] Assets や [!DNL Adobe Experience Manager] Assets などの [!DNL Slack]、[!DNL Google Drive]、[!DNL Adobe] 製品など、企業で使用される最も一般的なアプリの多くを扱っています。企業でこれらのアプリを既に使用している場合、統合はユーザーの既存のワークフローにスムーズに組み込まれます。
* [!DNL Workfront] を頻繁に使用するアプリケーションと統合すると、ユーザーの間での採用件数が増加します。

>[!INFO]
>
>**例：**
>
>[!DNL Workfront for Microsoft Teams integration] を使用すると、[!DNL Workfront] の作業項目に関する通知を [!DNL Microsoft Teams] で受け取ることができます。[!DNL Microsoft Teams] を離れずに、作業項目の承認、コメントの追加、ステータスの変更などのアクションを実行できます。 [!DNL Microsoft Teams] から作業項目に加えた変更は、[!DNL Workfront] にも反映されます。

現在使用可能な組み込み統合のリストなど、組み込み統合について詳しくは、[[!DNL Adobe Workfront] 組み込み統合の概要](../workfront-integrations-and-apps/built-in-integrations-non-admin.md)を参照してください。

## カスタム OAuth2 アプリケーション

Adobe [!DNL Workfront] 管理者は、[!DNL Workfront] のインスタンス用の OAuth2 アプリケーションを作成して、他のアプリケーションが [!DNL Workfront] にアクセスできるようします。その後、ユーザーは他のアプリケーションに [!DNL Workfront]データへのアクセス権を付与できます。 このようにして、Workfront を、独自の社内アプリケーションなど、選択したアプリケーションと統合できます。

>[!NOTE]
>
>OAuth2 のコンテキストでは、「アプリの作成」とは、アプリと Workfront などのサーバーとの間にこの種のアクセスリンクを作成するプロセスを指します。

[!UICONTROL OAuth2] アプリケーションを作成することには、次のような利点があります。

* ユーザーは、組み込みの統合と同様に、これらの統合を [!DNL Workfront] で直接使用できます。
* [!UICONTROL OAuth2] アプリケーションの設定または使用には、[!DNL Workfront] API の知識などの追加の技術知識を必要としません。
* お客様の組織では、[!DNL Workfront] 組み込みアプリケーションとして提供されていないソフトウェアを使用している場合があります。ソフトウェアが組織独自のものであっても、[!UICONTROL OAuth2] アプリケーションを使用すると、このソフトウェアを [!DNL Workfront] と統合できます。

詳しくは、[Workfront 統合用の OAuth2 アプリケーションを作成](../administration-and-setup/configure-integrations/create-oauth-application.md)を参照してください。

## [!DNL Workfront] API

[!DNL Workfront] は、Workfront エクスペリエンスを拡張および強化できるパブリック API（アプリケーションプログラミングインターフェイス）を提供します。[!DNL Workfront] API の目的は、HTTP 経由で動作する REST-ful アーキテクチャを導入することで、[!DNL Workfront] との統合の構築を簡略化することです。[!DNL Workfront] API には技術的な知識が必要ですが、データの取得、作成、変更を行う上で非常に強力なツールです。 API 呼び出しをカスタマイズすると、非常に特殊な機能を実行できます。

さらに、[!DNL Workfront] は、イベント登録 API を提供します。 イベント登録でサポートされている [!DNL Workfront] オブジェクトでアクションが発生した場合、目的のエンドポイントに応答を送信するように [!DNL Workfront] を設定できます。つまり、サードパーティアプリケーションは、発生後すぐに、[!DNL Workfront] API を介して [!DNL Workfront] とのやり取りから更新を受け取ることができます。

[!DNL Workfront] API を使用する利点には、次のものが含まれます。

* [!DNL Workfront] API を使用すると、パブリック API を提供する他のほとんどの web サービスやアプリに接続できます。したがって、[!DNL Workfront] を使用するほとんどすべての web サービスやアプリと統合することが可能です。
* [!DNL Workfront] API の柔軟性は、お客様のビジネス独自のソフトウェアにも拡張されます。 独自のソフトウェア内から [!DNL Workfront] データを使用したり、変更したりできます。
* API はソフトウェアによく使用されるので、社内の開発者は API に精通していると考えられます。 [!DNL Workfront] は、最も一般的なタイプの API である REST-ful API を使用しているので、開発者にとって短期間で習得しやすくなっています。

>[!INFO]
>
>**例：**
>
>次の API 呼び出しは、指定された ID を持つタスクの更新ストリームにコメントを入れます。
>
>```
>https://`<your domain>`.workfront.com/attask/api-internal/note?noteText=<text of comment>&noteObjCode=TASK&objID=<task ID>&apiKey=<your API key>
>```

詳しくは、[!DNL Workfront] API について詳しくは、[API の基本](../wf-api/general/api-basics.md)を参照してください。

イベント登録について詳しくは、[Event Subscription API](../wf-api/general/event-subs-api.md) を参照してください。

## [!DNL Adobe Workfront Fusion]

[!DNL Workfront Fusion] では、ワークフローを自動化できます。[!DNL Workfront Fusion for Work Automation and Integration] ライセンスを使用すると、複数のアプリや web サービスにわたってこれらの自動化を作成し、アプリが連携してタスクを実行するシナリオを作成できます。シナリオとは、モジュールを使用して構築されたタスクまたはワークフローを視覚的に表現したものです。モジュールは、「ドキュメントのダウンロード」や「プロジェクトの作成」など、個別のタスクです。モジュールを連結してワークフローを定義し、トリガーの条件が満たされた場合に、トリガーを自動的に実行します。

[!DNL Workfront Fusion] のメリットには次のものが含まれます。

* [!DNL Workfront Fusion] では、API ほど技術的な知識は必要ありません。これは、視覚的なインターフェイスがワークフローの理解と設定に役立つからです。つまり、開発チーム以外の個人が使用できるので、組織の時間とコストを節約できます。
* [!DNL Workfront Fusion] は API を通じて動作するため、ほとんどのアプリや web サービスにアクセスできます。多くのアプリには API 呼び出しを行うモジュールがあります。または、HTTP、SOAP、または JSON モジュールを使用して、専用の [!DNL Workfront Fusion] コネクタを持たない web サービスの操作を行うことができます。

>[!INFO]
>
>**例：**
>
>[!DNL Workfront Fusion] 内の次の [!DNL Workfront] モジュールは、選択したプロジェクトにコメントを追加するように設定されています。モジュールを実行すると、Workfront のプロジェクトの更新ストリームにコメントが表示されます。
>
>![](assets/fusion-example-comment-350x416.png)

[!DNL Workfront Fusion] について詳しくは、[[!DNL Adobe Workfront Fusion]](../workfront-fusion/workfront-fusion-2.md) を参照してください。
