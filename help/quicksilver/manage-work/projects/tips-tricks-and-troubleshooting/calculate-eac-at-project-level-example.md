---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: 計算例 - プロジェクトレベルで EAC を計算
description: PIM = 時間ベース
author: Alina
feature: Work Management
exl-id: ff88b7e3-2a5b-464f-bed1-6848067840b8
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: ht
source-wordcount: '1768'
ht-degree: 100%

---

# 計算例 - プロジェクトレベルで EAC を計算

## EAC メソッド：プロジェクトレベルで計算

* [PIM = 時間ベース](#pim-hour-based)
* [PIM = コストベース](#pim-cost-based)

### PIM = 時間ベース {#pim-hour-based}

* [簡単な例：プロジェクトに子タスクがない](#simple-example-project-has-no-children-tasks)
* [複雑な例：プロジェクトに子タスクがある](#complicated-example-project-has-children-tasks)

#### 簡単な例：プロジェクトに子タスクがない {#simple-example-project-has-no-children-tasks}

PIM = 時間ベース

EAC メソッド = プロジェクトレベルで計算****

1. すべてのタスクがユーザー 1（コスト/時間が $100.00）に割り当てられた、3 つのタスク（子タスクなし）を持つプロジェクト A を作成します。
1. 下の表に従って、それぞれのタスクと完了率（%）に予定時間数と実際の時間数を追加します。

   <table style="table-layout:auto">
    <col>
    <col>
    <col>
    <col>
    <thead>
     <tr>
      <th><br><p><strong>タスク</strong></p></th>
      <th><br><p><strong>予定時間数</strong></p></th>
      <th><br><p><strong>実際の時間数</strong></p></th>
      <th><p><strong>完了率（％）</strong></p></th>
     </tr>
    </thead>
    <tbody>
     <tr>
      <td><p>タスク 1</p></td>
      <td><p>5 時間</p></td>
      <td><p>25 時間</p></td>
      <td><p>20％</p></td>
     </tr>
     <tr>
      <td><p>タスク 2</p></td>
      <td><p>10 時間</p></td>
      <td><p>25 時間</p></td>
      <td><p>30％</p></td>
     </tr>
     <tr>
      <td><p>タスク 3</p></td>
      <td><p>15 時間</p></td>
      <td><p>25 時間</p></td>
      <td><p>40％</p></td>
     </tr>
    </tbody>
   </table>

1. プロジェクトの財務を再計算します。
1. **タスク 1 の CPI** = .04 は以下のように計算されます。\
   **タスク 1 の CPI** = *IF* 実際の時間数 > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/実際の時間数\
   *ELSE* CPI = 1\
   **タスク 1 の CPI** = 1 / 25\
   **タスク 1 の CPI** = .04

1. **タスク 1 の EAC** = 125 時間は以下のように計算されます。\
   **タスク 1 の EAC** = *IF* CPI &lt;> 0 *THEN* EAC = 予定時間数/CPI\
   *ELSE* EAC = 予定時間数 + 実際の時間数\
   **タスク 1 の EAC** = 5 / .04\
   **タスク 1 の EAC** = 125 時間****

1. タスク 2 とタスク 3 の CPI / EAC は以下の通りです。\
   タスク 2 = .12 / 83.33 時間\
   タスク 3 = .24 / 62.5 時間

1. **プロジェクトの CPI** = .13 は以下のように計算されます。\
   **プロジェクトの CPI** = *IF* 実際の時間数 > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/実際の時間数\
   *ELSE* CPI = 1\
   **プロジェクトの CPI** = 10 / 75\
   **プロジェクトの CPI** = .13

1. **プロジェクトの EAC** = 225 時間は以下のように計算されます。\
   **プロジェクトの EAC** = *IF* CPI &lt;> 0 *THEN* EAC = 予定時間数/CPI\
   *ELSE* EAC = 予定時間数 + 実際の時間数\
   **プロジェクトの EAC** = 30 / .13333\
   **プロジェクトの EAC** = 225 時間

#### 複雑な例：プロジェクトに子タスクがある {#complicated-example-project-has-children-tasks}

PIM = 時間ベース

EAC メソッド = プロジェクトレベルで計算

1. 以下に示すように、プロジェクト A（6 つのタスクを持ち、タスク 3 が タスク 4 とタスク 5 の親、タスク 1 が タスク 2 とタスク 3 の親である）を作成します。\
   タスク 1\
   タスク 2\
   タスク 3\
   タスク 4\
   タスク 5\
   タスク 6

1. コスト/時間レートが $100.00 のユーザー 1 にタスク 2、4、5、6 を割り当てます。
1. 下の表に従って、それぞれのタスクと完了率（％）に予定時間数と実際の時間数を追加します。

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
   <th> <br> <p><strong>実際の時間数</strong> </p> </th> 
   <th> <p><strong>完了率（％）</strong> </p> </th> 
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

1. プロジェクトに 50 時間を直接追加します（その他／時間／時間の記録）。
1. **タスク 2 の CPI** = .1 は以下のように計算されます。\
   **タスク 2 の CPI** = *IF* 実際の時間数 > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/実際の時間数\
   *ELSE* CPI = 1\
   **タスク 2 の CPI** = 1 / 10\
   **タスク 2 の CPI** = .1

1. **タスク 2 の EAC** = 50 時間は以下のように計算されます。\
   **タスク 2 の EAC** = *IF* CPI &lt;> 0 *THEN* EAC = 予定時間数/CPI\
   *ELSE* EAC = 予定時間数 + 実際の時間数\
   **タスク 2 の EAC** = 5 / .1\
   **タスク 2 の EAC** = 50 時間

1. タスク 4、5、6 の CPI/EAC は以下のとおりです。\
   タスク 4：.4 / 25 時間\
   タスク 5：.75 / 20 時間\
   タスク 6：1.2 / 16.67 時間

1. **タスク 3 の CPI** = .38 は以下のように計算されます。\
   **タスク 3 の CPI** = *IF* 実際の時間数 > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/実際の時間数\
   *ELSE* CPI = 1\
   **タスク 3 の CPI** = 11.5 / 30\
   **タスク 3 の CPI** = .38

1. **タスク 3 の EAC** = 65.22 時間は以下のように計算されます。\
   **タスク 3 の EAC** = *IF* CPI &lt;> 0 *THEN* EAC = 予定時間数/CPI\
   *ELSE* EAC = 予定時間数 + 実際の時間数\
   **タスク 3 の EAC** = 25 / .383333\
   **タスク 3 の EAC** = 65.22 時間

1. **タスク 1 の CPI** = .25 は以下のように計算されます。\
   **タスク 1 の CPI** = *IF* 実際の時間数 > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/実際の時間数\
   *ELSE* CPI = 1\
   **タスク 1 の CPI** = 12.5 / 50\
   **タスク 1 の CPI** = .25

1. **タスク 1 の EAC** = 120 時間は以下のように計算されます。\
   **タスク 1 の EAC** = *IF* CPI &lt;> 0 *THEN* EAC = 予定時間数/CPI\
   *ELSE* EAC = 予定時間数 + 実際の時間数\
   **タスク 1 の EAC** = 30/.25\
   **タスク 1 の EAC** = 120 時間

1. **プロジェクトの CPI** = .22 は以下のように計算されます。\
   **プロジェクトの CPI** = *IF* 実際の時間数 > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/実際の時間数\
       *ELSE* CPI = 1\
   **プロジェクトの CPI** = 24.5 / 110\
   **プロジェクトの CPI** = .22272\
   **プロジェクトの CPI** = .22

1. **プロジェクトの EAC** = 224.49 時間は以下のように計算されます。\
   **プロジェクトの EAC** = *IF* CPI &lt;> 0 *THEN* EAC = 予定時間数/CPI\
       *ELSE* EAC = 予定時間数 + 実際の時間数\
   **プロジェクトの EAC** = 50 / .22272\
   **プロジェクトの EAC** = 224.49 時間

### PIM = コストベース {#pim-cost-based}

* [簡単な例：プロジェクトに子タスクがない](#simple-example-project-has-no-children-tasks)
* [複雑な例：プロジェクトに子タスクがある](#complicated-example-project-has-children-tasks)

#### 簡単な例：プロジェクトに子タスクがない {#simple-example-project-has-no-children-tasks-1}

PIM = コストベース

EAC メソッド = プロジェクトレベルで計算

1. すべてのタスクがユーザー 1（コスト/時間が $100.00）に割り当てられた、3 つのタスク（子タスクなし）を持つプロジェクト A を作成します。
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
   <th> <p><strong>完了率</strong> </p> </th> 
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
   <td> <p> $2,700.00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. 「プロジェクトアクション」から「財務の再計算」を実行します。
1. **タスク 1 の CPI** = .14
1. **タスク 1 の CPI****** = .14 は以下のように計算されます。\
   **タスク 1 の****CPI** = *IF* 実際の労力コスト + OpcedsActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *ELSE* CPI = CPI_Labor\
   **タスク 1 の CPI****** = (100+300) / (2500+400)\
   **タスク 1 の****CPI** = 400 / 2900\
   **タスク 1 の****CPI** = .14****

1. **タスク 1 の EAC****** = $13,400.00\
   **タスク 1 の****CPI 労力** = 実際の労力コスト &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

   ELSE CPI_Labor = 1\
   **タスク 1 の****CPI 労力** = 100/2500\
   **タスク 1 の****CPI 労力** = .04 **********タスク 1 の&#x200B;**EAC 労力 =*IF *CPI_Labor &lt;> 0*THEN *EAC 労力 = 予定労力コスト/CPI_Labor\
   *ELSE* EAC 労力 = 予定労力コスト + 実際の労力コスト\
   タスク 1**の**EAC 労力&#x200B;****= 500.00/.04 の場合\
   **タスク 1 の EAC 労力****** = $12,500.00\
   **タスク 1 の EAC****費用** = OccedsActualExpenseCost + NotOccededPlannedExpense\
   **タスク 1 の EAC****費用** = $400.00 + $500.00\
   **タスク 1 の EAC****費用** = $900.00 の場合\
   **タスク 1 の EAC****** = EAC 労力 + EAC 費用\
   **タスク 1 の EAC****** = $12,500.00 + $900.00\
   **タスク 1 の EAC****** = $13,400.00

1. タスク 2 とタスク 3 の CPI/EAC 値は以下の通りです。\
   タスク 2 = .19 / $8,433.33\
   タスク 3 = .44 / $6,950.00

1. **プロジェクトの CPI** = .32 は以下のように計算されます。\
   **プロジェクトの CPI****** = *IF* 実際の労力コスト + OpcedsActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/ActualLaborCost + IncurredActualExpenseCost)
   ```

   *ELSE* CPI = CPI_Labor\
   **プロジェクトの CPI****** = (1000 + 2300) / (7500 + 2700)\
   **プロジェクトの CPI****** = 3300 / 10200\
   **プロジェクトの CPI****** = .32

1. **プロジェクトの EAC** = $28,200.00 は以下のように計算されます。\
   **プロジェクトの CPI 労力****** = 実際の労力コスト &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

   ELSE CPI_Labor = 1\
   **プロジェクトの CPI 労力****** = 1000 / 7500\
   **プロジェクトの CPI 労力****** = .13333\
   **プロジェクトの CPI 労力****** = .13

   **プロジェクトの EAC労力****** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *ELSE* EAC 労力 = 予定労力コスト + 実際の労力コスト\
   **プロジェクトの EAC 労力****** = 3000/ .13333\
   **プロジェクトの EAC 労力****** = $22,500.00

   **EAC 費用****プロジェクト** =

   ```
   IncurredActualExpenseCost + NotIncurredPlannedExpense
   ```

   **EAC 費用****プロジェクト** = $3,000.00 + 2,700.00\
   **EAC 費用****プロジェクト** = $5,700.00

   **EAC****プロジェクト** = EAC 労力 + EAC 費用\
   **EAC****プロジェクト** = $22,500.00 + $5,700.00\
   **EAC****プロジェクト** = $28,200.00

#### 複雑な例：プロジェクトに子タスクがある {#complicated-example-project-has-children-tasks-1}

PIM = コストベース

EAC メソッド = プロジェクトレベルで計算

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
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>タスク</strong> </p> </th> 
   <th> <br> <p><strong>予定時間数</strong> </p> </th> 
   <th> <br> <p><strong>予定労力コスト</strong> </p> </th> 
   <th> <br> <p><strong>実際の時間数</strong> </p> </th> 
   <th> <br> <p><strong>実際の労力コスト</strong> </p> </th> 
   <th> <p><strong>完了率（％）</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>タスク 1</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>1,000.00 ドル</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 2</p> </td> 
   <td> <p>5 時間</p> </td> 
   <td> <p>500.00 ドル</p> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>1,000.00 ドル</p> </td> 
   <td> <p>20％</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 3</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>1,000.00 ドル</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 4</p> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>1,000.00 ドル</p> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>1,000.00 ドル</p> </td> 
   <td> <p>40％</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 5</p> </td> 
   <td> <p>15 時間</p> </td> 
   <td> <p>1,500.00 ドル</p> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>1,000.00 ドル</p> </td> 
   <td> <p>50％</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 6</p> </td> 
   <td> <p>20 時間</p> </td> 
   <td> <p>$2,000.00</p> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>1,000.00 ドル</p> </td> 
   <td> <p>60％</p> </td> 
  </tr> 
 </tbody> 
</table>

1. プロジェクトに 50 時間を直接追加し（その他／時間数／時間数を記録）し、実際の労力コストの 5,000.00 ドルがプロジェクトに直接記録されるようにします。****
1. 以下の表に従って、各タスクに費用を追加します（読みやすくするために、各タスクの間に空白行を追加しました）。

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
   <td> <p>-$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 1</p> </td> 
   <td> <p>タスク 1 費用 2</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>800.00 ドル</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 1</p> </td> 
   <td> <p>タスク 1 費用 3</p> </td> 
   <td> <p>400.00 ドル</p> </td> 
   <td> <p>0.00 ドル</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 2</p> </td> 
   <td> <p>タスク 2 費用 1</p> </td> 
   <td> <p>500.00 ドル</p> </td> 
   <td> <p>700.00 ドル</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 2</p> </td> 
   <td> <p>タスク 2 費用 2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>0.00 ドル</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 2</p> </td> 
   <td> <p>タスク 2 費用 3</p> </td> 
   <td> <p>-$200.00</p> </td> 
   <td> <p>$600.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 2</p> </td> 
   <td> <p>タスク 2 費用 4</p> </td> 
   <td> <p>700.00 ドル</p> </td> 
   <td> <p>-$200.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 3</p> </td> 
   <td> <p>タスク 3 費用</p> </td> 
   <td> <p>0.00 ドル</p> </td> 
   <td> <p>1,000.00 ドル</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 4</p> </td> 
   <td> <p>タスク 4 費用 1</p> </td> 
   <td> <p>800.00 ドル</p> </td> 
   <td> <p>0.00 ドル</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 4</p> </td> 
   <td> <p>タスク 4 費用 2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>300.00 ドル</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 4 </p> </td> 
   <td> <p>タスク 4 費用 3</p> </td> 
   <td> <p>-200.00</p> </td> 
   <td> <p>0.00 ドル</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 5</p> </td> 
   <td> <p>タスク 5 費用 1</p> </td> 
   <td> <p>700.00 ドル</p> </td> 
   <td> <p>800.00 ドル</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 5</p> </td> 
   <td> <p>タスク 5 費用 2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>300.00 ドル</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 5</p> </td> 
   <td> <p>タスク 5 費用 3</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>-$200.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 6</p> </td> 
   <td> <p>タスク 6 費用 1</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>700.00 ドル</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 6</p> </td> 
   <td> <p>タスク 6 費用 2</p> </td> 
   <td> <p>500.00 ドル</p> </td> 
   <td> <p>-$300.0</p> </td> 
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
   <td> <p> 0.00 ドル <strong></strong></p> </td> 
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
   <th> <p><strong>未発生の予定コスト</strong> </p> </th> 
   <th> <p><strong>発生した予定コスト</strong> </p> </th> 
   <th> <p><strong>発生した実際の費用</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>タスク 1</p> </td> 
   <td> <p>400.00 ドル</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>800.00 ドル</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>300.00 ドル</p> </td> 
   <td> <p>$1,300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 3</p> </td> 
   <td> <p>0.00 ドル</p> </td> 
   <td> <p>0.00 ドル</p> </td> 
   <td> <p>1,000.00 ドル</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 4</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>300.00 ドル</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 5</p> </td> 
   <td> <p>0.00 ドル</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$1,100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 6</p> </td> 
   <td> <p>0.00 ドル</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>700.00 ドル</p> </td> 
  </tr> 
  <tr> 
   <td> <p>プロジェクト</p> </td> 
   <td> <p>2,500.00 ドル</p> </td> 
   <td> <p>$1000.00</p> </td> 
   <td> <p>1,500.00 ドル</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 「プロジェクトアクション」から「財務の再計算」を実行します。
1. タスク 2 の **CPI** = .17 は以下のように計算されます。\
   **CPI タスク 2** = *IF* 実際の労力コスト + IncurredActualExpenseCost  &lt;> 0 *THEN* CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)\
   *   ELSE* CPI = CPI_Labor\
   **CPI****タスク 2** = (100+300) / (1000+1300)\
   **CPI****タスク 2**  = 400 / 2300\
   **CPI****タスク 2**  = .17

1. タスク 2 の **EAC** = $5,900.00\
   **CPI 労力****タスク 2** = IF 実際の労力コスト &lt;> 0 THEN CPI_Labor = TotalBudgetedCostWorkPerformed / 実際の労力コスト\
   ELSE CPI_Labor = 1\
   **CPI 労力****タスク 2** = 100/1000\
   **CPI 労力****タスク 2** = .1

   **EAC 労力****タスク 2** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC  Labor = 予定労力コスト + 実際の労力コスト\
   **EAC 労力****タスク 2** = 500.00/.1\
   **EAC 労力****タスク 2** = $5,000.00 ****** EAC 費用&#x200B;****タスク 2 **= IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **EAC 費用&#x200B;****タスク 2** = $1,300.00 + -$400.00\
   **EAC 費用****タスク 2** = $900.00

   **EAC****タスク 2** = EAC 労力+ EAC 費用\
   **EAC****タスク 2**  = $5,000.00 + $900.00\
   **EAC****タスク 2**  = $5,900.00

1. タスク 4、5、6 の CPI/EAC は同じ方法で決定されるので、ここでは値だけを以下に示します。\
   タスク 4：.23 / $3,400.00\
   タスク 5：.64 / $3,100.00\
   タスク 6：1.06 / $2,366.67

1. タスク 3 の CPI = .31 は以下のように計算されます。\
   **CPI****タスク 3** = *IF* 実際の労力コスト + IncurredActualExpenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****タスク 3**  = (1,150 + 500) / (3000 + 2400)\
   **CPI****タスク 3**  =  1650 / 5400\
   **CPI****タスク 3**  = .31 ******&#x200B;タスク 3 のEAC **= $9,521.74 は以下のように計算されます。\
   **CPI 労力&#x200B;****タスク 3** = IF 実際の労力コスト &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

   ELSE CPI_Labor = 1\
   **CPI 労力****タスク 3** = 1150/3000\
   **CPI 労力****タスク 3** = .383333\
   **CPI 労力****タスク 3** = .38

   **EAC 労力****タスク 3** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC  Labor = 予定労力コスト + 実際の労力コスト\
   **EAC 労力****タスク 3** = $2,500.00 / .383333\
   **EAC 労力****タスク 3** = 6,521.74 ドル

   **EAC 費用****タスク 3** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **EAC 費用****タスク 3** = 2,400.00 ドル + 600.00 ドル\
   **EAC 費用****タスク 3** = 3,000.00 ドル

   **EAC****タスク 3** = EAC 労力 + EAC 費用\
   **EAC****タスク 3**  = 6,521.74 ドル + 3,000.00 ドル\
   **EAC****タスク 3**  = 9,521.74 ドル

1. 以下の計算のとおり、タスク 1 の CPI = .16 になります。\
   **CPI****タスク 1** = *IF* 実際の労力コスト + IncurredActualExpenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****タスク 1**  = (1250 + 300) / (5000 + 4500)\
   **CPI****タスク 1**  =  1550 / 9500=\
   **CPI****タスク 1**  = .16

1. 以下の計算のとおり、タスク 1 の EAC は 17,100.00 ドルになります。\
   **CPI 労力****タスク 1** = IF 実際の労力コスト &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

   ELSE CPI_Labor = 1\
   **CPI 労力****タスク 1** = 1250 / 5000\
   **CPI 労力****タスク 1** = .25

   **EAC 労力****タスク 1** = *IF* CPI_Labor &lt;> 0 *THEN* EAC 労力 = 予定労力コスト / CPI_Labor\
   *   ELSE* EAC 労力 = 予定労力コスト + 実際の労力コスト\
   **EAC 労力****タスク 1** = 3,000.00 ドル / .25\
   **EAC 労力****タスク 1** = 12,000.00 ドル

   **EAC 費用****タスク 1** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **EAC 費用****タスク 1** = 4500 ドル + 600\
   **EAC 費用****タスク 1** = 5,100.00 ドル

   **EAC****タスク 1** = EAC 労力 + EAC 費用\
   **EAC****タスク 1**  = 12,000.00 ドル + 5,100.00\
   **EAC****Task 1**  = 17,100.00 ドル

1. プロジェクトの CPI は .25 になります。\
   **CPI****プロジェクト** = *IF* 実際の労力コスト + IncurredActualExpenseCost  &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor

   **CPI****プロジェクト** = (2450 + 1900) / (11000 + 6700)\
   **CPI****プロジェクト** = 4350 / 17700\
   **CPI****プロジェクト** = .25

1. 以下の計算のとおり、**プロジェクトの EAC** = 32,248.98 ドルになります。\
   **CPI 労力****プロジェクト** = IF 実際の労力コスト &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

   ELSE CPI_Labor = 1\
   **CPI 労力****プロジェクト** = 2450 / 11000\
   **CPI 労力****プロジェクト** = .22272\
   **CPI 労力****プロジェクト** = .22

   **EAC 労力****プロジェクト** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC 労力 = 予定労力コスト + 実際の労力コスト\
   **EAC 労力****プロジェクト** = 5,000.00 ドル / .22272\
   **EAC 労力****プロジェクト** = 22,448.97959 ドル\
   **EAC 労力****プロジェクト** = 22,448.98 ドル

   **EAC 費用****プロジェクト** = IncurredActualExpenseCost + NotIncurredPlannedExpense\
   **EAC 費用****プロジェクト** = 3,100.00 ドル + 6,700.00 ドル\
   **EAC 費用****プロジェクト** = 9,800.00 ドル

   **EAC****プロジェクト** = EAC 労力 + EAC 費用\
   **EAC****プロジェクト** = 22,448.98 ドル + 9,800.00\
   **EAC****プロジェクト** = $32,248.98
