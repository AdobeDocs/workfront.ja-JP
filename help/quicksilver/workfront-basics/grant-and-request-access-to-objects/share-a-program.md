---
title: プログラムの共有
product-area: projects
keywords: 共有，プログラム，権限
navigation-topic: grant-and-request-access-to-objects
description: Adobe Workfront管理者は、アクセスレベルを割り当てる際に、プログラムの表示や編集のアクセス権を付与できます。 プログラムを編集するには、プランライセンスが必要です。
author: Alina
feature: Get Started with Workfront
exl-id: bfa6ce97-24ad-44b3-9c2f-7fac6b748f94
source-git-commit: e608cf5bdb0227ea5b8d3109db411e98145aaa38
workflow-type: tm+mt
source-wordcount: '368'
ht-degree: 1%

---

# プログラムの共有

Adobe Workfront管理者は、アクセスレベルを割り当てる際に、プログラムの表示や編集のアクセス権を付与できます。 プログラムを編集するには、プランライセンスが必要です。 詳しくは、 [プログラムへのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md).

自分が付与されているアクセスレベルに加えて、自分と共有できるユーザーから特定のプログラムを表示または管理する権限を受け取ることもできます。 アクセスレベルと権限の詳細については、 [アクセスレベルと権限の連携](../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md).

権限は、Workfrontの各項目に固有で、ユーザーがその項目に対して実行できるアクションを定義します。

## プログラムの共有に関する考慮事項

以下の考慮事項に加えて、 [オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

>[!NOTE]
>
>Workfront管理者は、システム内のすべてのユーザーに対して、それらの項目の所有者にならずに、システム内の項目に対する権限を追加または削除できます。

* プログラムの作成者には、デフォルトで、プログラムに対する管理権限が付与されています。

* プログラムは個別に共有することも、一度に複数共有することもできます。

   Workfrontでの項目の共有について詳しくは、 [オブジェクトの共有](../../workfront-basics/grant-and-request-access-to-objects/share-an-object.md).

* プログラムに対する表示または管理の権限のみ付与できます。

   ![](assets/screen-shot-2014-01-23-at-12.45.15-pm.png)    ![](assets/screen-shot-2014-01-22-at-10.03.43-am-190x167.png)

* プログラムを共有する場合、ユーザーは、デフォルトでは、プログラムに関連付けられているすべての子オブジェクトに同じ権限を継承します。

   Workfrontのオブジェクトの階層について詳しくは、 [Adobe Workfrontのオブジェクトについて](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

* 継承された権限をプログラムから削除できます。 オブジェクトから権限を削除する方法について詳しくは、  [オブジェクトから権限を削除](../../workfront-basics/grant-and-request-access-to-objects/remove-permissions-from-objects.md).

## プログラム権限

次の表に、ユーザーがプログラムの表示や管理を許可する際に付与できる権限を示します。

| **アクション** | **管理** | **ビュー** |
|---|---|---|
| プログラムの詳細を編集 | ✓ |   |
| プログラムの表示 | ✓ | ✓ |
| プログラムの削除 | ✓ |   |
| カスタムフォームの添付 | ✓ |   |
| カスタムフィールドの編集 | ✓ |   |
| プロジェクトを追加または削除する&#42; | ✓ |   |
| プロジェクトを承認 | ✓ |   |
| ドキュメントフォルダーを追加&#42; | ✓ | ✓ |
| ドキュメントを追加 | ✓ | ✓ |
| 更新/コメントを追加 | ✓ | ✓ |
| 共有 | ✓ | ✓ |
| システム全体で共有 |   | ✓ |

*これらの権限は、プロジェクトなどの他のオブジェクトに対するアクセスレベルおよび権限によって制御されます。 
