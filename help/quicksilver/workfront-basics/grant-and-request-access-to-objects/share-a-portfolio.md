---
title: ポートフォリオの共有
description: ポートフォリオにアクセスする権限を持っている場合は、そのポートフォリオを他のユーザーと共有できます。
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 79643202-2d91-4028-b673-c3443b50d898
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 100%

---

# ポートフォリオの共有

Adobe Workfront 管理者は、アクセスレベルを割り当てる際に、ユーザーにポートフォリオの表示または編集のアクセス権を付与できます。ポートフォリオの編集に対するアクセス権には、プランライセンスが必要です。詳しくは、[ポートフォリオへのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)を参照してください。

付与されたアクセスレベルに加えて、ユーザーに特定のポートフォリオを共有できる別のユーザーから、そのポートフォリオを表示または管理する権限を受け取ることもできます。アクセスレベルと権限について詳しくは、[アクセスレベルと権限の連携方法](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md)を参照してください。

権限は Workfront の 1 つの項目に固有で、その項目に対してユーザーが実行できるアクションが定義されます。

## ポートフォリオの共有に関する考慮事項

以下の考慮事項に加えて、[オブジェクトの共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)も参照してください。

>[!NOTE]
>
>Workfront 管理者は、システム内のすべてのユーザーに対して、システム内のアイテムに対する権限の追加や削除を、それらのアイテムの所有者にならなくても行うことができます。

* ポートフォリオの作成者にはデフォルトで、ポートフォリオに対する管理権限があります。
* ポートフォリオは個別に共有することも、複数のポートフォリオを同時に共有することもできます。ポートフォリオの共有は、Workfront で他のオブジェクトを共有することと同じです。詳しくは、[オブジェクトの共有](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md)を参照してください。

* 表示権限や管理権限の付与は、ポートフォリオに対してのみ可能です。

  ![](assets/screen-shot-2014-01-23-at-12.45.15-pm.png)    ![](assets/screen-shot-2014-01-22-at-10.03.43-am-190x167.png)

* ポートフォリオを共有する際、デフォルトでは、ポートフォリオに関連付けられているすべての子オブジェクトに対して同じ権限が継承されます。

  Workfront のオブジェクトの階層について詳しくは、[Adobe Workfront のオブジェクトについて](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md)を参照してください。

* ポートフォリオから継承された権限は削除できます。オブジェクトから権限を削除する方法について詳しくは、[オブジェクトからの権限の削除](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md)を参照してください。

## ポートフォリオの権限

次の表には、ユーザーにポートフォリオの表示または管理を許可する際に付与できる権限が示されています。

| **アクション** | **管理** | **表示** |
|---|---|---|
| ポートフォリオの詳細の編集 | ✓ |   |
| ポートフォリオの表示 | ✓ | ✓ |
| ポートフォリオの削除 | ✓ |   |
| カスタムフォームの添付 | ✓ |   |
| カスタムフィールドの編集 | ✓ |   |
| プログラムの追加または削除&#42; | ✓ |   |
| プロジェクトの追加または削除&#42; | ✓ |   |
| プロジェクトを承認 | ✓ |   |
| ポートフォリオ最適化&#42; | ✓ |   |
| ドキュメントフォルダーを追加&#42; | ✓ | ✓ |
| ドキュメントを追加 | ✓ | ✓ |
| アップデート／コメント | ✓ | ✓ |
| 共有 | ✓ | ✓ |
| システム全体で共有 |   | ✓ |

*これらの権限は、プロジェクト、プログラム、ドキュメントなどの、他のオブジェクトに対するアクセスレベルと権限によって制御されます。
