---
title: 階層とパンくずの概要
description: ワークスペース内のレコードタイプ間に複数のワークスペース階層を作成できます。
hide: true
hidefromtoc: true
source-git-commit: 1f1db1c9184a6a8a2abcd3139e4e4e61d2f08bc4
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Hierarchy and Breadcrumb Overview
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---
-->

# 階層とパンくずの概要

Workspace Manager では、Adobe Workfront Planning のレコード・タイプと他のオブジェクト・タイプの間に、柔軟だが構造化された階層を定義できます。

階層は、レコードタイプ間の接続です。 最大 4 つのレコード タイプとオブジェクト タイプを 1 つの階層に接続できます。

階層の作成については、「[&#x200B; ワークスペース階層の作成 &#x200B;](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md)」を参照してください。

ワークスペースで階層を使用する利点は次のとおりです。

* チームが実際にどのように計画、運営、配信するかを反映した方法で作業を整理する。
* ユーザーが、システム内の場所を示す一連のパンくずリストを参照して、レコードタイプの接続方法や、戦略が実行に流れ込む方法を理解できるようにします。
* より良いナビゲーションを提供し、すべてのワークフローにわたって明確さと継続性を生み出します。
* 組織の仕組みに合ったフローを定義し、すべての作業段階にわたる柔軟性と一貫性の両方をサポートします。

## 階層を使用する場合の考慮事項

* ワークスペースマネージャーは、1 つのワークスペースに対して複数の階層を作成できます。
* 選択したレコードタイプ間に接続が既に存在する場合は、既存の接続が再利用されます。
* 連携が存在しない場合、Workfrontは階層設定の一環として自動的に連携を作成します。
* 階層設定のルールを次に示します。
   * レコードタイプは、特定のワークスペースに 1 つの親レコードタイプのみを持つことができます。

     例えば、戦術レコードタイプに同じワークスペース内の親として、キャンペーン レコードタイプと目標レコードタイプの両方を設定することはできません。
   * 1 つのレコードを同じタイプの複数の親レコードに接続できるのは、1 つのレコードを複数のレコード タイプに接続する場合か、複数のレコード タイプに接続する場合です。
例えば、戦術 A はキャンペーン X とキャンペーン Y の両方に属することができます。
   * 1 つのレコードタイプを複数の子レコードタイプに接続できます。

     例えば、キャンペーンレコードタイプは、戦術、テスト、その他のレコードタイプなど、他の複数のレコードタイプの親にすることができます。
   * 階層には、Planning レコード・タイプとWorkfrontオブジェクト・タイプの両方を含めることができます。

     例えば、計画戦術とWorkfront プロジェクトを子として使用したキャンペーンレコードタイプを指定できます。

     <!--asking if ONLY projects are supported here in slack; if yes, make a note to say that only Projects are supported; also add a note about AEM -->
   * グローバルレコードタイプは、複数の階層内の複数のワークスペースに表示される場合があります。<!--not sure if this AFTER they were added to another workspace; right now, I can see only the current workspace when building one??-->
   * Workfrontのオブジェクトタイプは、複数の階層や異なるワークスペースに表示することもできます。
   * グローバル レコード タイプは、異なるワークスペースの階層の一部にすることはできません。

     例えば、キャンペーンがグローバルレコードタイプで、Workspace 1 内の階層の一部である場合、Workspace 2 には既存のレコードタイプとして追加できますが、階層に含めることはできません。<!--verifying that this is not connectable RT and it is about global ones - checking in slack-->
   * リンクされたレコードタイプに対応するフィールドを作成しない接続を持つレコードタイプも、階層の一部にすることができます。 階層設定時に作成された新しい接続では、デフォルトで常に、リンクされたレコードタイプに対応するフィールドが作成されます。

## パンくずリストを表示する際の考慮事項

レコードタイプ間に階層を作成すると、これらのレコードタイプに属するレコードのパンくずリストが生成されます。

例えば、階層を作成し、「プログラム」に続いて「プロジェクト」を使用して「戦術」を使用してキャンペーンを接続した場合、階層内で接続されたいずれかのタイプのレコードに移動すると、階層内でレコードが配置されている場所を確認できます。

次の点に注意してください。

* レコードタイプが複数のワークスペースの複数の階層の一部である場合、レコードのページ上のレコードのパンくずリストから階層を切り替えることができます。
* パンくずリストは、Workfrontと Planning をまたいで機能します。

  例えば、Planning のキャンペーンと戦術およびWorkfrontのポートフォリオとプログラムに接続されたプロジェクトを見ると、パンくずリストから Planning とWorkfrontの両方の階層を切り替えることができます。

  詳しくは、[&#x200B; ワークスペース階層の作成 &#x200B;](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md) を参照してください。


