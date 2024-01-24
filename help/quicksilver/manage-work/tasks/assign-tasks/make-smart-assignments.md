---
product-area: projects;user-management
navigation-topic: assign-tasks
title: スマート割り当てを行う
description: スマート割り当てを使用して、作業を完了するのが最適なユーザーを特定できます。 スマート割り当ては、ジョブに最も適したリソースを決定するアルゴリズムに基づいて作業項目をリソースに割り当てる際にAdobe Workfrontが表示するユーザーに対する提案です。 スマート割り当ての詳細は、「スマート割り当ての概要」を参照してください。
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 03894773e61fc0706148695572a164a2e778da9b
workflow-type: tm+mt
source-wordcount: '558'
ht-degree: 0%

---

# スマート割り当てを行う

<!--update "Results" to "Other assignments" with Prod-->

<span class="preview">このページで強調表示されている情報は、まだ一般に利用できない機能を示しています。 この機能は、すべての顧客のプレビュー環境でのみ使用できます。</span>

<span class="preview">現在のリリーススケジュールについて詳しくは、 [2024 年第 1 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span>

スマート割り当てを使用して、作業を完了するのが最適なユーザーを特定できます。

スマート割り当ては、ジョブに最も適したリソースを決定するアルゴリズムに基づいて作業項目をリソースに割り当てる際にAdobe Workfrontが表示するユーザーに対する提案です。

<span class="preview">Workfrontには、タスクと問題に関する 2 つの異なるアルゴリズムがあります。 </span>
スマート割り当ての詳細については、 [スマート割り当ての概要](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>新規：標準</p>
      または
      <p>現在：作業以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タスクおよび問題へのアクセスを編集</p> <p>プロジェクトへのアクセス権を表示または高くする</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>タスクや問題に対する割り当てを行う権限を付与する</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## スマート割り当てを行う

スマート割り当ては、Workfrontで割り当てをおこなうほとんどの場所で使用できます。

1. 次の領域に移動し、 **割当て** または **これをに割り当てる** フィールド：

   * タスク、タスクリスト、またはレポート
   * タスクまたはイシューのヘッダー
   * タスクまたは問題の概要パネル
   * 「ホーム」領域にリストされた項目の「割り当て」フィールド
   * ワークロードバランサーのタスクまたは問題

1. 割り当てフィールドにカーソルを置き、2 秒間待ちます。

   <span class="preview">The **推奨割り当て** リストが表示されます。</span> <!--check the casing for "assignments" should be lower case in task lists??-->

   >[!TIP]
   >
   >   リストヘッダーが表示されます **以下に、いくつかの推奨事項を示します。** の代わりに **推奨割り当て** をクリックします。

   ![](assets/smart-assignments-task-header-nwe-350x302.png)

   問題の場合、スマート割り当ての候補が「 **推奨割り当て** 領域。

   タスクの場合、スマート割り当ては、アルゴリズムの計算のどの段階で割り当てが特定されたかに応じて、次のセクションに表示されます。

   * **推奨割り当て**：タスクのスマート割り当てのアルゴリズム計算の第 1 段階で特定された割り当て。
   * <span class="preview">**結果**：タスクのスマート割り当てのアルゴリズム計算の第 2 段階で識別された割り当て。 この節は、問題に対しては使用できません。 </span> <!--replace this with the new UI: "Other assignments"-->

   ![](assets/smart-assignments-task-list.png)

   詳しくは、 [スマート割り当ての概要](../../../manage-work/tasks/assign-tasks/smart-assignments.md) .

1. レコメンデーションリストでユーザー名をクリックして選択します。

1. （オプション）「 **自分に割り当て** 作業項目を自分に割り当てる。

   >[!TIP]
   >
   >候補がない場合、候補リストは開きません。

1. （オプション）スマート割り当てリストから推奨ユーザーの 1 つを使用しない場合は、目的のユーザーの名前を入力し、リストに表示されたら名前を選択します。
1. クリック **入力** をクリックして割り当てを行います。

   選択したユーザーがタスクまたはイシューに割り当てられます。
