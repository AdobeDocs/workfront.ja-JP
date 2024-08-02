---
title: Adobe Workfront Planning での共有権限の概要
description: Adobe Workfront Planning のワークスペースまたはビューに対する権限を共有または削除できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 1ffd8a3dbb31154186dc37132c7e77c35de42ac3
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 52%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront Planning. This article describes the levels of access that users could have to Adobe Workfront Planning. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Adobe Workfront Planning での共有権限の概要

{{planning-important-intro}}

Adobe Workfront Planning のワークスペースまたはビューに対する権限を共有または削除できます。

この記事では、Workfront Planning オブジェクトの権限レベルについて説明します。

ワークスペースまたはビューを共有する方法については、次の記事を参照してください。

* [ワークスペースの共有](/help/quicksilver/planning/access/share-workspaces.md)

* [ビューの共有](/help/quicksilver/planning/access/share-views.md)

## Adobe Workfront Planning で共有できるオブジェクト

以下のオブジェクトを共有できます。

* ワークスペース

   * 組織内のユーザーとワークスペースを共有できます。
   * ワークスペースを共有すると、ワークスペースに関連付けられているすべてのレコードタイプ、レコード、フィールドも共有されます。ビューは共有されません。

* ビュー

   * ワークスペースへのアクセス権限とは別に、ビューへのアクセス権限をユーザー（システム管理者を含む）に付与する必要があります。
   * ビューに公開リンクを生成すると、組織外のユーザーとビューを公開で共有できます。公開リンクからレコードページにアクセスしたユーザーは、接続されたレコードやフィールドを含むすべてのレコードとそのフィールドを表示できます。

  詳しくは、[ ビューの共有 ](/help/quicksilver/planning/access/share-views.md) を参照してください。

内部的には、次のWorkfront エンティティとワークスペースまたはビューを共有できます。

* ユーザー
* グループ

## Adobe Workfront Planning でのオブジェクトの共有に関する考慮事項

* Adobe Workfrontのライセンスタイプは、Workfront Planning の権限と組み合わせて機能し、ワークスペースとそのオブジェクトの表示、投稿、管理に対するアクセス権を付与します。

  ライセンスタイプが Workfront Planning の権限レベルに与える影響については、[Adobe Workfront Planning 使用時のライセンスタイプの概要](/help/quicksilver/planning/access/license-type-overview.md)を参照してください。
* システム管理者は、未作成のワークスペースを含め、システム内のすべてのワークスペースを管理できます。
* システム管理者を含む他のユーザーは、自分が作成したビューまたは自分と共有されているビューにのみアクセスできます。システム管理者には、ビューの管理権限のみを付与できます。
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
>標準（またはプラン）ライセンスのユーザーのみが、Contributeまたはワークスペースに対する管理権限、およびビューに対する管理権限を持つことができます。
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

レコードタイプの権限は、ワークスペースに権限を付与すると継承されます。

レコードタイプの権限のレベルは次のとおりです。


|        | 管理 | 参加 | 表示 |
|--------|--------|------------|-------|
| 作成 | ✓ |            |       |
| 削除 | ✓ |            |       |
| 編集 | ✓ |            |       |
| 表示 | ✓ | ✓ | ✓ |

### レコード権限

レコード権限は、ワークスペースに対して権限を付与すると継承されます。

レコードの権限レベルは次のとおりです。


|        | 管理 | 参加 | 表示 |
|--------|--------|------------|-------|
| 作成 | ✓ |            |       |
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