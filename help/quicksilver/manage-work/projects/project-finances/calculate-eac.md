---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 完了時の推定 (EAC) を計算
description: パフォーマンス指標の「完了時の予測」(EAC) は、完了時のプロジェクトまたはタスクの推定総コストを表します。
author: Alina
feature: Work Management
exl-id: 9061fa56-cff3-4fe2-866e-1fdda9d43efc
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '861'
ht-degree: 0%

---

# 完了時の推定 (EAC) を計算

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link!) </p>
-->

パフォーマンス指標の「完了時の予測」(EAC) は、完了時のプロジェクトまたはタスクの推定総コストを表します。

設定として、EAC 値の計算方法を定義できます。 

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
   <td> <p>プロジェクトおよび財務データへのアクセスの表示</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>財務を表示する権限を持つプロジェクトに対する表示権限以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## EAC の計算方法を定義する

プロジェクトシステム環境設定の一環として、Adobe Workfront管理者は EAC の計算方法を定義できます。 EAC は、次の 2 つの方法のいずれかで計算できます。

* [プロジェクトレベルで計算](#calculate-at-the-project-level)
* [タスクおよびサブタスクからのロールアップ](#roll-up-from-tasks-and-subtasks)

完了時の推定を計算する方法など、Workfrontでプロジェクトの環境設定を行う方法について詳しくは、 [システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

プロジェクトマネージャは、プロジェクトの「財務」サブタブで、プロジェクトレベルでこの環境設定を変更することもできます。 プロジェクトの「財務」サブタブの編集の詳細については、 [プロジェクトの財務エリアで情報を管理します](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

### プロジェクトレベルで計算 {#calculate-at-the-project-level}

親タスクおよびプロジェクトの EAC は、EAC 式に実績時間/実績労務費を入力することで決定されます。 この計算には、実績時間数/コストと費用が親タスクまたはプロジェクトに直接追加されます。

### タスクおよびサブタスクからのロールアップ {#roll-up-from-tasks-and-subtasks}

親タスクとプロジェクトの EAC は、各子タスクの EAC を合計することで決定されます。 この計算では、親タスクまたはプロジェクトに直接追加された実績時間/コストと費用が除外されます。

## パフォーマンスインデックスメソッド (PIM) に基づく EAC の計算方法

Workfrontでの EAC の計算は、プロジェクトで選択したパフォーマンスインデックスメソッド (PIM) に依存します。 お使いのシステムまたはプロジェクトでの PIM の設定について詳しくは、 [パフォーマンスインデックスメソッド (PIM) の設定](../../../manage-work/projects/project-finances/set-pim.md).

* [時間ベースの PIM を使用して EAC を計算](#calculate-eac-using-hour-based-pim)
* [コストベースの PIM を使用して EAC を計算](#calculate-eac-using-cost-based-pim)

### 時間ベースの PIM を使用して EAC を計算 {#calculate-eac-using-hour-based-pim}

```
EAC = Total Planned Hours / CPI*
```

&#42;コスト効果指数の場合 [コスト効果指数 (CPI) の計算](../../../manage-work/projects/project-finances/calculate-cpi.md) = 0、EAC =計画時間合計+実際の時間 これは、時間がキャプチャされたが、プロジェクト/タスクが 0%完了した場合に発生します。

CPI の計算の詳細については、 [コスト効果指数 (CPI) の計算](../../../manage-work/projects/project-finances/calculate-cpi.md).

### コストベースの PIM を使用して EAC を計算 {#calculate-eac-using-cost-based-pim}

プロジェクトの EAC は、次の式を使用して計算されます。

```
EAC = EAC Labor + EAC Expense 
```

<pre>EAC の労務=  <em>IF</em> CPI 労務 &lt;&gt; 0 THEN EAC 労務=計画労務費/CPI 労務</pre><pre><em>ELSE</em> EAC 労務=計画労務費+実績労務費</pre><pre>CPI 労務=実績労務費の場合 &lt;&gt; 0 THEN CPI Labor = TotalBudgetedCostWorkPerformed /実績労務費</pre><pre>ELSE CPI Labor = 1 </pre>EAC の計算時には、次のフィールドが考慮されます。

* BCWP (Total Budgeted Cost Work Performed) =予定作業の予算コスト（予算コスト）と、それまでに完了したタスクの割合を乗算した結果。

   BCWP (Total Budgeted Cost Work Performed) の詳細については、 [予算原価実績の計算 (BCWP)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

   * **親以外のタスクの場合：**

      ```
      Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete/100)
      ```

   * **親タスクの場合：**
Total Budgeted Cost Work Performed =すべての直接の子タスクの「Total Budgeted Cost Work Performed」フィールドの合計です。

   * **プロジェクトの場合：**
Total Budgeted Cost Work Performed =すべての最上位タスク（親タスクおよびスタンドアロンタスク）の「Total Budgeted Cost Work Performed」フィールドの合計。 

* EAC 費用=発生した実際の費用を未発生の計画費用に追加した結果。 次の式で計算されます。

   ```
   EAC Expense = Incurred Actual Expense Cost + Not Incurred Planned Expense
   ```

   * 発生費実費原価= 「実績金額」フィールドが 0 より大きいすべての費用の「計画金額」フィールドの合計。 たとえば、タスク 1 に費用を作成し、「計画金額」フィールドに$500.00 と入力し、「実績金額」フィールドに 0 より大きい金額を入力した場合 ( 例：$600.00) の場合、このタスクの発生予定費用は$500.00 です。
   * 未発生計画費用= 「実績金額」フィールド= 0 の全費用の「計画金額」フィールドの合計。 たとえば、タスク 1 で、最初の費用に対して、[ 計画金額 ] フィールドの値が$500.00 で、[ 実績金額 ] フィールドの値が$600.00 で、[ 計画金額 ] フィールドの値が$300.00 で、[ 実績金額 ] フィールドの値が$0.00 の場合、0 の場合、このタスクの未発生予定費の値は$300.00 です。 

## プロジェクトまたはタスク内で EAC を見つける

1. EAC を表示するプロジェクトまたはタスクに移動します。
1. 展開 **プロジェクトの詳細** または **タスクの詳細** （EAC を表示する場所に応じて）プロジェクトまたはタスクの左パネル

1. クリック **金融**. 

   EAC の値は、 **完了時の推定** フィールドに入力します。

   ![](assets/eac-highlighted-on-project-350x112.png)
