---
content-type: reference
product-area: projects
navigation-topic: financials
title: プロジェクトの予算労務費と予算時間の把握
description: プロジェクトの予算労務費と予算時間の把握
author: Alina
feature: Work Management
exl-id: 01020bbb-7cf9-4461-b0b6-dcbbc537c616
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 0%

---

# プロジェクトの予算労務費と予算時間の把握

<!--
<(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)</p>
-->

Adobe Workfront Resource Planner を使用すると、作業用にリソースを予算設定できます。

プロジェクトでの作業用のリソースを予算化すると、Workfrontでは、時間当たりの原価の値に基づいて、役割、プロジェクトおよびユーザーの予算労務費が計算されます。

プロジェクトのリソース・プランナの予算労務費は、プロジェクトの作業を完了するために割り当てられた役職に関連する原価と、各役割が作業を完了するために必要になる推定時間数（リソース・プランナの予算時間）との間の計算です。

>[!IMPORTANT]
>
>ユーザーのリソース・プランナの予算労務費は、プロジェクトの予算労務費には影響しません。 プロジェクトのコストに影響を与えるのは、ジョブロールの人件費だけです。

## 役職の予算労務費とプロジェクトの概要

Workfrontは、プロジェクトの役職の予算労務費を使用して、プロジェクトの予算労務費を計算します。

>[!TIP]
>
>ビジネス・ケースのプロジェクトの予算労務費は、レポートおよびリストで、リソース・プランナの予算労務費として表示されます。

この **予算労務費** プロジェクトの（または Resource Planner の予算労務費）は、次の式で計算されます。

`Resource Planner Budgeted Labor Cost = SUM ( Resource Planner Budgeted Hours for each job role on the project * Cost per Hour rate of each job role on the project)`

上記の計算で使用されるフィールドは、次を参照します。

