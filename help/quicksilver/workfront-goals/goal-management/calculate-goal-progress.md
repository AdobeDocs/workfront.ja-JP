---
product-previous: workfront-goals
navigation-topic: goal-management
title: Adobe Workfront Goals の目標の進捗と状況の概要
description: 目標の進捗は、アクティビティ、結果、子目標などの進捗状況インジケーターによって推進されます。目標の状況は、現在の時点での目標の進捗によって決定されます。
author: Alina
feature: Workfront Goals
exl-id: 3050f7ff-a579-4fb8-82fd-bef850f27c20
source-git-commit: 1d221d10e5845e477dff825f853330b9b4df0adf
workflow-type: ht
source-wordcount: '821'
ht-degree: 100%

---

# Adobe Workfront Goals の目標の進捗と状況の概要

<!--drafted for P&P release: the note at the top will need to be replaced with this:

Your organization must have the following to use the functionality described in this article:

* For the legacy plan and license structure: 

  * A Pro or higher [Adobe Workfront plan](https://www.workfront.com/plans). 
  * An Adobe Workfront Goals license in addition to a Workfront license.

* For the current plan and license structure:

  * An Ultimate plan 
    
    Or
    
    An additional license for Adobe Workfront Goals for the Prime or Select Adobe Workfront plans. <is there a link we can add here for the plans and what they contain?!>

Contact your Workfront account manager to learn about a Workfront Goals license.

For additional information about access to Workfront Goals, see [Requirements to use Workfront Goals](../../workfront-goals/goal-management/access-needed-for-wf-goals.md).
-->

>[!NOTE]
>
>この記事で説明している機能を使用するには、組織に以下が必要です。
>
>* Pro 以上の [Adobe Workfront プラン](https://www.workfront.com/plans)。
>* Workfront ライセンスに加えて、Adobe Workfront Goals ライセンス。
>
>Workfront Goals ライセンスについては、Workfront のアカウントマネージャーにお問い合わせください。
>Workfront Goals へのアクセス権について詳しくは、[Workfront Goals の使用要件](../../workfront-goals/goal-management/access-needed-for-wf-goals.md)を参照してください。

Adobe Workfront は、進捗状況インジケーターの進捗に基づいて、目標の進捗状況を自動的に計算します。

## 前提条件

開始するには、まず以下が必要です。

* メインメニューの目標エリアを含むレイアウトテンプレート。

## 目標の進捗としきい値の概要

目標をアクティブ化すると、Workfront Goals は、進捗と状況の計算を開始し、進捗フィールドにポインタを合わせると、以下のインジケーターを表示します。

| インジケーター | インジケーターの説明 |
|---|---|
| 実際の完了率 | これまでの目標の実際の達成度。Workfront Goals は、目標に関連付けられているすべての進捗状況インジケーターの完了率を平均化して、この値を計算します。 |
| 予想完了率 | 目標が時間どおりに完了するために、これまでに完了する必要がある目標の比率。Workfront Goals は、目標の期間と現在の時刻から、この値を計算します。目標が時間どおりに完了する場合、目標には現時点でのこの値が表示されるはずです。 |
| 進捗状況 | 目標が予定どおりに完了できるか、あるいは目標を完了できないリスクや問題があるかを示すラベルです。 |

![](assets/in-trouble-goal-progress-expanded.png)

<!--drafted for the redesign: replace the screen shot above with the redesigned one which is white, not black-->

* [実際の完了率](#actual-percent-complete)
* [予想完了率](#expected-percent-complete)
* [進捗と状況](#progress)

### 実際の完了率 {#actual-percent-complete}

Workfront Goals は、目標の進捗状況インジケーターの完了率平均に基づいて、目標の実際の完了率を自動的に計算します。

以下の項目は、目標の進捗状況インジケーターと見なされます。

* 結果

  目標への結果の追加について詳しくは、[Adobe Workfront Goals の目標に結果を追加](../../workfront-goals/results-and-activities/add-results-to-goals.md)を参照してください。

* アクティビティ

  プロジェクトなどのアクティビティの目標への追加について詳しくは、[Adobe Workfront Goals の目標にアクティビティを追加](../../workfront-goals/results-and-activities/add-activities-to-goals.md)を参照してください。

* 調整された子目標

  親目標と子目標について詳しくは、[目標を Adobe Workfront Goals に結び付けて調整](../../workfront-goals/goal-alignment/align-goals-by-connecting-them.md)を参照してください。

  Workfront は、以下の式を使用して実際の完了率を計算します。

  ```
  Actual percent complete of goal = SUM(Percent complete of goal progress indicators)* 100 / Number of progress indicators
  ```

  例えば、目標の結果が 20％完了、手動進行状況バーが 30％完了、プロジェクトが 10％完了、子目標が 40％完了している場合、目標の完了パーセントは 25％です。

### 予想完了率 {#expected-percent-complete}

Workfront Goals は、目標期間の合計日数と目標開始日からの経過日数に基づいて、目標の予想完了率を自動的に計算します。

Workfront は、以下の式を使用して予想完了率を計算します。

```
Expected percent complete of goal = Number of days since the goal start date * 100/ Number of days in the goal duration
```

例えば、目標が 90 日で完了する予定で、今日がその期間の 45 日目の場合、予想完了率は 50％です。

### 進捗と状況 {#progress}

Workfront Goals は、現時点で予想完了率のうち何パーセントに達しているかに基づいて、進捗率を計算し、目標に進捗ラベルを割り当てます。目標完了率のバーの色は、目標の進行状況を示すように変化します。

また、目標の状況もアップデートされ、目標が時間どおりに完了するか、遅れているかが示されます。

Workfront Goals は、以下の式を使用して目標の進捗率を計算します。

```
Goal progress percentage = Actual percent complete * 100 / Expected percent complete
```

例えば、予想完了率が現時点で 53％、実際の完了率が 30％の場合、目標進捗率は 56％です。Workfront Goals は、この目標に「トラブル発生中」という状況のラベルを付けます。

次のグラフは、状況のラベルと進捗率の関係を示しています。

![](assets/progress-status-labels-charted-after-match-with-project-condition-350x147.png)

次の表に、それぞれのラベルに関連付けられた「目標の状況」ラベルと目標の進捗率を示します。

>[!TIP]
>
>「目標の進捗」ラベルは、Workfront プロジェクトの状況の名前と色に一致します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>目標進捗の名前</b></td> 
   <td><b>目標進捗の定義</b></td> 
   <td><b>目標の進捗率</b></td> 
   <td><b>完了率の色</b></td> 
   <td><b>状況インジケーターアイコン</b></td> 
  </tr> 
  <tr> 
   <td>新規</td> 
   <td> <p>目標が新しく作成されており、まだ進行状況が記録されていません。目標の進行状況は、初めて更新するまで「新規」として表示されます。 </p> <p>目標のアップデートについて詳しくは、<a href="../../workfront-goals/goal-review-and-workfront-goals-sections/check-in-goals.md" class="MCXref xref">Adobe Workfront Goals での目標の進捗状況の更新</a>を参照してください。</p> </td> 
   <td>割合なし</td> 
   <td>バーなし</td> 
   <td><img src="assets/new-goal-icon-condition.png" alt="new_goal_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>目標どおり</span> </p> </td> 
   <td>想定どおりに進捗していて、目標を時間内に達成できる可能性が高い状況です。 </td> 
   <td>90～100%</td> 
   <td>緑</td> 
    <td><img src="assets/on-target-icon-condition.png" alt="on_target_icon_condition.png"></td>
  </tr> 
  <tr> 
   <td> <p><span>リスクあり</span> </p> </td> 
   <td>遅れてはいるものの、目標を予定どおりに完了できる可能性があります。 </td> 
   <td>70～89.99%</td> 
   <td>黄</td>
   <td><img src="assets/at-risk-icon-condition.png" alt="at_risk_icon_condition.png"></td> 
  </tr> 
  <tr> 
   <td> <p><span>トラブル発生中</span> </p> </td> 
   <td> <p>目標が予定どおりに完了しない可能性が非常に高い状況です。 </p> </td> 
   <td>0～69.99%</td> 
   <td>赤</td> 
   <td><img src="assets/in-trouble-icon-condition.png" alt="in_troble_icon_condition.png"></td> 
  </tr> 
 </tbody> 
</table>