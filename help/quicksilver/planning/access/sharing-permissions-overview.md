---
title: Adobe Workfront Planningでの共有権限の概要
description: 組織内のすべてのユーザーが、Adobe Workfront Planningを使用するための同じアクセス権と権限を持つわけではありません。 ここでは、Adobe Workfront Planning ワークスペースまたはビューに対する権限の共有または削除に関する一般的な情報について説明します。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 22%

---


<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

<!--remove the Prod and Preview references when we release to Prod-->

# Adobe Workfront Planning での共有権限の概要

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->



{{planning-important-intro}}

Adobe Workfront Planning ワークスペース、レコードタイプ、またはビューに対する権限を共有または削除できます。

また、Planning リクエストフォームを共有することもできます。 詳しくは、[Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md)でのリクエストフォームの作成と管理を参照してください。

ここでは、Workfront Planning ワークスペース、レコードタイプ、レコード、フィールドおよびビューの権限レベルについて説明します。

## Adobe Workfront Planning で共有できるオブジェクト

一部のWorkfront Planning オブジェクトは手動で共有できますが、他のオブジェクトは他のオブジェクトからこれらの権限を継承します。

Workfront Planningでは、次のオブジェクトを手動で共有できます。

* ワークスペース

   * 組織内のユーザーとワークスペースを共有できます。
   * ワークスペースを共有すると、ワークスペースに関連付けられたすべてのレコードタイプ、レコード、フィールドも共有されます。
   * ワークスペースを共有する場合、ビューは共有されません。 ビューは個別に共有されます。

  詳しくは、[ ワークスペースの共有](/help/quicksilver/planning/access/share-workspaces.md)を参照してください

* レコードタイプ

   * レコードタイプは、組織内の他のユーザーと共有できます。
   * ワークスペースに付与された権限レベルは、レコードタイプの継承された権限として表示されます。
   * ユーザーがワークスペース上で持つ権限レベルよりも高い権限レベルのレコードタイプを共有することはできません。

  詳しくは、[ レコードタイプの共有](/help/quicksilver/planning/access/share-record-types.md)を参照してください。


* ビュー

   * システム管理者を含むユーザーに、ワークスペースへのアクセス権とは別にビューにアクセスする権限を付与する必要があります。
   * ビューを共有すると、フィルター、グループ化、並べ替え、設定など、すべてのビュー要素が共有されます。
   * ビューを共有すると、ビューに表示されるレコードは共有されません。 レコードは、ワークスペースを共有することによって共有する必要があります。
   * ビューの公開リンクを生成すると、組織外のユーザーとビューを公開できます。公開リンクからレコードページにアクセスするユーザーは、接続されたレコードとフィールドを含むすべてのレコードとそのフィールドを表示できます。

  詳しくは、[ビューの共有](/help/quicksilver/planning/access/share-views.md)を参照してください。

## Adobe Workfront Planning でのオブジェクトの共有に関する考慮事項

* Adobe Workfrontのライセンスタイプは、Workfrontのプランニング権限と連携して、ワークスペースとそのオブジェクトを表示、提供、管理するためのアクセス権を付与します。

  ライセンスタイプが Workfront Planning の権限レベルに与える影響については、[Adobe Workfront Planning 使用時のライセンスタイプの概要](/help/quicksilver/planning/access/license-type-overview.md)を参照してください。
* システム管理者は、作成しなかったワークスペースを含め、システム内のすべてのワークスペースを管理できます。
* システム管理者を含む他のユーザーは、自分が作成したビューまたは自分と共有されているビューにのみアクセスできます。システム管理者には、ビューの管理に対してのみ権限を付与できます。

* ワークスペースとレコードタイプを他のユーザーと共有すると、レコードタイプの権限レベルは、関連するレコードとフィールドに自動的に継承されます。

  >[!IMPORTANT]
  >
  >組織のWorkfront インスタンスがAdobe Unified Experienceにオンボーディングされている場合、プランニングオブジェクトを共有するユーザーをAdobe Admin Consoleに追加する必要があります。 Adobe Admin Consoleに追加されていないWorkfront ユーザーとPlanning オブジェクトを共有することはできません。

* Planning オブジェクトは、次の方法で共有できます。

   * 内部的には、ワークスペース、ビュー、またはレコードタイプを次のWorkfront エンティティと共有できます。

      * ユーザー
      * グループ
      * チーム
      * 会社
      * 担当業務

     1つのオブジェクトにつき最大100個のエンティティを持つPlanning オブジェクトを共有できます。

   * 内部的には、ワークスペースまたはビューへのリンクを他のPlanning ユーザーと共有することによって行います。 次のシナリオが存在します。

      * ワークスペースへのリンクを受け取るユーザーは、アクティブユーザーで、Workfrontにログインしてワークスペースにアクセスする必要があります。
      * ビューの内部共有リンクを受け取るユーザーは、アクティブなユーザーで、Workfrontにログインしてビューにアクセスする必要があります。
   * 外部では、Workfront アカウントを持たない外部ユーザーとビューへの公開共有リンクを共有します。

## Adobe Workfront Planning オブジェクトに対する権限の共有

次の節の表に、ワークスペースまたはビューを共有する際に選択できる権限のレベルと、各レベルで許可される機能を示します。

