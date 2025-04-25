---
product-area: projects
navigation-topic: update-work-in-a-project
title: タスクおよび問題のコミット日の更新
description: 割り当てられたタスクやイシューのコミット日は手動で更新できます。Adobe Workfront でのコミット日について詳しくは、「コミット日の概要」を参照してください。
author: Alina
feature: Work Management
exl-id: 003c52c7-baf3-4316-bb4b-83b600172d48
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 51%

---


# タスクやイシューのコミット日の更新

<!--Audited: 07/2024-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers, or in the Production environment for customers who enabled fast releases.</span>

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

<span class="preview">For information about the current release, see [Third Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>-->

割り当てられたタスクやイシューのコミット日は手動で更新できます。Adobe Workfront でのコミット日について詳しくは、[コミット日の概要](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)を参照してください。

## アクセス要件

<!--Audited: 01/2024-->

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> 
   新規：
   <ul>
   <li><p>タスクの標準</p> </li>
   <li><p>イシューの場合は Contributor 以上</p></li>
   </ul>
   現在：
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
   <p> コミット日を更新するには、タスクまたは問題に割り当てられている必要があります </p>
    </td> 
  </tr> 
 </tbody> 
</table>

* 詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

タスクまたは問題のコミット日を編集する前に、コミット日を更新する必要があるタスクまたは問題に割り当てる必要があります。

## タスクやイシューのコミット日の更新


Workfrontの次の領域で、タスクまたはイシューのコミット日を更新できます。

* タスクまたは問題の「詳細」セクション
* タスクまたはイシューのヘッダー

  Workfront管理者またはグループ管理者は、レイアウトテンプレートのタスクまたはイシューヘッダーにコミット日を追加して、タスクまたはイシューページから表示する必要があります。
詳しくは、[レイアウトテンプレートを使用してオブジェクトヘッダーをカスタマイズ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)を参照してください。

コミット日の更新は、タスクとイシューで同じです。

>[!NOTE]
>
>システム管理者またはグループ管理者に依頼して、「コミット日」フィールドを概要パネルに追加し、Workfrontの様々な領域で更新しやすくすることができます。
>
>詳しくは、次の記事を参照してください。
>
>* [ 概要 ](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [ レイアウトテンプレートを使用して概要パネルをカスタマイズする ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)。


1. 自分が&#x200B;**所有者**&#x200B;として割り当てられているタスクまたはイシューに移動します。

   タスクやイシューのタスク所有者の確認方法について詳しくは、[タスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md)の記事で[タスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md#assignments)の節を参照してください。

1. （条件付きおよびオプション）Workfront管理者またはグループ管理者がコミット日をタスクまたは問題ヘッダーに追加した場合は、ヘッダーの **コミット日** フィールドをクリックし、カレンダーから日付を選択します。 コミット日がヘッダーにない場合は、次の手順に進みます。

   ![](assets/commit-date-task-header.png)

1. 左側のパネルで「**タスクの詳細**」または「**イシューの詳細**」をクリックします。
1. 「**概要**」をクリックして展開します。
1. 「**コミット日**」フィールドを更新します。

   ![](assets/task-commit-date-edit-highlighted-details-page.png)

1. 「**変更を保存**」をクリックします。

   この変更を行った後、次の処理が行われます。

   * タスクまたはイシューのコミット日と予定完了日が同じになります。

     代わりに、コミット日と、タスクまたはイシューの見込み完了日が同じになります。

     ![](assets/task-projected-completion-date-in-details-highlighted-nwe-350x230.png)

   * プロジェクト所有者には、タスクまたは問題の新しいコミット日を提案したことがWorkfrontのアプリ内通知で通知されます。
   * 「更新」セクションでは、新しいコミット日が提案されたことがプロジェクト所有者に通知されます。この時点で、プロジェクト所有者はタスクまたは問題の予定完了日を提案したコミット日に一致するように更新できます。

     ![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline.png)


     <!--![](assets/project-owner-notification-update-stream-that-commit-date-affects-project-timeline-highlighted-nwe-350x139.png)-->

     この変更によってトリガーされる通知と更新について詳しくは、[コミット日の概要](/help/quicksilver/manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)の記事で「コミット日の変更でトリガーされる通知と更新」の節を参照してください。

<!--at the Production update stream when removing legacy - replace the last bullet with: The Project Owner is notified in the Systems Activity and the All tabs of the Updates section that you have suggested a new Commit Date. They can then update the Planned Completion Date accordingly by editing the task or the issue.-->
