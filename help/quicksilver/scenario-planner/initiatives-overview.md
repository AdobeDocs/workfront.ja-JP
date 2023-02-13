---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: シナリオプランナーのイニシアチブの概要
description: シナリオプランナーは、新しいAdobe Workfrontエクスペリエンスでのみ使用でき、追加のライセンスが必要です。 Workfrontシナリオプランナーの詳細は、「シナリオプランナーの概要」を参照してください。
author: Alina
feature: Workfront Scenario Planner
exl-id: d67f51e5-7c5c-436b-b0c3-e5afbd7cebca
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 0%

---

# 以下のイニシアティブの概要 [!DNL Scenario Planner]

この [!DNL Scenario Planner] は、新しい [!DNL Adobe Workfront] を使用し、追加のライセンスが必要です。 詳しくは、 [!DNL Workfront Scenario Planner]を参照してください。 [この [!DNL Scenario Planner] 概要](../scenario-planner/scenario-planner-overview.md).
ビジネスマネージャは、 [!DNL Adobe Workfront Scenario Planner]. プランの作成について詳しくは、この記事を参照してください。 [でプランを作成および編集 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## イニシアチブの概要

の使用 [!DNL Workfront Scenario Planner]では、各イニシアチブについて次の情報を見積もり、確認できます。

* イニシアチブの完了に必要なジョブの役割の種類と数を見積もります。 これにより、計画の必須の役割数が増加し、イニシアチブで確認できる「個人原価」が計算されます。
* イニシアチブの完了に必要な作業に関連する固定コストを見積もります。
* イニシアチブが完了したときに企業が得る可能性のある計画特典を見積もります。

イニシアチブに関する情報を表示するには、プラン内の個々のイニシアチブにアクセスできます。 イニシアチブの作成とアクセスについては、「 [のイニシアチブを作成および編集します [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## イニシアチブに関する考慮事項

イニシアチブを作成する際は、次の点を考慮してください。

* イニシアチブを作成する前に、プランを作成する必要があります。
* イニシアチブをゼロから作成したり、プランにプロジェクトをインポートしたりできます。 プロジェクトはプラン内のイニシアチブになります。

   イニシアチブをゼロから作成する方法については、 [のイニシアチブを作成および編集します [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

   プロジェクトからイニシアチブを作成するプランにプロジェクトをインポートする方法については、 [内のプランにプロジェクトをインポート [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* イニシアチブは計画よりも小さい計画単位で、計画の一部としてのみ作成されます。
* 最短のイニシアチブの期間は 1 か月にすることができます。 最も長いイニシアチブの期間は 5 年です。
* イニシアチブで実際の作業を行うことはできません。 イニシアチブレベルで、必要なリソースとそれらのリソースに発生するコストを定義して、計画の要求の 1 つを実行できるようにします。 例えば、会社が新しい場所に新しいオフィスを拡張し、新しい場所に新しいオフィスを取得する計画を立てている場合、その新しい場所のネットワークインフラストラクチャを導入するイニシアチブが部署にある可能性があります。
* 1 つのプランに複数のイニシアチブを作成できます。 各イニシアチブでは、部門での作業を達成するための高レベルな戦略の概要を説明できます。
* プラン内のイニシアチブに優先順位を付けて、最も重要なイニシアチブが最も多くの予算と最も多くのリソースを確実に受け取るようにできます。
* プラン内でイニシアチブを作成する場合、そのプランを表示するすべての人が、プラン内のすべてのイニシアチブを表示することもできます。

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change when we add to the access levels granularity)</p>
  -->

* イニシアチブをパブリッシュして、プロジェクトを作成したり、プロジェクトにリンクされているプロジェクトを更新したりできます。 イニシアチブの公開について詳しくは、 [プロジェクトを更新または作成するには、 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

## イニシアチブに関する財務情報

個々のイニシアチブに関する財務情報を確認して、計画内でのイニシアチブの適合を把握できます。 イニシアチブへのアクセスについては、「 [のイニシアチブを作成および編集します [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

計画内でイニシアチブにアクセスすることで、イニシアチブに関する次の財務指標を表示できます。

<!--
<p>(NOTE: several instances drafted in the table below!) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL コストの合計金額 ]</td> 
   <td> <p style="font-weight: normal;">これは、イニシアチブの総コストの計算です。 </p> <p style="font-weight: normal;">[!DNL Workfront] 次の式を使用して、イニシアチブの総コスト値を計算します。</p> <p style="font-weight: normal;"><code>Initiative Costs = Fixed Costs + People Costs</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 固定コスト ]</td> 
   <td> <p><span style="font-weight: normal;">これは、見積もりが可能な手動入力です <span>イニシアティブの各月の固定コストの月額。</span> これには、「[!UICONTROL 人物コスト ]」フィールドに取り込まれるイニシアチブに追加された役割に関連するコストは含まれません。</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL People Costs]</td> 
   <td> <p style="font-weight: normal;">これは、イニシアチブの期間中にイニシアチブのジョブの役割に関連付けられたコストの合計計算です。 この数は、イニシアチブの各月のジョブロールに対して見積もる工数または時間数によって異なります。 </p> 
     <p><b>ヒント</b>  
     <ul> 
      <li> <p>同じジョブロールの月別の工数の数は、月ごとに異なる場合があります。</p> </li> 
      <li> <p>[!DNL Workfront] では、1 ヶ月に 160 の労働時間があると考えています。 </p> </li> 
     </ul> 
     <p>[!DNL Workfront] イニシアチブの [!UICONTROL 個人原価 ] を次の式で計算します。</p> <p><code>Initiative People Costs = SUM(Monthly people cost)</code> </p> 
    <p> [!DNL Workfront] 次の式を使用して、イニシアティブ期間中の各月の月別人物原価を計算します。</p> 
     <p><code>Monthly People Costs = SUM(Job role hourly rate * 160 * Number of FTEs)</code> </p> 
      <p><b>例</b></p>
      <p>期間が 6 か月のイニシアチブがあり、毎月 1 回の FTE に対して$50 の時間率を持つ 1 人の Designer と、イニシアティブの 2 か月に対して$100 の時間率を持つ Web デザイナーが必要な場合、イニシアチブの人々のコストは次のように計算されます。</p>
      <code>Initiative People Costs = 50*160*6 + 100*160*2 = 48,000 + 32,000 = 80,000</code>        
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planned Benefit]</td> 
   <td>これは、このイニシアチブを完了することで、部門が得る全体的な利益を見積もるための手動エントリです。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 正味値 ]</td> 
   <td> <p style="font-weight: normal;">これは、全体的なコストと、イニシアチブに関して推定される計画福利厚生を考慮した場合のイニシアチブの価値を表します。 [!DNL Workfront] 次の式を使用してイニシアチブの正味値を計算します。</p> <p style="font-weight: normal;"><code>Initiative Net Value = Initiative Planned Benefit - Initiative Costs</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

<!--drafted content from People Costs:
(NOTE: drafted below)</p> 
       <p>Depending on whether the plan is set up to use FTEs or hours, Workfront uses the following formulas to calculate People Cost:</p> 
       <ul> 
        <li> <p>When using FTEs: </p> <p><code>People Costs = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>, where 160 is the total number of working hours in a month. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><span style="font-weight: normal;"> When estimating resources using FTEs,(NOTE: drafted and yellow and fix the rest of the sentence)
      <p>When using hours:</p> 
      <p><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> 
      <p>For information about setting up the plan to use hours or FTE, see <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Create and edit plans in the Scenario Planner</a>.</p>-->

## レポート内のイニシアチブ情報

次の表に示すように、イニシアチブ情報をレポートに表示できます。 この情報は、会社がWorkfront Scenario Planner ライセンスを購入した場合にのみ、Workfrontインスタンスで使用できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>レポートタイプ</b></td> 
   <td><b>イニシアチブ情報</b></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative] </td> 
   <td>名前、期間、開始日、終了日、入力者、ID、最終発行日*、カスタムフィールドを含むすべてのプロジェクトフィールド*</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL イニシアチブジョブの役割 ]</td> 
   <td>上記のすべてのイニシアチブ情報（ジョブの役割）、ID、プロジェクト*、プロジェクト割り当て予定時間*、イニシアチブのジョブの役割の時間数、（ジョブの役割）数、カスタムフィールドを含むすべてのプロジェクトフィールド*</td> 
  </tr> 
  <tr> 
   <td><p>[!UICONTROL プロジェクト ]*</p></td> 
   <td> <p>上記のすべてのイニシアチブ情報*</p> </td> 
  </tr> 
 </tbody> 
</table>

*これらのフィールドには、イニシアチブがプロジェクトから作成されたか、少なくとも 1 回プロジェクトに公開された場合にのみ、イニシアチブにリンクされたプロジェクトの情報が入力されます。 イニシアチブの公開について詳しくは、 [プロジェクトを更新または作成するには、 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
