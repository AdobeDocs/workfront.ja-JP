---
product-area: projects
navigation-topic: approvals
title: 新規または既存の承認プロセスと作業の関連付け
description: この記事では、承認プロセスを作業項目に関連付ける方法について説明します。 承認を配達確認またはドキュメントと関連付ける方法について詳しくは、次の記事を参照してください。
author: Courtney and Alina
feature: Work Management
exl-id: 20bc2f2a-3ec7-4531-a0a8-ec54c14e15d0
source-git-commit: 7dbb9ca9b26f17710a7897e98dca109b5c886bd7
workflow-type: tm+mt
source-wordcount: '1869'
ht-degree: 0%

---

# 新規または既存の承認プロセスと作業の関連付け

この記事では、承認プロセスを作業項目に関連付ける方法について説明します。 承認を配達確認またはドキュメントと関連付ける方法について詳しくは、次の記事を参照してください。

* [自動ワークフローを使用した高度な配達確認の作成](../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md)
* [ドキュメント承認のリクエスト](../../review-and-approve-work/manage-approvals/request-document-approvals.md)

グローバルまたは単一使用の承認プロセスをAdobe Workfrontの作業項目に関連付けることができます。 次のシナリオが存在します。

* 既存のグローバル承認プロセスをプロジェクト、タスク、タスク、発行、テンプレートまたはテンプレートタスクに関連付けます。 一部のグローバル承認プロセスは、システム内のすべてのグループで使用できます。 グループレベルのグローバル承認プロセスは、特定のグループに対してのみ使用できます。
* 単一使用の承認プロセスを作成し、既存のプロジェクト、タスク、タスク、問題、テンプレートまたはテンプレートタスクに関連付けます。

>[!NOTE]
>
>この記事では、「グローバルな承認プロセス」という用語を使用して、「単一使用の承認プロセス」と区別します。 グローバルな承認プロセスは繰り返し使用できます。
>
>「グループレベルのグローバル承認プロセス」とは、特定のグループにのみ関連付けられたステータスを持つ品目に対して繰り返し使用できる承認プロセスを指します。