>[!IMPORTANT]
>
>以下に示された権限のレベルは、すべてのユーザーに付与できるわけではありません。Workfront Planning オブジェクトに対して持つことができる権限のレベルは、ユーザーの個々のライセンスによって決まります。
>
>ワークスペースに対するContribute権限またはManage権限とビューに対するManage権限を持つことができるのは、Standard （またはプラン）のライセンスユーザーのみです。
> 
>他のすべてのライセンスタイプを持つユーザーは、ワークスペースとビューに対する表示権限を持つことができます。
>
>詳しくは、[Adobe Workfront Planning 使用時のライセンスタイプの概要](/help/quicksilver/planning/access/license-type-overview.md)を参照してください。


### ワークスペースへの権限

ユーザーが次のエンティティにアクセスできるようにするには、ユーザーにワークスペースへの権限を付与する必要があります。

* ワークスペース
* レコードタイプ
* レコード
* フィールド

ワークスペースの権限レベルは次のとおりです。

|        | 管理 | 参加 | 表示 |
|--------|--------|------------|-------|
| 編集 | ✓ |            |       |
| 共有 | ✓ |            |       |
| 削除 | ✓ |            |       |
| 表示 | ✓ | ✓ | ✓ |

### レコードタイプに対する権限

<!--
 old access:
In the Production environment, Record Type permissions are always inherited when you grant permissions to the workspace.

The following are the levels of permissions for record types: 


|        | Manage | Contribute | View  |
|--------|--------|------------|-------|
| Create | ✓      |            |       |
| Delete | ✓      |            |       |
| Edit   | ✓      |            |       |
| View   | ✓      | ✓          | ✓     |

-->

レコードタイプの権限は、ワークスペースに権限を付与する際に常に継承されます。

ワークスペースから受け取ったレコードタイプの継承された権限を削除できます。

ユーザーには、ワークスペースよりもレコードタイプに対する権限を低く設定できます。

ただし、次の操作はできません。

* ユーザーがワークスペースで持っているよりも高い権限をレコードタイプに付与します。
* ワークスペースのマネージャーに、レコードタイプに対する低い権限を付与します。
* レコードタイプの権限からユーザーを削除して、レコードタイプまたはワークスペースに対する表示権限を削除します。

次のシナリオが存在します。

| ワークスペース権限 | レコードタイプの自動継承された権限 | 継承された権限がオフになっている場合に可能なレコードタイプの権限（手動で付与） |
|--------|--------|-------------|
| 管理 | 管理 | 管理、権限の削除* |
| 参加 | 参加 | 貢献、表示、権限の削除* |
| 表示 | 表示 | 表示、権限の削除* |

>[!NOTE]
>
>レコードタイプから権限を削除しても、ユーザーは、ワークスペースから権限を削除しない限り、ワークスペースとすべてのレコードタイプに対する表示権限を保持します。

### レコードへの権限

レコードの権限は、ワークスペースとレコードタイプに権限を付与する際に、レコードタイプから継承されます。

レコードの権限レベルは次のとおりです。


|        | 管理 | 参加 | 表示 |
|--------|--------|------------|-------|
| 作成 | ✓ | ✓ |       |
| 削除 | ✓ | ✓ |       |
| 編集 | ✓ | ✓ |       |
| 表示 | ✓ | ✓ | ✓ |

### レコードフィールドへの権限

フィールド権限は、ワークスペースとレコードタイプに権限を付与する際に、レコードタイプから継承されます。

次の権限は、各フィールドに関連付けられた値ではなく、フィールド自体を参照します。フィールド値を編集するには、レコードを編集する権限が必要です。

|        | 管理 | 参加 | 表示 |
|--------|--------|------------|-------|
| 作成 | ✓ |            |       |
| 削除 | ✓ |            |       |
| 編集 | ✓ |            |       |
| 表示 | ✓ | ✓ | ✓ |


### ビューに対する権限

ビューを記録するには、別の権限を付与する必要があります。ワークスペースに権限を付与しても、ワークスペースのレコードビューに対する権限は付与されません。

ユーザーが次のビュー要素にアクセスできるようにするには、ユーザーにビューへの権限を付与する必要があります。

* フィルター
* フィールドの表示
* 並べ替え
* グループ化
* 行の高さ
* 設定

社内または社外で意見を共有することができます。

ビューとビュー要素に対する権限のレベルは次のとおりです。

| 内部共有 | 管理（招待されたユーザーのみがアクセスできます） | 表示（招待されたユーザーのみがアクセスできます） | ワークスペース内のすべてのユーザーが表示できます* |
|--------|--------|-------|------------------------------|
| 編集 | ✓ |       |                            |
| 削除 | ✓ |       |                            |
| 共有 | ✓ |       |                           |
| 表示 | ✓ | ✓ | ✓ |
| 適用 | ✓ | ✓ | ✓ |

| パブリック共有 | 表示 |
|--------|-------|
| 表示 | ✓ |
| 適用 | ✓ |

* この表示アクセス権を取得するには、ユーザーがワークスペースに対する表示権限またはそれ以上の権限を持っている必要があります。

<!--
old view permissions, before sharing View permissions to a view through a workspace:
|        | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |                            
| Delete | ✓      |       |                            
| Share  | ✓       |       |                           
| View   | ✓      | ✓     |                         
| Apply  | ✓      | ✓     |


|        | Manage (Only invited people can access) | View (Only invited people can access)  |Everyone in the workspace can view*|
|--------|--------|-------|------------------------------|
| Edit   | ✓      |       |                            |
| Delete | ✓      |       |                            |
| Share  | ✓       |       |                           |
| View   | ✓      | ✓     | ✓                         |
| Access the view  | ✓      | ✓     | ✓                          |
| Apply temporary filters, groupings, sort  | ✓      | ✓     | ✓                          |
-->
