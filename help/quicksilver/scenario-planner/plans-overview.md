---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: シナリオ・プランナのプランの概要
description: ビジネスマネージャーは、Adobe Workfrontシナリオプランナーを使用して、1 年、3 年または 5 年の計画を概説することで、組織の近い将来および長期的な将来に向けた戦略の概要を説明できます。
author: Alina
feature: Workfront Scenario Planner
exl-id: df2b895b-8bc1-4a55-b0d7-8a06db420315
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '1290'
ht-degree: 0%

---

# 「プランの概要」( [!DNL Scenario Planner]

この [!DNL Scenario Planner] に加えて、別のライセンスが必要です。 [!DNL Adobe Workfront] ライセンス。 詳しくは、 [!DNL Workfront Scenario Planner]を参照してください。 [この [!DNL Scenario Planner] 概要](../scenario-planner/scenario-planner-overview.md).

ビジネスマネージャーは、 [!DNL Adobe Workfront Scenario Planner] 1 年、3 年、5 年の計画を概説し、近い将来および長期的な将来の戦略の概要を示します。

## アクセス要件

次の手順で [!DNL Adobe Workfront Scenario Planner] 次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] 計画</a>*</p> </td> 
   <td>[!UICONTROL Business] 以降</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ライセンスの種類*</p> </td> 
   <td> <p>[!UICONTROL レビュー ] 以降 詳しくは、 <a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] ライセンスの概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td> <p>の追加ライセンスを購入する必要があります。 [!DNL Adobe Workfront Scenario Planner] をクリックして、この記事で説明する機能にアクセスします。</p> <p>詳しくは、 [!DNL Workfront Scenario Planner]を参照してください。 <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">を使用するために必要なアクセス [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>[!UICONTROL 表示 ] 以降の [!DNL Scenario Planner]</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>オブジェクト権限</p> </td> 
   <td> <p>プランの [!UICONTROL 表示 ] 権限以上<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (NOTE: this might change if they have permissions for initiatives/ scenarios, etc) 
      </MadCap:conditionalText>
     --></p> <p>プランへの追加アクセス権のリクエストについて詳しくは、 <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">内のプランへのアクセスをリクエスト [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*お持ちのプラン、ライセンスの種類、アクセス権を調べるには、 [!DNL Workfront] 管理者。

## プランの概要

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: add information about utilization percentage for job roles - per this story?? - https://hub.workfront.com/task/5eb0784900083e1f2cabb60d6e0d04d3/overview)</p>
-->

組織の各大まかな結果を特定し、計画として [!DNL Workfront Scenario Planner]. プランは、 [!DNL Scenario Planner]. 計画を容易に実現するために、計画を複数のイニシアチブに分割して、個々の組織単位が完了に向けてどのような手順をとる必要があるかを示すことができます。

その後、実際のプロジェクトとイニシアチブを結び付けて、実際の作業が計画を実際に完了するのにどのように影響するかを示すことができます。 この記事では、プランに関する一般的な情報を提供します。 イニシアチブの詳細については、 [以下のイニシアティブの概要 [!DNL Scenario Planner]](../scenario-planner/initiatives-overview.md).

計画で特定された作業を完了するために必要な労務および財務リソースを定義できます。 また、計画のイニシアチブが完了するために必要な労務および財務リソースも表示できます。

各プランに関する次の情報を見積もって確認できます。

* プランの実行に使用できるジョブロールのタイプと数を見積もります。
* 計画の完了に必要な予算を見積もります。
* イニシアチブに関連付けられた必要な役割に対する各役割の使用率をレビューします。
* 計画の予算の使用率を、イニシアチブに関連するコストと比較して確認します。
* 任意の時点で、計画の正味価値を確認します。
* プランレベルの情報は、別のシナリオを選択した場合に変更されます。 各シナリオには、異なる予算と人物情報が含まれます。

