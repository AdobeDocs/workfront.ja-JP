---
title: Adobe Workfront Planning 使用時のライセンスタイプの概要
description: Adobe Workfront Planning へのアクセスは、オブジェクトに対する権限に加え、ライセンスタイプに応じて異なります。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: 502ab27759749ed428f8adbf486e39165d61fcf0
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 51%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront plannint. This article describes the levels of access that users could have to Adobe Workfront Planning. -->
<!--update the title and the metadata title if Workfront Planning is NOT its own product - because the title is too generic for it being a Workfront capability-->

# Adobe Workfront Planning 使用時のライセンスタイプの概要

{{planning-important-intro}}

Adobe Workfront ライセンスタイプは Adobe Workfront Planning の権限と連携して機能し、ワークスペースの表示、投稿、管理へのアクセス権を付与します。<!--add more objects here when we can grant other object-specific permissions-->

すべてのライセンスタイプを持つユーザーは、Workfront Planning ビューを表示、作成、編集または管理できます。

ここでは、Workfrontで必要なライセンスの種類と、各ライセンスの種類に基づいてWorkfront Planning のワークスペースに付与される権限について説明します。

Workfront Planning の機能を使用する場合、下位レベルのライセンス・タイプを持つユーザーは作業領域へのアクセス権が制限されています。

>[!INFO]
>
>**例：**
>
>リクエスター（または新しいライセンスモデルによるコラボレータ）は、ワークスペースとそのオブジェクトに投稿または管理できません。
>
>共有ボックスには、ユーザーが下位レベルのライセンスを所有している場合、ワークスペースに参加したりワークスペースを管理したりするための権限を付与できないという表示があります。
>
>![](assets/permissions-grayed-out-for-requestor-user.png)


Workfront Planning のオブジェクトに対する権限について詳しくは、[Adobe Workfront Planning での共有権限の概要](/help/quicksilver/planning/access/sharing-permissions-overview.md)を参照してください。

## Workfront のライセンスタイプと Workfront Planning の権限の関係

次の表に、Adobe Workfrontのユーザーのライセンスタイプと、ユーザーに付与できる、そのライセンスに基づくAdobe Workfront Planning オブジェクトへの権限レベルとの関係を示します。

ワークスペースにユーザー権限を付与すると、レコードタイプ、レコード、フィールドへの権限も付与されます。


| Adobe Workfront ライセンスタイプ* | Adobe Workfront Planning で許可される権限 |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 新規：標準 <br> または <br>現在：プラン | ユーザーは、ワークスペース、レコードタイプ、レコードを作成および管理できます。<br> システム管理者には、未作成のワークスペースを含むすべてのワークスペースに対する管理権限があります。 |
| 新規：ライト <br> または <br>現在：ワーク | ユーザーは、共有ワークスペースに加え、そのワークスペースのレコードタイプとレコードを投稿および表示できます。 <br> ユーザーは、投稿権限を持つワークスペース内のレコードを作成、編集、削除できます。 |
| 新規：コントリビューター<br>または<br>現在：レビュアーまたはリクエスター | ユーザーは、共有されているワークスペースだけでなく、それらのワークスペースのレコードタイプとレコードも表示できます。<br> レコードタイプやレコードを作成、編集、削除することはできません。 |

*詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。