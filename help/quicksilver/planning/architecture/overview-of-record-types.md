---
title: レコードタイプの概要
description: レコードタイプは、Adobe Workfront Planning ワークスペースの構成要素です。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '294'
ht-degree: 49%

---


# レコードタイプの概要

{{planning-important-intro}}

オブジェクト型が事前定義されているWorkfrontとは異なり、Adobe Workfront Planning では独自のオブジェクト型を作成できます。

例えば、Workfront では、プログラム、ポートフォリオ、プロジェクト、タスクまたはイシューのオブジェクトタイプがあらかじめ作成されています。

Workfront Planning のオブジェクト・タイプは「レコード・タイプ」と呼ばれ、ユーザーが作成した場合にのみ存在します。

レコードタイプは、Workfrontの計画ワークスペースの構築ブロックで、ワークフローやその他の情報に関連付けられるようにするには、すべてを作成する必要があります。

レコードタイプはワークスペースで整理されます。

ワークスペースについて詳しくは、[ワークスペースの作成](/help/quicksilver/planning/architecture/create-workspaces.md)を参照してください。

## レコードタイプの概要

Workfront Planning では、組織のニーズに合ったカスタムレコードタイプを作成できます。

レコードタイプの作成について詳しくは、[ レコードタイプの作成 ](/help/quicksilver/planning/architecture/create-record-types.md) を参照してください。

* テンプレートからワークスペースを作成する際、次のワークスペースセクションにレコードタイプが作成されます。

   * **運用レコードタイプ**：戦略的計画、イニシアチブ、または予定作業を表すレコードタイプ。 例えば、キャンペーン、アクティビティ、戦術、商談は、運用レコードタイプです。
   * **分類**：運用レコードタイプに関する属性を取り込むレコードタイプ。例えば、地域、住所、オーディエンスは分類です。

  これらのセクションの名前を変更または削除したり、さらに作成したりできます。

* 最初から作成したワークスペースにレコードタイプを作成する際、ワークスペース内に作成した任意のセクションにレコードタイプを配置できます。
* レコードタイプの作成時、自分とワークスペースへのアクセス権を付与したユーザーのみが、このレコードタイプを表示できます。
* ワークスペースのレコードタイプを作成する前に、ワークスペースを作成する必要があります。
* 1 つのワークスペースまたはWorkfront インスタンスに含めることができるレコードタイプの数の制限については、[Adobe Workfront Planning オブジェクトの制限事項の概要 ](/help/quicksilver/planning/general/limitations-overview.md) を参照してください。


<!--

### Operational Record Type{#operational-record-type}

An operational record type is a Wrorkfront Planning record type that represents work-related objects.  

(***********insert screen shot**************)
For more information about operational record types including how to create them, see [Create record types](/help/quicksilver/planning/architecture/create-record-types.md). 

### Taxonomy{#taxonomy}

A taxonomy is a record type that captures attributes about an operational record type. 

(**********add screen shot**********)

Although creating taxonomies is identical to creating operational record types, Workfront Planning distinguishes conceptually between an operational record type and a taxonomy record type. The purpose of taxonomies is to enhance operational record types. Taxonomies should not directly represent work objects.  (***********this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.***********) 

(********mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc*************)

For example, Audience, Region, or Address can be taxonomy-type record types.  

## Similarities and differences between operational record types and taxonomies

The following table illustrates some of the similarities and differences between operational record types and taxonomies: 

| Record type and characteristic                              | Operational Record Type | Taxonomy Record Type |
|-------------------------------------------------------------|:-----------------------:|:--------------------:|
| They are part of a workspace                                |            ✓            |           ✓          |
| You can create them automatically, from a workspace template                    |            ✓            |           ✓          |
| You can create them manually, from scratch                    |            ✓            |           ✓          |
| You can create them by copying and pasting information from an external file or list                   |            ✓            |           ✓          |
| You can create by importing an Excel or CSV file                    |            ✓            |                     |
| You can create read-only record types by connecting to object types from other applications                    |            ✓            |                     |
| They represent work-related objects                         |            ✓            |                      |
| They represent attributes about work-related objects        |                         |           ✓          |
| You can create from scratch                                 |            ✓            |           ✓          |
| You can create by importing an Excel or CSV file            |            ✓            |                      |
| You can connect the record type to an object from another application|            ✓            |                      |
| You can connect to other record types               |            ✓            |                    |
| You can view their associated records in a table view       |            ✓            |           ✓          |
| You can view their associated records in a timeline view    |            ✓            |           ✓          |

-->
