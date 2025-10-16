---
product-area: projects
navigation-topic: use-predecessors
title: タスクを連鎖して先行タスク関係を作成する
description: Adobe Workfront では、複数の方法で先行タスクの関係を作成できます。方法の 1 つは、タスクを連鎖させることです。
author: Alina
feature: Work Management
exl-id: 38ea13a5-ab95-4617-a47f-9dde5f752fb4
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '278'
ht-degree: 92%

---

# タスクを連鎖させて先行タスクの関係を作成

Adobe Workfront では、複数の方法で先行タスクの関係を作成できます。方法の 1 つは、タスクを連鎖させることです。

先行タスクについて詳しくは、[先行タスクの概要](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md)を参照してください。

タスクを連結することにより、各タスクの関係を自分で手動で作成するのではなく、システムが選択したタスクに先行タスクの関係を自動的に作成できるようにすることができます。タスク間では、異なる先行タスクの関係タイプを引き続き使用できます。

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
   <td><p>標準</p> 
   <p>プラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>タスクおよびプロジェクトへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクおよびプロジェクトに対する権限の管理</p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:
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
   <p>Standard </p>
    <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Tasks and Projects</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the tasks and the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## タスクを連鎖させて先行タスクの関係を作成

1. 連鎖させたいタスクが含まれるプロジェクトに移動します。
1. 左パネルで「**タスク**」をクリックします。
1. （条件付き）タスクリストの右上隅にある「**自動保存**」を選択し、連鎖させたいタスクを選択します。

   ![](assets/nwe-autosave-icon-on-highlighted-350x295.png)

   >[!IMPORTANT]
   >
   >タスクへの変更を手動で保存する場合、またはタスクの保存にタイムライン計画モードを使用する場合は、タスクリスト内のタスクを連鎖することはできません。

1. 選択したタスクを右クリックし、「**連鎖**」を選択します。
1. 次の依存関係タイプから選択します。

   * **終了 - 開始**
   * **終了 - 終了**
   * **開始 - 開始**
   * **開始 - 終了**

   先行タスクの依存関係タイプについて詳しくは、[タスク依存関係タイプの概要](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md)を参照してください。

1. （オプション）一部のタスクが以前に連鎖されている場合は、「**連鎖解除**」をクリックします。

   >[!CAUTION]
   >
   >タスクの一括編集時にチェーン解除オプションを使用すると、連続する先行タスクのみが削除されます。

   選択した先行タスクの関係によってリンクされました。
