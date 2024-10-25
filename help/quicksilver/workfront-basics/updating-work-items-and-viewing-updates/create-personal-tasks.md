---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 個人タスクの作成
description: 個人タスクは、ユーザーに送信するアドホックな作業リクエストや、ホームエリアで自分で作成する To Do アイテムです。 Workfrontは、個人のタスクとして行うアドホックな作業リクエストとタスクを保存します。
author: Lisa
feature: Get Started with Workfront
source-git-commit: 1e69d715f343bfef1e5aee658a1dff12abfc61a0
workflow-type: tm+mt
source-wordcount: '545'
ht-degree: 7%

---


# 個人用タスクを作成する

<!--Audited: 10/2024-->

個人タスクは、ユーザーに送信するアドホックな作業リクエストや、ホームエリアで自分で作成する To Do アイテムです。

Workfrontは、個人のタスクとして行うアドホックな作業リクエストとタスクを保存します。

デフォルトでは、Workfrontのすべてのユーザーには、「&lt; フルネーム > のタスク」というプロジェクトがあります。 例えば、「Rick Kuvec の Tasks」などです。

このプロジェクトは検索では表示されず、非表示になっています。 すべての個人タスクは、このプロジェクトに保存されます。

必要に応じて、個人タスクをプロジェクトに移動できます。

個人タスクは、次の方法で作成できます。

* ホームエリアで To Do アイテムを作成する

  詳しくは、[ ホームエリアからの作業項目とプロジェクトの作成 ](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md) を参照してください。

* 別のユーザーへの個人的な作業要求の作成
* ユーザーの個人作業要求を作成します

この記事では、ユーザーの個人作業要求を作成する方法について説明します。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン*</strong></td> 
   <td> 
   <p>現在：他のユーザーにリクエストを送信することを計画します。 すべてのユーザーは、自分で作業リクエストを作成できます。</p>
   <p>新規：他のユーザーにリクエストを送信するための標準。 すべてのユーザーは、自分で作業リクエストを作成できます。</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>ユーザーへのアクセスを編集して、ユーザーの作業要求を作成します。 自分の個人用作業要求を作成するための表示アクセス権。 </p>
   </td> 
  </tr>

</tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++


## 個人の作業要求の作成

1. 自分のユーザーのプロファイルページに移動するか、表示するためのアクセス権を持つ別のユーザーのプロファイルページに移動します。

   >[!TIP]
   >
   >Workfront管理者は、特定のユーザーがアクセスレベルを設定する際に、そのユーザーが表示されるのを防ぐ可能性があります。

1. ヘッダーでユーザー名の右側にある **詳細メニュー**![](assets/more-menu.png) をクリックします。
1. **作業を送信** リクエストをクリックします。
**作業要求をユーザーに送信** ボックスが表示されます。

   ![](assets/personal-task-box.png)
1. 次の情報を更新します。

   * **タスク名**：アドホック作業要求または個人タスクの名前です。
   * **説明**：タスクの説明を追加します。
   * **割り当て先**：選択したユーザーの名前がデフォルトで表示されます。 ユーザーまたはチームをさらに追加できます。
   * **期限**：このタスクを完了する期限です。 デフォルトでは、今日の日付になります。 過去の日付は選択できません
   * **時間**：このタスクを完了する時間です。 デフォルトでは、これは現在の時間です。

1. 「**リクエストを送信**」をクリックして、作業要求を保存します。

   作業要求はWorkfrontで個人用タスクとして保存され、ホーム領域の To do ウィジェットに追加されます。

   <!--this last step will need to be updated when they fix this functionality and the work requests you create for others actually go to their To do widget instead of yours-->

## 個人タスクの検索

次の領域で個人のタスクを検索できます。

* ホームエリアの To do ウィジェット。 詳しくは、[ ホームエリアからの作業項目とプロジェクトの作成 ](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md) を参照してください。

* 個人のタスクレポートまたはリスト。 個人タスク・フィルタを作成して、タスク・レポートまたはリストに適用できます。詳細は、[ フィルタ：個人タスク ](/help/quicksilver/reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-personal-tasks.md) を参照してください。





