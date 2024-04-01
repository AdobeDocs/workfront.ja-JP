---
title: レコードタイプの概要
description: レコードタイプは、Adobe Workfront Planning ワークスペースの構成要素です。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
source-git-commit: e54142e189cd4f407161401203a7f13c752ad404
workflow-type: tm+mt
source-wordcount: '270'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# レコードタイプの概要

{{maestro-important-intro}}

オブジェクト・タイプが事前に定義されているWorkfrontとは異なり、Adobe Workfront Planning では、独自のオブジェクト・タイプを作成できます。 例えば、Workfrontでは、プログラム、Portfolio、プロジェクト、タスク、またはイシューのオブジェクトの種類が既に作成されています。

Workfront Planning のオブジェクトタイプは「レコードタイプ」と呼ばれ、すべてのオブジェクトタイプを作成してカスタマイズできます。 レコードタイプは、Workfront Planning ワークスペースの構成要素です。 ワークスペースについて詳しくは、 [ワークスペースの作成](../architecture/create-workspaces.md).

## レコードタイプの概要

Workfront Planning では、組織のニーズに合ったカスタムレコードタイプを作成できます。

* テンプレートからワークスペースを作成する場合、次のワークスペースセクションにレコードタイプが作成されます。

   * [オペレーショナルレコードのタイプ](#operational-record-type)：戦略計画、イニシアチブまたは計画済み作業を表すレコードタイプです。 例えば、キャンペーン、アクティビティ、戦術、商談は、オペレーショナルレコードタイプにすることができます。
   * [分類](#taxonomy)：オペレーショナルレコードタイプに関する属性を取り込むレコードタイプ。 例えば、地域、住所、オーディエンスは、分類にすることができます。

* 最初から作成したワークスペースでレコードタイプを作成する場合は、ワークスペースで作成した任意のセクションにレコードタイプを配置できます。
* レコードタイプを作成する場合、自分と、ワークスペースへのアクセス権を付与したユーザーだけがレコードタイプを表示できます。
* ワークスペースのレコードタイプを作成する前に、ワークスペースを作成する必要があります。
* 1 つのワークスペースには、ワークスペースのセクション数に関係なく、合計 1,000 個のレコードタイプを含めることができます。 これには、最初から作成したレコードタイプや、テンプレートを使用して作成したレコードタイプが含まれます。


<!--

### Operational Record Type{#operational-record-type}

An operational record type is a Maestro record type that represents work-related objects.  

![](assets/operational-record-type-blank.png)

For more information about operational record types including how to create them, see [Create record types](../architecture/create-record-types.md). 

### Taxonomy{#taxonomy}

A taxonomy is a record type that captures attributes about an operational record type. 

![](assets/taxonomy-record-type-blank.png)

For more information about taxonomy record types, see [Create a taxonomy](../architecture/create-a-taxonomy.md). 

Although creating taxonomies is identical to creating operational record types, Maestro distinguishes conceptually between an operational record type and a taxonomy record type. The purpose of taxonomies is to enhance operational record types. Taxonomies should not directly represent work objects.  (***********this is no longer true, but might be later?!: A taxonomy is a record without dates, like a static list of attributes.***********) 

(********mimic what you did above for operational record types to say that we can also import taxonomies from other applications too - this will be possible later; for example Team would be a taxonomy record type, etc*************)

For example, Audience, Region, or Address can be taxonomy-type record types.  

For more information, see [Create a taxonomy](../architecture/create-a-taxonomy.md). 

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
| You can connect to other Maestro record types               |            ✓            |                    |
| You can view their associated records in a table view       |            ✓            |           ✓          |
| You can view their associated records in a timeline view    |            ✓            |           ✓          |

-->