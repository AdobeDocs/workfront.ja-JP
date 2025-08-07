---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: プロジェクトチームの管理
description: プロジェクトチームは、プロジェクトに関連付けられているユーザーで構成されます。プロジェクトチームのメンバーは、プロジェクトの「人物」セクションまたはプロジェクトの作成に使用される可能性のあるテンプレートの「人物」セクションに表示されます。
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: 89e15f6d99514e11e43e06487a4477d35a155cb0
workflow-type: tm+mt
source-wordcount: '1183'
ht-degree: 26%

---

# プロジェクトチームの管理

<!--take preview and production references out at production - August 7-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div>

-->

プロジェクトチームは、プロジェクトに関連付けられているユーザーで構成されます。詳しくは、[プロジェクトチームの概要](/help/quicksilver/manage-work/projects/planning-a-project/project-team-overview.md)を参照してください。

プロジェクトチームのメンバーは、プロジェクトの「ユーザー」セクションに表示されます。

プロジェクトテンプレートの人物セクションに表示されるユーザーは、プロジェクトがテンプレートから作成された後、プロジェクトチームになります。

次のユーザーは、プロジェクトとテンプレートの両方について、プロジェクトチームに自動的に追加されます。

* 所有者
* スポンサー
* タスクに割り当てられたユーザー
* イシューに割り当てられたユーザー（プロジェクトの場合のみ）

プロジェクトチームのユーザーは、プロジェクトに関する通知を受け取ります。 詳しくは、[ イベント通知タイプ ](/help/quicksilver/administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md) を参照してください。

プロジェクトおよびテンプレートのチームのユーザーを追加（プロジェクトに対してのみ）、削除、または更新を送信することで、ユーザーを管理できます。

## アクセス要件

+++ 展開すると、アクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>標準 </p>
    <p>プラン </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル</td> 
   <td> <p>プロジェクトとテンプレートへの編集アクセス権</p> <p>ユーザーに対する表示以上のアクセス権</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトまたはテンプレートに対する表示以上の権限</p> </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

<!--Old access: 

You must have the following access to perform the steps in this article:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p>View or higher access to Users</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*To find out what plan, license type, or access you have, contact your Workfront administrator.

## Add users to a Project Team

When you add users to the project team, they gain View permissions on the project and the tasks, issues, and documents of the project. For more information, see the article [Project Team overview](../../../manage-work/projects/planning-a-project/project-team-overview.md).

>[!TIP]
>
>Users on the Project Team are not automatically added to the resource management tools for the project.

You can add users to the project team in the following ways:

