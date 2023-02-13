---
content-type: overview
product-previous: workfront-goals
navigation-topic: goal-alignment
title: Adobe Workfront目標の目標揃えの概要
description: 目標の調整により、目標を相互に合わせ、チーム、グループ、会社の組織目標に合わせて、組織内の全員が同じページで達成すべきことについて確認できます。
author: Alina
feature: Workfront Goals
exl-id: e073cf10-2333-4095-b932-73d105f0c5a4
source-git-commit: afc2124a7fd0d9d52c04be1c174fdba314beec7a
workflow-type: tm+mt
source-wordcount: '762'
ht-degree: 0%

---

# Adobe Workfront目標の目標揃えの概要

>[!NOTE]
>
>この記事で説明する機能を使用するには、以下が必要です。
>* プロ以上 [Adobe Workfrontプラン](https://www.workfront.com/plans).
>* Workfrontライセンスに加えて、Adobe Workfront Goals ライセンスが必要です。 Workfront Goals ライセンスについて詳しくは、Workfrontのアカウントマネージャーにお問い合わせください。
>
>Workfront Goals へのアクセスについて詳しくは、 [Workfront目標の使用要件](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).

<!--drafted for P&P new model: the note at the top will need to be replaced with this:    
    
Your organization must have the following to use the functionality described in this article:    
    
* For the legacy plan and license structure:     
    
  * A Pro or higher [Adobe Workfront plan](https://www.workfront.com/plans).     
  * An Adobe Workfront Goals license in addition to a Workfront license.    
    
* For the current plan and license structure:    
    
  * An Ultimate plan     
        
    Or    
        
    An additional license for Adobe Workfront Goals for the Prime or Select Adobe Workfront plans. <is there a link we can add here for the plans and what they contain?!>    
    
Contact your Workfront account manager to learn about a Workfront Goals license.    
    
For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](../workfront-goals/goal-management/access-needed-for-wf-goals.md).    
-->

目標の整合は、目標管理の重要な部分です。 お互いの目標を合わせ、チーム、グループおよび会社の組織目標に合わせることで、戦略を前進させるために何が必要かについて、組織の全員が同じページにいることを確認できます。

トップレベルの企業、チーム、またはグループの目標を設定し、確認した後、ダイレクトレポートとチームメンバーは、トップレベルから重点的に目標を作成する必要があります。 これらの目標の範囲は、より狭く、目標の責任者として指定された個人とその影響範囲を考慮に入れる必要があります。 目標は、何を達成し、何を達成し、何を、それが一致する親の目標を達成する必要があるかという問いに答える必要があります。

目標を揃える際のベストプラクティスについて詳しくは、 [Adobe Workfront目標の概要](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).

## 目標を揃えるための考慮事項

* 目標は、同時に複数の他の目標に貢献することはできません。 同じ親目標に複数の子目標を整列させることはできますが、子目標に設定できる親は 1 つだけです。 親と子の目標について詳しくは、 [親と子の目標の理解](#understand-parent-and-children-goals) 」の節を参照してください。
* 目標には、複数の目標（または子）のほか、複数のアクティビティと結果を含めることができます。 さらに、各子目標には、進行状況および親目標の進行状況に影響を与える他のアクティビティや結果を含めることができます。

   >[!TIP]
   >
   >この構造は、できるだけ簡単にすることをお勧めします。

* 役割に応じて、様々な種類の目標を更新する必要があります。 例：

   * 個々のコントリビューターは、チーム、グループ、企業レベルの目標に合わせて調整する必要がある、独自の目標にコントリビューションすることをお勧めします。 独自の目標を更新すると、他のすべての親目標の進捗状況が更新されます。
   * CEO またはビジネスマネージャとして、目標に貢献し、チーム、グループ、会社に割り当てられた目標を更新することをお勧めします。

## 目標の整列のタイプ

目標を揃えるには、次の 2 つの方法があります。

* **下から上への配置**:子の目標を親の目標に直接接続できます。 ボトムアップ目標の位置合わせについては、 [目標をAdobe Workfront目標に結び付けて整列させる](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md).

* **上下揃え**:目標の結果またはアクティビティを別の目標に変換できます。 新しいゴールは、親になる元のゴールの子ゴールになります。 トップダウン目標の整列について詳しくは、 [結果とアクティビティを目標に変換して目標を揃える](../../workfront-goals/goal-alignment/align-goals-by-converting-results-activities.md).

親と子の目標について詳しくは、 [親と子の目標の理解](#understand-parent-and-children-goals) 」の節を参照してください。

## 親と子の目標の理解 {#understand-parent-and-children-goals}

ゴールを互いに合わせると、1 つのゴールが親ゴールになり、もう 1 つが子ゴールになります。 子目標の進行は親目標の進行に影響します。 これにより、目標階層が作成されます。

子と親の目標を使用する際は、次の点に注意してください。

* 複数の子目標を同じ親目標に合わせることができます。
* 1 つの子目標には、1 つの親目標のみを設定できます。
* 子の目標の進捗状況は、その結果とアクティビティによって示され、親の目標の進捗状況に影響を与えます。 親目標に関連付けられたその他のアクティビティや結果も、親目標の進行状況に影響します。
* 親目標のレベルで子目標の進捗状況を更新することはできません。 子目標のアクティビティと結果を更新する必要があります。これにより、子の進行状況と親目標の進捗状況が自動的に更新されます。

   目標の進捗の更新について詳しくは、 [Adobe Workfront目標での目標の進捗状況の更新](../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md).

## 整列した目標を配置

目標を揃えた後、それらは同じ階層の一部となり、Workfront目標の様々な領域に表示されます。

<!--
* In the Production enviroment, you can view children and parent goals in the following areas:

    * The Goal Details panel
    * Goal List
    * Goal Alignment section
    * Check-in section
    * Pulse section
    * You can view all the parent goals of a goal in the Goal Hierarchy field of a Project or Goal report.
-->
以下の領域で、子と親の目標を表示できます。

* 目標のページの「進捗状況指標」セクション（タイプ：目標グループ）
* 目標ページの「目標の整列」セクションを参照してください。




