---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: 計算の例 — EAC をタスクからのロールアップとして計算
description: PIM =時間ベース
author: Alina
feature: Work Management
exl-id: 68b582c9-f72a-4000-9d28-f7dafa23541f
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 8%

---

# 計算の例 — EAC をタスクからのロールアップとして計算

## EAC メソッド：タスクまたはサブタスクからロールアップ

* [PIM=時間ベース](#pim-hour-based)
* [PIM=コストベース](#pim-cost-based)

### PIM=時間ベース {#pim-hour-based}

* [簡単な例：プロジェクトに子タスクがありません](#simple-example-project-has-no-children-tasks)
* [複雑な例：プロジェクトに子タスクがあります](#complicated-example-project-has-children-tasks)

#### 簡単な例：プロジェクトに子タスクがありません {#simple-example-project-has-no-children-tasks}

PIM =時間ベース

EAC メソッド=タスク/サブタスクからのロールアップ

1. 3 つのタスク（子タスクなし）を持つプロジェクト A を作成し、すべてのタスクが 100.00 ドルのコストを持つユーザー 1 に割り当てます。
1. 次の表に従って、各タスクに計画時間/実績時間を追加し、完了率を%にします。

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
   <td> <p>5 時間</p> </td> 
   <td> <p>25 時間</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 2</p> </td> 
   <td> <p>10 時間</p> </td> 
   <td> <p>25 時間</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>タスク 3</p> </td> 
   <td> <p>15 時間</p> </td> 
   <td> <p>25 時間</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. 財務の再計算
1. **タスク 1 の CPI** = .04 次のように計算されます。\
   **タスク 1 の CPI** = *IF* 実際の時間 > 0 *THEN* CPI = TotalBudgetedCostWorkPerformed/Actual 時間\
       *ELSE* CPI = 1\
   **タスク 1 の CPI** = 1 / 25\
   **タスク 1 の CPI** = .04

1. **タスク 1 の EAC** = 125 時間、次のように計算されます。\
   **タスク 1 の EAC** = *IF* CPI &lt;> 0 *THEN* EAC =計画時間/CPI\
       *ELSE*

   ```
   EAC = Planned  Hours + Actual  Hours
   ```

   **タスク 1 の EAC** = 5 / .04\
   **タスク 1 の EAC** = 125 時間

1. タスク 2 とタスク 3 の CPI/EAC は次のとおりです。\
   タスク 2 = .12 / 83.33 時間\
   タスク 3 = .24 / 62.5 時間

1. **プロジェクトの CPI** = .13 次のように計算されます。\
   **プロジェクトの CPI** = *IF* 実際の時間 > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **プロジェクトの CPI** = 10 / 75\
   **プロジェクトの CPI** = .13

1. **プロジェクトの EAC** = 270.83 時間（次のように計算）\
   **プロジェクトの EAC** = EAC タスク 1 + EAC タスク 2 + EAC タスク 3\
   **プロジェクトの EAC** = 125 + 83.33 + 62.5\
   **プロジェクトの EAC** = 270.83 時間

#### 複雑な例：プロジェクトに子タスクがあります {#complicated-example-project-has-children-tasks}

PIM =時間ベース

EAC メソッド=タスク/サブタスクからのロールアップ

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

1. プロジェクトに直接 50 時間を追加（「その他」>「時間」>「ログ時間」）し、実際の人件費が直接プロジェクトに記録されるようにします。
1. 財務の再計算の実行
1. **タスク 2 の CPI** = .1 は次のように計算されます。\
   **タスク 2 の CPI** = *IF* 実際の時間 > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **タスク 2 の CPI** = 1 / 10\
   **タスク 2 の CPI** = .1

1. **タスク 2 の EAC** = 50 時間、次のように計算されます。\
   **タスク 2 の EAC** = *IF* CPI &lt;> 0 *THEN*

   ```
   EAC = Planned Hours / CPI
   ```

       *ELSE* EAC =計画時間+実際の時間\
   **タスク 2 の EAC** = 5 / .1\
   **タスク 2 の EAC** = 50 時間

1. タスク 4、タスク 5、タスク 6 の CPI/EAC:\
   タスク 4 = .4 / 25 時間\
   タスク 5 = .75 / 20 時間\
   タスク 6 = 1.2 / 16.67 時間

1. **タスク 3 の CPI** = .38\
   **タスク 3 の CPI** = *IF* 実際の時間 > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **タスク 3 の CPI** = 11.5 / 30\
   **タスク 3 の CPI** = .38

1. **タスク 3 の EAC** = EAC タスク 4 + EAC タスク 5\
   **タスク 3 の EAC** = 25 + 20\
   **タスク 3 の EAC** = 45 時間

1. **タスク 1 の CPI** = .25 次のように計算されます。\
   **タスク 1 の CPI** = *IF* 実際の時間 > 0 *THEN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **タスク 1 の CPI** = 12.5 / 50\
   **タスク 1 の CPI** = .25

1. **タスク 1 の EAC** = EAC タスク 2 + EAC タスク 3\
   **タスク 1 の EAC** = 50 + 45\
   **タスク 1 の EAC** = 95 時間

1. Project の CPI = .22 は、次のように計算されます。\
   **プロジェクトの CPI** = *IF* 実際の時間 > 0 *THEN*

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

### PIM=コストベース {#pim-cost-based}

* [簡単な例：プロジェクトに子タスクがありません](#simple-example-project-has-no-children-tasks)

#### 簡単な例：プロジェクトに子タスクがありません {#simple-example-project-has-no-children-tasks-1}

PIM =コストベース

EAC メソッド=タスク/サブタスクからのロールアップ

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
   <td> <p>$2,700.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. プロジェクト処理から、「財務の再計算」を実行します。
1. **タスク 1 の CPI****** = .14 次のように計算されます。\
   **タスク 1 の CPI******  = *IF* 実際の労務費+ OpcedsActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **タスク 1 の CPI******  = (100+300) / (2500+400)\
   **タスク 1 の CPI******  = 400 / 2900\
   **タスク 1 の CPI******  = .14

1. **タスク 1 の EAC****** = 13,400.00 ドル\
   **タスク 1 の CPI****労働** =実際の労務費 &lt;> 0 の場合

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **タスク 1 の CPI****労働** = 100/2500\
   **タスク 1 の CPI****労働** = .04

   **タスク 1 の EAC Labor****** = *IF* CPI_Labor &lt;> 0 *THEN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC 労務=計画労務費+実績労務費\
   **タスク 1 の EAC Labor****** = 500.00/.04\
   **タスク 1 の EAC Labor****** = 12,500.00 ドル

   **タスク 1 の EAC****費** = OccedsActualExpenseCost + NotOccededPlannedExpense\
   **タスク 1 の EAC****費** = 400.00 ドル+ 500.00 ドル\
   **タスク 1 の EAC****費** = 900.00 ドル

   **タスク 1 の EAC****** = EAC 労務費+EAC 費用\
   **タスク 1 の EAC******  = 12,500.00 ドル+ 900.00 ドル\
   **タスク 1 の EAC******  = 13,400.00 ドル

1. タスク 2 とタスク 3 の CPI/EAC 値は次のとおりです。\
   タスク 2 = .19 / $8,433.33\
   タスク 3 = .44 / $6,950.00****

1. プロジェクトの CPI = .32\
   **プロジェクトの CPI****** = *IF* 実際の労務費+ OpcedsActualExpenseCost &lt;> 0 *THEN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **プロジェクトの CPI****** = (1000 + 2300) / (7500 + 2700)\
   **プロジェクトの CPI****** = 3300 / 10200\
   **プロジェクトの CPI****** = .32

1. プロジェクトの EAC は 28,783.33 ドル\
   **プロジェクト用 EAC****** = EAC タスク 1 + EAC タスク 2 + EAC タスク 3\
   **プロジェクト用 EAC****** = $13,400.00 + $8,433.33 + $6,950.00\
   **プロジェクト用 EAC****** = 28,783.33 ドル
