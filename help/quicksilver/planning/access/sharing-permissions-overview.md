---
title: Adobe Workfront Planning での共有権限の概要
description: Adobe Workfront Planning を使用する際、組織内のすべてのユーザーが同じアクセス権と権限を持っているわけではありません。 ここでは、Adobe Workfront Planning のワークスペースまたはビューに対する権限の共有または削除に関する一般的な情報を説明します。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: fd8e5d3baf6af0dbdd1275494fad54b204abd1a5
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 41%

---


<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Adobe Workfront Planning での共有権限の概要

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>



{{planning-important-intro}}

Adobe Workfront Planning のワークスペースまたはビューに対する権限を共有または削除できます。

この記事では、Workfront Planning オブジェクトの権限レベルについて説明します。

## Adobe Workfront Planning で共有できるオブジェクト

以下のオブジェクトを共有できます。

* ワークスペース

   * 組織内のユーザーとワークスペースを共有できます。
   * ワークスペースを共有すると、そのワークスペースに関連付けられているすべてのレコードタイプ、レコードおよびフィールドも共有されます。
   * ワークスペースを共有する場合、ビューは共有されません。 ビューは個別に共有されます。

  詳しくは、「ワークスペースの共有 [ を参照してください ](/help/quicksilver/planning/access/share-workspaces.md)

<!--
<div class="preview">

* Record types

    * You can share record types with people inside your organization.
    * The level of permissions granted for the workspace displays as Inherited permissions for the record type. 
    * You cannot share a workspace with a higher permission level than the user has on the workspace. 

    For more information, see [Share record types](/help/quicksilver/planning/access/share-record-types.md). 

</div>
-->

* ビュー

   * システム管理者を含むユーザーに、ワークスペースへのアクセス権限とは別に、ビューへのアクセス権限を付与する必要があります。
   * ビューを共有すると、フィルター、グループ化、並べ替え、設定を含むすべてのビュー要素が共有されます。
   * ビューを共有すると、そのビューに表示されているレコードは共有されません。 レコードは、ワークスペースを共有することで共有する必要があります。
   * ビューに公開リンクを生成すると、組織外のユーザーとビューを公開で共有できます。公開リンクからレコードページにアクセスしたユーザーは、接続されたレコードやフィールドを含むすべてのレコードとそのフィールドを表示できます。

  詳しくは、[ビューの共有](/help/quicksilver/planning/access/share-views.md)を参照してください。

内部的には、次のWorkfront エンティティとワークスペースまたはビューを共有できます。

* ユーザー
* グループ

<div class="preview">

* チーム
* 会社
* 担当業務

</div>

## Adobe Workfront Planning でのオブジェクトの共有に関する考慮事項

* Adobe Workfrontのライセンスタイプは、Workfront Planning の権限と組み合わせて機能し、ワークスペースとそのオブジェクトの表示、投稿、管理に対するアクセス権を付与します。

  ライセンスタイプが Workfront Planning の権限レベルに与える影響については、[Adobe Workfront Planning 使用時のライセンスタイプの概要](/help/quicksilver/planning/access/license-type-overview.md)を参照してください。
* システム管理者は、未作成のワークスペースを含め、システム内のすべてのワークスペースを管理できます。
* システム管理者を含む他のユーザーは、自分が作成したビューまたは自分と共有されているビューにのみアクセスできます。システム管理者には、ビューを管理する権限のみを付与できます。
* ワークスペースまたはビューへのリンクを他のユーザーと共有できます。

  次のシナリオが存在します。
   * ワークスペースへのリンクを受け取ったユーザーは、アクティブユーザーであり、ワークスペースにアクセスするためにWorkfrontにログインする必要があります。
   * ビューへのリンクを受け取ったユーザーは、次の方法でビューにアクセスできます。

      * ビューへのリンクが内部的に共有されている場合、アクティブユーザーで、Workfrontにログインする必要があります。
      * Workfrontの外部ユーザーであり、Workfrontにログインすることなく、公開共有リンクからビューにアクセスできる。

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


### ワークスペース権限

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

### レコードタイプの権限

<!--In the Production environment,--> ワークスペースに権限を付与すると、レコードタイプの権限は常に継承されます。

レコードタイプの権限のレベルは次のとおりです。


|        | 管理 | 参加 | 表示 |
|--------|--------|------------|-------|
| 作成 | ✓ |            |       |
| 削除 | ✓ |            |       |
| 編集 | ✓ |            |       |
| 表示 | ✓ | ✓ | ✓ |

<!--

<div class="preview">

In the Preview environment, Record Type permissions are inherited when you grant permissions to the workspace. 

You can remove inherited permissions from the record type, but you can never grant higher permissions for the record type than users have on the workspace. 

The following scenarios exist: 

|   Workspace permissions     | Automatic inherited permissions for a Record Type |Possible Record Type permissions when Inherited permissions are turned off (granted manually)| 
|--------|--------|-------------|
| Manage |   Manage    |   Manage, No permissions           | 
| Contribute |     Contribute |  Contribute, View, No permissions        |
| View   |  View     |      View, No permissions        |     


</div>

-->

### レコード権限

レコード権限は、ワークスペースに対して権限を付与すると継承されます。

レコードの権限レベルは次のとおりです。


|        | 管理 | 参加 | 表示 |
|--------|--------|------------|-------|
| 作成 | ✓ | ✓ |       |
| 削除 | ✓ | ✓ |       |
| 編集 | ✓ | ✓ |       |
| 表示 | ✓ | ✓ | ✓ |

### フィールド権限

ワークスペースに対して権限を付与すると、フィールド権限が継承されます。
次の権限は、各フィールドに関連付けられた値ではなく、フィールド自体を参照します。フィールド値を編集するには、レコードを編集する権限が必要です。

|        | 管理 | 参加 | 表示 |
|--------|--------|------------|-------|
| 作成 | ✓ |            |       |
| 削除 | ✓ |            |       |
| 編集 | ✓ |            |       |
| 表示 | ✓ | ✓ | ✓ |


### 権限を表示

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