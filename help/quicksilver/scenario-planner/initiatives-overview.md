---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Scenario Planner のイニシアチブの概要
description: シナリオプランナーは、新しい Adobe Workfront エクスペリエンスでのみ使用でき、追加のライセンスが必要です。Workfront シナリオプランナーについて詳しくは、シナリオプランナーの概要を参照してください。
author: Alina
feature: Workfront Scenario Planner
exl-id: d67f51e5-7c5c-436b-b0c3-e5afbd7cebca
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: ht
source-wordcount: '956'
ht-degree: 100%

---

# [!DNL Scenario Planner] のイニシアチブの概要

[!DNL Scenario Planner] は、新しい [!DNL Adobe Workfront] エクスペリエンスで使用可能で、追加のライセンスが必要です。[!DNL Workfront Scenario Planner] について詳しくは、[ [!DNL Scenario Planner]  の概要](../scenario-planner/scenario-planner-overview.md)を参照してください。
ビジネスマネージャーとして、[!DNL Adobe Workfront Scenario Planner] でのプランのイニシアチブを作成できます。プランの作成について詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md) でのプランの作成および編集の記事を参照してください。

## イニシアチブの概要

[!DNL Workfront Scenario Planner] を使用して、各イニシアチブについて次の情報を見積もり、確認できます。

* イニシアチブの完了に必要な担当業務のタイプと数量を見積もります。これにより、プランに必要な担当業務数に追加され、イニシアチブで確認できる人件費が計算されます。
* イニシアチブの完了に必要な作業に関連する固定コストを見積もります。
* イニシアチブが完了する際に会社が得る可能性のある予定利益を見積もります。

イニシアチブに関する情報を表示するには、プラン内の個々のイニシアチブにアクセスできます。イニシアチブの作成とアクセスについて詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md) のイニシアチブの作成および編集の記事を参照してください。

## イニシアチブに関する考慮事項

イニシアチブを作成する際は、次の点を考慮してください。

* イニシアチブを作成する前に、プランを作成する必要があります。
* イニシアチブを最初から作成したり、プランにプロジェクトを読み込んだりできます。プロジェクトはプラン内のイニシアチブになります。

  最初からイニシアチブを作成する方法について詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md) でのイニシアチブの作成および編集を参照してください。

  プランにプロジェクトを読み込んで、プロジェクトからイニシアチブを作成する方法について詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) でプランにプロジェクトを読み込むを参照してください。

* イニシアチブはプランよりも小さい計画単位でプランの一部としてのみ作成されます。
* イニシアチブの最短期間は 1 か月です。イニシアチブの最長期間は 5 年です。
* イニシアチブに対する実際の作業を行うことはできません。イニシアチブレベルで、必要なリソースとそれらのリソースに発生するコストを定義して、プランの需要の 1 つを実行できるようにします。例えば、会社が事業を拡大し、新しい場所に新しいオフィスを設けるプランがある場合、所属されている部署にその新しい拠点のネットワークインフラストラクチャを導入するイニシアチブが存在する可能性があります。
* 1 つのプランに複数のイニシアチブを作成できます。各イニシアチブでは、部署での作業を達成するための高レベルな戦略の概要を説明できます。
* プラン内のイニシアチブに優先順位を付けて、最も重要なイニシアチブに対して最も多くの予算と最も多くのリソースを確実に確保されるようにできます。
* プラン内でイニシアチブを作成する場合、そのプランを表示するすべてのユーザーが、プラン内のすべてのイニシアチブを表示することもできます。

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change when we add to the access levels granularity)</p>
  -->

* イニシアチブを公開して、プロジェクトを作成したり、リンクされたプロジェクトを更新したりできます。イニシアチブの公開について詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) でイニチアチブを公開することでプロジェクトの更新または作成を参照してください。

## イニシアチブに関する財務情報

個々のイニシアチブに関する財務情報を確認して、プラン内でのイニシアチブの適合を把握できます。イニシアチブへのアクセスについて詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md) のイニシアチブを作成および編集を参照してください。

