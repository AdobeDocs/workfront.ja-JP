---
title: 階層とパンくずリストの概要
description: Workspace Managerでは、Adobe Workfront Planningで、接続されたレコードタイプと他のオブジェクトタイプの間に、柔軟でありながら構造化された階層を定義できます。 階層とは、レコードタイプ間、またはレコードタイプとWorkfront プロジェクト間のつながりです。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: de066d44-d214-47cc-8483-37c2623585ea
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 453dbf1c7598858e99d963f7a3806355a8cc80a9
workflow-type: tm+mt
source-wordcount: '1042'
ht-degree: 0%

---

# 階層とパンくずリストの概要

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

Workspace Managerでは、Adobe Workfront Planningで、接続されたレコードタイプと他のオブジェクトタイプの間に、柔軟でありながら構造化された階層を定義できます。

階層とは、レコードタイプ間、またはレコードタイプとWorkfront プロジェクト間のつながりです。

階層の作成について詳しくは、[ ワークスペース階層の作成](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md)を参照してください。

ワークスペースで階層を使用する利点は次のとおりです。

* チームが実際にどのように計画、運営、実施するかを反映した方法で作業を整理できます。
* 利用者が、システム内での自分の場所を示すパンくずリストを参照することで、自分がどこにいるのか、レコードタイプがどのように接続しているのか、戦略がどのように実行されるのかを把握できます。
* ナビゲーションを改善し、あらゆるワークフローを明確化して連続性を高めることです。
* To define flows that fit how your organization works, supporting both flexibility and consistency across all stages of work.

## 階層を操作する際の考慮事項

* 1つのワークスペースに対して最大5つの階層を作成できます。
* 1つの階層に接続できるレコードタイプとオブジェクトタイプは、最大4つまでです。
* ワークスペース階層内の次のオブジェクトタイプのみを接続できます。
   * Record types that belong to the workspace you&#39;re building the hierarchies in.
   * Workfront projects. Workfront projects cannot be added as parents of other record types. They are always the last object type in a hierarchy.
* You cannot add the following object types in a hierarchy:
   * Record types from other workspaces, even when they are set as connectable or global record types. You can add global record types to hierarchies only when they have been added to the workspace you&#39;re building the hierarchy from.
   * その他すべてのWorkfront オブジェクト。
   * Adobe Experience Manager Assetsまたはコンテンツフラグメント：
* 階層には、Planning レコードタイプとWorkfront プロジェクトの両方を同時に含めることができます。

  例えば、計画戦術とWorkfront プロジェクトを含むCampaign レコードタイプを、同じワークスペース階層の子として設定できます。

* If a connection between the selected record types already exists, the system reuses the existing connection.
* If no connection exists, Workfront will create one as part of the hierarchy setup.
* 階層に含めるレコードとオブジェクトタイプの接続フィールドに対して、**リンクされたレコードタイプに対応するフィールドを作成**&#x200B;設定を有効にする必要があります。
* レコードタイプが階層の一部である場合、そのタイプを削除することはできません。
* フィールドで参照されているレコードタイプが階層の一部である場合、接続フィールドを削除することはできません。 レコードタイプを削除する前に、まず階層からレコードタイプを削除するか、階層を削除する必要があります。
* 接続されたレコードタイプからルックアップフィールドを削除できます。 フィールド内の情報は復元できません。
* The following are rules for hierarchy setup:
   * レコードタイプは、特定のワークスペース内の親レコードタイプを1つだけ持つことができます。

     例えば、戦術レコードタイプは、Campaignと目標レコードタイプの両方を同じワークスペースの親として持つことはできません。
   * レコードタイプは、複数の階層の親にすることができます。

     例えば、1つのワークスペースに3つの異なる階層を持つことができ、それぞれに親レコードタイプとしてCampaignsを持つことができます。
   * 1つのレコードを同じタイプの複数の親レコードに接続できるのは、1つのレコードを複数のレコードタイプに接続したり、複数のレコードタイプに接続したりする場合です。

     For example, Tactic A can belong to both Campaign X and Campaign Y.
   * A record type can connect to only one child record type at a time. A child record type can also be a parent for another record type.

     For example, a Campaign record type can be the parent to only one other record type in the same hierarchy (Tactics), and Tactics can in turn be the parent of Programs which can be a parent to Projects.
   * A record type cannot be the parent in one hierarchy and the child in another hierarchy in the same workspace.
   * Global record types may appear in multiple workspaces inside multiple hierarchies, after they are added to those workspaces.

     例えば、Campaignがグローバルレコードタイプで、Workspace 1の階層の一部である場合、既存のレコードタイプとしてWorkspace 2に追加でき、そのレコードタイプは階層の一部になります。 ただし、Workspace 1でグローバルレコードタイプとして指定され、Workspace 2に追加されていない場合にのみ、Workspace 2の階層に含めることはできません。
   * 接続されたレコードタイプが階層の一部である場合、子レコードタイプの1つのレコードを、親レコードタイプの最大10件のレコードに接続できます。

     例えば、親としてCampaignsと子レコードとしてPersonaの間に階層を作成する場合、同じペルソナを最大10件のキャンペーンに接続できます。

## Considerations when viewing breadcrumbs

When you create hierarchies between record types, they generate breadcrumbs for records that belong to those record types.

For example, if you create a hierarchy and connect Campaigns with Tactics, then with Activities, when you navigate to a record of any of the types connected in the hierarchy, you can view where in the hierarchy the record is placed. レコードが複数のワークスペースに表示される場合は、各ワークスペースのパスをパンくずリストのワークスペース名で始めて表示できます。

![ パンくずリスト ](assets/breadcrumbs-on-activities-planning-only.png)

次の点に注意してください。

* パンくずリストは、レコードのプレビュー領域と、レコードの詳細ページに表示されます。
* レコードタイプが複数の階層に属している場合は、レコードのページ上のレコードのパンくずリストから階層を切り替えることができます。
* If the record type in a hierarchy has multiple records, you can select records from the breadcrumb.
* Breadcrumbs work across Workfront and Planning.

  For example, when looking at a project which is connected to Planning campaigns and tactics, and also to Workfront portfolios and programs, you can switch between both the Planning and the Workfront object types from the breadcrumb.

  For more information, see [Create workspace hierarchies](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).
* When you edit a record, the changes are visible from all the workspaces and all hierarchies the record is part of.
