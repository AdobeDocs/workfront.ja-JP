---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: コスト効率指数（CPI）の計算
description: コスト効率指数（CPI）は、予定コストと実際のコストの間のプロジェクトレベルまたはタスクレベルでの関係を表します。プロジェクトマネージャーは、この指標をレビューして、特定の時点で現在コスト未満またはコスト超過をトラッキングするタスクやプロジェクトを特定します。
author: Lisa
feature: Work Management
exl-id: 7f2efe26-7292-482d-986c-2d2077a7ca52
source-git-commit: f88b6ec019963ff6256e35b9c94eb4d1b7e99730
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 88%

---

# コスト効率指数（CPI）の計算

<!-- Audited: 5/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

コスト効率指数（CPI）は、予定コストと実際のコストの間のプロジェクトレベルまたはタスクレベルでの関係を表します。プロジェクトマネージャーは、この指標をレビューして、特定の時点で現在コスト未満またはコスト超過をトラッキングするタスクやプロジェクトを特定します。コストは、パフォーマンスインデックスメソッド（PIM）に応じて、時間単位または通貨単位で測定できます。 パフォーマンスインデックスメソッドの設定について詳しくは、[パフォーマンスインデックスメソッド（PIM）の設定](../../../manage-work/projects/project-finances/set-pim.md)を参照してください。

CPI を使用できるのは、時間入力が必要な組織のみです。さらに、コストベースの PIM 値は、組織がタスク担当者（担当業務またはユーザー）のコスト率を定義した場合のみ正確になります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td>
   <p>ライト以上</p>
   <p>レビュー以上</p></td>  
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>プロジェクトおよび財務データへのアクセス権を表示</td> 
  </tr> 
  <tr> 
   <td>オブジェクト権限</td> 
   <td>財務情報を表示する権限を持つプロジェクトに対する表示以上の権限</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## コスト効率指数（CPI）の概要

### CPI 値 {#the-cpi-value}

プロジェクトマネージャーは、CPI 値が 1 の場合は、プロジェクトが予算通りであることを意味します。1 より大きい値は、プロジェクトが予算を下回っている（当初の予定よりも少ない時間または費用が記録されている）ことを示し、1 未満の値は、プロジェクトが予算を超えている（当初の予定より多い時間または費用が記録されている）ことを示します。1 からの偏差が大きいほど、プランからの偏差が大きくなります。

| **CPI 値** | **予算の表示** |
|---|---|
| 1 | プランまたは予算 |
| > 1（1 より大きい） | 予算未満 |
| &lt; 1（1 未満） | 予算超過 |


### CPI の計算方法 {#how-cpi-is-calculated}

Adobe Workfront では、CPI の計算は、プロジェクトで選択したパフォーマンスインデックスメソッドに依存します。パフォーマンスインデックスメソッドの設定について詳しくは、[パフォーマンスインデックスメソッド（PIM）の設定](../../../manage-work/projects/project-finances/set-pim.md)を参照してください。

* [時間ベースの PIM を使用する場合の CPI の計算](#cpi-calculations-when-using-hour-based-pim)
* [コストベースの PIM を使用する場合の CPI 計算](#cpi-calculations-when-using-cost-based-pim)

#### 時間ベースの PIM を使用する場合の CPI の計算 {#cpi-calculations-when-using-hour-based-pim}

次の場合：

```
Actual Hours > 0 THEN CPI = Total Budgeted Cost Work Performed / Actual Hours
```

それ以外の場合

```
CPI = 1
```

* **親タスク以外の場合：**

  ```
  Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete / 100)
  ```

* **親タスクの場合：**
BCWP（作業実行の予算）合計 = すべての直接の子タスクで実行された「BCWP」フィールドの合計です。

* **プロジェクトの場合：**
合計予算コスト作業実行済=すべての最上位タスク（親およびスタンドアロン・タスク）の合計予算コスト作業実行済フィールドの合計。

作業実行の予算（BCWP）合計について詳しくは、[作業実行の予算（BCWP）合計の計算](../../../manage-work/projects/project-finances/calculate-bcwp.md)を参照してください。

#### コストベースの PIM を使用する場合の CPI 計算 {#cpi-calculations-when-using-cost-based-pim}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>CPI = (Planned Cost of Work Performed + Planned Cost of Incurred Expenses) / (Total Actual Cost + Actual Cost of Incurred Expenses) </code> </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>NOTE: this used to be here before - above - but Anna sent me the one below. I kept the other one, although she is still researching its validity - see this issue: https://hub.workfront.com/issue/5fc7b1cf00012aeebf9e822db8ea2513/overview)</code> </p>
-->

次の場合：

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

発生したコストは、実際のコストが 0 より大きい費用です

```
Planned Cost of Incurred Expenses = Total of Planned Cost of all incurred expenses
```



<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Old calculation - taken out by Lilit and replaced below: Planned Cost of Work Performed= (planned labor cost) * (percent complete) / 100 where planned labor cost is the planned hours allocated to assignees * their rates.)</p>
  -->

* 作業実行の予算は、次の式で計算されます。

  ```
  Planned Cost of Work Performed = Planned cost * Percent Complete / 100
  ```

作業実行の予算（BCWP）合計は、次の項目に対して計算されます。

* **親タスク以外の場合：**

  ```
  Total Budgeted Cost Work Performed = Planned Labor Cost * Percent Complete / 100
  ```

* **親タスクの場合：**

  ```
  Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field from all direct child tasks)
  ```

* **プロジェクトの場合：**

  ```
  Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field for all top-level tasks)
  ```



## プロジェクトまたはタスクで CPI を見つける

プロジェクトまたはタスクの CPI は、プロジェクト、タスクリストまたはレポートに表示できます。 また、プロジェクトレベルまたはタスクレベルで表示できます。

1. CPI を表示するプロジェクトまたはタスクに移動します。
1. プロジェクトまたはタスクの CPI を表示しているかどうかに応じて、左側のパネルで&#x200B;**プロジェクトの詳細**&#x200B;または&#x200B;**タスクの詳細**&#x200B;を展開します。

1. **財務** をクリックします。 CPI は「**CPI／SPI／CSI**」フィールドを表示します。

   ![ プロジェクトの CPI](assets/cpi-on-project-nwe.png)
