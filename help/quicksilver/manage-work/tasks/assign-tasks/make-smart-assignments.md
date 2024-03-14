---
product-area: projects;user-management
navigation-topic: assign-tasks
title: スマート割り当ての実行
description: スマート割り当てを使用して、作業を完了するのが最適なユーザーを特定できます。スマート割り当ては、ジョブに最も適したリソースを決定するアルゴリズムに基づいて作業項目をリソースに割り当てる際に、Adobe Workfrontが表示するユーザー、役割、またはチームに対する提案です。 スマート割り当てについて詳しくは、スマート割り当ての概要を参照してください。
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: c50ff48bbc492199b39db17b8c445207209bb6a5
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 33%

---

# スマート割り当ての実行

<!--Audited: 02/2024-->

{{preview-and-fast-release}}

スマート割り当てを使用して、作業を完了するのが最適なユーザーを特定できます。

スマート割り当ては、作業項目をリソースに割り当てる際にAdobe Workfrontが提示するユーザー、役割、またはチームに対する提案です。 Workfrontでは、ジョブに最も適したリソースを決定するアルゴリズムに基づいて提案します。

<span class="preview">Workfrontには、タスクと問題に関する 2 つの異なるアルゴリズムがあります。 </span>

スマート割り当ての決定に使用される基準の詳細については、 [スマート割り当ての概要](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>新規：標準</p>
      または
      <p>現在：作業以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>タスクおよびイシューに対する編集アクセス権</p> <p>プロジェクトに対する表示以上のアクセス権</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクやイシューに対する割り当てを行う権限の付与</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。 詳しくは、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## スマート割り当ての実行

スマート割り当ては、Workfront で割り当てを行うほとんどの場所で使用できます。

1. 次の領域に移動し、 **割当て** または **これをに割り当てる** フィールド：

   * タスクまたはイシューのリストやレポート
   * タスクまたはイシューのヘッダー
   * タスクまたはイシューの概要パネル
   * <span class="preview">プロジェクトに新しいタスクまたはイシューを追加するときの [ 新しいタスク ] ボックスまたは [ 新しいイシュー ] ボックス</span>
   * ホームエリアにリストされた項目の「割り当て」フィールド
   * ワークロードバランサーのタスクまたはイシュー

1. 割り当てフィールドにカーソルを置き、2 秒間待ちます。

   <span class="preview">The **推奨割り当て** リストが表示されます。</span> <!--check the casing for "assignments" should be lower case in task lists??-->

   >[!TIP]
   >
   >   リストヘッダーが表示されます **以下に、いくつかの推奨事項を示します。** の代わりに **推奨割り当て** をクリックします。

   ![](assets/smart-assignments-task-header-nwe-350x302.png)

   問題の場合、スマート割り当ての候補が「 **推奨割り当て** 領域。

   タスクの場合、スマート割り当ては、アルゴリズムの計算のどの段階で割り当てが特定されたかに応じて、次のセクションに表示されます。

   * **推奨割り当て**：タスクのスマート割り当てのアルゴリズム計算の第 1 段階で特定された割り当て。
   * <span class="preview">**その他の割り当て**：タスクのスマート割り当てのアルゴリズム計算の第 2 段階で識別された割り当て。 この節は、問題に対しては使用できません。 </span> <!--replace this with the new UI: "Other assignments"-->

   ![](assets/smart-assignments-task-list.png)

   詳しくは、[スマート割り当ての概要](../../../manage-work/tasks/assign-tasks/smart-assignments.md)を参照してください。

1. レコメンデーションリストでユーザー名をクリックして選択します。

1. （オプション）「 **自分に割り当て** 作業項目を自分に割り当てる。

   >[!TIP]
   >
   >候補の提案がない場合、候補リストは開きません。

1. （オプション）スマート割り当てリストから推奨ユーザーの 1 つを使用しない場合は、目的のリソースの名前を入力し、リストに表示されたら名前を選択します。
1. 「**入力**」をクリックして割り当てを行います。

   選択したユーザーがタスクまたはイシューに割り当てられます。
