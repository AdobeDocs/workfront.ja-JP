---
product-area: projects;user-management
navigation-topic: assign-tasks
title: スマート割り当ての実行
description: スマート割り当てを使用して、作業を完了するのが最適なユーザーを特定できます。スマート割り当ては、業務に最も適したリソースを決定するアルゴリズムに基づいて作業アイテムをリソースに割り当てる際に Adobe Workfront に表示される、ユーザー、役割またはチームに関する提案です。スマート割り当てについて詳しくは、スマート割り当ての概要を参照してください。
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 412645a802bdf9057bb61a5a96df257daa1c3948
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 65%

---

# スマート割り当ての実行

<!--Audited: 07/2024-->

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview"> このページで強調表示されている情報は、高速リリースを有効にしたお客様向けの実稼動環境でのみ使用できる機能を指しています。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

<span class="preview"> この機能は、2025 年 1 月に 25.1 リリースで高速リリースを有効にしたお客様向けに実稼動環境から削除されます。 25.1 リリースについて詳しくは、[2025 年第 1 四半期リリースの概要 ](/help/quicksilver/product-announcements/product-releases/25-q1-release-activity/25-q1-release-overview.md) を参照してください。

スマート割り当てを使用して、作業の完了に最適なユーザーを特定できます。

スマート割り当ては、作業アイテムをリソースに割り当てる際に Adobe Workfront に表示される、ユーザー、役割またはチームに関する提案です。Workfront は、業務に最も適したリソースを決定するアルゴリズムに基づいて提案します。

<span class="preview">Workfrontには、タスクとイシューに異なる機能を持つスマート割り当てを計算する 2 つのアルゴリズムがあります。</span>

スマート割り当ての決定に使用される基準について詳しくは、[スマート割り当ての概要](/help/quicksilver/manage-work/tasks/assign-tasks/smart-assignments.md)を参照してください。

## アクセス要件

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
   <td> <p>新規：標準</p>
      または
      <p>現在：ワーク以上</p> </td> 
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

*詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## スマート割り当ての実行

スマート割り当ては、Workfront で割り当てを行うほとんどの場所で使用できます。

1. 次のエリアに移動し、「**割り当て**」または「**割り当て先**」フィールドをクリックします。

   * タスクまたはイシューのリストやレポート
   * タスクまたはイシューのヘッダー
   * タスクまたはイシューの概要パネル
   * <span class="preview"> 新規タスク </span> またはイシューをプロジェクトに追加する際の <span class="preview"> 新規タスク </span> または新規イシューボックス
   * ワークロードバランサーのタスクまたはイシュー

1. 「割り当て」フィールドにカーソルを置き、2 秒間待ちます。

   イシューの場合、スマート割り当ては次のセクションに表示されます。

   * **ユーザーとチーム**
   * **担当業務**

   ![](assets/smart-assignments-issue-header.png)

   タスクについては、割り当てが特定されたアルゴリズムの計算のフェーズに応じて、スマート割り当てが次のセクションに表示されます。

   * <span class="preview">**提案された割り当て**：タスクスマート割り当てアルゴリズムの最初のフェーズで識別された割り当てを表示します。</span>
   * **ユーザーとチーム**、**担当業務** または <span class="preview">**評価カードの担当業務**</span>：タスクスマート割り当てのアルゴリズム計算の第 2 段階で特定された割り当て。

   <span class="preview">![](assets/smart-assignments-task-list.png)</span>

   詳しくは、[スマート割り当ての概要](../../../manage-work/tasks/assign-tasks/smart-assignments.md)を参照してください。

1. 名前をクリックして、レコメンデーションリストのリソースを選択します。

1. （オプション）「**自分に割り当て**」をクリックして、作業アイテムを自分に割り当てます。

   >[!TIP]
   >
   >候補の提案がない場合、候補リストは開きません。

1. （オプション）スマート割り当てリストから候補ユーザーの 1 人を使用しない場合は、目的のリソースの名前を入力していき、リストに名前が表示されたらそれを選択します。
1. 「**入力**」をクリックして割り当てを行います。

   選択したユーザーがタスクまたはイシューに割り当てられます。
