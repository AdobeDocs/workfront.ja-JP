---
title: Adobe Workfront Planning 使用時のライセンスタイプの概要
description: Adobe Workfront Planning へのアクセス権は、オブジェクトへの権限だけでなく、ライセンスの種類にも依存します。 Adobe Workfront Planning を使用する際、組織内のすべてのユーザーが同じアクセス権と権限を持っているわけではありません。 この記事では、Adobe Workfront Planning に対して実行できるアクセスレベルについて説明します。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: 1c2303fe2cea51e3339335c433d2be6475949cb1
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 9%

---


# Adobe Workfront Planning 使用時のライセンスタイプの概要

{{planning-important-intro}}

お使いのAdobe Workfrontのライセンスタイプは、Adobe Workfront Planning の権限と組み合わせて、次のアクセス権を付与します。

* ワークスペースの表示、投稿、または管理
* ビューの表示または管理

Workfront Planning のオブジェクトに対する権限について詳しくは、[Adobe Workfront Planning での共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)を参照してください。

Workfront Planning へのアクセスについて詳しくは、[Adobe計画へのアクセスの概要 ](/help/quicksilver/planning/access/access-overview.md) を参照してください。

## Workfront のライセンスタイプと Workfront Planning の権限の関係

次の表に、Adobe Workfrontのユーザーのライセンスタイプと、ユーザーに付与できる、そのライセンスに基づくAdobe Workfront Planning オブジェクトへの権限レベルとの関係を示します。

ワークスペースにユーザー権限を付与すると、レコードタイプ、レコード、フィールドへの権限も付与されます。

ビューにアクセスして管理できるようにするには、ワークスペースに対する権限に加えて、ユーザーにビューへの個別の権限を付与する必要があります。

| Adobe Workfront ライセンスタイプ* | Adobe Workfront Planning で許可されている最上位の権限 |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 標準 | <p>ユーザーは、ワークスペースとビューを管理できます。 ワークスペース、レコードタイプ、レコード、フィールドおよびビューを作成、編集または削除できます。</p> <br> <p>システム管理者には、未作成のワークスペースを含むすべてのワークスペースに対する管理権限があります。</p> |
| ライトまたはコントリビューター | <p>ユーザーは、共有されているワークスペースに加え、それらのワークスペースのレコードタイプ、レコード、フィールドを表示できます。</p> <br> <p>ユーザーは、共有されたビューを表示できますが、独自のビューを作成することはできません。 </p><br> <p>ユーザーは、ワークスペース、レコードタイプ、レコード、フィールドを作成、編集、削除できません。</p> |

*Workfront Planning は、従来のWorkfront ライセンスでは使用できません。
詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。


<!--OLD 

| Adobe Workfront license type*                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|New: Standard <br> or <br>Current: Plan                    | Users can manage workspaces. They can create, edit, or delete workspaces, record types, records, and fields. <br> System administrators have Manage permissions to all workspaces, including the ones they did not create.                                                                                                                     |
| New: Light, Contributor <br> or <br>Current: Work, Requestor, Reviewer                      | Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces. <br> Users cannot create, edit, or delete workspaces, record types, records, or fields.|

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
-->

### ライセンスタイプとワークスペース権限

Standard ライセンスを持つユーザーのみが、ワークスペースに対するContribute権限または管理権限を持つことができます。 他のすべてのライセンスタイプを持つユーザーは、自分と共有されているワークスペースに対する表示権限を持つことができます。

システム管理者は、システム内のすべてのワークスペース（作成しなかったワークスペースを含む）を表示できます。

>[!INFO]
>
>**例：**
>
>コントリビューターまたはライトライセンスのユーザーは、ワークスペースとそのオブジェクトに投稿または管理することはできません。
>
>共有ボックスには、下位レベルのライセンスを保持しているユーザーに対して、ワークスペースへの投稿またはワークスペースの管理を行う権限を付与できないことが示されます。これは、これらの権限レベルがグレー表示されているためです。
>
>![](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)


### ライセンスタイプと表示権限

標準ライセンスを持つユーザーのみが、ビューに対する管理権限を持つことができます。 他のすべてのライセンスタイプを持つユーザーは、自分と共有されたビューに対する表示権限を持つことができます。

>[!INFO]
>
>**例：**
>
>コントリビューターまたはライトライセンスのユーザーは、ビューを管理できません。 アクセス可能なビューに一時的なフィルター、並べ替え、グループ化を適用できます。
>
>共有ボックスには、下位レベルのライセンスを持つユーザーにビューを管理する権限を付与できないことが示されます。これは、これらの権限レベルがグレー表示されているためです。
>
>![](assets/permissions-grayed-out-for-light-user.png)
