---
title: 階層とパンくずの概要
description: ワークスペース内のレコードタイプ間に複数のワークスペース階層を作成できます。
hide: true
hidefromtoc: true
source-git-commit: f345cc0d41dc1bd62e7361fa0755cb7ba72465a0
workflow-type: tm+mt
source-wordcount: '405'
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

ワークスペースで階層を使用する利点は次のとおりです。

* チームが実際にどのように計画、運営、配信するかを反映した方法で作業を整理する。
* ユーザーは、システム内の場所を示す一連のパンくずリストを参照することで、レコードタイプの接続方法や、戦略が実行に進む方法を理解できます。
* ナビゲーションを改善し、すべてのワークフローで明確さと継続性を確保します。
* 階層では、システム定義の厳密な構造が適用されず、代わりに、組織の動作方法に合ったフローを定義でき、すべての作業段階にわたる柔軟性と一貫性の両方がサポートされます。

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
   * グローバルレコードタイプは、複数の階層内の複数のワークスペースに表示される場合があります。
   * Workfrontのオブジェクトタイプは、複数の階層や異なるワークスペースに表示することもできます。
     <!--Not sure what this means: * Shared record can't be part of hierarchies.-->
   * リンクされたレコードタイプに対応するフィールドを作成しない接続を持つレコードタイプも、階層の一部にすることができます。 階層設定時に作成された新しい接続では、デフォルトで常に、リンクされたレコードタイプに対応するフィールドが作成されます。

## パンくずリストを表示する際の考慮事項


