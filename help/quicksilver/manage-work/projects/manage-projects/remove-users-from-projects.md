---
product-area: projects;user-management
navigation-topic: manage-projects
title: プロジェクトからユーザーを削除
description: プロジェクトの作業の完了に関与しなくなったユーザーを、プロジェクトから削除できます。
author: Alina
feature: Work Management
exl-id: 3a75c78d-faed-41cd-a0a4-59504bb981af
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 93%

---

# プロジェクトからユーザーを削除

プロジェクトの作業の完了に関与しなくなったユーザーを、プロジェクトから削除できます。プロジェクトからユーザーを削除すると、タスクとイシューの割り当て、およびプロジェクトの役割に影響を与えます。削除されたユーザーは、プロジェクトチーム宛ての通知を受信しなくなります。プロジェクトチームへの通知について詳しくは、[イベント通知タイプ](../../../administration-and-setup/manage-workfront/emails/event-notifications-available-in-wf.md)を参照してください。

プロジェクトに関連付けられているユーザーは、プロジェクトのユーザーエリアにリストされます。プロジェクトチームを表します。プロジェクトチームに関して詳しくは、[プロジェクトチームの概要](../../../manage-work/projects/planning-a-project/project-team-overview.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p> 
   <p>プラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する権限を管理</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:

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
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## ユーザーの削除が既存のタスク、イシュー、プロジェクトに与える影響

ユーザーがプロジェクトから削除されると、ユーザーが削除されたときにタスクまたはタスクが完了していたかどうかに応じて、ユーザーに割り当てられたタスクやイシューが影響を受ける場合があります。

* **ユーザーが削除された時点で項目が完了していない：**&#x200B;担当業務が既に割り当てられていた場合は、項目は担当業務に再割り当てされます。または、項目でユーザーが実行していた担当業務にその項目が割り当てられます。項目またはユーザーに担当業務が割り当てられていなかった場合は、項目を手動で再割り当てする必要があります。
* **ユーザーが削除されたときに項目が完了している：**&#x200B;削除されたユーザーの名前は、項目に残ります。
* **削除されたユーザーがプロジェクトの作成者でもある場合：**&#x200B;プロジェクトは、プロジェクトエリアの&#x200B;**担当プロジェクト**&#x200B;リストから削除されません。プロジェクトは、入力者フィールドでそのプロジェクトをフィルタリングした他のすべてのユーザーのリストから削除されます。
* **ユーザーがプロジェクト所有者またはスポンサーの場合：**&#x200B;ユーザーは、プロジェクトのスポンサーまたは所有者としての役割に留まります。

## プロジェクトおよびプロジェクトチームからユーザーを削除

ユーザーをプロジェクトチームから削除することにより、プロジェクトからユーザーを削除できます。

ユーザーがプロジェクト上の役割を果たすと、プロジェクトチームの一員になります。

プロジェクト上のユーザーの役割からユーザーを削除しても、そのユーザーはプロジェクトチームの一員に留まりす。

プロジェクトでのユーザーの役割について詳しくは、[プロジェクトチームを管理](../planning-a-project/manage-project-team.md)を参照してください。

プロジェクトチームからユーザーを削除するには、以下のように行います。

1. ユーザーを削除するプロジェクトに移動します。

1. 左側のパネルで **ユーザー** をクリックし、削除するユーザーを選択します。

1. ユーザーのリスト上部にある&#x200B;**削除**&#x200B;アイコン ![項目を削除](assets/remove-icon---x-in-circle.png) をクリックします。

1. 「**はい、選択したユーザーを削除します**」をクリックして、削除を確定します。

   ユーザーは、プロジェクトチームや、割り当てられる可能性のある未完了のタスクやイシューから、削除されます。プロジェクトチーム宛ての通知を受信しなくなります。
