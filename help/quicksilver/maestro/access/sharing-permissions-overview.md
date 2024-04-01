---
title: Adobe Workfront Planning での共有権限の概要
description: Adobe Workfront Planning のワークスペースまたはビューに対する権限を共有または削除できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: e54142e189cd4f407161401203a7f13c752ad404
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 13%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront Planning. This article describes the levels of access that users could have to Adobe Workfront Planning. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Adobe Workfront Planning での共有権限の概要

{{maestro-important-intro}}

Adobe Workfront Planning で、ワークスペースまたはビューに対する権限を共有または削除できます。

この記事では、Workfront Planning オブジェクトの権限レベルについて説明します。

ワークスペースまたはビューの共有方法については、次の記事を参照してください。

* [ワークスペースの共有](/help/quicksilver/maestro/access/share-workspaces.md)

* [ビューの共有](/help/quicksilver/maestro/access/share-views.md)

## Adobe Workfront Planning で共有できるオブジェクト

次のオブジェクトを共有できます。

* ワークスペース

  ワークスペースを共有すると、ワークスペースに関連付けられているすべてのレコードタイプ、レコード、フィールドも共有されます。 ビューは共有されません。

* ビュー

## Adobe Workfront Planning でのオブジェクトの共有に関する考慮事項

* Adobe Workfrontのライセンスの種類は、Workfront Planning 権限と組み合わせて、Workfront Planning を使用する際に、オブジェクトの表示、投稿、管理に対するアクセス権を付与します。

  ライセンスの種類がWorkfront Planning の権限レベルに与える影響について詳しくは、 [Adobe Workfront Planning を使用する際のライセンスタイプの概要](/help/quicksilver/maestro/access/license-type-overview.md).
* システム管理者は、他のユーザーが作成したワークスペースを管理および共有できます。
* システム管理者でない場合は、他のユーザーが作成したワークスペース（共有している場合）に投稿できます。
* ワークスペースを一括で共有することはできません。
* ワークスペースまたはビューを次のエンティティと共有できます。
   * ユーザー
   * グループ
* システム管理者を含む他のユーザーは、自分が作成したビューまたは自分と共有されているビューにのみアクセスできます。 システム管理者には、ビューを管理する権限のみを与えることができます。
* ワークスペースへのリンクや、レコードタイプのページからのビューへのリンクを他のユーザーと共有できます。 リンクを受け取ったユーザーが、選択したビューに表示されるワークスペースまたはレコードタイプのページにアクセスできるようにするには、アクティブユーザーであり、Workfrontにログインする必要があります。

## Adobe Workfront Planning オブジェクトに対する権限の共有

次の節の表では、ワークスペースやビューを共有する際に選択できる権限のレベルと、各レベルで許可される機能を示します。

>[!IMPORTANT]
>
>一部のユーザーが以下に説明する権限レベルを持つことはできません。 ユーザーの個々のライセンスは、Workfront Planning オブジェクトに対して受け取る権限のレベルを決定します。
>
>詳しくは、 [Adobe Workfront Planning を使用する際のライセンスタイプの概要](/help/quicksilver/maestro/access/license-type-overview.md).


### Workspace 権限

|        | 管理 | 参加 | ビュー |
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

レコード権限は、ワークスペースに権限を付与すると継承されます。

|        | 管理 | 参加 | 表示 |
|--------|--------|------------|-------|
| 作成 | ✓ |            |       |
| 削除 | ✓ | ✓ |       |
| 編集 | ✓ | ✓ |       |
| 表示 | ✓ | ✓ | ✓ |

### フィールド権限

ワークスペースに権限を付与すると、フィールド権限が継承されます。
次の権限は、各フィールドに関連付けられた値ではなく、フィールド自体を参照します。 フィールド値を編集するには、レコードを編集する権限が必要です。

|        | 管理 | 参加 | 表示 |
|--------|--------|------------|-------|
| 作成 | ✓ |            |       |
| 削除 | ✓ |            |       |
| 編集 | ✓ |            |       |
| 表示 | ✓ | ✓ | ✓ |


### 権限を表示

ビューを記録するには、別の権限を付与する必要があります。 ワークスペースに権限を付与しても、ワークスペースのレコードビューに対する権限は付与されません。

|        | 管理 | 表示 |
|--------|--------|-------|
| 編集 | ✓ |       |
| 削除 | ✓ |       |
| 表示 | ✓ | ✓ |
| 適用 | ✓ | ✓ |