* プロジェクトまたはリソース・プランナの「生産資源予算設定」領域での製造オーダーの役割に予算を作成する時間数。

   リソース・プランナの予算リソースの詳細は、この記事の「リソース・プランナの予算リソース」の節を参照してください [リソースプランナーの概要](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   ビジネス・ケースの「生産資源予算作成」領域での生産資源の予算作成の詳細は、 [ビジネス事例の予算リソース](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

* この **ジョブロールの 1 時間あたりのコスト率** 上記の計算では、プロジェクトの各ジョブの役割に関連付けられたコストを指します。\
   ジョブの役割の作成と管理、およびコスト率との関連付けについて詳しくは、この記事を参照してください [ジョブの役割の作成と管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

>[!NOTE]
>
>Workfrontは、プロジェクトの通貨を使用してすべてのコスト情報を計算します。 リソース・プランナでリソースに予算時間を指定した場合、プロジェクト通貨を変更するオプションは無効になります。\
>プロジェクトの通貨の変更の詳細については、「 [プロジェクト通貨を変更](../../../manage-work/projects/project-finances/change-project-currency.md).

## ユーザーの予算労務費の概要

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Update the following section in the Create a Business Case article, as well, when you update it here.)</p>
-->

>[!IMPORTANT]
>
>ユーザーの予算労務費は、プロジェクトの予算労務費には影響しません。 プロジェクトのジョブ・ロールの労務費のみが、プロジェクトのリソース・プランナの予算労務費に影響を与えます。
> 
>すべてのユーザーの全労務費の合計は、ユーザーに関連付けられたジョブロールのリソース・プランナの予算労務費と等しくなる場合と異なる場合があります。
>
>リソース・プランナでユーザーの予算時間を見積もる場合、ユーザーに関連付けられた原価は、ユーザーに関連付けられた役職の原価になります。 ユーザーやその料金に関連するコストではありません。

ユーザーがプロジェクトの役職に関連付けられ、その時間がリソース・プランナで予算に入っている場合、その予算労務費は、Workfrontでの表示場所に応じて、次の名前で表示されます。

* [!UICONTROL **予算労務費**]:ビジネス・ケースの各ロールの下のリソース予算領域。

   ![](assets/budgeted-labor-cost-for-users-in-business-case-highlighted-350x73.png)

* [!UICONTROL **BDG**]:「プロジェクト」ビューと「ロール」ビューの情報を原価別に表示する場合の「リソース・プランナ」。

   ![](assets/budgeted-labor-cost-for-users-in-rp-project-view-cost--highlighted-350x115.png)

次の要件を満たす場合は、ビジネス・ケースの「生産資源予算設定」領域に、それぞれの役割の下、または生産資源プランナに表示されます。

* プロジェクト上のジョブの役割の 1 つに関連付けられています。
* リソース・プランナで予算時間が指定されています。
* 顧客のプロファイルには「時間あたりのコスト」レートが関連付けられています。

   ユーザーに時間あたりのコスト率を追加する方法の詳細については、 [ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* ユーザーは、プロジェクトに関連付けられたリソースプールの 1 つに属しています。

ユーザーの予算労務費は、次の式で計算されます。

`User Budgeted Labor Cost = Budgeted hours for the user on the project * Cost per Hour rate of the user`

## プロジェクトの予算労務費の検索

ビジネス・ケースの「生産資源予算」領域または「生産資源計画担当」領域に反映された予算労務費は、Workfrontの次の領域に、次の名前で表示されます。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>予算労務費表示名</strong></td> 
     <td><strong>Workfrontの面積</strong></td> 
    </tr> 
    <tr> 
     <td>予算計上労力コスト</td> 
     <td>ビジネス事例のリソース予算領域</td> 
    </tr> 
    <tr> 
     <td>予算計上コスト</td> 
     <td><p>使用率レポートのコストビュー</p><p>詳しくは、 <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">使用率情報の表示</a> .</p></td> 
    </tr> 
    <tr> 
     <td>BDG </td> 
     <td>リソースプランナープロジェクトビューまたはロールビュー（コスト別）</td> 
    </tr> 
    <tr> 
     <td>生産資源プランナ・プロジェクトの予算労務費</td> 
     <td> <p>プロジェクトレポート</p> <p>プロジェクト（金融データ）レポート</p> <p>タスクレポート</p> <p>問題レポート</p> <p>予算時間レポート</p> <p>レポートの作成について詳しくは、 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">カスタムレポートの作成</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>

>[!NOTE]
>
>Adobe Workfrontシナリオ・プランナを使用してプロジェクト・リソースを予算する場合、ビジネス・ケースの「生産資源予算」領域の予算労務費は、プロジェクトにリンクされているイニシアチブの「個人原価」と同じになります。 シナリオプランナーは、新しいAdobe Workfrontエクスペリエンスでのみ使用でき、追加のライセンスが必要です。 Workfront Scenario Planner の詳細は、 [シナリオプランナーの概要](../../../scenario-planner/scenario-planner-overview.md). シナリオ・プランナを使用したリソースの予算作成の詳細は、 [シナリオ・プランナを使用したビジネス・ケースの予算生産資源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## プロジェクトの予算時間の検索

<!--
(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)
-->

予算時間は、プロジェクトの予算労務費（またはリソースプランナの予算原価）の値に影響を与えます。

プロジェクトの予算労務費は、プロジェクトの作業を完了するために割り当てられた役職に関連する原価と、各役割が作業を完了するために必要になる推定時間数（予算時間）です。

次の表に示すフィールドで、Workfrontの予算時間を表示できます。

>[!NOTE]
>
>Workfrontでの「Budgeted Hours」のその他の言及は、Workfrontから削除された廃止された機能を使用して予算に入った時間を指します。 これらは表示のみのフィールドで、現在のリソース予算ツールを使用する際に、現在の情報では更新されません。

ビジネス・ケースの「生産資源予算編成」領域または「生産資源計画担当」領域に予算計上された時間は、Workfrontの次の領域と、次の名前で表示されます。

* **時間**:ビジネス事例のリソース予算領域
* **BDG**：時間単位で表示されたリソースプランナー
* **予算時間**:稼働状況レポート時間表示詳しくは、 [リソース使用率情報の表示](../../../resource-mgmt/resource-utilization/view-utilization-information.md).
* **バド。 時間**:予算時間レポート

   予算時間レポートの予算時間オブジェクトは、廃止されたリソース管理ツールに関連する情報を参照します。 「バドだけ。 このレポートの「時間」フィールドは、プロジェクトのビジネスケースの「リソース・プランナ」または「リソース予算設定」領域で予算された時間を参照します。

   レポートの作成について詳しくは、 **カスタムレポートの作成**.
* **リソースプランナーの予算時間**:次のレポート内：

   * プロジェクトレポート
   * プロジェクト（金融データ）レポート
   * タスクレポート
   * 問題レポート
   * 予算時間レポート
