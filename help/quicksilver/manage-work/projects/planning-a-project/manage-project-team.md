---
product-area: projects;agile-and-teams
navigation-topic: plan-a-project
title: プロジェクトチームの管理
description: プロジェクトチームは、プロジェクトに関連付けられているユーザーで構成されます。プロジェクトチームのメンバーは、プロジェクトの「ユーザー」セクションに表示されます。
author: Alina
feature: Work Management, Projects
role: User
exl-id: 6e8036fc-feda-4277-9502-0b973028fccb
source-git-commit: 4041d61ada0be7195b3af3260d419a686e1ada4a
workflow-type: ht
source-wordcount: '684'
ht-degree: 100%

---

# プロジェクトチームの管理

プロジェクトチームは、プロジェクトに関連付けられているユーザーで構成されます。プロジェクトチームのメンバーは、プロジェクトの「ユーザー」セクションに表示されます。

## アクセス要件

<!--drafted for P&P:
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
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p>
    </td> 
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
-->

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> <p>ユーザーに対する表示以上のアクセス権</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトの表示またはそれ以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

## プロジェクトチームへのユーザーの追加

プロジェクトチームに追加されたユーザーには、プロジェクトおよびプロジェクトのタスク、イシュー、ドキュメントに対する表示権限が付与されます。詳しくは、[プロジェクトチームの概要](../../../manage-work/projects/planning-a-project/project-team-overview.md)を参照してください。

>[!TIP]
>
>プロジェクトチームのユーザーは、プロジェクトのリソース管理ツールに自動的には追加されません。

次の方法でプロジェクトチームにユーザーを追加できます。

* [プロジェクトチームへのユーザーの自動追加](#automatically-add-users-to-a-project-team)
* [プロジェクトチームへのユーザーの手動追加](#manually-add-users-to-a-project-team)

### プロジェクトチームへのユーザーの自動追加 {#automatically-add-users-to-a-project-team}

プロジェクトで以下の役割を果たすユーザーは、プロジェクトチームに自動的に追加され、プロジェクトの作成時に「ユーザー」セクションに表示されます。

* プロジェクトの作成者
* プロジェクト所有者
* プロジェクトスポンサー

次の項目に割り当てられたユーザーは、プロジェクトチームにも自動的に追加されます。

* タスク
* イシュー

### プロジェクトチームへのユーザーの手動追加 {#manually-add-users-to-a-project-team}

プロジェクト上で何の役割も果たさないユーザーが、プロジェクトの期間中に特定の更新や変更に関する通知を受け取りたい場合は、手動でプロジェクトチームに追加できます。

プロジェクトチームのユーザーに対して有効にできる通知の詳細については、[Adobe Workfront で使用可能なイベント通知](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)を参照してください。

<!--drafted - this used to be the case, in the note below but this limitation was removed on Jan 5, 2023 - as a patch, not a release feature:

>[!IMPORTANT]
>
>You can add to the Project Team only users that belong to the Group associated with the project. You cannot add users that belong to the Subgroups of the project's group. 

-->

1. ユーザーを追加するプロジェクトに移動します。

1. 左のパネルで&#x200B;**ユーザー**&#x200B;をクリックします。最初に&#x200B;**さらに表示**&#x200B;をクリックする必要がある場合もあります。

1. 「**ユーザーを追加**」をクリックします。

   プロジェクトチームにユーザーを追加ダイアログボックスが表示されます。

   ![add_users_dialog.png](assets/add-users-dialog-350x217.png)

1. 「**ユーザーを追加**」ボックスに、プロジェクトチームに追加するアクティブな Workfront ユーザーの名前を入力し始め、ドロップダウンリストに表示されたら名前をクリックします。

   複数のユーザーをプロジェクトチームに追加するには、この手順を繰り返します。ユーザーは、プロジェクトに関連付けられたグループに属している必要があります。

   >[!TIP]
   >
   >* チーム、グループ、会社または担当業務を追加してユーザーを追加することはできません。
   >* ユーザーを追加する際に、アバター、ユーザーのプライマリの役割およびメールアドレスに注目して、同名のユーザーを区別します。ユーザーを追加したときに表示するには、少なくとも 1 つの担当業務に関連付ける必要があります。
   >
   >  ユーザーがユーザーのメールを表示するには、アクセスレベルで、連絡情報の表示の設定を有効にしておく必要があります。詳しくは、[ユーザーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)を参照してください。


1. 「**追加**」をクリックします。

   ユーザーは、プロジェクトに対する表示権限を取得し、プロジェクトチームの一部として、プロジェクトに関する通知を受け取ります。

## プロジェクトチームからのユーザーの削除

プロジェクト上のユーザーの役割からユーザーを削除しても、そのユーザーはプロジェクトチームの一員に留まりす。

プロジェクトのタスクまたはイシューに割り当てられているユーザーをプロジェクトチームから削除すると、そのユーザーは未完了のタスクとイシューから割り当て解除されます。この場合、タスクとイシューはワークロードバランサーの未割り当て作業エリアに戻ります。

完了したタスクとイシューに割り当てられているユーザーをプロジェクトチームから削除しても、割り当てられたままになります。

プロジェクトチームからのユーザーの削除について詳しくは、[プロジェクトからのユーザーの削除](../../../manage-work/projects/manage-projects/remove-users-from-projects.md)を参照してください。
