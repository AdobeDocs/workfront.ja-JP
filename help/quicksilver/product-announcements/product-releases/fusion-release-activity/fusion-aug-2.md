---
title: Workfront Fusion リリースアクティビティ：&nbsp;2021 年 8 月 2 日の週
description: Workfront Fusion リリースアクティビティ：&nbsp;2021 年 8 月 2 日の週
author: Luke
draft: Probably
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
exl-id: 051fb2b6-336e-432c-b2cb-0286e5bdf168
hidefromtoc: true
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '245'
ht-degree: 0%

---

# Workfront Fusion リリースアクティビティ： 2021 年 8 月 2 日の週

このページでは、2021 年 8 月 2 日の週にAdobe Workfront Fusion でおこなわれたすべての機能強化について説明します。

最近のすべての変更の一覧については、 [Adobe Workfront Fusion リリースアクティビティ](../../../product-announcements/product-releases/fusion-release-activity/fusion-release-activity.md).

Workfront Fusion の最近のバグ修正の一覧については、 [Workfrontメンテナンスの更新](https://experienceleague.adobe.com/docs/workfront-known-issues/releases/current-updates.html) ページを開き、 Workfront Fusion メンテナンスアップデートというラベルの付いたアップデートがないか確認します。

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Filter and sort Workfront Fusion scenario execution history</h2>
<p>To make it easier to find specific scenario executions, we've made it possible to filter by more fields in the scenario execution history. Now, in addition to existing filters, you can filter by the following:</p>
<ul>
<li> <p>Execution duration</p> </li>
<li> <p>Number of operations</p> </li>
<li> <p>Amount of data transferred</p> </li>
<li> <p>Action type (run or update)</p> </li>
</ul>
<p>Previously, execution history could be filtered only by start time or status.</p>
<p>You can also now sort the scenario execution history. You can sort by the following values:</p>
<ul>
<li> <p>Execution start time</p> </li>
<li> <p>Execution status</p> </li>
<li> <p>Execution duration</p> </li>
<li> <p>Number of operations</p> </li>
<li> <p>Amount of data transferred</p> </li>
</ul>
<p>For more information on filtering and sorting execution history, see <a href="../../../workfront-fusion/scenarios/view-scenario-execution-history.md" class="MCXref xref" xrefformat="{para}">View a scenario's execution history in Adobe Workfront Fusion</a>.</p>
</div>
-->

## マッピングパネルで使用できる新しい関数

マッピングパネルで 2 つの新しい関数を使用できるようになりました。

* 新しい日付と時間関数： dateDifference

  シナリオで時間の範囲を簡単に計算できるように、新しい「dateDifference」日時関数を追加しました。 この関数は、2 つの日付または時間と時間の単位を取り、選択した時間の単位で表される、日付または時間の間の時間を返します。

  以前は、日付と時間の差異は、ユーザーが入力した数式でのみ計算できました。

  詳しくは、 [Adobe Workfront Fusion の日付および時間関数](../../../workfront-fusion/functions/date-and-time-functions.md).

* 新しい配列関数：arrayDifference

  この関数は、2 つの配列を取り、新しい配列を返します。 モジュールが返す新しい配列のタイプを選択できます。

   * 他の配列に含まれていない、1 つの配列の要素の配列
   * 1 つの配列または他の配列に含まれるが、両方には含まれない要素の配列。

  詳しくは、 [Adobe Workfront Fusion の配列関数](../../../workfront-fusion/functions/array-functions.md).
