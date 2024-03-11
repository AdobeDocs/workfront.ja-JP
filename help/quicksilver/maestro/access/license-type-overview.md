---
title: Adobe Workfrontの計画機能を使用する際のライセンスタイプの概要
description: Adobe Workfront Planning 機能へのアクセスは、オブジェクトに対する権限に加えて、ライセンスの種類によって異なります。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 1da2e6448f7ac6f4bd5bd76846fbfc1a23c3da77
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 0%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->
<!--update the title and the metadata title if Maestro is NOT its own product - because the title is too generic for it being a Workfront capability-->

# Adobe Workfrontの計画機能を使用する際のライセンスタイプの概要

{{maestro-important-intro}}

Adobe Workfrontのライセンスの種類は、Adobe Workfrontの計画機能の権限と組み合わせて、ワークスペースやビューの表示、投稿、管理に対するアクセス権を付与します。 <!--add more objects here when we can grant other object-specific permissions-->

この記事では、必要なライセンスの種類と、各ライセンスの種類に基づいてオブジェクトに付与されるアクセスについて説明します。

下位レベルのライセンスタイプを持つユーザーは、Workfrontの計画機能を使用する際に、オブジェクトに対する権限が制限されています。

>[!INFO]
>
>**例：** 新しいライセンスモデルに従ってリクエスト担当者（または共同作業者）は、ワークスペースとそのオブジェクトに対して投稿または管理できません。
>
>共有ボックスには、ユーザーが下位レベルのライセンスを持っている場合に、ワークスペースに投稿または管理する権限をユーザーに付与できないことを示すメッセージが表示されます。
>
>![](assets/permissions-grayed-out-for-requestor-user.png)


Workfrontの計画機能でオブジェクトに対する権限について詳しくは、 [AdobeMaestro での共有権限の概要](/help/quicksilver/maestro/access/sharing-permissions-overview.md).

## Workfrontのライセンスの種類とWorkfrontの計画機能の権限との関係

次の表に、ユーザーのライセンスの種類と、そのライセンスに基づいてユーザーに付与できる権限のレベルとの関係を示します。


| ライセンスの種類 | Workfront Planning Capabilities オブジェクトで許可される権限 |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| 新規：標準 <br> または <br>現在：プラン | ユーザーは、ワークスペース、レコードタイプ、およびレコードを作成および管理できます。 |
| 新規：ライト <br> または <br>現在：作業 | ユーザーは、自分と共有しているワークスペースに加えて、そのワークスペースのレコードの種類やレコードを投稿および表示できます。  ユーザは、Contribute 権限を持つワークスペース内のレコードを作成、編集、削除できます。 |
| 新規：投稿者 <br> または <br>現在：レビュー担当者またはリクエスト元 | ユーザーは、自分と共有しているワークスペースのほか、それらのワークスペースのレコードの種類とレコードを表示できます。 レコードの種類やレコードを作成、編集、削除することはできません。 |



