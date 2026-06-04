---
product-area: projects
navigation-topic: create-tasks
title: サブタスクの作成
description: Adobe Workfrontでは、タスクは親子関係を持つことができます。 子タスクはサブタスクと呼ばれます。 メインタスクをサブタスクにすることで、タスクリストにサブタスクを作成できます。 サブタスクをメインタスクにすることもできます。
author: Alina
feature: Work Management
exl-id: 3d970794-b5ea-422f-bc92-51846cb7db35
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/FTIJQXYSmMiUcYnmU7wVnYJKBZxae8XhLcNlH-vxvZQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b91c0848-76c4-4da4-8b81-3aade0518dd0
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 580
ht-degree: 68%

---

# サブタスクを作成

<!-- Audited: 01/2025 -->

Adobe Workfrontでは、タスクは親子関係を持つことができます。 子タスクはサブタスクと呼ばれます。 メインタスクを別のタスクのサブタスクにすることで、タスクリストにサブタスクを作成できます。 サブタスクをメインタスクにすることもできます。

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
   <p>Work またはそれ以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>タスクおよびプロジェクトへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対して、タスクを追加する機能以上を持つ参加権限</p> 
   <p>タスクを作成すると、タスクに対する「権限を管理」が自動的に付与される</p> 
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
   <td role="rowheader">Adobe Workfront license</td> 
   <td> 
   <p>New: Standard</p>
   <p>Current: Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks and Projects</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Contribute permissions to the project and the parent task with ability to Add Tasks or higher</p> <p>You automatically receive Manage permissions to the task after you create it.</p>  </td> 
  </tr> 
 </tbody> 
</table>
-->

## サブタスクを作成

タスクリストまたはタスクの「サブタスク」セクションからサブタスクを作成できます。

>[!TIP]
>
>プロジェクトのサブタスクの作成は、テンプレート上のテンプレートタスクにテンプレートサブタスクを作成することと似ています。


### タスクリストからサブタスクを作成 {#create-subtasks-from-the-task-list}

1. サブタスクを作成するプロジェクトに移動します。
1. 左パネルの「**タスク**」セクションをクリックします。
1. （条件付き）子タスクを作成するタスクが、親タスクを作成するタスクの直下にない場合は、タスクリストの適切な場所にドラッグ&amp;ドロップします。
1. サブタスクにするタスクを選択し、以下のいずれかの操作を行います。

   * **インデント** アイコン ![&#x200B; インデントアイコン &#x200B;](assets/indent-icon-nwe-33x29.png)をクリックして、選択したタスクをその上のタスクのサブタスクにします。
   * 標準の英語 QWERTY キーボードを使用する場合は、キーボードの Option + >（Mac）または Alt + >（Windows）を押します。 他の言語では、Option +（Mac）または Alt +（Windows）コマンドを使用してインデントすることができます。

     >[!TIP]
     >
     >インライン編集でタスクを編集する際には、キーボードショートカットは機能しません。 この場合、インデントアイコン ![&#x200B; インデントアイコン &#x200B;](assets/indent-icon-nwe-33x29.png)を使用して、サブタスクを作成します。

   * 親タスクとして指定したいタスクの上に、タスクをドラッグ＆ドロップします。

     >[!NOTE]
     >
     >タスクの一覧がタスク番号で並べられている場合、およびタスクリストにグループが適用されていない場合にのみ、タスクのインデントを設定できます。

### タスクのサブタスクセクションからサブタスクを作成 {#create-subtasks-from-the-task-subtasks-section}

>[!NOTE]
>
>Workfrontまたはグループ管理者は、レイアウトテンプレートを使用して、環境内の「サブタスク」セクションを削除する場合があります。

1. サブタスクを作成するプロジェクトに移動します。
1. 左側のパネルで「**タスク**」セクションをクリックします。
1. サブタスクを作成するタスクの名前をクリックします。
1. 左側のパネルにある「**サブタスク**」セクションをクリックします（使用可能な場合）。
1. 「**新規タスク**」をクリックします。

   タスクの作成について詳しくは、[プロジェクトでのタスクの作成](../../../manage-work/tasks/create-tasks/create-tasks-in-project.md)を参照してください。

1. 「**タスクを作成」をクリックします。**

   新しいタスクは、手順3で選択したタスクのサブタスクとして作成されます。<!--ensure this is accurate-->

## サブタスクをメインタスクにする

1. サブタスクをメインタスクにするプロジェクトに移動します。
1. 左側のパネルで「**タスク**」セクションをクリックします。
1. メインタスクにしたいサブタスクを選択します。
1. **アウトデント** アイコン ![&#x200B; アウトデントアイコン &#x200B;](assets/outdent-icon-nwe-31x29.png)をクリックして、サブタスクをメインタスクにします。

   または

   標準の英語 QWERTY キーボードで、Option + &lt;（Mac）または Alt + &lt;（Windows）を押します。 他の言語では、Option + コマンドが使用される場合があります。 （Mac）または Alt +。 （Windows）インデントを解除する。

   >[!NOTE]
   >
   >タスクのリストがタスク番号で並べ替えられていて、タスクリストにグループ化が適用されていない場合にのみ、タスクのインデントを解除できます。
