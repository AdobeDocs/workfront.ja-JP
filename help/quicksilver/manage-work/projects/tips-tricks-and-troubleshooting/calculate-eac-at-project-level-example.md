---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: 計算の例 — プロジェクトレベルでの EAC の計算
description: PIM =時間ベース
author: Alina
feature: Work Management
exl-id: ff88b7e3-2a5b-464f-bed1-6848067840b8
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1768'
ht-degree: 9%

---

# 計算の例 — プロジェクトレベルでの EAC の計算

## EAC メソッド：プロジェクトレベルで計算

* [PIM =時間ベース](#pim-hour-based)
* [PIM=コストベース](#pim-cost-based)

### PIM =時間ベース {#pim-hour-based}

* [簡単な例：プロジェクトに子タスクがありません](#simple-example-project-has-no-children-tasks)
* [複雑な例：プロジェクトに子タスクがあります](#complicated-example-project-has-children-tasks)

#### 簡単な例：プロジェクトに子タスクがありません {#simple-example-project-has-no-children-tasks}

PIM =時間ベース

EAC メソッド=プロジェクトレベルで計算****

1. 3 つのタスク（子タスクなし）を持つプロジェクト A を作成し、すべてのタスクが 100.00 ドルのコストを持つユーザー 1 に割り当てます。
1. 次の表に従って、各タスクに計画時間と実績時間を追加し、完了率を%にします。

   <table style="table-layout:auto">
    <col>
    <col>
    <col>
    <col>
    <thead>
     <tr>
      <th><br><p><strong>タスク</strong></p></th>
      <th><br><p><strong>予定時間数</strong></p></th>
      <th><br><p><strong>実時数</strong></p></th>
      <th><p><strong>完了率</strong></p></th>
     </tr>
    </thead>
    <tbody>
     <tr>
      <td><p>タスク 1</p></td>
      <td><p>5 時間</p></td>
      <td><p>25 時間</p></td>
      <td><p>20%</p></td>
     </tr>
     <tr>
      <td><p>タスク 2</p></td>
      <td><p>10 時間</p></td>
      <td><p>25 時間</p></td>
      <td><p>30%</p></td>
     </tr>
     <tr>
      <td><p>タスク 3</p></td>
      <td><p>15 時間</p></td>
      <td><p>25 時間</p></td>
      <td><p>40%</p></td>
     </tr>
    </tbody>
   </table>

1. プロジェクトの財務を再計算します。
1. **タスク 1 の CPI** = .04 次のように計算されます。\
   **タスク 1 の CPI** = *IF* 実際の時間 > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual 時間\
      *ELSE* CPI = 1\
   **タスク 1 の CPI** = 1 / 25\
   **タスク 1 の CPI** = .04

1. **タスク 1 の EAC** = 125 時間、次のように計算されます。\
   **タスク 1 の EAC** = *IF* CPI &lt;> 0 *THEN* EAC =計画時間/CPI\
       *ELSE* EAC =計画時間+実際の時間\
   **タスク 1 の EAC** = 5 / .04\
   **タスク 1 の EAC** = 125 時間****

1. タスク 2 とタスク 3 の CPI/EAC は次のとおりです。\
   タスク 2 = .12 / 83.33 時間\
   タスク 3 = .24 / 62.5 時間

1. **プロジェクトの CPI** = .13 次のように計算されます。\
   **プロジェクトの CPI** = *IF* 実際の時間 > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual 時間\
       *ELSE* CPI = 1\
   **プロジェクトの CPI** = 10 / 75\
   **プロジェクトの CPI** = .13

1. **プロジェクトの EAC** = 225 時間、次のように計算されます。\
   **プロジェクトの EAC** = *IF* CPI &lt;> 0 *THEN* EAC =計画時間/CPI\
       *ELSE* EAC =計画時間+実際の時間\
   **プロジェクトの EAC** = 30 / .13333\
   **プロジェクトの EAC** = 225 時間

#### 複雑な例：プロジェクトに子タスクがあります {#complicated-example-project-has-children-tasks}

PIM =時間ベース

EAC メソッド=プロジェクトレベルで計算

1. 次に示すように、Task 3 が Task 4 と 5 の親、Task 1 が Task 2 と 3 の親である 6 つのタスクを持つプロジェクト A を作成します。\
   タスク 1\
      タスク 2\
      タスク 3\
         タスク 4\
         タスク 5\
   タスク 6

1. コスト/時間レートが$100.00 のユーザー 1 にタスク 2、4、5、6 を割り当てます。
1. 以下の表に従って、各タスクの計画時間/実際時間と%完了時間を追加します。

   >[!NOTE]
   >
   >タスク 1 および 3 の場合は、実際の時間のみを追加します。

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
   <th> <p><strong>% 完了</strong> </p> </th> 
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
   <td> <p>20%</p> </td> 
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
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 5</p> </td> 
   <td> <p>15 時間</p> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 6</p> </td> 
   <td> <p>20 時間</p> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. プロジェクトに 50 時間を直接追加します（その他/時間/ログ時間）。
1. **タスク 2 の CPI** = .1 は次のように計算されます。\
   **タスク 2 の CPI** = *IF* 実際の時間 > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual 時間\
       *ELSE* CPI = 1\
   **タスク 2 の CPI** = 1 / 10\
   **タスク 2 の CPI** = .1

1. **タスク 2 の EAC** = 50 時間、次のように計算されます。\
   **タスク 2 の EAC** = *IF* CPI &lt;> 0 *THEN* EAC =計画時間/CPI\
       *ELSE* EAC =計画時間+実際の時間\
   **タスク 2 の EAC** = 5 / .1\
   **タスク 2 の EAC** = 50 時間

1. タスク 4、5、6 の CPI/EAC は次のとおりです。\
   タスク 4:.4 / 25 時間\
   タスク 5:.75 / 20 時間\
   タスク 6:1.2/16.67 時間

1. **タスク 3 の CPI** = .38 次のように計算されます。\
   **タスク 3 の CPI** = *IF* 実際の時間 > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual 時間\
       *ELSE* CPI = 1\
   **タスク 3 の CPI** = 11.5 / 30\
   **タスク 3 の CPI** = .38

1. **タスク 3 の EAC** = 65.22 時間（次のように計算）:\
   **タスク 3 の EAC** = *IF* CPI &lt;> 0 *THEN* EAC =計画時間/CPI\
       *ELSE* EAC =計画時間+実際の時間\
   **タスク 3 の EAC** = 25 / .383333\
   **タスク 3 の EAC** = 65.22 時間

1. **タスク 1 の CPI** = .25 次のように計算されます。\
   **タスク 1 の CPI** = *IF* 実際の時間 > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual 時間\
       *ELSE* CPI = 1\
   **タスク 1 の CPI** = 12.5 / 50\
   **タスク 1 の CPI** = .25

1. **タスク 1 の EAC** = 120 時間、次のように計算されます。\
   **タスク 1 の EAC** = *IF* CPI &lt;> 0 *THEN* EAC =計画時間/CPI\
       *ELSE* EAC =計画時間+実際の時間\
   **タスク 1 の EAC** = 30/.25\
   **タスク 1 の EAC** = 120 時間

1. **プロジェクトの CPI** = .22 次のように計算されます。\
   **プロジェクトの CPI** = *IF* 実際の時間 > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual 時間\
       *ELSE* CPI = 1\
   **プロジェクトの CPI** = 24.5 / 110\
   **プロジェクトの CPI** = .22272\
   **プロジェクトの CPI** = .22

1. **プロジェクトの EAC** = 224.49 時間（次のように計算）:\
   **プロジェクトの EAC** = *IF* CPI &lt;> 0 *THEN* EAC =計画時間/CPI\
       *ELSE* EAC =計画時間+実際の時間\
   **プロジェクトの EAC** = 50 / .22272\
   **プロジェクトの EAC** = 224.49 時間

### PIM=コストベース {#pim-cost-based}

* [簡単な例：プロジェクトに子タスクがありません](#simple-example-project-has-no-children-tasks)
* [複雑な例：プロジェクトに子タスクがあります](#complicated-example-project-has-children-tasks)

#### 簡単な例：プロジェクトに子タスクがありません {#simple-example-project-has-no-children-tasks-1}

PIM =コストベース

EAC メソッド=プロジェクトレベルで計算

1. 3 つのタスク（子タスクなし）を持つプロジェクト A を作成し、すべてのタスクが 100.00 ドルのコストを持つユーザー 1 に割り当てます。
1. 次の表に従って、各タスクに計画時間/実績時間を追加し、完了率を%にします。

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
   <th> <br> <p><strong>Pln Lbr コスト</strong> </p> </th> 
   <th> <br> <p><strong>実時数</strong> </p> </th> 
   <th> <br> <p><strong>ライブラリコスト</strong> </p> </th> 
   <th> <p><strong>% 完了</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>タスク 1</p> </td> 
   <td> <p>5 時間</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>25 時間</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 2</p> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>25 時間</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 3</p> </td> 
   <td> <p>15 時間</p> </td> 
   <td> <p>$1,500.00</p> </td> 
   <td> <p>25 時間</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 以下の表に従って、各タスクに費用を追加します。

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
   <td> <p>タスク 1 有効期限 1</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 1</p> </td> 
   <td> <p>タスク 1 有効期限 2</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 2</p> </td> 
   <td> <p>タスク 2 の有効期限</p> </td> 
   <td> <p>$200.00</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 3</p> </td> 
   <td> <p>タスク 3 の有効期限</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 次のように、2 つの費用をプロジェクトに追加します（タスクに結び付けられていません）。

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
   <td> <p>プロジェクト有効期限 1</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 1 有効期限 2</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
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
   <th> <p><strong>予定費用未発生</strong> </p> </th> 
   <th> <p><strong>発生した予定費用</strong> </p> </th> 
   <th> <p><strong>発生した実費</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>タスク 1</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 2</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$200.00</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 3</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>プロジェクト</p> </td> 
   <td> <p>$3,000.00</p> </td> 
   <td> <p>$2,300.00</p> </td> 
   <td> <p> $2,700.00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. プロジェクト処理から、「財務の再計算」を実行します。
1. **タスク 1 の CPI** = .14
1. **タスク 1 の CPI****** = .14 次のように計算されます。\
   **CPI**  **（タスク 1）** = *IF* 実際の労務費+ OpcedsActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *    ELSE* CPI = CPI_Labor\
   **タスク 1 の CPI****** = (100+300) / (2500+400)\
   **CPI**  **（タスク 1）** = 400 / 2900\
   **CPI**  **（タスク 1）**  = .14****

1. **タスク 1 の EAC****** = 13,400.00 ドル\
   **CPI 労務**  **（タスク 1）** =実際の労務費 &lt;> 0 の場合

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI 労務**  **（タスク 1）** = 100/2500\
   **CPI 労務**  **（タスク 1）** = .04 ****** EAC 労務&#x200B;****（タスク 1）**=*IF *CPI_Labor &lt;> 0*THEN *EAC 労務=計画労務費/CPI_Labor\
   *    ELSE* EAC 労務=計画労務費+実績労務費\
   **EAC 労務&#x200B;****タスク 1** = 500.00/.04 の場合\
   **タスク 1 の EAC Labor****** = 12,500.00 ドル\
   **タスク 1 の EAC****費** = OccedsActualExpenseCost + NotOccededPlannedExpense\
   **タスク 1 の EAC****費** = 400.00 ドル+ 500.00 ドル\
   **タスク 1 の EAC****費** = 900.00 ドル\
   **タスク 1 の EAC****** = EAC 労務費+EAC 費用\
   **タスク 1 の EAC******  = 12,500.00 ドル+ 900.00 ドル\
   **タスク 1 の EAC******  = 13,400.00 ドル

1. タスク 2 とタスク 3 の CPI/EAC 値は次のとおりです。\
   タスク 2 = .19 / $8,433.33\
   タスク 3 = .44 / $6,950.00

1. **プロジェクトの CPI** = .32 次のように計算されます。\
   **プロジェクトの CPI****** = *IF* 実際の労務費+ OpcedsActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **プロジェクトの CPI****** = (1000 + 2300) / (7500 + 2700)\
   **プロジェクトの CPI****** = 3300 / 10200\
   **プロジェクトの CPI****** = .32

1. **プロジェクトの EAC** = $28,200.00 次のように計算されます。\
   **CPI Labor**** for Project** =実際の労務費 &lt;> 0 の場合

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI Labor**** for Project** = 1000 / 7500\
   **CPI Labor**** for Project** = .13333\
   **CPI Labor**** for Project** = .13

   **プロジェクトの EAC Labor****** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC 労務=計画労務費+実績労務費\
   **プロジェクトの EAC Labor****** = 3000/ .13333\
   **プロジェクトの EAC Labor****** = 22,500.00 ドル

   **EAC Expense****Project** =

   ```
   IncurredActualExpenseCost + NotIncurredPlannedExpense
   ```

   **EAC Expense****Project** = 3000.00 ドル+ 2,700.00 ドル\
   **EAC Expense****Project** = 5,700.00 ドル

   **EAC****Project** = EAC 労務費+EAC 費用\
   **EAC****Project**  = 22,500.00 ドル+ $5,700.00\
   **EAC****Project**  = 28,200.00 ドル

#### 複雑な例：プロジェクトに子タスクがあります {#complicated-example-project-has-children-tasks-1}

PIM =コストベース

EAC メソッド=プロジェクトレベルで計算

1. 次に示すように、Task 3 が Task 4 と 5 の親、Task 1 が Task 2 と 3 の親である 6 つのタスクを持つプロジェクト A を作成します。\
   タスク 1\
      タスク 2\
      タスク 3\
         タスク 4\
         タスク 5\
   タスク 6

1. コスト/時間レートが$100.00 のユーザー 1 にタスク 2、4、5、6 を割り当てます。
1. 以下の表に従って、各タスクの計画時間/実際時間と%完了時間を追加します。

   >[!NOTE]
   >
   >タスク 1 および 3 の場合は、実際の時間のみを追加します。

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
   <th> <br> <p><strong>Pln Lbr コスト</strong> </p> </th> 
   <th> <br> <p><strong>実時数</strong> </p> </th> 
   <th> <br> <p><strong>ライブラリコスト</strong> </p> </th> 
   <th> <p><strong>% 完了</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>タスク 1</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 2</p> </td> 
   <td> <p>5 時間</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 3</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 4</p> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 5</p> </td> 
   <td> <p>15 時間</p> </td> 
   <td> <p>$1,500.00</p> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 6</p> </td> 
   <td> <p>20 時間</p> </td> 
   <td> <p>$2,000.00</p> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. プロジェクトに直接 50 時間を追加（「その他」>「時間」>「ログ時間」）し、実際の人件費が直接プロジェクトに記録されるようにします。 ****
1. 以下の表に従って、各タスクに費用を追加します（読みやすくするために各タスクの間に空白行を追加しました）。

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
   <td> <p>タスク 1 有効期限 1</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>-$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 1</p> </td> 
   <td> <p>タスク 1 有効期限 2</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 1</p> </td> 
   <td> <p>タスク 1 有効期限 3</p> </td> 
   <td> <p>$400.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 2</p> </td> 
   <td> <p>タスク 2 Exp 1</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 2</p> </td> 
   <td> <p>タスク 2 Exp 2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 2</p> </td> 
   <td> <p>タスク 2 Exp 3</p> </td> 
   <td> <p>-$200.00</p> </td> 
   <td> <p>$600.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 2</p> </td> 
   <td> <p>タスク 2 有効期限 4</p> </td> 
   <td> <p>$700.00</p> </td> 
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
   <td> <p>タスク 3 の有効期限</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$1,000.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 4</p> </td> 
   <td> <p>タスク 4 Exp 1</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 4</p> </td> 
   <td> <p>タスク 4 有効期限 2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 4 </p> </td> 
   <td> <p>タスク 4 Exp 3</p> </td> 
   <td> <p>-200.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 5</p> </td> 
   <td> <p>タスク 5 有効期限 1</p> </td> 
   <td> <p>$700.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 5</p> </td> 
   <td> <p>タスク 5 有効期限 2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 5</p> </td> 
   <td> <p>タスク 5 有効期限 3</p> </td> 
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
   <td> <p>タスク 6 Exp 1</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 6</p> </td> 
   <td> <p>タスク 6 Exp 2</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>-$300.0</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 次のように、2 つの費用をプロジェクトに追加します（タスクに結び付けられていません）。

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
   <td> <p>プロジェクト有効期限 1</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 1 有効期限 2</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p> $0.00 <strong></strong></p> </td> 
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
   <th> <p><strong>予定費用未発生</strong> </p> </th> 
   <th> <p><strong>発生した予定費用</strong> </p> </th> 
   <th> <p><strong>発生した実費</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>タスク 1</p> </td> 
   <td> <p>$400.00</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$1,300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 3</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$1,000.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 4</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 5</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$1,100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 6</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>プロジェクト</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>$1000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. プロジェクト処理から、「財務の再計算」を実行します。
1. **CPI** タスク 2 = .17 の場合、次のように計算されます。\
   **CPI タスク 2** = *IF* 実際の労務費+ OpcedsActualExpenseCost &lt;> 0 *THEN* CPI = (TotalBudgetedCostWorkPerformed + OccedPlannedExpenseCost) / (ActualLaborCost + OccedActualExpenseCost)\
   *   ELSE* CPI = CPI_Labor\
   **CPI****タスク 2** = (100+300) / (1000+1300)\
   **CPI****タスク 2**  = 400 / 2300\
   **CPI****タスク 2**  = .17

1. **EAC** （タスク 2 = $5,900.00）\
   **CPI Labor****タスク 2** = IF 実績労務費 &lt;> 0 THEN CPI_Labor = TotalBudgetedCostWorkPerformed /実績労務費\
      ELSE CPI_Labor = 1\
   **CPI Labor****タスク 2** = 100/1000\
   **CPI Labor****タスク 2** = .1

   **EAC Labor****Task 2** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC 労務=計画労務費+実績労務費\
   **EAC Labor****Task 2** = 500.00/.1\
   **EAC Labor****Task 2** = 5,000.00 ドル&#x200B;****** EAC 費用&#x200B;****タスク 2 **= OccedsActualExpenseCost + NotOccededPlannedExpense\
   **EAC 費用&#x200B;****タスク 2** = $1,300.00 + -$400.00\
   **EAC 費用****タスク 2** = 900.00 ドル

   **EAC****タスク 2** = EAC 労務費+EAC 費用\
   **EAC****タスク 2**  = 5,000.00 ドル+ 900.00 ドル\
   **EAC****タスク 2**  = 5,900.00 ドル

1. タスク 4、5、6 の CPI/EAC は同じ方法で決定されるので、次の値を指定します。\
   タスク 4:.23 / $3,400.00\
   タスク 5:.64 / $3,100.00\
   タスク 6:1.06 / $2,366.67

1. タスク 3 の CPI = .31 は次のように計算されます。\
   **CPI****タスク 3** = *IF* 実際の労務費+ OpcedsActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****タスク 3**  = (1,150 + 500) / (3000 + 2400)\
   **CPI****タスク 3**  = 1650 / 5400\
   **CPI****タスク 3**  = .31 ******&#x200B;タスク 3 の EAC **= $9,521.74 次のように計算されます。\
   **CPI 労働&#x200B;****タスク 3** = IF 実績労務費 &lt;> 0 THEN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI Labor****タスク 3** = 1150/3000\
   **CPI Labor****タスク 3** = .383333\
   **CPI Labor****タスク 3** = .38

   **EAC Labor****Task 3** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC 労務=計画労務費+実績労務費\
   **EAC Labor****Task 3** = $2,500.00 / .383333\
   **EAC Labor****Task 3** = 6,521.74 ドル

   **EAC 費用****タスク 3** = OccedsActualExpenseCost + NotOccededPlannedExpense\
   **EAC 費用****タスク 3** = $2,400.00 + $600.00\
   **EAC 費用****タスク 3** = 3,000.00 ドル

   **EAC****タスク 3** = EAC 労務費+EAC 費用\
   **EAC****タスク 3**  = 6,521.74 + $3,000.00\
   **EAC****タスク 3**  = 9,521.74 ドル

1. タスク 1 の CPI = .16 は、次のように計算されます。\
   **CPI****タスク 1** = *IF* 実際の労務費+ OpcedsActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****タスク 1**  = (1250 + 300) / (5000 + 4500)\
   **CPI****タスク 1**  = 1550 / 9500=\
   **CPI****タスク 1**  = .16

1. タスク 1 の EAC は$17,100.00 で、次のように計算されます。\
   **CPI Labor****タスク 1** =実際の労務費 &lt;> 0 の場合

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI Labor****タスク 1** = 1250 / 5000\
   **CPI Labor****タスク 1** = .25

   **EAC Labor****Task 1** = *IF* CPI_Labor &lt;> 0 *THEN* EAC 労務=計画労務費/CPI_Labor\
   *   ELSE* EAC 労務=計画労務費+実績労務費\
   **EAC Labor****Task 1** = 3,000.00 / .25\
   **EAC Labor****Task 1** = 12,000.00 ドル

   **EAC 費用****タスク 1** = OccedsActualExpenseCost + NotOccededPlannedExpense\
   **EAC 費用****タスク 1** = 4500 ドル+ 600 ドル\
   **EAC 費用****タスク 1** = 5,100.00 ドル

   **EAC****タスク 1** = EAC 労務費+EAC 費用\
   **EAC****タスク 1**  = 12,000.00 $ + 5,100.00\
   **EAC****タスク 1**  = 17,100.00 ドル

1. プロジェクトの CPI は 0.25 です\
   **プロジェクトの CPI****** = *IF* 実際の労務費+ OpcedsActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor

   **プロジェクトの CPI****** = (2450 + 1900) / (11000 + 6700)\
   **プロジェクトの CPI****** = 4350 / 17700\
   **プロジェクトの CPI****** = .25

1. **プロジェクトの EAC** = $32,248.98 次のように計算されます。\
   **CPI Labor**** for Project** =実際の労務費 &lt;> 0 の場合

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI Labor**** for Project** = 2450 / 11000\
   **CPI Labor**** for Project** = .22272\
   **CPI Labor**** for Project** = .22

   **プロジェクトの EAC Labor****** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC 労務=計画労務費+実績労務費\
   **プロジェクトの EAC Labor****** = $5,000.00 / .22272\
   **プロジェクトの EAC Labor****** = 22,448.97959\
   **プロジェクトの EAC Labor****** = 22,448.98 ドル

   **EAC Expense****Project** = OccedsActualExpenseCost + NotOccededPlannedExpense\
   **EAC Expense****Project** = $3,100.00 + $6,700.00\
   **EAC Expense****Project** = 9,800.00 ドル

   **EAC****Project** = EAC 労務費+EAC 費用\
   **EAC****Project**  = 22,448.98 + 9,800.00\
   **EAC****Project**  = 32,248.98 ドル
