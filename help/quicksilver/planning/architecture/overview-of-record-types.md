---
title: レコードタイプの概要
description: レコードタイプは、Adobe Workfront Planning ワークスペースの構成要素です。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 1de095b3-78d9-44df-a678-51f4238deb91
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '352'
ht-degree: 38%

---


# レコードタイプの概要

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

オブジェクトタイプが事前に定義されているWorkfrontとは異なり、Adobe Workfront Planningでは、独自のオブジェクトタイプを作成できます。

例えば、Workfront では、プログラム、ポートフォリオ、プロジェクト、タスクまたはイシューのオブジェクトタイプがあらかじめ作成されています。

Workfront Planningのオブジェクト・タイプは「レコード・タイプ」と呼ばれ、ユーザーが作成する場合にのみ存在します。

レコードタイプは、Workfrontプランニングワークスペースの構成要素であり、ワークフローやその他の情報に関連付けるには、それらをすべて作成する必要があります。

レコードタイプは、ワークスペースで整理されます。

ワークスペースについて詳しくは、[ワークスペースの作成](/help/quicksilver/planning/architecture/create-workspaces.md)を参照してください。

## レコードタイプの概要

Workfront Planning では、組織のニーズに合ったカスタムレコードタイプを作成できます。

レコードタイプの作成について詳しくは、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

* テンプレートからワークスペースを作成する際、次のワークスペースセクションにレコードタイプが作成されます。

   * **操作レコードタイプ**：戦略的プランニング、イニシアチブ、または計画作業を表すレコードタイプ。 たとえば、キャンペーン、アクティビティ、戦術、商談は、運用上のレコードタイプです。
   * **分類**：運用レコードタイプに関する属性を取り込むレコードタイプ。例えば、地域、住所、オーディエンスは分類基準です。

  セクションとレコードタイプの名前を変更したり、削除したり、さらに作成したりできます。

* 最初から作成したワークスペースにレコードタイプを作成する際、ワークスペース内に作成した任意のセクションにレコードタイプを配置できます。
* レコードタイプを作成する場合、ワークスペースへのアクセス権を付与するのは自分と自分のユーザーのみです。レコードタイプは自分のユーザーのみがアクセスできます。
* ワークスペースのレコードタイプを作成する前に、ワークスペースを作成する必要があります。

  1つのワークスペースまたはWorkfront インスタンスに含めることができるレコードタイプの数に関する制限については、[Adobe Workfront プランニングオブジェクトの制限の概要](/help/quicksilver/planning/general/limitations-overview.md)を参照してください。
* 複数のワークスペースでレコードタイプを使用するには、レコードタイプをグローバルまたは接続可能として指定できます。

   * グローバルレコードタイプは、既存のレコードタイプとして他のワークスペースに追加できます。
   * 接続可能なレコードタイプは、他のワークスペースから接続できます。

  詳細については、[&#x200B; レコードタイプのクロスワークスペース機能の設定](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md)を参照してください。


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
