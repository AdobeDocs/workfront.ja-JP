---
title: Adobe Workfront Planningの使用時のライセンスタイプの概要
description: Adobe Workfront Planningへのアクセスは、オブジェクトに対する権限に加えて、ライセンスの種類によって異なります。 組織内のすべてのユーザーが、Adobe Workfront Planningを使用するための同じアクセス権と権限を持つわけではありません。 この記事では、Adobe Workfront Planningに対するユーザーのアクセス権のレベルについて説明します。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 6%

---


# Adobe Workfront Planning 使用時のライセンスタイプの概要

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Adobe Workfrontのライセンスタイプは、Adobe Workfront Planningの権限と連携して次のアクセス権を付与します。

* ワークスペースまたはレコードタイプの表示、投稿、管理
* ビューの表示または管理。<!--<span class="preview">and records</span>-->

Workfront Planning のオブジェクトに対する権限について詳しくは、[Adobe Workfront Planning での共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)を参照してください。

Workfront Planningへのアクセスについて詳しくは、[Adobe Planningへのアクセスの概要](/help/quicksilver/planning/access/access-overview.md)を参照してください。

## Workfront のライセンスタイプと Workfront Planning の権限の関係

次の表は、Adobe Workfrontのユーザーのライセンスタイプと、そのライセンスに基づいてAdobe Workfront Planning オブジェクトに付与できる権限レベルの関係を示しています。

ユーザー権限をワークスペースに付与すると、レコードタイプ、レコード、フィールドに対する権限も付与されます。

ユーザーがビューにアクセスして管理できるようにするには、ワークスペース用の権限に加えて、ビューに対する個別の権限をユーザーに付与する必要があります。

レコードタイプの権限を使用する場合は、次の点を考慮してください。

* ユーザーは、ワークスペースからレコードタイプの権限を自動的に継承します。
* ユーザーがワークスペースに対する管理権限を持っている場合、レコードタイプに対するアクセス権を減らすことはできません。
* ユーザーは、レコードタイプが属するワークスペースに対して持っている権限よりも、レコードタイプに対して大きな権限を持つことはできません。
* レコードタイプに対するユーザーの権限を削除しても、ワークスペース内のすべてのレコードタイプに対する表示アクセス権は削除されません。これは、ワークスペースに対するユーザーの権限が削除されないためです。

| Adobe Workfront ライセンスタイプ | Adobe Workfront Planningで許可される最高の権限 |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 標準 | <p>ユーザーは、ワークスペース、レコードタイプ、<!--<span class="preview">records</span>-->およびビューを管理できます。 ワークスペース、レコードタイプ、レコード、フィールド、ビューを作成、編集、削除できます。</p><br><p>システム管理者は、作成しなかったワークスペースを含め、すべてのワークスペースに対して管理権限を持っています。</p> |
| LightまたはContributor | <p>ユーザーは、共有されているワークスペースと、それらのワークスペースのレコードタイプ、レコード、フィールドを表示できます。</p> <br> <p>ユーザーは自分と共有したビューを表示できますが、自分でビューを作成することはできません。 </p><br> <p>ユーザーは、ワークスペース、レコードタイプ、レコード、フィールドを作成、編集、削除できません。</p> |

<!--
Old: 
*Workfront Planning is not available for legacy Workfront licenses. 
For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
-->


### ワークスペースとレコードタイプに対するライセンスタイプと権限

標準ライセンスを持つユーザーのみが、ワークスペースおよびレコードタイプに対するContributeまたはManage権限を持つことができます。 ワークスペースおよびレコードタイプに対するContribute権限とManage権限も、レコードおよびフィールドに転送されます。

システム管理者は、作成しなかったワークスペースを含め、システム内のすべてのワークスペースを表示できます。

他のすべてのライセンスタイプを持つユーザーは、ワークスペースと共有されているレコードタイプ、およびレコードやフィールドに対して表示権限を持つことができます。


>[!INFO]
>
>**例：**
>
>コントリビューターまたはライトライセンスのユーザーは、ワークスペースとそのオブジェクトにコントリビューターを割り当てたり、管理したりすることはできません。
>
>共有ボックスには、ユーザーが下位レベルのライセンスを保持している場合に、ワークスペースに対して貢献または管理する権限をユーザーに付与できないという表示があります。これらの権限レベルはグレー表示されます。
>
>![&#x200B; ワークスペース上のコントリビューターユーザーの権限がグレー表示される](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)


### ライセンスの種類と表示の権限

標準ライセンスを持つユーザーのみが、ビューに対する管理権限を持つことができます。

システム管理者は、作成しなかったビューにアクセスできません。 それらを共有する必要があります。

他のすべてのライセンスタイプを持つユーザーは、共有されたビューに対する表示権限を持つことができます。

>[!INFO]
>
>**例：**
>
>コントリビューターまたはライトライセンスユーザーは、ビューを管理できません。 ユーザーがアクセスできるビューに、一時的なフィルター、並べ替え、またはグループ化を適用することができます。
>
>共有ボックスには、ユーザーが下位レベルのライセンスを保持している場合、これらの権限レベルがグレー表示されるため、ビューを管理するための権限をユーザーに付与できないという表示があります。
>
>![&#x200B; ビュー共有のライトユーザーの権限がグレー表示される](assets/permissions-grayed-out-for-light-user.png)
