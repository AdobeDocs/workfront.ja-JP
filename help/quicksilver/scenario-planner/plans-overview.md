---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: シナリオプランナーの計画の概要
description: ビジネスマネージャーは、Adobe Workfront シナリオプランナーを使用して、1年、3年、または 5年計画の概要を示し、組織の短期および長期の将来の戦略を概説できます。
author: Alina
feature: Workfront Scenario Planner
exl-id: df2b895b-8bc1-4a55-b0d7-8a06db420315
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: ht
source-wordcount: '1290'
ht-degree: 100%

---

# [!DNL Scenario Planner] の計画概要

[!DNL Scenario Planner] には、[!DNL Adobe Workfront] ライセンスに加えて別のライセンスが必要です。[!DNL Workfront Scenario Planner] について詳しくは、[ [!DNL Scenario Planner]  の概要](../scenario-planner/scenario-planner-overview.md)を参照してください。

ビジネスマネージャーは、[!DNL Adobe Workfront Scenario Planner] を使用して、1年、3年、または 5年計画の概要を示し、組織の短期的および長期的な将来の戦略を概説できます。

## アクセス要件

[!DNL Adobe Workfront Scenario Planner] を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] プラン</a>*</p> </td> 
   <td>[!UICONTROL Business] 以降</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ライセンスタイプ*</p> </td> 
   <td> <p>[!UICONTROL Review]以上詳しくは、<a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront]ライセンスの概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td> <p>この記事で説明する機能にアクセスするには、[!DNL Adobe Workfront Scenario Planner] 用の追加ライセンスを購入する必要があります。</p> <p>[!DNL Workfront Scenario Planner] の取得について詳しくは、<a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">[!DNL Scenario Planner]</a> を使用する場合に必要なアクセス権を参照してください。 </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>[!UICONTROL View]以上のアクセス権 [!DNL Scenario Planner]</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>オブジェクト権限</p> </td> 
   <td> <p>計画に対する[!UICONTROL View]以上の権限<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (NOTE: this might change if they have permissions for initiatives/ scenarios, etc) 
      </MadCap:conditionalText>
     --></p> <p>プランへの追加アクセス権のリクエストについて詳しくは、<a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">[!DNL Scenario Planner]</a>でのプランへの利用申請を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

*ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront]管理者にお問い合わせください。

## 計画の概要

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: add information about utilization percentage for job roles - per this story?? - https://hub.workfront.com/task/5eb0784900083e1f2cabb60d6e0d04d3/overview)</p>
-->

組織の各高レベルの成果を特定し、それを計画として [!DNL Workfront Scenario Planner] に追加できます。計画は、[!DNL Scenario Planner] の最大の作業アイテムです。計画の達成を容易にするために、計画を複数の取り組みに分割して、計画の完了に向けて個々の組織単位がどのような手順を実行する必要があるかを示すことができます。

その後、イニシアチブを実際のプロジェクトと関連付けて、実際の作業が実際に計画を完了する際にどのように考慮されるかを示すことができます。この記事では、計画に関する一般的な情報を説明します。イニシアチブの詳細については、[ [!DNL Scenario Planner]](../scenario-planner/initiatives-overview.md) のイニシアチブの概要を参照してください。

計画で特定された作業を完了するために必要な労働力と財務リソースを定義できます。計画内のイニシアチブを完了するために必要な労働力と財務リソースを表示することもできます。

各計画について次の情報を見積もり、確認できます。

* 計画を実行するために利用できる職務の種類と数を見積もります。
* 会社が計画を完了するために必要な予算を見積もります。
* イニシアチブに関して必要な担当業務に対する、各担当業務の稼働率をレビューします。
* イニシアチブに関連するコストに対する計画の予算の稼働率をレビューします。
* 任意の時点での計画の純価値をレビューします。
* 別のシナリオを選択すると、計画レベルの情報が変わります。各シナリオには異なる予算と人材情報があります。

