---
product-area: projects;user-management
navigation-topic: assign-tasks
title: スマート割り当てを行う
description: スマート割り当てを使用して、作業を完了するのが最適なユーザーを特定できます。 スマート割り当ては、ジョブに最も適したリソースを決定するアルゴリズムに基づいて作業項目をリソースに割り当てる際にAdobe Workfrontが表示するユーザーに対する提案です。 スマート割り当ての詳細は、「スマート割り当ての概要」を参照してください。
author: Alina
feature: Work Management
exl-id: 073a3234-3156-4b4f-a3e1-dbb32d61068a
source-git-commit: daba001c28df268721c87df7d2516ffb76e535d9
workflow-type: tm+mt
source-wordcount: '470'
ht-degree: 0%

---

# スマート割り当てを行う

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers.</span>   
  
<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> 
-->

スマート割り当てを使用して、作業を完了するのが最適なユーザーを特定できます。 スマート割り当ては、ジョブに最も適したリソースを決定するアルゴリズムに基づいて作業項目をリソースに割り当てる際にAdobe Workfrontが表示するユーザーに対する提案です。 スマート割り当ての詳細については、 [スマート割り当ての概要](../../../manage-work/tasks/assign-tasks/smart-assignments.md).

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
   * 「スケジュール設定」領域または「スケジュール設定」領域のタスクまたはイシュー
   * ワークロードバランサーのタスクまたは問題

1. 割り当てフィールドにカーソルを置き、2 秒間待ちます。 The **推奨割り当て** または **以下に、いくつかの推奨事項を示します。** リストが表示されます。

   <!--check the casing for "assignments" should be lower case in task lists??-->

   <!--replace the last sentence above with this when we release smarter assignments:
   The **Suggested assignments** list displays. 
   NOTE (********and add preview tags for the note*****)
   The list header displays **Here are a few recommendations** instead of **Suggested assignments** in an issue list.
   -->

   ![](assets/smart-assignments-task-header-nwe-350x302.png)

   このリストに表示されるユーザーは、タスクまたはタスクに対するスマート割り当ての候補です。

   スマート割り当てが表示される場所の詳細については、この記事の「スマート割り当ての候補の検索」の節を参照してください [スマート割り当ての概要](../../../manage-work/tasks/assign-tasks/smart-assignments.md) .

1. レコメンデーションリストでユーザー名をクリックして選択します。 クリック **自分に割り当て** 作業項目を自分に割り当てます。

   >[!TIP]
   >
   >候補がない場合、候補リストは開きません。

1. （オプション）スマート割り当てリストから推奨ユーザーの 1 つを使用しない場合は、目的のユーザーの名前を入力し、リストに表示されたら名前を選択します。
1. クリック **入力** をクリックして割り当てを行います。

   選択したユーザーがタスクまたはイシューに割り当てられます。
