---
content-type: api
navigation-topic: api-navigation-topic
title: デフォルトの API バージョン管理を使用する統合を更新
description: デフォルトの API バージョン管理を使用する統合を更新
author: Becky
feature: Workfront API
exl-id: ac394b41-63cb-481a-a858-30d8d7f840bb
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '693'
ht-degree: 0%

---

# デフォルトの API バージョン管理を使用する統合を更新

<!-- This article is going to need a complete revamp or to be removed-->

<span class="preview">このページで強調表示されている情報は、まだ一般に利用できない機能を示しています。 この機能は、プレビューサンドボックス環境でのみ使用できます。</span>

Adobe Workfront API の新しいバージョンを年 2 回リリースします。 各バージョンはリリース後 3 年間サポートされ、追加の年は廃止済み状態で、バージョンは使用可能ですがサポートされていません。

URI で API のバージョンを指定しない統合は、自動的にデフォルトにルーティングされます。 API 呼び出しで特定のバージョンの API を使用する場合は、Workfront API リクエストでそのバージョンを指定する必要があります。

>[!NOTE]
>
>お客様の組織が現在デフォルト API を使用している場合、Workfront管理者に、デフォルト API に関する詳細な手順を含むアナウンスセンターのメッセージが届きました。


<!--
Integrations that do not specify a version of the API in the URI are automatically routed to Default, which has been deprecated. In order for your Workfront integrations to be valid, you must specify a supported API version in your Workfront API requests.
-->

API リクエストでバージョンを指定する方法については、 [統合での API バージョンの指定](../../wf-api/api/specify-api-version-integrations.md).

## デフォルト API を使用する際の考慮事項

Workfront Default API を使用する際は、次の点に注意してください。

* 23.2 リリース以降、API のデフォルトバージョンは最新バージョンに設定されます。 バージョンが指定されていない API 呼び出しでは、デフォルトバージョンが使用されます。 Workfrontが API の新しいバージョンをリリースするたびに、デフォルトのバージョンが最新バージョンに更新されます。 **したがって、新しいバージョンのWorkfront API がリリースされた後は、デフォルトバージョンを使用する API 呼び出しをチェックして、機能が引き続きサポートされていることを確認する必要があります**.
* お客様の組織が現在非推奨のデフォルト API を使用している場合、Workfront管理者に、デフォルト API に関する詳細な手順を含むアナウンスセンターのメッセージが届きます。
* <span class="preview">プレビュー環境のデフォルト API は、現在、最新バージョンに設定されています。 実稼動環境のデフォルト API は、23.2 リリース以降、最新バージョンに設定されます。</span>

この API の最新バージョンについては、 [API のバージョン管理とサポートのスケジュール](../../wf-api/api/api-version-support-schedule.md).

<!--

## Deprecating Default

In an effort to improve the Workfront API, we are in the process of removing older API versions that have exceeded our support window of three years. One of these versions is Version 2, to which Default is mapped. This version was released in 2010, and much of the logic supported in the Attask/Workfront application at that time either no longer exists or has substantially changed.

We deprecated Default in July 2017, and we will no longer designate a specific version of the API to be the default version. Instead, all Workfront API requests must specify a specific API version.

>[!IMPORTANT]
>
> By July 1, 2018 all of your Workfront integrations that use Default must be updated to call a specific supported API version. After that date, all of your Workfront API requests used by integrations that do not specify a version will fail.

To learn about the Workfront deprecation cadence, see [API versioning and support schedule](../../wf-api/api/api-version-support-schedule.md).

-->

## サポートされる API バージョンへの統合の更新

Workfront API リクエストでバージョンが指定されていない場合は、デフォルトが使用されます。 API リクエストには、サポートされている API のバージョン（できれば最新のサポートされている API）を指定することをお勧めします。

例えば、次のWorkfront API リクエストでは API バージョンが指定されていません。

`https://davidwhite.my.workfront.com/attask/api/project/metadata`

このリクエストがおこなわれると、Workfrontインスタンスからデータを指定する JSON エンコードされたテキストで応答を受け取ります。 この URI では API バージョンが指定されていないので、呼び出しはデフォルトになります。

デフォルト API リクエストをバージョン管理された API リクエストに変換するには、サポートされている API バージョンを呼び出すだけです。 例えば、次の URI はバージョン 15 を要求します。

`https://davidwhite.my.workfront.com/attask/api/`**v15.0**`/project/metadata`

Workfront API リクエストを更新する際に、サポートされているアドビの API の任意のバージョンを指定できます。 特定の API の参照について詳しくは、 [統合での API バージョンの指定](../../wf-api/api/specify-api-version-integrations.md).

最大サポート期間を確保するには、最新バージョンにお問い合わせください。 サポートされている API のリストは、 [API のバージョン管理とサポートのスケジュール](../../wf-api/api/api-version-support-schedule.md).

## API のデフォルトバージョンの履歴

「デフォルト API」（デフォルト）の元の目的は、API を最新バージョンのWorkfront API にマッピングすることでした。 これにより、デフォルトと呼ばれる基本的な統合をおこなったお客様は、API リクエストを更新する必要がなくなります。

2011 年に、Workfrontは API のバージョン 3.0 をリリースしました。 デフォルトは自動的にバージョン 3.0 に移動され、バージョン 3.0 を更新せずに使用するには複雑すぎた多くの顧客統合が機能しなくなりました。 その結果、Workfrontはこの変更を元に戻し、デフォルトバージョンのバージョンをバージョン 2 のままにしました。

2011 年以降、Workfrontは API 機能を大幅に向上させました。 このため、API の古いバージョンは非推奨（廃止予定）となりました。 2017 年に、デフォルトバージョンの概念を完全に削除しました。 これは、お客様がアドビの API の安定したバージョンを使用し、統合を最大 3 年のサイクルで維持するよう促すためでした。

Workfrontがデフォルトの API バージョンを回復します。 デフォルト API は、Workfront API の最新バージョンに設定され、新しいバージョンがリリースされるたびに最新バージョンに更新されます。