計画の作成の詳細については、[ [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md)での計画の作成と編集を参照してください。

シナリオの作成の詳細については、[ [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md) の計画シナリオの作成と比較を参照してください。

## 計画に関する考慮事項

計画を作成するときは、次の点を考慮してください。

* チーム、部門全体、さらには会社全体の計画を立てることができます。計画は、企業の戦略を高レベルで概説する大きな計画単位です。
* 最も短い計画の期間は 1年間です。最長の計画の期間は 5年間です。
* 計画に基づいて実際の作業を行うことはできません。予定作業を開始するために必要なリソースと予算があるかどうかを大まかに見積もることができます。例えば、会社が拡張して新しい場所に新しいオフィスを取得したい場合、それを達成するために必要な手順を、まず経営幹部レベルの計画で概説できます。
* 同じ計画の複数のシナリオを作成できます。元の計画に矛盾するイニシアチブが多すぎる場合は、計画を達成するための理想的な状況を確認するために、イニシアチブ、予算、コストを編集できるいくつかのシナリオを作成する必要があります。同じ期間内に同じリソースを使用しようとすると、イニシアチブが互いに競合する可能性があります。その後、シナリオを比較して、シナリオを達成するための実際の作業を追加する前に、何が最も合理的で、会社が採用すべきシナリオを確認できます。シナリオの作成の詳細については、[ [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md) のプランシナリオの作成と比較を参照してください。
* 複数のイニシアチブを計画に追加して、より小さなプラン単位が計画の完了にどのように貢献するかを示すことができます。例えば、特定の市場に進出する計画がある場合、部門レベルではいくつもの取り組みが考えられます。それらのイニシアチブは、最終的に、組織のあらゆるレベルでの進出を実現することに貢献します。イニシアチブの作成について詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md) でのイニシアチブの作成と編集を参照してください。
* 計画を作成する際、計画を表示できるのは自分だけです。他のユーザーが計画にアクセスするには、[!DNL Scenario Planner] へのアクセスレベルとして少なくとも表示アクセス権を持っている必要があります。

## 計画の担当業務情報

計画に関する担当業務の一般情報を確認できます。一般情報では、計画で利用できる担当業務の量と、イニシアチブを実施するのに必要な担当業務の量を示しています。この情報は、計画のヘッダーの「[!UICONTROL 担当業務]」ボックスに表示されます。

![](assets/job-role-box-on-plan-not-expanded-fte-350x141.png)

「担当業務」ボックスには、次の情報が表示されます。

| 情報 | 説明 |
|---|---|
| FTE／時間数インジケーター | 「[!UICONTROL 担当業務]」タイトルの横にある「[!UICONTROL FTE]」または「[!UICONTROL 時間数]」のインジケーターは、計画が FTE または時間数のどちらを使用して作成時に設定されたかを示しています。この単位は、計画、すべてのシナリオ、イニシアチブで使用されます。 |
| [!UICONTROL 利用可能] | 現在のシナリオで使用可能な担当業務の FTE または時間数。 |
| 必須 | 現在のシナリオで、すべてのイニシアチブを完了するために必要な担当業務の FTE 数または時間数。 |

計画へのアクセスと、担当業務に関する詳細情報の表示については、[ [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md) での計画の作成と編集を参照してください。

## 計画の財務情報

計画に関する財務情報を確認できます。具体的には、計画した予算、予算の執行状況、計画の正味価値を確認できます。計画の正味価値は、各イニシアチブの正味価値に基づいています。この情報は、計画のヘッダーの「[!UICONTROL 財務]」ボックスと「[!UICONTROL 概要]」ボックスに表示されます。

![](assets/budget-net-value-boxes-on-plan-not-expanded-350x86.png)

以下は、計画の「[!UICONTROL 財務]」ボックスと「[!UICONTROL 概要]」ボックスに表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL Budget] </p> <p role="rowheader"> </p> </td> 
   <td>これは、計画の実施に使用できる、会社が決裁した金額です。Workfront は、計画期間の各月に予算を均等に配分します。予算は通常 1 年に設定されますが、3 年または 5 年に設定することもできます。「財務」ボックスのタイトルの左側にある括弧内の通貨は、システムの通貨を示しています。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costs]</td> 
   <td> <p>これは、計画のすべてのイニシアチブから発生する費用の合計です。Workfront は、次の式を使用して計画の費用を計算します。</p> <p><code>Plan Costs = SUM(Initiative Costs)</code> </p> <p>イニシアチブ費用の計算方法については、<a href="../scenario-planner/create-and-edit-initiatives.md" class="MCXref xref">[!DNL Scenario Planner]</a> でのイニシアチブの作成と編集を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">UTIL（予算使用率）</td> 
   <td> <p>これは、イニシアチブに関する費用と、計画で定めた予算との割合を計算したものです。 </p> <p>[!DNL Workfront] 次の式を使用して、計画の予算使用率を計算します。 </p> <p><code>Utilization percentage = (Plan Costs* 100))/ Plan Budget</code> </p> <p>費用は次の式を使用して計算します。</p> <p><code>Plan Costs = SUM(Initiatives People Costs, Initiatives Fixed Costs)</code> </p> <p>ヒント：使用率は丸められ、小数点以下は 1 桁です。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader"><span>[!UICONTROL Summary]ボックスの</span>[!UICONTROL Net Value]エリア</p> <p role="rowheader"> </p> </td> 
   <td> <p>これは、計画内のすべてのイニシアチブのすべての正味価値を計算したものです。 </p> <p>Workfront は、次の式を使用して計画の正味価値を計算します。 </p> <p><code>Plan Net Value = SUM(Initiative Planned Benefit - People Costs)</code> </p> <p>または</p> <p><code>Plan Net Value = SUM(Initiative Net Value)</code> </p> <p>イニシアチブの正味価値については、<a href="../scenario-planner/initiatives-overview.md" class="MCXref xref">[!DNL Scenario Planner]</a> のイニシアチブの概要の記事を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

計画へのアクセスと、計画に関する詳細な財務情報の表示については、[ [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md) での計画の作成と編集を参照してください。


