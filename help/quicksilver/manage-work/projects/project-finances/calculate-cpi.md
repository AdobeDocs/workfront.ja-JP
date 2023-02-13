---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: コスト効果指数 (CPI) の計算
description: CPI (Cost Performance Index) は、計画コストと実績コストの間のプロジェクトレベルまたはタスクレベルでの関係を表します。 プロジェクトマネージャーは、この指標をレビューして、特定の時点で現在コストが超過している、または超過しているタスクを特定します。
author: Alina
feature: Work Management
exl-id: 7f2efe26-7292-482d-986c-2d2077a7ca52
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '635'
ht-degree: 0%

---

# コスト効果指数 (CPI) の計算

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

CPI (Cost Performance Index) は、計画コストと実績コストの間のプロジェクトレベルまたはタスクレベルでの関係を表します。 プロジェクトマネージャーは、この指標をレビューして、特定の時点で現在コストが超過している、または超過しているタスクを特定します。 コストは、PIM(Performance Index Method) に応じて、時間単位またはドル単位で測定できます。 Performance Index メソッドの設定の詳細については、「 [パフォーマンスインデックスメソッド (PIM) の設定](../../../manage-work/projects/project-finances/set-pim.md).

CPI を使用できるのは、時間入力が必要な組織のみです。 さらに、コストベースの PIM 値は、タスク担当者（ジョブの役割またはユーザー）のコスト率を定義した組織でのみ正確になります。

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
   <td> <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトおよび財務データへのアクセスの表示</p> <p> まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>財務を表示する権限を持つプロジェクトに対する表示権限以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## CPI（コスト効果指数）の概要

* [CPI 値](#the-cpi-value)
* [CPI の計算方法](#how-cpi-is-calculated)

### CPI 値 {#the-cpi-value}

プロジェクトマネージャーは、CPI 値が 1 の場合は、プロジェクトが予算に正確に基づいていることを意味します。 1 より大きい値は、プロジェクトが予算を下回っている（当初の計画よりも少ない時間または費用）ことを示し、1 未満の値は、プロジェクトが予算を超えている（当初の計画より多い時間または費用が計画されている）ことを示します。 1 からの偏差が大きいほど、プランからの偏差が大きくなります。

| **CPI 値** | **予算の表示** |
|---|---|
| 1 | 計画または予算 |
| > 1 （1 より大きい） | 予算未満 |
| &lt; 1 （1 未満） | 予算超過 |


### CPI の計算方法 {#how-cpi-is-calculated}

Adobe Workfrontでは、CPI の計算は、プロジェクトで選択したパフォーマンスインデックス方法に依存します。 Performance Index メソッドの設定の詳細については、「 [パフォーマンスインデックスメソッド (PIM) の設定](../../../manage-work/projects/project-finances/set-pim.md).

* [時間ベースの PIM を使用する場合の CPI の計算](#cpi-calculations-when-using-hour-based-pim)
* [原価ベースの PIM を使用する場合の CPI 計算](#cpi-calculations-when-using-cost-based-pim)

#### 時間ベースの PIM を使用する場合の CPI の計算 {#cpi-calculations-when-using-hour-based-pim}

もし

```
Actual Hours > 0 THEN CPI = Total Budgeted Cost Work Performed / Actual Hours
```

それ以外の場合

```
CPI = 1
```

* **親以外のタスクの場合：**

   ```
   Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete / 100)
   ```

* **親タスクの場合：**
Total Budgeted Cost Work Performed =すべての直接の子タスクの「Total Budgeted Cost Work Performed」フィールドの合計です。

* **プロジェクトの場合：**
Total Budgeted Cost Work Performed =すべての最上位タスク（親タスクおよびスタンドアロンタスク）の「Total Budgeted Cost Work Performed」フィールドの合計。

BCWP (Total Budgeted Cost Work Performed) の詳細については、 [予算原価実績の計算 (BCWP)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

#### 原価ベースの PIM を使用する場合の CPI 計算 {#cpi-calculations-when-using-cost-based-pim}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>CPI = (Planned Cost of Work Performed + Planned Cost of Incurred Expenses) / (Total Actual Cost + Actual Cost of Incurred Expenses) </code> </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>NOTE: this used to be here before - above - but Anna sent me the one below. I kept the other one, although she is still researching its validity - see this issue: https://hub.workfront.com/issue/5fc7b1cf00012aeebf9e822db8ea2513/overview)</code> </p>
-->

もし

```
Actual Labor Cost + Incurred Actual Expense Cost <> 0 THEN CPI = (Total Budgeted Cost Work Performed + Incurred Planned Expense Cost) / (Actual Labor Cost + Incurred Actual Expense Cost)
```



それ以外の場合

```
CPI = 1
```

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>(NOTE: above: this used to say: CPI = CPI Labor, but Anna had me fix it on July 21, 2021)</code> </p>
-->

この計算のフィールドを次に示します。

```
Total Actual Cost = Actual (logged) Hours * Hourly Rate of assignees
```

```
Incurred Actual Expense Cost = Actual Cost
```

発生費は、実費が 0 より大きい費用です

```
Planned Cost of Incurred Expenses = Total of Planned Cost of all incurred expenses
```



<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Old calculation - taken out by Lilit and replaced below: Planned Cost of Work Performed= (planned labor cost) * (percent complete) / 100 where planned labor cost is the planned hours allocated to assignees * their rates.)</p>
  -->

* 「計画作業原価実行」は、次の式で計算されます。

   ```
   Planned Cost of Work Performed = Planned cost * Percent Complete / 100
   ```

「Total Budgeted Cost Work Performed」は、次の項目に対して計算されます。

* **親以外のタスクの場合：**

   ```
   Total Budgeted Cost Work Performed = Planned Labor Cost * Percent Complete / 100
   ```

* **親タスクの場合：**

   ```
   Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field from all direct child tasks)
   ```

* **プロジェクトの場合：**

   ```
   Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field for all top level tasks)
   ```



## プロジェクトまたはタスクで CPI を検索

プロジェクトの CPI、またはプロジェクト、タスクリスト、またはレポートにタスクを表示できます。 また、プロジェクトレベルまたはタスクレベルで表示できます。

1. CPI を表示するプロジェクトまたはタスクに移動します。
1. 展開 **プロジェクトの詳細** または **タスクの詳細** 左のパネルで、プロジェクトまたはタスクの CPI を表示しているかどうかに応じて表示されます。

1. クリック **金融**.

   CPI が **CPI/SPI/CSI** フィールドに入力します。

   ![](assets/cpi-on-project-nwe.png)