* [Automatically add users to a Project Team](#automatically-add-users-to-a-project-team) 
* [Manually add users to a Project Team](#manually-add-users-to-a-project-team)

### Automatically add users to a Project Team {#automatically-add-users-to-a-project-team}

The users that fulfill the following roles on the project are automatically added to the project team and appear  in the People section when the project is created:

* The creator of the project
* The project owner
* The project sponsor

Users are also automatically added to the project team when they are assigned to the following:

* Tasks
* Issues

### Manually add users to a Project Team {#manually-add-users-to-a-project-team}

If users that don't fulfill any role on the project want to be notified about certain updates or changes during the life of the project, you can manually add them to the project team. 

 For more information about what notifications can be enabled for users on the project team, see [Event notification types](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md). 

 <!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 

-->

## プロジェクトでのユーザーの管理

1. プロジェクト チームを管理するプロジェクトに移動します。

   >[!TIP]
   >
   >ユーザーを「人物」セクションに表示するには、タスク、イシュー、またはプロジェクトの関係者としてユーザーが割り当てられている必要があります。

1. 左側のパネルで **人物** をクリックします。

1. 「**ユーザーを追加**」をクリックします。

   **プロジェクトチームにユーザーを追加** ボックスが表示されます。

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. 「**ユーザーを追加**」ボックスで、プロジェクトチームに追加するアクティブなWorkfront ユーザーの名前の入力を開始し、リストに表示される名前をクリックします。

   複数のユーザーをプロジェクトチームに追加するには、この手順を繰り返します。ユーザーは、プロジェクトに関連付けられたグループに属している必要があります。

   >[!TIP]
   >
   >* チーム、グループ、会社または担当業務を追加してユーザーを追加することはできません。
   >* ユーザーを追加する際に、アバター、ユーザーのプライマリの役割およびメールアドレスに注目して、同名のユーザーを区別します。ユーザーを追加したときに表示するには、少なくとも 1 つの担当業務に関連付ける必要があります。
   >
   >  ユーザーがユーザーのメールを表示するには、アクセスレベルで、連絡情報の表示の設定を有効にしておく必要があります。詳しくは、[ユーザーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)を参照してください。

1. 「**追加**」をクリックします。

   ユーザーは、プロジェクトに対する表示権限を取得し、プロジェクトチームの一部として、プロジェクトに関する通知を受け取ります。

1. （オプション）担当業務がタスク、イシュー、プロジェクトの承認に追加されたときにユーザーに通知を受信させたい場合は、ユーザーの **担当業務** 列内をクリックして、承認に関連付けられる担当業務を選択します。

   ユーザーは、選択した担当業務に割り当てられた承認に関連する通知を受け取ります。

   詳しくは、記事「プロジェクトチームの概要 [ の「役割ベースの承認」の節を参照し ](/help/quicksilver/manage-work/projects/planning-a-project/project-team-overview.md) ください。

1. リストで 1 人または複数のユーザーを選択し、**削除** アイコン ![ 削除アイコン ](assets/remove-icon.png) をクリックして、チームから削除します。

1. **はい、選択したユーザーを削除** をクリックして、ユーザーを確認して削除します。

   未完了の作業アイテムからユーザーが削除され、割り当て解除される。

   詳細については、この記事の [ プロジェクトチームからユーザーを削除する際の考慮事項 ](#considerations-for-removing-users-from-a-project-team) の節を参照してください。
1. （任意）このプロジェクトの更新をユーザーに送信するには、[ すべて更新 ] をクリックしてチームの全員に更新を送信します

   または

   リストから 1 人または複数のユーザーを選択し、「**ユーザーに更新を送信**」をクリックします。

   <!--update screen shot when they fix the bug - the text above the box needs to match the OLD box, below-->

   ![ プロジェクトの「ユーザーに更新を送信」ボックス ](assets/send-update-to-user-on-project-box-2025.png)

   <!--Old UI for projects but the text above the comment box is right and matches the functionality):
   ![OLD Send update to user on a project](assets/send-update-to-user-on-project-box.png)-->

   **ユーザーに更新を送信** ボックスが開きます。

1. 次のいずれかの操作を行います。

   * 選択したユーザーの更新を追加します。
   * ロックアイコンをクリックして、会社内のユーザーに対して更新を非公開にします。
   * 同じアップデートを受け取るように追加のユーザーにタグを付けます。
   * 「**送信**」をクリックします。

   更新内容がプロジェクトの「**更新**」セクションに追加され、選択したすべてのユーザーがタグ付きユーザーとして表示されます。

   ユーザーに対して有効になっている場合はユーザーにメール通知が届き、新しい更新に関するアプリ内通知が届く場合があります。

1. （任意） **エクスポート** アイコン ![ エクスポートアイコン ](assets/export-icon.png) をクリックして、ユーザーのリストをファイルにエクスポートします

   または

   ユーザーを選択して「**書き出し** アイコンをクリックし、特定のユーザーのみを書き出します。

## テンプレートでの人物の管理

1. プロジェクト チームを管理するテンプレートに移動します。

   >[!TIP]
   >
   >人物セクションに表示するには、タスクまたはテンプレートの関係者に割り当てられたユーザーが必要です。

1. 左側のパネルで **人物** をクリックします。

1. リストから 1 人または複数のユーザーを選択し、「**削除**」をクリックしてチームから削除します。

1. **はい、選択したユーザーを削除** をクリックして、ユーザーを確認して削除します。

   ユーザーがテンプレートタスクから削除され、割り当て解除されます。

   詳細については、この記事の [ プロジェクトチームからユーザーを削除する際の考慮事項 ](#considerations-for-removing-users-from-a-project-team) の節を参照してください。

1. （オプション）ユーザーに更新を送信するには、「すべて更新」をクリックして、リストのすべてのユーザーに更新を送信します

   または

   リストで 1 人または複数のユーザーを選択し、「**更新**」をクリックします。

   <!--update screen shot for unshim production, notice the text above the box - it needs to say "Post an update to each person's profile"-->

   ![ テンプレートの「ユーザーに更新を送信」ボックス ](assets/send-update-to-user-on-template-box.png)

   **ユーザーに更新を送信** ボックスが開きます。

1. 次の操作を実行します。

   * 選択したユーザーの更新を追加します。
   * **ユーザーをタグ付け** をクリックして、同じ更新を受信する追加のユーザーをタグ付けします。
   * 「**会社に非公開**」オプションを選択して、会社内のユーザーに対して更新を非公開にします。
   * 「**送信**」をクリックします。

   更新内容は、タグ付けされた各ユーザーのプロファイルの「**更新**」セクションに追加されます。

   ユーザーに対して有効になっている場合はユーザーにメール通知が届き、新しい更新に関するアプリ内通知が届く場合があります。

1. （任意）「**エクスポート**」をクリックして、ユーザーのリストをファイルにエクスポートします

   または

   ユーザーを選択して **書き出し** をクリックし、特定のユーザーのみを書き出します。

## プロジェクトチームからユーザーを削除する際の考慮事項

プロジェクト上のユーザーの役割からユーザーを削除しても、そのユーザーはプロジェクトチームの一員に留まりす。

プロジェクトチームに送信された通知を受信しないようにするには、プロジェクトチームまたはプロジェクトの「ユーザー」セクションからユーザーを削除する必要があります。

プロジェクトのタスクまたはイシューに割り当てられているユーザーをプロジェクトチームから削除すると、そのユーザーは未完了のタスクとイシューから割り当て解除されます。この場合、タスクとイシューはワークロードバランサーの未割り当て作業エリアに戻ります。

完了したタスクと問題に割り当てられたユーザーは、プロジェクトチームから削除した後でも、タスクと問題に引き続き割り当てられます。

次のユーザーは、プロジェクトまたはテンプレートの人物セクションから削除すると、プロジェクトでの役割から削除されます。

* 未完了タスクに割り当てられたユーザー
* 未完了の問題に割り当てられたユーザー

次のユーザーは、プロジェクトまたはテンプレートの人物セクションから削除しても、プロジェクトでの役割から削除されません。

* 所有者
* スポンサー

プロジェクトチームからのユーザーの削除について詳しくは、[プロジェクトからのユーザーの削除](../../../manage-work/projects/manage-projects/remove-users-from-projects.md)を参照してください。

