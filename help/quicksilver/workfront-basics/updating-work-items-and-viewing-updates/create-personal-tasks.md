---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 個人タスクの作成
description: 個人タスクは、ユーザー、自分自身、または自分のホームエリアで自分用に作成した To Do アイテムに送信するアドホックな作業リクエストです。 Workfrontは、個人のタスクとして行うアドホックな作業リクエストとタスクを保存します。
author: Lisa
feature: Get Started with Workfront
exl-id: b40d6b10-19c7-4e11-a74f-a8af3ebafb65
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '655'
ht-degree: 4%

---

# 個人用タスクを作成する

<!--Audited: 10/2024-->

個人タスクは、ユーザーに送信したり、自分で送信または追加したりするアドホックな作業要求です。

Adobe Workfrontは、Wprfront が各ユーザーに対して自動的に作成する、ユーザーの個人プロジェクトに対する個人のタスクとして、アドホックな作業要求および作業アイテムを保存します。

ユーザーの個人プロジェクトの特徴を次に示します。

* Workfrontのすべてのユーザーには、「&lt; ユーザーのフルネーム > のタスク」という個人用プロジェクトがあります。 例えば、「John Smith の Tasks」と入力します。
* 各ユーザーの個人プロジェクトは検索では表示されず、非表示になります。
* ユーザーがアクティベート解除されている場合でも、個人プロジェクトは削除できません。
* 個人プロジェクトのステータスは、常に最新です。 個人プロジェクトは完了またはキャンセルできません。
* すべての個人タスクは、ユーザーの個人プロジェクトに保存されます。
* 必要に応じて、個人タスクを別のプロジェクトに移動できます。

個人タスクは、次の方法で作成できます。

* ホームエリアで To Do アイテムを作成する

  詳しくは、[&#x200B; ホームエリアからの作業項目とプロジェクトの作成 &#x200B;](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md) を参照してください。

* ユーザープロファイルページからの個人の作業要求の作成と別のユーザーへの送信
* ユーザープロファイルページからの個人の作業要求の作成と送信

この記事では、ユーザープロファイル ページからユーザーまたは自分用の個人用作業要求を作成する方法について説明します。

個人のタスクをどのように追加するかに関係なく、Workfrontの同じ領域でそれらを見つけることができます。 詳細については、この記事の「個人のタスクを検索する [&#x200B; を参照し &#x200B;](#locate-personal-tasks) ください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront パッケージ</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン</strong></td> 
   <td> 
   <p>標準<p>
   <p>プラン</p>
   <p>これは、他のユーザーにリクエストを送信するために必要なライセンスです。 すべてのユーザーは、自分で作業リクエストを作成できます。</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>ユーザーへのアクセスを編集して、ユーザーの作業要求を作成します。 自分の個人用作業要求を作成するための表示アクセス権。 </p>
   </td> 
  </tr>

</tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> 
   <p>New: Standard to send requests to other users. All users can create a work request for themselves.</p> 
   <p>Current: Plan to send requests to other users. All users can create a work request for themselves.</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configurations</strong></td> 
   <td> <p>Edit access to Users to create a work request for them. View access to create a personal work request for yourself. </p>
   </td> 
  </tr> 
 
 </tbody> 
</table>-->


## 個人の作業要求の作成

1. 自分のユーザーのプロファイルページに移動するか、表示するためのアクセス権を持つ別のユーザーのプロファイルページに移動します。

   >[!TIP]
   >
   >Workfront管理者は、特定のユーザーがアクセスレベルを設定する際に、そのユーザーが表示されるのを防ぐ可能性があります。

1. ヘッダーでユーザー名の右側にある **詳細メニュー**![](assets/more-menu.png) をクリックします。
1. 「**作業要求を送信**」をクリックします。
**作業要求をユーザーに送信** ボックスが表示されます。

   ![](assets/personal-task-box.png)
1. 次の情報を更新します。

   * **タスク名**：アドホック作業要求または個人タスクの名前です。
   * **説明**：タスクの説明を追加します。
   * **割り当て先**：選択したユーザーの名前がデフォルトで表示されます。 ユーザーまたはチームをさらに追加できます。
   * **期限**：このタスクを完了する期限です。 デフォルトでは、今日の日付になります。 過去の日付は選択できません
   * **時間**：このタスクを完了する時間です。 デフォルトでは、これは現在の時間です。

1. 「**リクエストを送信**」をクリックして、作業要求を保存します。

   作業要求はWorkfrontで個人のタスクとして保存され、ユーザーのホームエリアの To-Do ウィジェットに追加されます。 作業要求を自分宛てに送信すると、ホームの To-Do ウィジェットに表示されます。


## 個人タスクの検索

次の領域で個人のタスクを検索できます。

* 個人の要求が送信されたユーザーのホーム領域の To-Do ウィジェット。

  詳しくは、[&#x200B; ホームエリアからの作業項目とプロジェクトの作成 &#x200B;](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md) を参照してください。

* 個人のタスクレポートまたはリスト。 個人タスク フィルターを作成してタスク報告書またはリストに適用し、個人タスクのみを表示して、プロジェクト タスクを除外することができます。

  詳しくは、[&#x200B; フィルター：個人用タスク &#x200B;](/help/quicksilver/reports-and-dashboards/reports/custom-view-filter-grouping-samples/filter-personal-tasks.md) を参照してください。
