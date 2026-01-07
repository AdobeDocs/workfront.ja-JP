---
title: Adobe Workfront Planning での共有権限の概要
description: Adobe Workfront Planning を使用する際、組織内のすべてのユーザーが同じアクセス権と権限を持っているわけではありません。 ここでは、Adobe Workfront Planning のワークスペースまたはビューに対する権限の共有または削除に関する一般的な情報を説明します。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 22%

---


<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

<!--remove the Prod and Preview references when we release to Prod-->

# Adobe Workfront Planning での共有権限の概要

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->



{{planning-important-intro}}

Adobe Workfront Planning のワークスペース、レコード・タイプまたはビューに対する権限を共有または削除できます。

また、Planning 要求フォームを共有することもできます。 詳しくは、[Adobe Workfront Planning でのリクエストフォームの作成と管理 ](/help/quicksilver/planning/requests/create-request-form.md) を参照してください。

ここでは、Workfront Planning の作業領域、レコード・タイプ、レコード、フィールドおよびビューの権限レベルについて説明します。

## Adobe Workfront Planning で共有できるオブジェクト

一部のWorkfront Planning オブジェクトは手動で共有できますが、他のオブジェクトはこれらのアクセス許可を他のオブジェクトから継承します。

Workfront Planning では、次のオブジェクトを手動で共有できます。

* ワークスペース

   * 組織内のユーザーとワークスペースを共有できます。
   * ワークスペースを共有すると、そのワークスペースに関連付けられているすべてのレコードタイプ、レコードおよびフィールドも共有されます。
   * ワークスペースを共有する場合、ビューは共有されません。 ビューは個別に共有されます。

  詳しくは、「ワークスペースの共有 [ を参照してください ](/help/quicksilver/planning/access/share-workspaces.md)

* レコードタイプ

   * レコードタイプは、組織内のユーザーと共有できます。
   * ワークスペースに付与された権限のレベルは、レコードタイプの継承権限として表示されます。
   * ユーザーがワークスペースで持っている権限レベルよりも高い権限レベルを持つレコードタイプを共有することはできません。

  詳しくは、[ レコードタイプの共有 ](/help/quicksilver/planning/access/share-record-types.md) を参照してください。


* ビュー

   * システム管理者を含むユーザーに、ワークスペースへのアクセス権限とは別に、ビューへのアクセス権限を付与する必要があります。
   * ビューを共有すると、フィルター、グループ化、並べ替え、設定を含むすべてのビュー要素が共有されます。
   * ビューを共有すると、そのビューに表示されているレコードは共有されません。 レコードは、ワークスペースを共有することで共有する必要があります。
   * ビューに公開リンクを生成すると、組織外のユーザーとビューを公開で共有できます。公開リンクからレコードページにアクセスしたユーザーは、接続されたレコードやフィールドを含むすべてのレコードとそのフィールドを表示できます。

  詳しくは、[ビューの共有](/help/quicksilver/planning/access/share-views.md)を参照してください。

## Adobe Workfront Planning でのオブジェクトの共有に関する考慮事項

* Adobe Workfrontのライセンスタイプは、Workfront Planning の権限と組み合わせて機能し、ワークスペースとそのオブジェクトの表示、投稿、管理に対するアクセス権を付与します。

  ライセンスタイプが Workfront Planning の権限レベルに与える影響については、[Adobe Workfront Planning 使用時のライセンスタイプの概要](/help/quicksilver/planning/access/license-type-overview.md)を参照してください。
* システム管理者は、未作成のワークスペースを含め、システム内のすべてのワークスペースを管理できます。
* システム管理者を含む他のユーザーは、自分が作成したビューまたは自分と共有されているビューにのみアクセスできます。システム管理者には、ビューを管理する権限のみを付与できます。

* ワークスペースとレコードの種類を他のユーザーと共有すると、レコードの種類のアクセス許可レベルが、それらに関連付けられたレコードとフィールドに自動的に継承されます。

  >[!IMPORTANT]
  >
  >組織のWorkfrontのインスタンスがAdobe Unified Experience にオンボードされている場合、計画オブジェクトを共有するユーザーはAdobe Admin Consoleに追加する必要があります。 Adobe Admin Consoleに追加されていないWorkfront ユーザーと Planning オブジェクトを共有することはできません。

* Planning オブジェクトは、次の方法で共有できます。

   * 内部的には、次のWorkfront エンティティでワークスペース、ビュー、またはレコードタイプを共有できます。

      * ユーザー
      * グループ
      * チーム
      * 会社
      * 担当業務

     Planning オブジェクトは、オブジェクトごとに最大 100 個のエンティティで共有できます。

   * 内部的には、ワークスペースまたはビューへのリンクを他の Planning ユーザーと共有します。 次のシナリオが存在します。

      * ワークスペースへのリンクを受け取るユーザーは、アクティブユーザーで、Workfrontにログインしてワークスペースにアクセスする必要があります。
      * ビューに対する内部共有リンクを受け取るユーザーは、アクティブユーザーであり、ビューにアクセスするためにWorkfrontにログインする必要があります。
   * 外部的には、Workfront アカウントを持たない外部ユーザーと、ビューへの公開共有リンクを共有する。

