---
title: AdobeMaestro での共有権限の概要
description: AdobeMaestro のワークスペースまたはビューに対する権限を共有または削除できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 811eb1453c140808b0d6c5d9a3b4a0729cb16b2d
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 8%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# AdobeMaestro での共有権限の概要

>[!IMPORTANT]
>
>この記事の情報は、Adobe Workfrontからの新しいオファーであるAdobe・マエストロを指します。
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。 Maestro にアクセスするには、Ypu がWorkfrontのお客様である必要があります。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

AdobeMaestro のワークスペースまたはビューに対する権限を共有または削除できます。

この記事では、Maestro オブジェクトの権限レベルについて説明します。

ワークスペースまたはビューの共有方法については、次の記事を参照してください。

* [ワークスペースの共有](/help/quicksilver/maestro/access/share-workspaces.md)

* [ビューの共有](/help/quicksilver/maestro/access/share-views.md)

## AdobeMaestro で共有できるオブジェクト

Maestro では、以下のオブジェクトを共有できます。

* ワークスペース

  ワークスペースを共有すると、ワークスペースに関連付けられているすべてのレコードタイプ、レコード、フィールドも共有されます。 ビューは共有されません。

* ビュー

## Maestro でのオブジェクトの共有に関する考慮事項

* Maestro でワークスペースを作成するには、次のライセンスが必要です。

   * 新しい価格モデル：標準ライセンス
   * 現行価格モデル：プラン・ライセンス。

  詳しくは、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)
* システム管理者は、他のユーザーが作成したワークスペースを管理および共有できます。
* システム管理者でない場合は、他のユーザーが作成したワークスペース（共有している場合）に投稿できます。
* ワークスペースを一括で共有することはできません。
* ワークスペースを次のエンティティと共有できます。
   * ユーザー
   * グループ
* システム管理者を含む他のユーザーは、自分が作成したビューまたは自分と共有されているビューにのみアクセスできます。

## Maestro オブジェクトに対する権限の共有

次のセクションの表に、Maestro ワークスペースまたは表示を共有する際に選択できる権限のレベルと、各レベルで許可される機能を示します。

### Workspace 権限

|        | 管理 | 貢献 | 表示 |
|--------|--------|------------|-------|
| 編集 | ✓ |            |       |
| 共有 | ✓ |            |       |
| 削除 | ✓ |            |       |
| 表示 | ✓ | ✓ | ✓ |

### レコードタイプの権限

レコードタイプの権限は、ワークスペースに権限を付与すると継承されます。

|        | 管理 | 貢献 | 表示 |
|--------|--------|------------|-------|
| 以下を作成  | ✓ |            |       |
| 削除 | ✓ |            |       |
| 編集 | ✓ |            |       |
| 表示 | ✓ | ✓ | ✓ |

### レコード権限

レコード権限は、ワークスペースに権限を付与すると継承されます。

|        | 管理 | 貢献 | 表示 |
|--------|--------|------------|-------|
| 以下を作成  | ✓ |            |       |
| 削除 | ✓ | ✓ |       |
| 編集 | ✓ | ✓ |       |
| 表示 | ✓ | ✓ | ✓ |

### フィールド権限

ワークスペースに権限を付与すると、フィールド権限が継承されます。
次の権限は、各フィールドに関連付けられた値ではなく、フィールド自体を参照します。 フィールド値を編集するには、レコードを編集する権限が必要です。

|        | 管理 | 貢献 | 表示 |
|--------|--------|------------|-------|
| 以下を作成  | ✓ |            |       |
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






