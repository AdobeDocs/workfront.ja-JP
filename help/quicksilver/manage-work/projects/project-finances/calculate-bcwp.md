---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: BCWP (Budgeted Cost of Work Performed) の計算
description: BCWP (Budgeted Cost of Work Performed) は、達成額とも呼ばれ、この指標の計算時に実際に完了したタスクの量を表すプロジェクトパフォーマンス指標です。
author: Alina
feature: Work Management
exl-id: 203709a7-e522-4875-b3eb-40b967a938ec
source-git-commit: 1d5de5ff0ebebd84482507c71730cfbd05c513a5
workflow-type: tm+mt
source-wordcount: '620'
ht-degree: 0%

---

# BCWP (Budgeted Cost of Work Performed) の計算

## BCWP(Budgeted Cost of Work Performed) の概要

BCWP (Budgeted Cost of Work Performed) は、達成額とも呼ばれ、この指標の計算時に実際に完了したタスクの量を表すプロジェクトパフォーマンス指標です。

Adobe Workfrontは、プロジェクトとタスクの両方について、BCWP (Budgeted Cost of Work Performed) を計算します。

タスクまたはプロジェクトの BCWP の値を確認する際は、次の点に注意してください。

* Workfrontは、プロジェクトの PMI(Performance Index Method) の構成に基づいてタスクの BCWP を計算します。

   時間やコストを使用して PMI を計算するようにプロジェクトを設定し、BCWP も同じ値を使用して計算します。

   BCWP の計算方法の設定については、「 [BCWP の計算方法を設定する](#configure-how-bcwp-is-calculated) 」を参照してください。

* Workfrontは、プロジェクト上のすべての親タスクと個々のタスクのすべての BCWP 値を追加することで、プロジェクトの BCWP を計算します。

   子タスクの値は、プロジェクトの BCWP には追加されません。

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

## BCWP の計算方法を設定する {#configure-how-bcwp-is-calculated}

BCWP を時間単位で計算するかコスト単位で計算するかは、プロジェクトの Performance Index Method (PIM) の計算方法を設定することで設定できます。

1. プロジェクトに移動して展開します。 **プロジェクトの詳細** をクリックします。
1. 内 **金融** 領域で、 **パフォーマンスインデックスメソッド** 「 」フィールドに入力し、ダブルクリックして編集します。

   ![](assets/pim-options-hour-cost-based-nwe.png)

1. 次のオプションから選択します。

   | オプション | 計算の実行方法 |
   |---|---|
   | 時間ベース | Workfrontは、タスクの計画時間を使用して BCWP を計算します。 |
   | コスト ベース | Workfrontは、タスクの計画コストを使用して BCWP を計算します。 |

1. クリック **変更を保存**.

プロジェクトのタスクの BCWP は、時間またはコストを使用して計算されます。

## BCWP を計算

Workfrontは、次の式を使用して、タスクまたはプロジェクトの Budgeted Cost of Work Performed (BCWP) を計算します。

```
Task BCWP = Actual Percent Complete x Task Budget
```

```
Project BCWP = SUM(BCWP values of all parent and individual tasks)
```

これらの計算では、次の値が使用されます。

| 使用値 | 使用する値の説明 |
|---|---|
| 実際の完了率 | これは、Workfrontに表示されるタスクの実際の完了率です。 |
| タスクの予算 | これは、タスクの計画時間または計画コストの値です。 |

たとえば、タスクの実績完了率が 25%で、タスクの予算または計画コストが$10,000 の場合、タスクの BCWP は次のようになります。

```
BCWP = 25% x $10,000 = $2,500
```

## プロジェクトまたはタスクの BCWP を見つける

BCWP 列をビューに追加すると、レポートまたはリストで Budgeted Cost of Work Performed の値を表示できます。

1. タスクまたはプロジェクトのリストに移動します。
1. を展開します。 **表示** メニューと選択 **新しいビュー** または **表示をカスタマイズ**.

1. クリック **列を追加**.
1. 内 **この列に表示：** フィールド入力を開始する **BCWP** をクリックして、リストに表示されたら選択します。

   ![](assets/bcwp-project-view.png)

1. クリック **ビューを保存**.
1. [BCWP] フィールドがビューに表示されます。
