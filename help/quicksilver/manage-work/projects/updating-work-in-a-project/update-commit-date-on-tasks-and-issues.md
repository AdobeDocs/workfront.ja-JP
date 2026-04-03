---
product-area: projects
navigation-topic: update-work-in-a-project
title: タスクと問題に関するコミット日の更新
description: 割り当てられたタスクやイシューのコミット日は手動で更新できます。Adobe Workfront でのコミット日について詳しくは、「コミット日の概要」を参照してください。
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '599'
ht-degree: 50%

---


# タスクやイシューのコミット日の更新

<!--Audited: 07/2024-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>
-->

割り当てられたタスクやイシューのコミット日は手動で更新できます。Adobe Workfront でのコミット日について詳しくは、[コミット日の概要](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)を参照してください。

## アクセス要件

<!--Audited: 01/2024-->

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
   <td> 
   <ul>
   <li><p>タスクの標準</p> </li>
   <li><p>イシューの場合は Contributor 以上</p></li>
   </ul>
   <p>または</p>
<ul>
   <li><p>タスクの場合はワーク以上</p></li> 
   <li><p>イシューの場合はリクエスト以上</p></li>
</ul>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>タスクおよびイシューに対する編集アクセス権</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクまたはイシューの管理権限</p>
   <p> コミット日を更新するには、タスクまたはイシューに割り当てられる必要があります </p>
    </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--
Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> 
   New:
   <ul>
   <li><p>Standard for tasks</p> </li>
   <li><p>Contributor or higher for issues</p></li>
   </ul>
   Current:
<ul>
   <li><p>Work or higher for tasks</p></li> 
   <li><p>Request or higher for issues</p></li>
</ul>

   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Issues</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions on the task or issue</p>
   <p> You must be assigned to the task or issue to update the commit date </p>
    </td> 
  </tr> 
 </tbody> 
</table>
-->

## 前提条件

タスクまたはイシューのコミット日を編集するには、タスクまたはイシューのコミット日を更新する必要があるタスクまたはイシューに割り当てる必要があります。

## タスクやイシューのコミット日の更新


Workfrontの次の領域で、タスクまたはイシューのコミット日を更新できます。

* タスクまたは問題の詳細セクション
* タスクまたはイシューのヘッダー

  Workfrontまたはグループ管理者は、レイアウトテンプレートのタスクまたはイシューのヘッダーにコミット日を追加して、タスクまたはイシューのページから表示する必要があります。
詳しくは、[レイアウトテンプレートを使用してオブジェクトヘッダーをカスタマイズ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)を参照してください。

コミット日の更新は、タスクとイシューで同じです。

>[!NOTE]
>
>システム管理者またはグループ管理者に、Workfrontの様々な領域で簡単に更新できるように、「コミット日」フィールドを概要パネルに追加するように依頼できます。
>
>詳しくは、次の記事を参照してください。
>
>* [概要](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [ レイアウトテンプレートを使用して概要パネルをカスタマイズする](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)。


1. 自分が&#x200B;**所有者**&#x200B;として割り当てられているタスクまたはイシューに移動します。

   タスクやイシューのタスク所有者の確認方法について詳しくは、[タスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md)の記事で[タスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments)の節を参照してください。

1. （条件付きとオプション）Workfrontまたはグループ管理者がコミット日をタスクまたはイシューのヘッダーに追加した場合は、ヘッダーの「**コミット日**」フィールドをクリックし、カレンダーから日付を選択します。 コミット日がヘッダーにない場合は、次の手順に進みます。

   ![ タスクヘッダーのコミット日](assets/commit-date-task-header.png)

1. 左側のパネルで「**タスクの詳細**」または「**イシューの詳細**」をクリックします。
1. 「**概要**」をクリックして展開します。
1. 「**コミット日**」フィールドを更新します。

   詳細ページで![ タスクのコミット日の編集がハイライト表示されている](assets/task-commit-date-edit-highlighted-details-page.png)

1. 「**変更を保存**」をクリックします。

   この変更を行うと、次のようになります。

   * タスクまたはイシューのコミット日と予定完了日が同じになります。

     代わりに、コミット日と、タスクまたはイシューの見込み完了日が同じになります。

     ![ タスクの予定完了日（詳細が強調表示されている） ](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * プロジェクト所有者には、タスクまたは問題の新しいコミット日が提案されたことをWorkfront アプリ内通知で通知します。
   * プロジェクト所有者には、「更新」セクションで新しいコミット日を提案したことが通知され、この時点で、タスクまたは問題の予定完了日を、提案したコミット日と一致するように更新できます。

     ![ コミット日がプロジェクトのタイムラインに影響する更新ストリームのプロジェクト所有者の通知](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)


     <!--![Project owner notification in update stream that commit date affects the project timeline](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)-->

     この変更によってトリガーされる通知と更新について詳しくは、[コミット日の概要](/help/quicksilver/manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)の記事で「コミット日の変更でトリガーされる通知と更新」の節を参照してください。

<!--at the Production update stream when removing legacy - replace the last bullet with: The Project Owner is notified in the Systems Activity and the All tabs of the Updates section that you have suggested a new Commit Date. They can then update the Planned Completion Date accordingly by editing the task or the issue.-->