## Adobe Workfront Planning オブジェクトに対する権限の共有

次の節の表に、ワークスペースまたはビューを共有する際に選択できる権限のレベルと、各レベルで許可される機能を示します。

>[!IMPORTANT]
>
>以下に示された権限のレベルは、すべてのユーザーに付与できるわけではありません。Workfront Planning オブジェクトに対して持つことができる権限のレベルは、ユーザーの個々のライセンスによって決まります。
>
>標準（またはプラン）ライセンスのユーザーのみが、ワークスペースに対する投稿権限または管理権限、およびビューに対する管理権限を持つことができます。
> 
>他のすべてのライセンスタイプを持つユーザーは、ワークスペースおよびビューに対する表示権限を持つことができます。
>
>詳しくは、[Adobe Workfront Planning 使用時のライセンスタイプの概要](/help/quicksilver/planning/access/license-type-overview.md)を参照してください。


### ワークスペースに対する権限

ユーザーに以下のエンティティへのアクセスを許可するには、ワークスペースへの権限を付与する必要があります。

* ワークスペース
* レコードタイプ
* レコード
* フィールド

ワークスペースの権限のレベルは次のとおりです。

|        | 管理 | 参加 | 表示 |
|--------|--------|------------|-------|
| 編集 | ✓ |            |       |
| 共有 | ✓ |            |       |
| 削除 | ✓ |            |       |
| 表示 | ✓ | ✓ | ✓ |

### レコードタイプに対する権限

<!-- old access:
In the Production environment, Record Type permissions are always inherited when you grant permissions to the workspace.

The following are the levels of permissions for record types: 


|        | Manage | Contribute | View  |
|--------|--------|------------|-------|
| Create | ✓      |            |       |
| Delete | ✓      |            |       |
| Edit   | ✓      |            |       |
| View   | ✓      | ✓          | ✓     |

-->

ワークスペースに権限を付与すると、レコードタイプの権限は常に継承されます。

ワークスペースから受信したレコードタイプの継承された権限を削除できます。

ユーザーに対して、ワークスペースでのレコードタイプに対する権限よりも低い権限を付与できます。

ただし、次の操作は実行できません。

* ユーザーがワークスペースで持っている権限よりも高い権限をレコードタイプに付与します。
* ワークスペースマネージャーに、レコードタイプに対するより低い権限を付与します。
* レコードタイプの権限からユーザーを削除することで、レコードタイプまたはワークスペースに対する表示権限を削除します。

次のシナリオが存在します。

| ワークスペース権限 | レコードタイプに対して継承された自動権限 | 継承された権限が無効になっている場合に考えられるレコードタイプの権限（手動で付与） |
|--------|--------|-------------|
| 管理 | 管理 | 権限の管理、削除* |
| 参加 | 参加 | 投稿、表示、権限の削除* |
| 表示 | 表示 | 権限の表示、削除* |

>[!NOTE]
>
>レコードタイプから権限を削除しても、ワークスペースから権限を削除しない限り、ユーザーはワークスペースとすべてのレコードタイプに対する表示権限を保持します。

### レコードに対する権限

ワークスペースとレコードタイプに権限を付与すると、レコードの権限はレコードタイプから継承されます。

レコードの権限レベルは次のとおりです。


|        | 管理 | 参加 | 表示 |
|--------|--------|------------|-------|
| 作成 | ✓ | ✓ |       |
| 削除 | ✓ | ✓ |       |
| 編集 | ✓ | ✓ |       |
| 表示 | ✓ | ✓ | ✓ |

### フィールドの記録権限

ワークスペースとレコードタイプに権限を付与すると、フィールド権限はレコードタイプから継承されます。

次の権限は、各フィールドに関連付けられた値ではなく、フィールド自体を参照します。フィールド値を編集するには、レコードを編集する権限が必要です。

|        | 管理 | 参加 | 表示 |
|--------|--------|------------|-------|
| 作成 | ✓ |            |       |
| 削除 | ✓ |            |       |
| 編集 | ✓ |            |       |
| 表示 | ✓ | ✓ | ✓ |


### ビューに対する権限

ビューを記録するには、別の権限を付与する必要があります。ワークスペースに権限を付与しても、ワークスペースのレコードビューに対する権限は付与されません。

ユーザーに次のビュー要素へのアクセス権を付与するには、ビューへの権限を付与する必要があります。

* フィルター
* フィールドの表示
* 並べ替え
* グループ化
* 行の高さ
* 設定

ビューは、内部または公開で共有できます。

ビューおよびビュー要素のアクセス許可のレベルは次のとおりです。

| 内部共有 | 管理（招待されたユーザーのみがアクセスできます） | 表示（招待されたユーザーのみがアクセスできます） | ワークスペース内の全員が表示* |
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

*この表示アクセス権を取得するには、ユーザーはワークスペースに対する表示以上の権限を持っている必要があります。

<!--old view permissions, before sharing View permissions to a view through a workspace:
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
