---
title: Adobe Workfront Planning 使用時のライセンスタイプの概要
description: Adobe Workfront Planning へのアクセス権は、オブジェクトへの権限だけでなく、ライセンスの種類にも依存します。 Adobe Workfront Planning を使用する際、組織内のすべてのユーザーが同じアクセス権と権限を持っているわけではありません。 この記事では、Adobe Workfront Planning に対して実行できるアクセスレベルについて説明します。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: a3c82d8be6945a91a249d64923c6377a5edfa268
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 8%

---


# Adobe Workfront Planning 使用時のライセンスタイプの概要

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

お使いのAdobe Workfrontのライセンスタイプは、Adobe Workfront Planning の権限と組み合わせて、次のアクセス権を付与します。

* ワークスペースの表示、投稿、管理 <!--<span class="preview">or record types</span>-->
* ビューの表示または管理

Workfront Planning のオブジェクトに対する権限について詳しくは、[Adobe Workfront Planning での共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)を参照してください。

Adobe Planning へのアクセスについて詳しくは、[Workfront Planning へのアクセスの概要 ](/help/quicksilver/planning/access/access-overview.md) を参照してください。

## Workfront のライセンスタイプと Workfront Planning の権限の関係

次の表に、Adobe Workfrontのユーザーのライセンスタイプと、ユーザーに付与できる、そのライセンスに基づくAdobe Workfront Planning オブジェクトへの権限レベルとの関係を示します。

ワークスペースにユーザー権限を付与すると、レコードタイプ、レコード、フィールドへの権限も付与されます。

ビューにアクセスして管理できるようにするには、ワークスペースに対する権限に加えて、ユーザーにビューへの個別の権限を付与する必要があります。

<!--

<div class="preview">

Consider the following when working with record type permissions: 

* Users automatically inherit record type permissions from workspaces. 
* When a user has Manage permissions to a workspace, they cannot have a lesser access to record type. 
* Users cannot have greater permissions to a record type than they have for the workspace the record type belongs to.

</div>
-->

| Adobe Workfront ライセンスタイプ* | Adobe Workfront Planning で許可されている最上位の権限 |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 標準 | <p>ユーザーは、ワークスペースの <!--<span class="preview">, record types, </span> --> とビューを管理できます。 ワークスペース、レコードタイプ、レコード、フィールドおよびビューを作成、編集または削除できます。</p> <br> <p>システム管理者には、未作成のワークスペースを含むすべてのワークスペースに対する管理権限があります。</p> |
| ライトまたはコントリビューター | <p>ユーザーは、共有されているワークスペースに加え、それらのワークスペースのレコードタイプ、レコード、フィールドを表示できます。</p> <br> <p>ユーザーは、共有されたビューを表示できますが、独自のビューを作成することはできません。 </p><br> <p>ユーザーは、ワークスペース、レコードタイプ、レコード、フィールドを作成、編集、削除できません。</p> |

*Workfront Planning は、従来のWorkfront ライセンスでは使用できません。
詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。


### ワークスペースのライセンスタイプと権限

<!--should we add "record types" in the title above and to this section?-->

Standard ライセンスを持つユーザーのみが、Workspace <!--<span class="preview">and record types</span>--> に対する投稿権限または管理権限を持つことができます。 ワークスペースへの投稿権限と管理権限は、レコードタイプ、レコード、フィールドにも転送で <!--<span class="preview">and record types</span>--> ます。

<!--take "record types" out from the end of the sentence above when we release record type-level access-->

他のすべてのライセンスタイプを持つユーザーは、共有 <!--<span class="preview"> and record types </span> --> のワークスペースおよびレコードタイプ、レコード、フィールドに対する表示権限を持つことができます。

<!--take "record types" out from the end of the sentence above when we release record type-level access-->

システム管理者は、自分が作成していないものを含め、システム内のすべてのワークスペースを表示できます。

<!--does the shot below need to be replaced for record types??-->

>[!INFO]
>
>**例：**
>
>コントリビューターまたはライトライセンスのユーザーは、ワークスペースとそのオブジェクトに投稿または管理することはできません。
>
>共有ボックスには、下位レベルのライセンスを保持しているユーザーに対して、ワークスペースへの投稿またはワークスペースの管理を行う権限を付与できないことが示されます。これは、これらの権限レベルがグレー表示されているためです。
>
>![Workspace の投稿者ユーザーに対してグレー表示されている権限 ](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)


### ライセンスの種類とビューへの権限

標準ライセンスを持つユーザーのみが、ビューに対する管理権限を持つことができます。 他のすべてのライセンスタイプを持つユーザーは、自分と共有されたビューに対する表示権限を持つことができます。

>[!INFO]
>
>**例：**
>
>コントリビューターまたはライトライセンスのユーザーは、ビューを管理できません。 アクセス可能なビューに一時的なフィルター、並べ替え、グループ化を適用できます。
>
>共有ボックスには、下位レベルのライセンスを持つユーザーにビューを管理する権限を付与できないことが示されます。これは、これらの権限レベルがグレー表示されているためです。
>
>![ ビュー共有のライトユーザーで権限がグレー表示される ](assets/permissions-grayed-out-for-light-user.png)