プランの作成について詳しくは、この記事を参照してください。 [でプランを作成および編集 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

シナリオの作成について詳しくは、 [でのプランシナリオの作成と比較 [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

## プランに関する考慮事項

プランを作成する際は、次の点に注意してください。

* チーム、部門全体、または会社全体のプランを作成できます。 プランとは、企業の戦略を高いレベルでまとめた大規模なプランニング・ユニットです。
* 最短の計画は 1 年の期間を持つことができます。 最も長い計画は 5 年の期間を持つことができます。
* 計画に対して実際の作業を行うことはできません。 計画作業を開始するのに必要なリソースと予算があるかどうかを概算できます。 例えば、新しい場所に新しいオフィスを拡張して取得したい場合、最初に上位の管理レベルのプランで、それを行うために必要な手順を説明します。
* 同じプランの複数のシナリオを作成できます。 元のプランに競合するイニシアチブが多すぎる場合は、イニシアチブまたは予算とコストを編集して、プランを完了するのに最適な状況を確認できるシナリオをいくつか作成する必要があります。 イニシアチブは、同じ期間に同じリソースを使用しようとすると、互いに競合する可能性があります。 その後、シナリオを比較して、実際の作業を追加して実行する前に、何が最も意味を持ち、どの会社を採用すべきかを確認できます。 シナリオの作成について詳しくは、「 [でのプランシナリオの作成と比較 [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).
* プランに複数のイニシアチブを追加して、小さいプラン・ユニットがプランの完了にどの程度貢献するかを指定できます。 例えば、特定の市場に進出する予定がある場合、組織のあらゆるレベルでの拡大を達成するために最終的に貢献する部門レベルの複数のイニシアチブを持つことができます。 イニシアチブの作成について詳しくは、「 [のイニシアチブを作成および編集します [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).
* プランを作成する場合、プランを表示できるのは自分だけです。 プランは他のユーザーと共に作成する必要があり、少なくとも次のユーザーに対する表示アクセス権がある場合は、そのユーザーがプランにアクセスできるようにする必要があります： [!DNL Scenario Planner] 」と表示されます。

## プランのジョブロール情報

計画に使用可能な役割の数と、計画の完了に必要な役割の数を示す計画に関する、役割の一般情報を確認できます。 この情報は、 [!UICONTROL ジョブの役割] 」ボックスを使用して、プランのヘッダーに表示されます。

![](assets/job-role-box-on-plan-not-expanded-fte-350x141.png)

「ジョブの役割」ボックスには、次の情報が表示されます。

| 情報 | 説明 |
|---|---|
| FTE/時間インジケーター | ([!UICONTROL FTE]) または ([!UICONTROL 時間]) 指標を「[!UICONTROL ジョブの役割]「タイトルは、プランが作成時に FTE を使用するように設定されたか、時間を使用するように設定されたかを示します。 この単位は、プラン、すべてのシナリオ、およびイニシアチブで使用されます。 |
| [!UICONTROL 利用可能] | 現在のシナリオで使用可能なジョブロールの工数または時間数。 |
| 必須 | 現在のシナリオのすべてのイニシアチブで、完了するために必要なジョブロールの工数または時間数。 |

プランへのアクセスおよびジョブの役割に関する詳細情報の表示については、 [でプランを作成および編集 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## プランの財務情報

計画、特に計画予算、その予算の使用方法、計画の純価値に関する財務情報を確認できます。 計画の正味価値は、その構想の正味価値に基づいています。 この情報は、 [!UICONTROL 金融] および [!UICONTROL 概要] 」ボックスを使用して、プランのヘッダーに表示されます。

![](assets/budget-net-value-boxes-on-plan-not-expanded-350x86.png)

以下は、 [!UICONTROL 金融] および [!UICONTROL 概要] ボックスを使用して、プランに表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL 予算 ] </p> <p role="rowheader"> </p> </td> 
   <td>これは、プランの実行に使用できる金額を会社が決定した金額です。 Workfrontは、計画期間内に、各月の予算を均等に配分します。 予算は通常 1 年に設定されますが、3 年または 5 年に設定することもできます。 [ 財務 ] ボックスのタイトルの左側にある括弧内の通貨は、システムの通貨を示します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL コスト ]</td> 
   <td> <p>これは、プランのすべてのイニシアチブから発生したコストの合計です。 Workfrontは、次の式を使用して計画のコストを計算します。</p> <p><code>Plan Costs = SUM(Initiative Costs)</code> </p> <p>イニシアチブ・コストの計算方法については、 <a href="../scenario-planner/create-and-edit-initiatives.md" class="MCXref xref">のイニシアチブを作成および編集します [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">UTIL （予算使用率の割合）</td> 
   <td> <p>これは、イニシアチブに関連するコストと計画に定義された予算との間の計算済みの割合です。 </p> <p>[!DNL Workfront] 次の式を使用して、計画の予算稼働率を計算します。 </p> <p><code>Utilization percentage = (Plan Costs* 100))/ Plan Budget</code> </p> <p>コストは次の式を使用して計算されます。</p> <p><code>Plan Costs = SUM(Initiatives People Costs, Initiatives Fixed Costs)</code> </p> <p>ヒント：使用率は丸められ、小数点以下 1 桁です。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL Net Value] 領域 <span>（[!UICONTROL 概要 ] ボックス）</span></p> <p role="rowheader"> </p> </td> 
   <td> <p>これは、プラン内のすべてのイニシアチブのすべての純値の計算です。 </p> <p>Workfrontは、次の式を使用して計画の正味値を計算します。 </p> <p><code>Plan Net Value = SUM(Initiative Planned Benefit - People Costs)</code> </p> <p>または</p> <p><code>Plan Net Value = SUM(Initiative Net Value)</code> </p> <p>[ イニシアチブの純値 ] の詳細については、この記事を参照してください。 <a href="../scenario-planner/initiatives-overview.md" class="MCXref xref">以下のイニシアティブの概要 [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

プランへのアクセスおよびプランに関する詳細な財務情報の表示については、 [でプランを作成および編集 [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).


