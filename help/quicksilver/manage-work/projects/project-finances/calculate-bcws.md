---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 予定作業コストの計算 (BCWS)
description: BCWS (Budgeted Cost of Work Scheduled) は、計画値とも呼ばれ、この指標が計算された時点で完了する必要があるタスクの量を表すプロジェクトのパフォーマンス指標です。
author: Alina
feature: Work Management
exl-id: b9a36333-9430-42bd-99dd-3ad82803b633
source-git-commit: 1d5de5ff0ebebd84482507c71730cfbd05c513a5
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 0%

---

# 予定作業コストの計算 (BCWS)

## BCWS(Budgeted Cost of Work Scheduled) の概要

BCWS (Budgeted Cost of Work Scheduled) は、計画値とも呼ばれ、この指標が計算された時点で完了する必要があるタスクの量を表すプロジェクトのパフォーマンス指標です。

Adobe Workfrontは、プロジェクトとタスクの両方について、Budgeted Cost of Work Scheduled (BCWS) を計算します。

タスクまたはプロジェクトの BCWS の値を確認する際は、次の点を考慮してください。

* Workfrontは、プロジェクトの Performance Index Method(PIM) の設定に基づいてタスクの BCWS を計算します。

   時間やコストを使用して PIM を計算するようにプロジェクトを設定し、BCWS も同じ値を使用して計算できます。

   BCWS の計算方法の設定については、「 [BCWS の計算方法の構成](#configure-how-bcws-is-calculated) 」を参照してください。

* Workfrontは、プロジェクトのすべての親タスクと個々のタスクのすべての BCWS 値を追加して、プロジェクトの BCWS を計算します。

   子タスクの値は、プロジェクトの BCWS には追加されません。

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
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> <p>まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## BCWS の計算方法の構成 {#configure-how-bcws-is-calculated}

BCWS を時間単位で計算するかコスト単位で計算するかは、プロジェクトの Performance Index Method (PIM) の計算方法を設定することで設定できます。

1. プロジェクトに移動し、「 **プロジェクトの詳細** をクリックします。
1. 内 **金融** 領域で、 **パフォーマンスインデックスメソッド** 編集するには、フィールドをダブルクリックします。

   ![](assets/pim-options-hour-cost-based-nwe.png)

1. 次のオプションから選択します。

   | オプション | 計算の実行方法 |
   |---|---|
   | 時間ベース | Workfrontは、タスクの計画時間を使用して BCWS を計算します。 |
   | コスト ベース | Workfrontは、タスクの計画コストを使用して BCWS を計算します。 |


1. クリック **変更を保存**.

   プロジェクトのタスクの BCWS は、時間またはコストを使用して計算されます。

## BCWS を計算

Workfrontは、次の式を使用して、タスクまたはプロジェクトの Budgeted Cost of Work Scheduled (BCWS) を計算します。

```
Task BCWS = Planned Percent Complete x Task Budget
```

```
Project BCWS = SUM(BCWS values of all parent and individual tasks)
```

この計算では、次の値が使用されます。

| 使用値 | 使用する値の説明 |
|---|---|
| 計画完了率 | タスクの完了率は、タスクの開始から今日までの経過時間を調べることで求められます。 |
| タスクの予算 | これは、タスクの計画時間または計画コストの値です。 |

例えば、今日が 2 月 12 日で、タスクが 2 月 10 日から 2 月 20 日まで続くようにスケジュールされている場合、タスクは今日完了率が 20%になるはずです。 タスク予算（計画コスト）が$10,000 の場合、タスクの BCWS は次のようになります。

```
Task BCWS = 20% x $10,000 = $2,000
```

## プロジェクトまたはタスクの BCWS を見つける

BCWS 列をビューに追加すると、レポートまたはリストで予定されている Budgeted Cost of Work Scheduled の値を表示できます。

1. タスクまたはプロジェクトのリストに移動します。
1. を展開します。 **表示** メニューと選択 **新しいビュー** または **表示をカスタマイズ**.

1. クリック **列を追加**.
1. 内 **この列に表示：** フィールド入力を開始する **BCWS** をクリックして、リストに表示されたら選択します。

   ![](assets/bcws-in-project-view.png)

1. クリック **ビューを保存**.
1. この **BCWS** フィールドがビューに表示されます。
