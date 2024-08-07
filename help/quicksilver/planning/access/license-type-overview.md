---
title: Adobe Workfront Planning 使用時のライセンスタイプの概要
description: Adobe Workfront Planning へのアクセスは、オブジェクトに対する権限に加え、ライセンスタイプに応じて異なります。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: 402fb9d279fec258390535100e8f3d2c3c1b913b
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 18%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront plannint. This article describes the levels of access that users could have to Adobe Workfront Planning. -->
<!--update the title and the metadata title if Workfront Planning is NOT its own product - because the title is too generic for it being a Workfront capability-->

# Adobe Workfront Planning 使用時のライセンスタイプの概要

{{planning-important-intro}}

お使いのAdobe Workfrontのライセンスタイプは、Adobe Workfront Planning の権限と組み合わせて、次のアクセス権を付与します。

* ワークスペースの表示、投稿、または管理
* ビューの表示または管理

Workfront Planning のオブジェクトに対する権限について詳しくは、[Adobe Workfront Planning での共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)を参照してください。

## Workfront のライセンスタイプと Workfront Planning の権限の関係

次の表に、Adobe Workfrontのユーザーのライセンスタイプと、ユーザーに付与できる、そのライセンスに基づくAdobe Workfront Planning オブジェクトへの権限レベルとの関係を示します。

ワークスペースにユーザー権限を付与すると、レコードタイプ、レコード、フィールドへの権限も付与されます。


| Adobe Workfront ライセンスタイプ* | Adobe Workfront Planning で許可されている最上位の権限 |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 新規：標準 <br> または <br>現在：プラン | ユーザーはワークスペースを管理できます。 ワークスペース、レコードタイプ、レコード、フィールドを作成、編集または削除できます。 システム管理者 <br>、未作成のワークスペースを含むすべてのワークスペースに対する管理権限を持っています。 |
| 新規：Light、Contributor <br> または <br> 現在：作業、依頼者、レビュアー | ユーザーは、共有されているワークスペースに加え、それらのワークスペースのレコードタイプ、レコード、フィールドを表示できます。 <br> ユーザーは、ワークスペース、レコードタイプ、レコード、フィールドを作成、編集、削除できません。 |

*詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

### ライセンスタイプとワークスペース権限

Standard （または Plan）ライセンスを持つユーザーのみが、ワークスペースに対するContribute権限または管理権限を持つことができます。 他のすべてのライセンスタイプを持つユーザーは、自分と共有されているワークスペースに対する表示権限を持つことができます。

システム管理者は、システム内のすべてのワークスペース（作成しなかったワークスペースを含む）を表示できます。

>[!INFO]
>
>**例：**
>
>リクエスター（または新しいライセンスモデルによるコラボレータ）は、ワークスペースとそのオブジェクトに投稿または管理できません。
>
>共有ボックスには、下位レベルのライセンスを保持しているユーザーに対して、ワークスペースへの投稿またはワークスペースの管理を行う権限を付与できないことが示されます。これは、これらの権限レベルがグレー表示されているためです。
>
>![](assets/permissions-grayed-out-for-requestor-user.png)

### ライセンスタイプと表示権限

標準（またはプラン）ライセンスを持つユーザーのみが、ビューに対する管理権限を持つことができます。 他のすべてのライセンスタイプを持つユーザーは、自分と共有されたビューに対する表示権限を持つことができます。

>[!INFO]
>
>**例：**
>
>共同作業者（または依頼者とレビュー担当者）は、ビューを管理できません。 アクセス可能なビューに一時的なフィルター、並べ替え、グループ化を適用できます。
>
>共有ボックスには、下位レベルのライセンスを持つユーザーにビューを管理する権限を付与できないことが示されます。これは、これらの権限レベルがグレー表示されているためです。
>
>![](assets/permissions-grayed-out-for-reviewer-user-on-a-view.png)


<!--Replace all of the above with this:

The table below describes the relationship between the license type of a user in Adobe Workfront and the level of permissions you can grant to them to Adobe Workfront Planning objects based on that license. 

Granting a user permissions to a workspace also grants them permissions to record types, records, and fields. 

You must grant view permissions separately from workspace permissions. 


| Adobe Workfront license type*                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|New: Standard <br> or <br>Current: Plan                    | <ul><li>Users can contribute to or manage workspaces and they can manage views. They can create, edit, or delete workspaces, record types, records, fields, and views.</li> <li> System administrators have Manage permissions to all workspaces, including the ones they did not create.</li> <li> System administrators can only access views they created.</li></ul>                                                                                                                     |
|New: Light, Contributor <br> or <br>Current: Work, Requestor, Reviewer                      | <ul><li>Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces.</li> <li>Users can access views shared with them and apply temporary filters, sorts, or groupings, but they cannot modify the views. </li><li> Users cannot create, edit, or delete workspaces, record types, records, fields, or views.</li></ul>|

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->