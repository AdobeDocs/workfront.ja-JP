---
title: レコード・タイプと分類の概要
description: レコードタイプは、Maestro ワークスペースの構成要素です。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: ce015eba8291995eec1611917896a0e797f820cc
workflow-type: tm+mt
source-wordcount: '581'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# レコード・タイプと分類の概要

>[!IMPORTANT]
>
>この記事の情報は、Adobe Workfrontからの新しいオファーであるAdobe・マエストロを指します。
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。 Maestro 機能を使用するには、Workfrontのお客様である必要があります。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

オブジェクトタイプが事前に定義されているWorkfrontとは異なり、Adobeマエストロでは、独自のオブジェクトタイプを作成できます。 例えば、Workfrontでは、プログラム、Portfolio、プロジェクト、タスク、またはイシューのオブジェクトの種類が既に作成されています。

マエストロオブジェクトタイプは「レコードタイプ」と呼ばれます。 レコードタイプは、Maestro ワークスペースの構成要素です。 ワークスペースについて詳しくは、 [ワークスペースの作成](../architecture/create-workspaces.md).

## レコードタイプの概要

Maestro では、組織のニーズに合ったカスタムレコードタイプを作成できます。

* 次に、Maestro レコードのタイプを示します。

   * [オペレーショナルレコードの種類](#operational-record-type)：戦略計画、イニシアチブまたは計画済み作業を表すレコードタイプです。 例えば、キャンペーン、アクティビティ、戦術、商談は、オペレーショナルレコードタイプにすることができます。
   * [分類](#taxonomy)：オペレーショナルレコードタイプに関する属性を取り込むレコードタイプ。 例えば、地域、住所、オーディエンスは、分類にすることができます。

* レコードタイプを作成する場合、自分と、ワークスペースへのアクセス権を付与したユーザーだけがレコードタイプを表示できます。
* ワークスペースのレコードタイプを作成する前に、ワークスペースを作成する必要があります。
* 1 つのワークスペースに、合計 1,000 個のオペレーショナル・レコード・タイプと分類を組み合わせることができます。 これには、最初から作成したレコードタイプや分類、または他のシステムからインポートしたレコードタイプや分類が含まれます。

### オペレーショナルレコードの種類{#operational-record-type}

操作レコードの種類は、作業関連のオブジェクトを表す Maestro レコードの種類です。

![](assets/operational-record-type-blank.png)

オペレーショナルレコードの種類の作成方法などの詳細については、「 [レコードタイプの作成](../architecture/create-record-types.md).

### 分類{#taxonomy}

分類とは、オペレーショナルレコードタイプに関する属性をキャプチャするレコードタイプです。

![](assets/taxonomy-record-type-blank.png)

分類レコードタイプの詳細については、「 [分類の作成](../architecture/create-a-taxonomy.md).

分類の作成は、オペレーショナルレコードタイプの作成と同じですが、Maestro では、概念上、オペレーショナルレコードタイプとタクソノミレコードタイプを区別します。 分類の目的は、オペレーショナル・レコード・タイプを強化することです。 分類は、作業オブジェクトを直接表すものではありません。  <!--this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.-->

<!--mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc -->

例えば、Audience、Region、Address は、分類タイプのレコードタイプにすることができます。

詳しくは、 [分類の作成](../architecture/create-a-taxonomy.md).

## オペレーショナル・レコード・タイプと分類の類似点と相違点

次の表に、オペレーショナル・レコード・タイプと分類の類似点と相違点を示します。

| レコードのタイプと特性 | オペレーショナルレコードの種類 | 分類レコードタイプ |
|-------------------------------------------------------------|:-----------------------:|:--------------------:|
| これらはワークスペースの一部です | ✓ | ✓ |
| ワークスペーステンプレートから自動的に作成できます | ✓ | ✓ |
| 一から手動で作成できます。 | ✓ | ✓ |
| 外部ファイルまたはリストから情報をコピー&amp;ペーストして作成できます | ✓ | ✓ |
| Excel または CSV ファイルをインポートして作成できます | ✓ |                     |
| 他のアプリケーションからオブジェクトタイプに接続すると、読み取り専用のレコードタイプを作成できます | ✓ |                     |
| 作業関連オブジェクトを表します。 | ✓ |                      |
| 作業関連オブジェクトに関する属性を表します。 |                         | ✓ |
| ゼロから作成できます | ✓ | ✓ |
| Excel または CSV ファイルをインポートして作成できます | ✓ |                      |
| レコードタイプをサードパーティのアプリケーションからオブジェクトに接続できます | ✓ |                      |
| 他の Maestro レコードタイプに接続できます | ✓ |                    |
| 関連するレコードをテーブルビューで表示できます | ✓ | ✓ |
| 関連するレコードをタイムライン表示で表示できます | ✓ | ✓ |
