---
title: Adobe Workfront Planning での共有権限の概要
description: Adobe Workfront Planning のワークスペースまたはビューに対する権限を共有または削除できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 2f8a5b2d2183090029966a13c7af37f20eb44fd0
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 56%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront Planning. This article describes the levels of access that users could have to Adobe Workfront Planning. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Adobe Workfront Planning での共有権限の概要

{{maestro-important-intro}}

Adobe Workfront Planning のワークスペースまたはビューに対する権限を共有または削除できます。

ここでは、Workfront Planning オブジェクトのアクセス許可レベルについて説明します。

ワークスペースまたはビューを共有する方法については、次の記事を参照してください。

* [ワークスペースを共有](/help/quicksilver/maestro/access/share-workspaces.md)

* [ビューを共有](/help/quicksilver/maestro/access/share-views.md)

## Adobe Workfront Planning で共有できるオブジェクト

次のオブジェクトを共有できます。

* ワークスペース

  ワークスペースを共有すると、ワークスペースに関連付けられているすべてのレコードタイプ、レコード、フィールドも共有されます。ビューは共有されません。

* ビュー

## Adobe Workfront Planning でのオブジェクトの共有に関する考慮事項

* お使いのAdobe Workfrontのライセンスタイプは、Workfront Planning の権限と組み合わせて機能し、Workfront Planning を使用する際にオブジェクトの表示、投稿、管理にアクセスできるようにします。

  ライセンスの種類がWorkfront Planning のアクセス許可レベルに与える影響については、を参照してください。 [Adobe Workfront Planning 使用時のライセンスタイプの概要](/help/quicksilver/maestro/access/license-type-overview.md).
* システム管理者は、他のユーザーが作成したワークスペースを管理および共有できます。
* システム管理者でない場合は、他のユーザーが作成したワークスペースに参加できます（ワークスペースが共有されている場合）。
* ワークスペースやビューを一括で共有することはできません。
* 以下のエンティティでワークスペースまたはビューを共有できます。
   * ユーザー
   * グループ
     <!--* You can share a view publicly, with people outside your organization when you generate a public link for a view.People accessing the record page from a public link can view all records and their fields, including connected records and fields.-->
* システム管理者を含む他のユーザーは、自分が作成したビューまたは共有されているビューにのみアクセスできます。 システム管理者には、ビューの管理権限のみを付与できます。
* ワークスペースへのリンクや、レコードタイプのページからのビューへのリンクを他のユーザーと共有できます。リンクを受け取ったユーザーが、選択したビューに表示されるワークスペースまたはレコードタイプのページにアクセスするには、そのユーザーがアクティブユーザーであり、Workfront にログインする必要があります。

## Adobe Workfront Planning オブジェクトのアクセス許可の共有

以下のセクションの表では、ワークスペースまたはビューを共有するときに選択できる権限のレベルと、各レベルで許可される機能について説明します。

>[!IMPORTANT]
>
>以下に示された権限のレベルは、すべてのユーザーに付与できるわけではありません。ユーザーの個々のライセンスによって、Workfront Planning オブジェクトに対してユーザーが受け取ることができるアクセス許可のレベルが決まります。
>
>詳しくは、を参照してください [Adobe Workfront Planning 使用時のライセンスタイプの概要](/help/quicksilver/maestro/access/license-type-overview.md).


### ワークスペース権限

|        | 管理 | 参加 | 表示 |
|--------|--------|------------|-------|
| 編集 | ✓ |            |       |
| 共有 | ✓ |            |       |
| 削除 | ✓ |            |       |
| 表示 | ✓ | ✓ | ✓ |

### レコードタイプの権限

レコードタイプの権限は、ワークスペースに権限を付与すると継承されます。

|        | 管理 | 参加 | 表示 |
|--------|--------|------------|-------|
| 作成 | ✓ |            |       |
| 削除 | ✓ |            |       |
| 編集 | ✓ |            |       |
| 表示 | ✓ | ✓ | ✓ |

### レコード権限

レコード権限は、ワークスペースに対して権限を付与すると継承されます。

|        | 管理 | 参加 | 表示 |
|--------|--------|------------|-------|
| 作成 | ✓ |            |       |
| 削除 | ✓ | ✓ |       |
| 編集 | ✓ | ✓ |       |
| 表示 | ✓ | ✓ | ✓ |

### フィールド権限

フィールド権限は、ワークスペースに対して権限を付与すると継承されます。
次の権限は、各フィールドに関連付けられた値ではなく、フィールド自体を参照します。フィールド値を編集するには、レコードを編集する権限が必要です。

|        | 管理 | 参加 | 表示 |
|--------|--------|------------|-------|
| 作成 | ✓ |            |       |
| 削除 | ✓ |            |       |
| 編集 | ✓ |            |       |
| 表示 | ✓ | ✓ | ✓ |


### 表示権限

レコードビューに対する個別の権限を付与する必要があります。ワークスペースに対する権限を付与しても、ワークスペース内のレコードビューに対する権限は付与されません。

<!--You can share views internally or publicly. -->

|        | 管理 | 表示 |
|--------|--------|-------|
| 編集 | ✓ |       |
| 削除 | ✓ |       |
| 共有 | ✓ |       |
| 表示 | ✓ | ✓ |
| 適用 | ✓ | ✓ |

<!--Replace the table above with the following when public sharing releases: 

|   Internal sharing     | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |
| Delete | ✓      |       |
| Share  | ✓       |       |
| View   | ✓      | ✓     |
| Apply  | ✓      | ✓     |

|   Public sharing      | View  |
|--------|-------|
| View   | ✓     |
| Apply  | ✓     |
-->