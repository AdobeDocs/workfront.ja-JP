---
title: Adobe Workfront Planning での共有権限の概要
description: Adobe Workfront Planning のワークスペースまたはビューに対する権限を共有または削除できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 3856e56036a9845387d7dc6498a6f20728c8234a
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 77%

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

  ワークスペースを共有すると、ワークスペースに関連付けられているすべてのレコードタイプ、レコード、フィールドも共有されます。ビューは共有されません。

* ビュー

## Adobe Workfront Planning でのオブジェクトの共有に関する考慮事項

* Adobe Workfront ライセンスタイプは Workfront Planning の権限と連動して機能し、Workfront Planning の使用時にオブジェクトの表示、投稿、管理を行うアクセス権を付与します。

  ライセンスタイプが Workfront Planning の権限レベルに与える影響については、[Adobe Workfront Planning 使用時のライセンスタイプの概要](/help/quicksilver/planning/access/license-type-overview.md)を参照してください。
* システム管理者は、他のユーザーが作成したワークスペースを管理および共有できます。
* システム管理者でない場合は、他のユーザーが作成したワークスペースに参加できます（ワークスペースが共有されている場合）。
* ワークスペースやビューを一括で共有することはできません。
* ワークスペースまたはビューは次のエンティティと共有できます。
   * ユーザー
   * グループ
     <!--* You can share a view publicly, with people outside your organization when you generate a public link for a view.People accessing the record page from a public link can view all records and their fields, including connected records and fields.-->
* システム管理者を含む他のユーザーは、自分が作成したビューまたは自分と共有されているビューにのみアクセスできます。システム管理者には、ビューの管理権限のみを付与できます。
* ワークスペースへのリンクや、レコードタイプのページからのビューへのリンクを他のユーザーと共有できます。リンクを受け取ったユーザーが、選択したビューに表示されるワークスペースまたはレコードタイプのページにアクセスできるようにするには、そのユーザーはアクティブユーザーであり、Workfront にログインする必要があります。

## Adobe Workfront Planning オブジェクトに対する権限の共有

次の節の表に、ワークスペースまたはビューを共有する際に選択できる権限のレベルと、各レベルで許可される機能を示します。

>[!IMPORTANT]
>
>以下に示された権限のレベルは、すべてのユーザーに付与できるわけではありません。Workfront Planning オブジェクトに対して持つことができる権限のレベルは、ユーザーの個々のライセンスによって決まります。
>
>詳しくは、[Adobe Workfront Planning 使用時のライセンスタイプの概要](/help/quicksilver/planning/access/license-type-overview.md)を参照してください。


### ワークスペース権限

ユーザーに以下のエンティティへのアクセスを許可するには、ワークスペースへの権限を付与する必要があります。

* ワークスペース
* レコードタイプ
* レコード
* フィールド
* ビュー*

  *ワークスペースに対する表示以上の権限を持つすべてのユーザーが、ワークスペースのビューにもアクセスできるようにすることができます。 これは、ビューを共有する際に有効にする必要がある追加の権限です。 詳しくは、を参照してください [ビューの共有](/help/quicksilver/planning/access/share-views.md).

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


<!--You can share views internally or publicly. -->

ビューおよびビュー要素のアクセス許可のレベルは次のとおりです。

|        | 管理（招待されたユーザーのみがアクセスできます） | 表示（招待されたユーザーのみがアクセスできます） | ワークスペース内の全員が表示* |
|--------|--------|-------|------------------------------|
| 編集 | ✓ |       |                            |
| 削除 | ✓ |       |                            |
| 共有 | ✓ |       |                           |
| 表示 | ✓ | ✓ | ✓ |
| 適用 | ✓ | ✓ | ✓ |

*この表示アクセス権を取得するには、ユーザーはワークスペースに対する表示以上の権限を持っている必要があります。

<!--Replace the table above with the following when public sharing releases: 

|   Internal sharing     | Manage (Only invited people can access) | View (Only invited people can access)  |Everyone in the workspace can view*|
|--------|--------|-------|------------------------------|
| Edit   | ✓      |       |                            |
| Delete | ✓      |       |                            |
| Share  | ✓       |       |                           |
| View   | ✓      | ✓     | ✓                         |
| Apply  | ✓      | ✓     | ✓                          |

|   Public sharing      | View  |
|--------|-------|
| View   | ✓     |
| Apply  | ✓     |
-->


<!--old view permissions, before sharing View permissions to a view through a workspace:
|        | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |                            
| Delete | ✓      |       |                            
| Share  | ✓       |       |                           
| View   | ✓      | ✓     |                         
| Apply  | ✓      | ✓     |    
-->