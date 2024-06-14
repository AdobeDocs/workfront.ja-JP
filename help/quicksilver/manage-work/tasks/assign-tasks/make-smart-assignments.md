---
product-area: projects;user-management
navigation-topic: assign-tasks
title: スマート割り当ての実行
description: スマート割り当てを使用して、作業を完了するのが最適なユーザーを特定できます。スマート割り当ては、業務に最も適したリソースを決定するアルゴリズムに基づいて作業アイテムをリソースに割り当てる際に Adobe Workfront に表示される、ユーザー、役割またはチームに関する提案です。スマート割り当てについて詳しくは、スマート割り当ての概要を参照してください。
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: 02a47566acd0fff151656fe2c5b59a6679748b15
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 75%

---

# スマート割り当ての実行

<!--keep the yellow around the Rate card job roles and the Preview intro for those-->

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべての顧客に対してプレビュー環境でのみ使用できるか、または迅速リリースを有効にした顧客の実稼動環境でのみ使用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

<span class="preview">現在のリリースについて詳しくは、を参照してください。 [2024 年第 3 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md).</span>

スマート割り当てを使用して、作業の完了に最適なユーザーを特定できます。

スマート割り当ては、作業アイテムをリソースに割り当てる際に Adobe Workfront に表示される、ユーザー、役割またはチームに関する提案です。Workfront は、業務に最も適したリソースを決定するアルゴリズムに基づいて提案します。

<span class="preview">Workfrontには、タスクとイシューに異なる機能を持つスマート割り当てを計算する 2 つの異なるアルゴリズムがあります。 </span>

スマート割り当ての決定に使用される基準について詳しくは、[スマート割り当ての概要](../../../manage-work/tasks/assign-tasks/smart-assignments.md)を参照してください。

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

*保有するプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## スマート割り当ての実行

スマート割り当ては、Workfront で割り当てを行うほとんどの場所で使用できます。

1. 次のエリアに移動し、「**割り当て**」または「**割り当て先**」フィールドをクリックします。

   * タスクまたはイシューのリストやレポート
   * タスクまたはイシューのヘッダー
   * タスクまたはイシューの概要パネル
   * <span class="preview">プロジェクトに新規タスクまたはイシューを追加するときの新規タスクボックスまたは新しい問題ボックス</span>
   * ホームエリアにリストされた項目の「割り当て」フィールド
   * ワークロードバランサーのタスクまたはイシュー

1. 「割り当て」フィールドにカーソルを置き、2 秒間待ちます。

   <div class="preview">
   スマート割り当て候補が表示された次のセクションの 1 つまたは複数が表示されます。

   * **提案された割り当て**：タスクに関する表示。 <!--remove the note when we go to production with smarter assignments-->

     >[!TIP]
     >
     >   リストヘッダーが表示されます **推奨事項を次に示します** の代わりに **提案された割り当て** 実稼動環境で上書きできます。
     >
   * **ユーザーとチーム**：タスクおよび問題に関する表示です。
   * **担当業務**：タスクおよび問題に対して表示します。
   * **評価カードの担当業務**：タスクに関する表示。 詳しくは、を参照してください [評価カードの管理](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/manage-rate-cards.md).<!--check later with Lisa to see if this also came to issues?! - and always keep this in yellow-->
   </div>

   <span class="preview">![](assets/smart-assignments-task-header-nwe-350x302.png)</span>


   タスクについては、割り当てが特定されたアルゴリズムの計算のフェーズに応じて、スマート割り当てが次のセクションに表示されます。

   * **提案された割り当て**：タスクスマート割り当てのアルゴリズム計算の最初のフェーズで特定された割り当て。 <span class="preview">このセクションは、問題に対しては使用できません。</span>
   * <span class="preview">**ユーザーとチーム**, **担当業務**、または **評価カードの担当業務**：タスクスマート割り当てのアルゴリズム計算の第 2 段階で特定された割り当て。 <!--no longer valid: This section is not available for issues. --></span> <!--replace this with the new UI: "Other assignments"-->

   <span class="preview">![](assets/smart-assignments-task-list.png)</span>

   詳しくは、[スマート割り当ての概要](../../../manage-work/tasks/assign-tasks/smart-assignments.md)を参照してください。

1. レコメンデーションリストでユーザー名をクリックして、ユーザーを選択します。

1. （オプション）「**自分に割り当て**」をクリックして、作業アイテムを自分に割り当てます。

   >[!TIP]
   >
   >候補の提案がない場合、候補リストは開きません。

1. （オプション）スマート割り当てリストから候補ユーザーの 1 人を使用しない場合は、目的のリソースの名前を入力していき、リストに名前が表示されたらそれを選択します。
1. 「**入力**」をクリックして割り当てを行います。

   選択したユーザーがタスクまたはイシューに割り当てられます。
