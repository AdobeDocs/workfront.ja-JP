---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: 計算の例 - タスクからのロールアップとして EAC を計算
description: PIM = 時間ベース
author: Alina
feature: Work Management
exl-id: 68b582c9-f72a-4000-9d28-f7dafa23541f
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: ht
source-wordcount: '873'
ht-degree: 100%

---

# 計算の例 - タスクからのロールアップとして EAC を計算

## EAC メソッド：タスクやサブタスクからのロールアップ

* [PIM = 時間ベース](#pim-hour-based)
* [PIM = コストベース](#pim-cost-based)

### PIM = 時間ベース {#pim-hour-based}

* [簡単な例：プロジェクトに子タスクがない](#simple-example-project-has-no-children-tasks)
* [複雑な例：プロジェクトに子タスクがある](#complicated-example-project-has-children-tasks)

#### 簡単な例：プロジェクトに子タスクがない {#simple-example-project-has-no-children-tasks}

PIM = 時間ベース

EAC メソッド = タスクやサブタスクからのロールアップ

1. すべてのタスクがユーザー 1（コスト/時間が $100.00）に割り当てられた、3 つのタスク（子タスクなし）を持つプロジェクト A を作成します。
1. 下の表に従って、それぞれのタスクと完了率（%）に予定時間数と実際の時間数を追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>タスク</strong> </p> </th> 
   <th> <br> <p><strong>予定時間数</strong> </p> </th> 
   <th> <br> <p><strong>実時数</strong> </p> </th> 
   <th> <p><strong>完了率</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>タスク 1</p> </td> 
   <td> <p>5 時間</p> </td> 
   <td> <p>25 時間</p> </td> 
   <td> <p>20％</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 2</p> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>25 時間</p> </td> 
   <td> <p>30％</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 3</p> </td> 
   <td> <p>15 時間</p> </td> 
   <td> <p>25 時間</p> </td> 
   <td> <p>40％</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 財務を再計算
1. **タスク 1 の CPI** = .04 は以下のように計算されます。\
   **タスク 1 の CPI** = *IF* 実際の時間 > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/実際の時間\
   *ELSE* CPI = 1\
   **タスク 1 の CPI** = 1 / 25\
   **タスク 1 の CPI** = .04

1. **タスク 1 の EAC** = 125 時間は、以下のように計算されます。\
   **タスク 1 の EAC** = *IF* CPI &lt;> 0 *THEN* EAC = 予定時間数/CPI\
   *ELSE*

   ```
   EAC = Planned  Hours + Actual  Hours
   ```

   **タスク 1 の EAC** = 5 / .04\
   **タスク 1 の EAC** = 125 時間

1. タスク 2 とタスク 3 の CPI / EAC は以下の通りです。\
   タスク 2 = .12 / 83.33 時間\
   タスク 3 = .24 / 62.5 時間

1. **プロジェクトの CPI** = .13 は以下のように計算されます。\
   **プロジェクトの CPI** = *IF* 実際の時間数 > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

   *ELSE* CPI = 1\
   **プロジェクトの CPI** = 10 / 75\
   **プロジェクトの CPI** = .13

1. **プロジェクトの EAC** = 270.83 時間は以下のように計算されます。\
   **プロジェクトの EAC** = EAC タスク 1 + EAC タスク 2 + EAC タスク 3\
   **プロジェクトの EAC** = 125 + 83.33 + 62.5\
   **プロジェクトの EAC** = 270.83 時間

#### 複雑な例：プロジェクトに子タスクがある {#complicated-example-project-has-children-tasks}

PIM = 時間ベース

EAC メソッド = タスクやサブタスクからのロールアップ

1. 以下に示すように、プロジェクト A（6 つのタスクを持ち、タスク 3 が タスク 4 とタスク 5 の親、タスク 1 が タスク 2 とタスク 3 の親である）を作成します。\
   タスク 1\
   タスク 2\
   タスク 3\
   タスク 4\
   タスク 5\
   タスク 6

1. コスト/時間レートが $100.00 のユーザー 1 にタスク 2、4、5、6 を割り当てます。
1. 下の表に従って、それぞれのタスクと完了率（%）に予定時間数と実際の時間数を追加します。

   >[!NOTE]
   >
   >タスク 1 および 3 には、実際の時間数のみを追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>タスク</strong> </p> </th> 
   <th> <br> <p><strong>予定時間数</strong> </p> </th> 
   <th> <br> <p><strong>実時数</strong> </p> </th> 
   <th> <p><strong>完了率</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>タスク 1</p> </td> 
   <td> </td> 
   <td> <p>10 時間</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 2</p> </td> 
   <td> <p>5 時間</p> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>20％</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 3</p> </td> 
   <td> </td> 
   <td> <p>10 時間</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 4</p> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>40％</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 5</p> </td> 
   <td> <p>15 時間</p> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>50％</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 6</p> </td> 
   <td> <p>20 時間</p> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>60％</p> </td> 
  </tr> 
 </tbody> 
</table>

1. プロジェクトに 50 時間を直接追加し（その他／時間数／時間数を記録）し、実際の労力コストの 5,000.00 ドルがプロジェクトに直接記録されるようにします。
1. 財務の再計算を実行
1. **タスク 2 の CPI** = .1 は以下のように計算されます。\
   **タスク 2 の CPI** = *IF* 実際の時間数 > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

   *ELSE* CPI = 1\
   **タスク 2 の CPI** = 1 / 10\
   **タスク 2 の CPI** = .1

1. **タスク 2 の EAC** = 50 時間は次のように計算されます。\
   **タスク 2 の EAC** = *IF* CPI &lt;> 0 *THEN*

   ```
   EAC = Planned Hours / CPI
   ```

   *ELSE* EAC = 予定時間数 + 実際の時間数\
   **タスク 2 の EAC** = 5 / .1\
   **タスク 2 の EAC** = 50 時間

1. タスク 4、タスク 5 およびタスク 6 の CPI / EAC は次のとおりです。\
   タスク 4 = .4 / 25 時間\
   タスク 5 = .75 / 20 時間\
   タスク 6 = 1.2 / 16.67 時間

1. **タスク 3 の CPI** = .38\
   **タスク 3 の CPI** = *IF*&#x200B;実際の時間数 > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **タスク 3 の CPI** = 11.5 / 30\
   **タスク 3 の CPI** = .38

1. **タスク 3 の EAC** = EAC タスク 4 + EAC タスク 5\
   **タスク 3 の EAC** = 25 + 20\
   **タスク 3 の EAC** = 45 時間

1. **タスク 1 の CPI** = .25 は、次のように計算されます。\
   **タスク 1 の CPI** = *IF* 実際の時間数 > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **タスク 1 の CPI** = 12.5 / 50\
   **タスク 1 の CPI** = .25

1. **タスク 1 の EAC** = EAC タスク 2 + EAC タスク 3\
   **タスク 1 の EAC** = 50 + 45\
   **タスク 1 の EAC** = 95 時間

1. プロジェクトの CPI = .22 は、次のように計算されます。\
   **プロジェクトの CPI** = *IF* 実際の時間数 > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **プロジェクトの CPI** = 24.5 / 110\
   **プロジェクトの CPI** = .22272\
   **プロジェクトの CPI** = .22

1. **プロジェクトの EAC** = EAC タスク 1 + EAC タスク 6\
   **プロジェクトの EAC** = 95 + 16.67\
   **プロジェクトの EAC** = 111.67 時間

### PIM = コストベース {#pim-cost-based}

* [簡単な例：プロジェクトに子タスクがない](#simple-example-project-has-no-children-tasks)

#### 簡単な例：プロジェクトに子タスクがない {#simple-example-project-has-no-children-tasks-1}

PIM = コストベース

EAC メソッド = タスクやサブタスクからのロールアップ

1. 3 つのタスク（子タスクなし）を持つプロジェクト A を作成し、すべてのタスクを 1 時間当たりのコスト 100.00 ドルのユーザー 1 に割り当てます。
1. 下の表に従って、それぞれのタスクと完了率（%）に予定時間数と実際の時間数を追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>タスク</strong> </p> </th> 
   <th> <br> <p><strong>予定時間数</strong> </p> </th> 
   <th> <br> <p><strong>予定労力コスト</strong> </p> </th> 
   <th> <br> <p><strong>実時数</strong> </p> </th> 
   <th> <br> <p><strong>実際の労力コスト</strong> </p> </th> 
   <th> <p><strong>完了率（％）</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>タスク 1</p> </td> 
   <td> <p>5 時間</p> </td> 
   <td> <p>500.00 ドル</p> </td> 
   <td> <p>25 時間</p> </td> 
   <td> <p>2,500.00 ドル</p> </td> 
   <td> <p>20％</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 2</p> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>1,000.00 ドル</p> </td> 
   <td> <p>25 時間</p> </td> 
   <td> <p>2,500.00 ドル</p> </td> 
   <td> <p>30％</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 3</p> </td> 
   <td> <p>15 時間</p> </td> 
   <td> <p>1,500.00 ドル</p> </td> 
   <td> <p>25 時間</p> </td> 
   <td> <p>2,500.00 ドル</p> </td> 
   <td> <p>40％</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 次の表に従って、各タスクに費用を追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>タスク</strong> </p> </th> 
   <th> <p><strong>費用</strong> </p> </th> 
   <th> <p><strong>予定金額</strong> </p> </th> 
   <th> <p><strong>実際の金額</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>タスク 1</p> </td> 
   <td> <p>タスク 1 費用 1</p> </td> 
   <td> <p>300.00 ドル</p> </td> 
   <td> <p>400.00 ドル</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 1</p> </td> 
   <td> <p>タスク 1 費用 2</p> </td> 
   <td> <p>500.00 ドル</p> </td> 
   <td> <p>0.00 ドル</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 2</p> </td> 
   <td> <p>タスク 2 費用</p> </td> 
   <td> <p>200.00 ドル</p> </td> 
   <td> <p>100.00 ドル</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 3</p> </td> 
   <td> <p>タスク 3 費用</p> </td> 
   <td> <p>800.00 ドル</p> </td> 
   <td> <p>700.00 ドル</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 次のように、2 つの費用をプロジェクトに追加します（つまり、タスクに紐付けられていません）。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>費用</strong> </p> </th> 
   <th> <p><strong>予定金額</strong> </p> </th> 
   <th> <p><strong>実際の金額</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>プロジェクト費用 1</p> </td> 
   <td> <p>1,000.00 ドル</p> </td> 
   <td> <p>1,500.00 ドル</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 1 費用 2</p> </td> 
   <td> <p>2,500.00 ドル</p> </td> 
   <td> <p>0.00 ドル</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 上記の値に基づいて、「発生コスト」と「未発生コスト」は次のように決定されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>タスク</strong> </p> </th> 
   <th> <p><strong>未発生の予定費用</strong> </p> </th> 
   <th> <p><strong>発生した予定費用</strong> </p> </th> 
   <th> <p><strong>発生した実際の費用</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>タスク 1</p> </td> 
   <td> <p>500.00 ドル</p> </td> 
   <td> <p>300.00 ドル</p> </td> 
   <td> <p>400.00 ドル</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 2</p> </td> 
   <td> <p>0.00 ドル</p> </td> 
   <td> <p>200.00 ドル</p> </td> 
   <td> <p>100.00 ドル</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 3</p> </td> 
   <td> <p>0.00 ドル</p> </td> 
   <td> <p>800.00 ドル</p> </td> 
   <td> <p>700.00 ドル</p> </td> 
  </tr> 
  <tr> 
   <td> <p>プロジェクト</p> </td> 
   <td> <p>$3,000.00</p> </td> 
   <td> <p>$2,300.00</p> </td> 
   <td> <p>$2,700.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 「プロジェクトアクション」から「財務の再計算」を実行します。
1. **タスク 1 の CPI****** = .14 は以下のように計算されます。\
   **タスク 1 の CPI****** = *IF* 実際の労力コスト + OpcedsActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *ELSE* CPI = CPI_Labor\
   **タスク 1 の CPI****** = (100+300) / (2500+400)\
   **タスク 1 の CPI****** = 400 / 2900\
   **タスク 1 の CPI****** = .14

1. **タスク 1 の EAC****** = 13,400.00 ドル\
   **タスク 1 の CPI 労力****** = IF 実際の労力コスト &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

   ELSE CPI_Labor = 1\
   **タスク 1 の CPI 労力****** = 100/2500\
   **タスク 1 の CPI 労力****** = .04

   **タスク 1 の EAC 労力****** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *ELSE* EAC 労力 = 予定労力コスト + 実際の労力コスト\
   **タスク 1 の EAC 労力****** = 500.00/.04\
   **タスク 1 の EAC 労力****** = 12,500.00 ドル

   **タスク 1 の EAC 費用****** = OccedsActualExpenseCost + NotOccededPlannedExpense\
   **タスク 1 の EAC 費用****** = 400.00 ドル + 500.00 ドル\
   **タスク 1 の EAC 費用****** = 900.00 ドル

   **タスク 1 の EAC****** = EAC 労力 + EAC 費用\
   **タスク 1 の EAC****** = 12,500.00 ドル + 900.00 ドル\
   **タスク 1 の EAC****** = 13,400.00 ドル

1. タスク 2 とタスク 3 の CPI/EAC 値は以下の通りです。\
   タスク 2 = .19 / $8,433.33\
   タスク 3 = .44 / 6,950.00 ドル****

1. プロジェクトの CPI = .32\
   **プロジェクトの CPI****** = *IF* 労力コスト + OpcedsActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *ELSE* CPI = CPI_Labor\
   **プロジェクトの CPI****** = (1000 + 2300) / (7500 + 2700)\
   **プロジェクトの CPI****** = 3300 / 10200\
   **プロジェクトの CPI****** = .32

1. プロジェクトの EAC は 28,783.33 ドル\
   **プロジェクトの EAC****** = EAC タスク 1 + EAC タスク 2 + EAC タスク 3\
   **プロジェクトの EAC****** = 13,400.00 ドル + 8,433.33 ドル + 6,950.00 ドル\
   **プロジェクトの EAC****** = 28,783.33 ドル