承認プロセスの一般情報について詳しくは、 [承認プロセスの概要](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

グローバルな承認プロセスの作成について詳しくは、 [作業項目の承認プロセスの作成](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>仕事以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>プロジェクト、タスク、問題、またはテンプレートへのアクセス権以上の編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクト、タスク、イシューまたはテンプレートに対する権限を管理します</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 承認プロセスと作業項目の関連付けに関する考慮事項

以下に説明する考慮事項に加えて、Workfrontの承認プロセスに関する一般的な考慮事項を再度参照することをお勧めします。 詳しくは、 [承認プロセスの概要](../../review-and-approve-work/manage-approvals/approval-process-in-workfront.md).

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Approvals can only be associated with the status of a project, task, or issue in Workfront.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>Each approval process corresponds with a status option in the Workfront system. When you change the status of a work item, an attached approval for that status requires the status change to be confirmed before the new status can be assigned to the item.</p> <p>(NOTE: the two drafted bullets have been moved to the approval-process-in-workfront article)</p> </li>
  -->

* 承認プロセスを関連付ける前に、プロジェクト、タスク、タスク、イシュー、テンプレートまたはテンプレートタスクを作成する必要があります。
* 通過したステータス、および現在アイテムが存在するステータスに対して承認プロセスをアイテムに添付する場合、承認プロセスはトリガーされず、承認者に通知は送信されません。

   **例：** タスクのステータスが「完了」で、「完了」ステータスに関連付けられた承認プロセスを添付した場合、承認はトリガーされません。

* アイテムの最初のステータスに承認プロセスを添付すると（タスクとプロジェクトのテンプレートを使用し、問題のキュー設定を使用し、新規タスクのプロジェクトのタスク設定を定義する）、送信された承認が取り消されると、承認プロセスは回避されます。 この場合、承認者は通知を受け取りません。

   承認の呼び出しについて詳しくは、 [承認を表示](../../review-and-approve-work/manage-approvals/view-approvals.md).

   >[!TIP]
   >
   >タスクまたはタスクの最初のステータスは [ 新規 ] です。 プロジェクトの最初のステータスは、Workfront管理者がシステムのプロジェクト環境設定で選択したステータスです。 詳しくは、 [システム全体のプロジェクト環境設定の指定](../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

* 承認プロセスとオブジェクトの関連付けは、オブジェクトの「更新」領域には記録されません。
* 承認プロセスを親タスクに関連付けることはできません。
* 承認者としてユーザー、チーム、または役割を追加しても、その承認に関連付けられたオブジェクトに対する権限は自動的には付与されません。 承認ステップがトリガーされると、オブジェクトに対する権限を受け取ります。 そうしない場合、承認を決定する前に、オブジェクトをオブジェクトと共有する必要があります。

次の節では、承認プロセスをプロジェクト、タスクまたはイシューに関連付ける様々な方法について説明します。

## グローバル承認プロセスと作業項目の関連付け {#associate-a-global-approval-process-with-a-work-item}

グローバルな承認プロセスを作業項目（プロジェクト、タスク、タスク、問題、テンプレート、テンプレートタスク）に関連付けることができます。

グローバル承認プロセスは、作業項目に関連付けられたグループまたはシステム内のすべてのグループに対して使用可能である必要があります。

>[!NOTE]
テンプレートにプロジェクト承認プロセスを添付し、テンプレートタスクにタスク承認プロセスを添付できます。 この操作を行うと、誰かがテンプレートを使用してプロジェクトを作成すると、承認プロセスがそれぞれプロジェクトまたはタスクの承認プロセスになります。 テンプレートタスクまたはテンプレートタスクに添付された単一使用の承認プロセスは、プロジェクトやタスクに対する単一使用の承認プロセスのままです。

Workfrontの管理者がシステム内のすべてのグループに対してグローバルな承認プロセスを設定する方法、およびグループ管理者がグループの承認を作成する方法について詳しくは、 [作業項目の承認プロセスの作成](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

>[!NOTE]
また、特定のニーズに合わせてグローバルな承認プロセスを変更することもできます。 詳しくは、 [特定のオブジェクトで使用するグローバル承認プロセスを変更する](#modify-a-global-approval-process-for-use-on-a-specific-object) 」を参照してください。

既存のグローバル承認プロセスをプロジェクト、タスク、タスク、発行、テンプレートまたはテンプレートタスクに関連付けるには、次の手順に従います。

1. 承認プロセスを関連付ける作業項目に移動します。
1. クリック **承認** をクリックします。

   クリックが必要になる場合があります **さらに表示**&#x200B;を選択し、「 **承認**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. ![](assets/use-existing-or-create-single-use-approvals-menus-on-pti-classic-350x50.png)

   選択した承認プロセスが表示されます。

1. を展開します。 **既存を使用** ドロップダウンメニューから既存の承認プロセスを選択します。

   ![](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

   選択した承認プロセスが表示されます。

   ![](assets/existing-approval-attached-to-task-redesigned-nwe-350x355.png)

1. 「**保存**」をクリックします。
1. （オプション）アイテムに添付した既存の承認を変更する場合は、「承認プロセスの編集」をクリックします。 これにより、グローバル承認プロセスが単一使用の承認プロセスに変更されます。 詳しくは、 [特定のオブジェクトで使用するグローバル承認プロセスを変更する](#modify-a-global-approval-process-for-use-on-a-specific-object) 」を参照してください。

## 特定のオブジェクトで使用するグローバル承認プロセスを変更する {#modify-a-global-approval-process-for-use-on-a-specific-object}

Workfront管理者またはグループ管理者が、使用するグローバルな承認プロセスを作成します。詳しくは、 [作業項目の承認プロセスの作成](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

アイテムに添付されたグローバル承認プロセスの変更は、単一使用の承認プロセスの変更と同じです。

関連付けたプロジェクト、タスクまたは問題に対する特定のニーズに合わせて、グローバルな承認プロセスを変更できます。

>[!IMPORTANT]
グローバル承認プロセスを変更すると、変更したオブジェクトでのみ使用できる単一使用の承認プロセスになります。 グローバルな承認プロセスは変更されません。
グローバル承認プロセスを変更する際は、次の制限事項を考慮してください。
* 承認プロセスは、承認プロセスを関連付けるプロジェクト、タスク、または問題に対してのみ変更されます。
* 管理者が元のグローバル承認プロセスに対して行った今後の変更は、変更したグローバル承認プロセスには反映されません。
>


項目に既に添付されている承認プロセスを変更するには、次の手順に従います。

1. プロジェクト、タスクまたはイシューにグローバルな承認プロセスを追加します。

   手順については、 [グローバル承認プロセスと作業項目の関連付け](#associate-a-global-approval-process-with-a-work-item) 」を参照してください。

   >[!IMPORTANT]
   次をクリックしていることを確認します。 **保存** 承認を追加する際に使用します。

1. グローバル承認プロセスを追加したら、 **編集**&#x200B;アイコン ![](assets/edit-icon.png) をクリックします。 このアクションにより、グローバルまたはグループレベルの承認プロセスが、単一使用の承認プロセスに変わります。
1. 既存の承認プロセスに変更を加えます。 詳しくは、 [単一使用の承認プロセスをプロジェクト、タスク、タスク、懸案事項、テンプレートまたはテンプレートタスクに関連付ける](#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task) 」を参照してください。
1. クリック **保存**&#x200B;を選択し、「 **保存** グローバル承認プロセスを、このオブジェクトでのみ使用可能な単一使用の承認プロセスに変換することを確認する場合に再度表示します。

## 単一使用の承認プロセスをプロジェクト、タスク、タスク、懸案事項、テンプレートまたはテンプレートタスクに関連付ける {#associate-a-single-use-approval-process-with-a-project-task-issue-template-or-template-task}

特定のプロジェクト、タスクまたはイシューでのみ使用する単一使用の承認プロセスを作成できます。

また、単一使用の承認プロセスをテンプレートタスクまたはテンプレートタスクに関連付けて、テンプレートから作成されたプロジェクトやタスクで使用できるようにすることもできます。

>[!NOTE]
単一使用の承認プロセスを、プロジェクト、タスク、タスク、イシュー、テンプレートまたはテンプレートタスクのシステムレベルまたはグループレベルのステータスに関連付けることができます。 Workfrontのステータスについて詳しくは、 [ステータスの作成または編集](../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

この方法で承認プロセスを作成すると、ニーズに合わせてカスタム承認プロセスを作成できます。 ただし、承認プロセスは、将来の他の作業項目と関連付けることはできません。

または、特定の品目のグローバル承認プロセスを変更し、そのプロセスを単一使用の承認プロセスにすることもできます。 詳しくは、 [特定のオブジェクトで使用するグローバル承認プロセスを変更する](#modify-a-global-approval-process-for-use-on-a-specific-object) 」を参照してください。

単一使用の承認プロセスを作成するには：

1. 承認プロセスを関連付けるプロジェクト、タスク、タスク、タスク、テンプレート、またはテンプレートタスクに移動します。
1. クリック **承認** をクリックします。

   クリックが必要になる場合があります **さらに表示** > **承認**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. クリック **単一使用を作成**.

   ![](assets/pti-approval-menus-to-attach-existing-or-single-use-approval-redesigned-nwe-350x115.png)

1. この記事の「作業項目のシステムレベルまたはグループレベルのグローバル承認プロセスの作成」の手順 6 から始まる手順を実行します [作業項目の承認プロセスの作成](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: overtime, ensure step 6 is still accurate here)&nbsp;</p>
   -->

   >[!TIP]
   単一使用の承認プロセスを添付すると、「`<Custom>`」と入力します。 テンプレートまたはテンプレートタスクの編集について詳しくは、次の記事を参照してください。
   * [プロジェクトテンプレートの編集](../../manage-work/projects/create-and-manage-templates/edit-templates.md)
   * [テンプレートタスクの編集](../../manage-work/projects/create-and-manage-templates/edit-template-task.md)


   <!--
   ><p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be removed when they bring the new Edit Template/ Template Task boxes to NWE) </p>   >
   -->

## 作業項目から承認プロセスを削除する

グローバルまたはグループレベルの承認プロセスを削除したり、以前に関連付けられていたプロジェクト、タスクまたはイシューから単一使用の承認プロセスを削除したりできます。

次のシナリオが存在します。 

* グローバルまたはグループレベルの承認プロセスを削除しても、承認は削除されません。 承認は、今後も使用できます。
* 1 人のユーザーの承認プロセスを削除すると、Workfrontからそのプロセスが削除され、復元できなくなります。

作業項目から承認プロセスを削除するには、次の手順に従います。

1. 以前に追加した承認プロセスを削除するプロジェクト、タスク、タスク、イシュー、テンプレート、またはテンプレートタスクに移動します。
1. クリック **承認** をクリックします。

   クリックが必要になる場合があります **さらに表示** > **承認**.

   ![](assets/approvals-section-on-task-highlighted-nwe-350x246.png)

1. 項目に関連付けられている承認のタイプに応じて、「承認」セクションの右上隅にある次のアイコンの 1 つをクリックします。

   * **削除**&#x200B;アイコン ![](assets/remove-icon---x-in-circle.png) グローバルまたはグループレベルの承認用。
   * **削除**&#x200B;アイコン ![](assets/delete.png) 単一使用承認用。

1. クリック **削除** または **削除** をクリックして確定します。

   承認プロセスが作業項目から削除されます。

## 承認プロセスと作業項目を自動的に関連付ける

次のワークフローを使用して、承認プロセスを作業項目に自動的に関連付けることができます。

* プロジェクトとタスクの場合、テンプレートを使用して承認プロセスを関連付けることができます。 既存の承認プロセスを「テンプレート承認」タブまたは「テンプレートタスク承認」タブに添付できます。 既存の承認と作業項目の関連付けについて詳しくは、 [グローバル承認プロセスと作業項目の関連付け](#associate-a-global-approval-process-with-a-work-item) 」を参照してください。
* 既存のプロジェクトの新規タスクの場合は、「プロジェクトを編集」ボックスの「タスク設定」領域で、グローバル承認プロセスまたはグループレベルのグローバル承認プロセスを関連付けることができます。 詳しくは、この記事の「タスク設定」の節を参照してください [プロジェクトを編集](../../manage-work/projects/manage-projects/edit-projects.md).
* イシューの場合、既存の承認プロセスをリクエストキューに関連付けることで、プロジェクトに追加されるすべての新しいイシューに承認を関連付けることができます。 リクエストキューの設定について詳しくは、 [リクエストキューの作成](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).
