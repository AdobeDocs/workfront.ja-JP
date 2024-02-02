---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: 完了時の見積もり（EAC）の計算
description: パフォーマンス指標として、完了時の見積もり（EAC）は、完了時のプロジェクトまたはタスクの見込み合計コストを表します。
author: Alina
feature: Work Management
exl-id: 9061fa56-cff3-4fe2-866e-1fdda9d43efc
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: ht
source-wordcount: '861'
ht-degree: 100%

---

# 完了時の見積もり（EAC）の計算

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link!) </p>
-->

パフォーマンス指標として、完了時の見積もり（EAC）は、完了時のプロジェクトまたはタスクの見込み合計コストを表します。

設定として、EAC 値の計算方法を定義できます。 

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトおよび財務データへのアクセス権を表示</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>財務情報を表示する権限を持つプロジェクトに対する表示以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## EAC の計算方法の定義

プロジェクトシステム環境設定の一環として、Adobe Workfront 管理者は EAC の計算方法を定義できます。EAC は、次の 2 つの方法のいずれかで計算できます。

* [プロジェクトレベルで計算](#calculate-at-the-project-level)
* [タスク／サブタスクからロールアップ](#roll-up-from-tasks-and-subtasks)

EAC を計算する方法など、Workfront でプロジェクトの環境設定を行う方法について詳しくは、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

プロジェクトマネージャーは、プロジェクトの「財務」サブタブで、プロジェクトレベルでこの環境設定を変更することもできます。プロジェクトの「財務」サブタブの編集について詳しくは、[プロジェクトの財務エリアでの情報管理](../../../manage-work/projects/project-finances/manage-project-finance-area.md)を参照してください。

### プロジェクトレベルで計算 {#calculate-at-the-project-level}

親タスクとプロジェクトの EAC は、EAC 式の実際の時間数／実際の労力コストを使用して決定されます。この計算には、親タスクまたはプロジェクトに直接追加された実際の時間数／コストと費用が含まれます。

### タスク／サブタスクからロールアップ {#roll-up-from-tasks-and-subtasks}

親タスクとプロジェクトの EAC は、各子タスクの EAC を合計することによって決定されます。この計算には、親タスクまたはプロジェクトに直接追加された実際の時間数／コストと費用は含まれません。

## パフォーマンスインデックスメソッド（PIM）に基づく EAC の計算方法

Workfront では、EAC の計算は、プロジェクトで選択したパフォーマンスインデックスメソッド（PIM）に依存します。お使いのシステムまたはプロジェクトでの PIM の設定について詳しくは、[パフォーマンスインデックスメソッド（PIM）の設定](../../../manage-work/projects/project-finances/set-pim.md)を参照してください。

* [時間ベースの PIM を使用する場合の EAC の計算](#calculate-eac-using-hour-based-pim)
* [コストベースの PIM を使用する場合の EAC の計算](#calculate-eac-using-cost-based-pim)

### 時間ベースの PIM を使用する場合の EAC の計算 {#calculate-eac-using-hour-based-pim}

```
EAC = Total Planned Hours / CPI*
```

&#42;コスト効率指数の場合 [コスト効率指数（CPI）の計算](../../../manage-work/projects/project-finances/calculate-cpi.md) = 0、EAC = 合計予定時間数 + 実際の時間。これは、時間が取り込まれたが、プロジェクト／タスクが 0%完了の場合に発生します。

CPI 計算について詳しくは、[コスト効率指数（CPI）の計算](../../../manage-work/projects/project-finances/calculate-cpi.md)を参照してください。

### コストベースの PIM を使用する場合の EAC の計算 {#calculate-eac-using-cost-based-pim}

プロジェクトの EAC は、次の式を使用して計算されます。

```
EAC = EAC Labor + EAC Expense 
```

<pre>EAC 労力 = <em>IF</em> CPI Labor &lt;&gt; 0 THEN EAC Labor = 予定労力コスト/CPI 労力</pre><pre><em>ELSE</em> EAC Labor = 予定労力コスト + 実際の労力コスト</pre><pre>CPI 労力 = IF 実際の労力コスト &lt;&gt; 0 THEN CPI Labor = TotalBudgetedCostWorkPerformed / 実際の労力コスト</pre><pre>ELSE CPI Labor = 1 </pre>EAC の計算時には、次のフィールドが考慮されます。

* 作業実行の予算（BCWP）合計 = 予定作業の予算計上コスト（予算計上コスト）と、それまでに完了したタスクの割合を乗算した結果。

  作業実行の予算（BCWP）合計について詳しくは、[作業実行の予算（BCWP）合計の計算](../../../manage-work/projects/project-finances/calculate-bcwp.md)を参照してください。

   * **親以外のタスクの場合：**

     ```
     Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete/100)
     ```

   * **親タスクの場合：**
作業実行の予算（BCWP）合計 = すべての直接の子タスクの「作業実行の予算（BCWP）合計」フィールドの合計。

   * **プロジェクトの場合：**
作業実行の予算（BCWP）合計 = すべての最上位レベルのタスク（親タスクおよびスタンドアロンタスク）の「作業実行の予算（BCWP）合計」フィールドの合計。

* EAC 費用 = 発生した実際の費用コストを未発生の予定費用コストに追加した結果。次の式で計算されます。

  ```
  EAC Expense = Incurred Actual Expense Cost + Not Incurred Planned Expense
  ```

   * 発生した実際の費用コスト = 「実際の金額」フィールド > 0 のすべての費用の「予定金額」フィールドの合計。例えば、タスク 1 の経費を作成し、「予定金額」フィールドに 500.00 ドルと入力し、「実際の金額」フィールドに金額 > 0（つまり 600.00 ドル）と入力した場合、このタスクで発生した予定費用コストは 500.00 ドルになります。
   * 未発生の予定費用 = 「実際の金額」フィールド = 0 のすべての費用の「予定金額」フィールドの合計。例えば、タスク 1 に 2 つの費用を作成して、最初の費用の「予定金額」フィールドの値が 500.00 ドルで「実際の金額」の値が 600.00 ドル、2 番目の費用の「予定金額」フィールドの値が 300.00 ドルで「実際の金額」フィールドの値が 0.00 ドルの場合、このタスクの未発生の予定費用の値は 300.00 ドルです。 

## プロジェクトまたはタスク内での EAC の検索

1. EAC を表示するプロジェクトまたはタスクに移動します。
1. EAC を表示する場所に応じて、プロジェクトまたはタスクの左側のパネルにある&#x200B;**プロジェクトの詳細**&#x200B;または&#x200B;**タスクの詳細**&#x200B;を展開します。

1. 「**財務**」をクリックします。

   EAC の値が「**完了時の見積もり**」フィールドに表示されます。

   ![](assets/eac-highlighted-on-project-350x112.png)
