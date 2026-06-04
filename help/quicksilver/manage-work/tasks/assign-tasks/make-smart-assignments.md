---
product-area: projects;user-management
navigation-topic: assign-tasks
title: スマート割り当ての実行
description: スマート割り当てを使用して、作業を完了するのが最適なユーザーを特定できます。 スマート割り当ては、業務に最も適したリソースを決定するアルゴリズムに基づいて作業アイテムをリソースに割り当てる際に Adobe Workfront に表示される、ユーザー、役割またはチームに関する提案です。 スマート割り当てについて詳しくは、スマート割り当ての概要を参照してください。
author: Lisa
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/0EhPmb9Y3Vus-62FzgaPy-gtb4ioBmtVwt6bf3axWXU
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b91c0848-76c4-4da4-8b81-3aade0518dd0id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 380
ht-degree: 88%

---

# スマート割り当ての実行

<!--Audited: 07/2024-->

スマート割り当てを使用して、作業の完了に最適なユーザーを特定できます。

スマート割り当ては、作業アイテムをリソースに割り当てる際に Adobe Workfront に表示される、ユーザー、役割またはチームに関する提案です。 Workfront は、業務に最も適したリソースを決定するアルゴリズムに基づいて提案します。

<!--<span class="preview">There are two separate algorithms in Workfront that calculate smart assignments that work differently for tasks and for issues.</span> -->

スマート割り当ての決定に使用される基準について詳しくは、[スマート割り当ての概要](/help/quicksilver/manage-work/tasks/assign-tasks/smart-assignments.md)を参照してください。

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
   <td> <p>標準</p>
   <p>Work またはそれ以上</p>
   </td> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>タスクおよびイシューに対する編集アクセス権</p> <p>プロジェクトに対する表示以上のアクセス権</p> </td> 
  </tr> 
  <tr> 
   <td>オブジェクト権限</td>
   <td>タスクやイシューに対する割り当てを行う権限の付与</td>
  </tr>
 </tbody>
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## スマート割り当ての実行

スマート割り当ては、Workfront で割り当てを行うほとんどの場所で使用できます。

1. 次のエリアに移動し、「**割り当て**」または「**割り当て先**」フィールドをクリックします。

   * タスクまたはイシューのリストやレポート
   * タスクまたはイシューのヘッダー
   * タスクまたはイシューの概要パネル
   * ワークロードバランサーのタスクまたはイシュー
     <!--* <span class="preview">A New Task</span> or New Issue box, as you add <span class="preview">a new task</span> or issue to a project-->

1. 「割り当て」フィールドにカーソルを置き、2秒間待ちます。

   <!--
   For issues, the smart assignments display in the following sections: 
      * **Users and teams**
      * **Job roles**
        ![Smart assignments issue header](assets/smart-assignments-issue-header.png)
        -->

   スマート割り当ては、次のセクション <!--, depending on which phase of the algorithm's calculation identified the assignments-->に表示されます。

   <!--* <span class="preview">**Suggested assignments**: Displays assignments identified in the first phase of the task smart assignment algorithm.</span> -->
   * **ユーザーとチーム**&#x200B;または&#x200B;**担当業務** <!--or **Rate card job roles**: Assignments identified in the second phase of the task smart assignment's algorithm calculation.-->

   ![ タスクリストのスマート割り当ての例](assets/smart-assignments-task-list.png)

   詳しくは、[スマート割り当ての概要](../../../manage-work/tasks/assign-tasks/smart-assignments.md)を参照してください。

1. 名前をクリックして、レコメンデーションリストのリソースを選択します。

1. （オプション）「**自分に割り当て**」をクリックして、作業アイテムを自分に割り当てます。

   >[!TIP]
   >
   >候補の提案がない場合、候補リストは開きません。

1. （オプション）スマート割り当てリストから候補ユーザーの 1 人を使用しない場合は、目的のリソースの名前を入力していき、リストに名前が表示されたらそれを選択します。
1. 「**入力**」をクリックして割り当てを行います。

   選択したユーザーがタスクまたはイシューに割り当てられます。