プラン内でイニシアチブにアクセスすることで、イニシアチブに関する次の財務指標を表示できます。

<!--
<p>(NOTE: several instances drafted in the table below!) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costs total amount]</td> 
   <td> <p style="font-weight: normal;">これは、イニシアチブの総コストの計算です。 </p> <p style="font-weight: normal;">[!DNL Workfront] この式を使用して、イニシアチブの総コスト値を計算します。</p> <p style="font-weight: normal;"><code>Initiative Costs = Fixed Costs + People Costs</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fixed Costs]</td> 
   <td> <p><span style="font-weight: normal;">これは、<span>イニチアチブの各月の固定コストの月額を見積もることができる手動入力です。</span> これには、「[!UICONTROL People Cost]」フィールドに取り込まれるイニシアチブに追加された役割に関連するコストは含まれません。</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL People Costs]</td> 
   <td> <p style="font-weight: normal;">これは、イニシアチブの期間中にイニシアチブの担当業務に関連付けられたコストの合計計算です。この数は、イニシアチブの各月の担当業務に対して見積もる FTE または時間数によって異なります。 </p> 
     <p><b>ヒント</b>  
     <ul> 
      <li> <p>同じ担当業務の月別の FTE の数は、月ごとに異なる場合があります。</p> </li> 
      <li> <p>[!DNL Workfront] では、1 か月に 160 時間の労働時間があると考えます。 </p> </li> 
     </ul> 
     <p>[!DNL Workfront] は、次の式を使用してイニシアチブの [!UICONTROL People Costs] を計算します。</p> <p><code>Initiative People Costs = SUM(Monthly people cost)</code> </p> 
    <p> [!DNL Workfront] は次の式を使用して、イニシアチブ期間中の毎月の人件費を計算します。</p> 
     <p><code>Monthly People Costs = SUM(Job role hourly rate * 160 * Number of FTEs)</code> </p> 
      <p><b>例</b></p>
      <p>イニシアチブの期間が 6 か月で、毎月デザイナー（1 FTE に対する時間レート：50 ドル）が 1 人、イニシアチブの 2 か月について Web デザイナー（時間レート：100 ドル）が 1 人必要な場合、イニシアチブの人件費は次のように算出されます。</p>
      <code>Initiative People Costs = 50*160*6 + 100*160*2 = 48,000 + 32,000 = 80,000</code>        
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planned Benefit]</td> 
   <td>このイニシアチブを完了することで、部門が得る全体的な利益を見積もるための、手動入力です。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Net Value amount]</td> 
   <td> <p style="font-weight: normal;">全体的なコストと、イニシアチブに関して推定される予定利益を考慮する際のイニシアチブの価値を表します。[!DNL Workfront] は、次の式を使用してイニシアチブの正味価値を計算します。</p> <p style="font-weight: normal;"><code>Initiative Net Value = Initiative Planned Benefit - Initiative Costs</code> </p> </td> 
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

以下の表に示すように、イニシアチブ情報をレポートに表示できます。この情報は、会社が Workfront Scenario Planner ライセンスを購入した場合にのみ、Workfront インスタンスで使用できます。

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
   <td>名前、期間、開始日と終了日、入力者、ID、最終公開日*、カスタムフィールドを含むすべてのプロジェクトフィールド*</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Job Role]</td> 
   <td>上記のすべてのイニシアチブ情報、（担当業務）ID、プロジェクト*、プロジェクト割り当て予定時間*、イニシアチブの担当業務の時間数、（担当業務）数、カスタムフィールドを含むすべてのプロジェクトフィールド*</td> 
  </tr> 
  <tr> 
   <td><p>[!UICONTROL Project]*</p></td> 
   <td> <p>上記のすべてのイニシアチブ情報*</p> </td> 
  </tr> 
 </tbody> 
</table>

*これらのフィールドには、イニシアチブがプロジェクトから作成されたか、少なくとも 1 回プロジェクトに公開された場合にのみ、イニシアチブにリンクされたプロジェクトの情報が入力されます。イニシアチブの公開について詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) でイニシアチブを公開することでプロジェクトを更新または作成を参照してください。
