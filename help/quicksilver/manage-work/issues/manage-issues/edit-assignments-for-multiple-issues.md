---
product-area: projects
navigation-topic: manage-issues
title: リスト内の複数のイシューに対するユーザー割り当ての変更
description: リスト内の複数のイシューに対するユーザー割り当ての変更
author: Lisa
feature: Work Management
exl-id: e1e75027-1847-44cf-afeb-b19394dc3ea5
source-git-commit: 8f7249e08268a8cb784d4c0ecc8c534542fa80cf
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 40%

---

# リスト内の複数のイシューに対するユーザー割り当ての変更

<!--Audited: 07/2024-->
<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: similar article exists for tasks)</p>
-->

<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

複数のイシューに対するユーザーの割り当てを同時に変更できます。 イシューの編集または一度に 1 つずつ割り当てる方法について詳しくは、次の記事も参照してください。

* [イシューの編集](../../../manage-work/issues/manage-issues/edit-issues.md)
* [イシューの割り当て](../../../manage-work/issues/manage-issues/assign-issues.md)

イシューの割り当てに関する一般情報については、[イシューの割り当て変更の概要](../../../manage-work/issues/manage-issues/modify-issue-assignments-overview.md)を参照してください。

>[!NOTE]
>
>イシューへの割り当てを行うには、少なくとも、そのイシューへの参加権限が必要です。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td> <p>投稿者以上</p>
   <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>イシューへのアクセス権を編集</p> <p>プロジェクトおよびタスクへの表示以上のアクセス権を持ち、1 つの問題を割り当てる</p> </td> 
  </tr> 
  <tr> 
   <td>オブジェクト権限</td> 
   <td> <p>イシューに対する権限の管理</p> <p>複数のイシューを割り当てる場合は、イシューが存在するプロジェクトまたはタスクに対する権限以上を投稿します。</p>  </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>When to modify user assignments on issues</h2>
<p>(NOTE:  drafted and moved to the overview article: Modify issue assignments overview)</p>
<p>You might want to modify the user assignments for multiple issues for a variety of  reasons, including the following:</p>
<ul>
<li>Users join or leave  your team</li>
<li>A user takes a vacation that extends beyond the issue  due dates</li>
<li>A specific role or user is set as the assignee for multiple issues and you want to quickly modify all items to be assigned to a different user or role</li>
</ul>
</div>
-->

## 複数のイシューの割り当てを変更

1. 割り当てを変更する問題を含む問題リストに移動します。
1. （オプション）変更する担当者に割り当てられているイシューのみを表示するフィルターを作成します。

   例えば、特定の役割を担当者として持つ問題のみを表示するフィルターを作成できます。  次に、役割を特定のユーザーに置き換えることができます。 次の操作を実行します。

   1. 「**フィルター**」ドロップダウンリストをクリックして、「**新しいフィルター**」をクリックします。

   1. 最初のフィールドに「**割り当てられた役割**」と入力し始め、リストから **割り当てられた役割：名前** を選択します。
   1. 修飾子のドロップダウンメニューから「**次のいずれか**」を選択して、役割の名前の入力を開始し、リストに表示されたら選択します。 複数の役割を入力できます。

      >[!TIP]
      >
      >このフィールドはイシューの所有者のみを指し、すべての担当者を指すわけではないので、**割り当て先** を使用しないでください。

      イシューのリストは、フィルター条件に合わせて自動的にフィルタリングされます。
   1. （オプション）「**新規保存**」をクリックして、「**保存**」をクリックします。

1. 割り当てを変更するイシューを選択して、**編集** アイコン ![&#x200B; 編集アイコン &#x200B;](assets/qs-edit-icon.png) をクリックします。

   **イシューの編集**&#x200B;が表示されます。選択した項目の数は、ページの左上隅に表示されます。

1. 左側のパネルで **割り当て** をクリックし、削除する担当者の横にある **x** アイコンをクリックします。

   >[!TIP]
   >
   >選択したすべてのイシューに割り当てられた担当者のみが **割り当て** 領域に表示されます。

   ![&#x200B; 一括編集のイシューの「割り当て」エリア &#x200B;](assets/assignments-area-on-bulk-edit-issues.png)

1. ユーザー、役割またはチームの名前の入力を開始して、選択したすべてのイシューに担当者を追加します。

   >[!TIP]
   >
   >複数のユーザー、担当業務やチームを割り当てることができます。アクティブなユーザー、担当業務およびチームのみを割り当てることができます。
   >
   >非アクティブ化前にユーザー、担当業務やチームが、非アクティブ化される前に割り当てられた場合、ユーザー、担当業務やチームは作業アイテムに割り当てられたままになります。この場合、以下の操作をお勧めします。
   >
   >* 作業アイテムをアクティブなリソースに再割り当てする。
   >* 非アクティブ化されたチームのユーザーをアクティブなチームに関連付け、作業アイテムをアクティブなチームに再割り当てする。

   追加された担当者は、既存の担当者に追加されます。 選択した各問題の既存の設定は置き換えられません。

1. （任意）「**自分に割り当て**」をクリックして、すべてのイシューを自分に割り当てます。
1. 「**保存**」をクリックします。


   <!--Old functionality for assignments for issues - before November 2025:
   1. (Conditional) In the Production environment, do the following: 
   1. Go to the **Assignments** section, then select **Assignee**.
      ![Assignments area](assets/classic-assignmens-area-on-edit-box-350x119.png)
   1. Do one of the following:
      1. To add a new assignee:
         1. Start typing the name of a user, role, or team, then select it when it displays in the list. The assignment is added and does not replace the current assignments on the selected issues.
         >[!TIP]
         >
         >You can assign multiple users, job roles, or teams. You can assign only active users, job roles, and teams.
         >
         >If a user, job role, or a team was assigned before they were deactivated, they remain assigned to the work item. In this case, we recommend the following:
         >
         >* Reassign the work item to active resources.
         >* Associate the users in a deactivated team with an active team and reassign the work item to the active team.
          Information that is common across all issues selected displays. For example, if the same user is assigned to all issues, that user displays in the **Assignee**  column. If information is not common across the issues selected, no information displays.
      1. To remove individual assignees:
         1. Click the **X icon** next to the name of the assignee that you want to remove if the assignee displays in the Assignments list.
            Or
            If the assignee that you want to remove does not display in the Assignments section because the assignee is assigned to only some of the issues that you have selected, click **Remove Assignee** and start typing the name of the assignee that you want to remove, then click the name when it appears in the drop-down list.
         1. Click  **Remove Assignee** again to add another assignee to remove.
      1. To remove all existing assignees:
         1. Click **Remove All Existing Assignees**, then click **Yes, Delete All Assignees**.
            This removes not only common assignees (assignees that are displayed in the edit  dialog box), but also all assignees on all the selected issues.
         1. (Optional) Modify any of the following options for the assignees you selected to associate with the issues:
          * **Issue Owner:**  Select the radio button to indicate which assignee is designated as the Issues Owner. If left unselected, Adobe Workfront designates the first assignee as the Issue Owner. This is not available for team assignments. 
            * **Assignee's Role**: Select a role from the drop-down list. If left unselected, Workfront automatically selects the Primary Role of the user.
      1. Click **Save Changes**.-->




