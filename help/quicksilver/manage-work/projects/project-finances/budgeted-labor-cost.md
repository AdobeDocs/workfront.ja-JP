---
content-type: reference
product-area: projects
navigation-topic: financials
title: プロジェクトの予算人権費と予算時間の概要
description: プロジェクトの予算人権費と予算時間の概要
author: Alina
feature: Work Management
exl-id: 01020bbb-7cf9-4461-b0b6-dcbbc537c616
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '1128'
ht-degree: 100%

---

# プロジェクトの予算人権費と予算時間の概要

<!--
<(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)</p>
-->

Adobe Workfront リソースプランナーを使用して、作業用リソースを予算計上できます。

プロジェクトで作業用のリソースを予算計上すると、Workfront では、1 時間当たりのコストの値に基づいて、役割、プロジェクトおよびユーザーの予算計上労力コストが計算されます。

プロジェクトのリソースプランナー予算計上労力コストは、プロジェクトの作業を完了するために割り当てられた担当業務に関連するコストおよび各役割の作業を完了するためにかかると推定される予定時間数（リソースプラナー予算計上時間数）との間の計算です。

>[!IMPORTANT]
>
>ユーザーのリソースプランナーの予算計上労力コストは、プロジェクトの予算計上労力コストには影響しません。担当業務の労力コストのみがプロジェクトのコストに影響します。

## 担当業務とプロジェクトの予算計上労力コストの概要

Workfront は、プロジェクトでの担当業務の予算計上労力コストを使用して、プロジェクトの予算計上労力コストを計算します。

>[!TIP]
>
>ビジネスケースでのプロジェクトの予算計上労力コストは、レポートおよびリストで、リソースプランナーの予算計上労力コストとして表示されます。

プロジェクトの&#x200B;**予算計上労力コスト**（またはリソースプラナーの予算計上労力コスト）は、次の式で計算されます。

`Resource Planner Budgeted Labor Cost = SUM ( Resource Planner Budgeted Hours for each job role on the project * Cost per Hour rate of each job role on the project)`

上記の計算で使用されるフィールドは、次を参照します。

* プロジェクトまたはリソースプランナーのリソース予算計上エリアで、担当業務について予算計上された時間数。

  リソースプランナーのリソースの予算計上について詳しくは、[リソースプランナーの概要](../../../resource-mgmt/resource-planning/get-started-resource-planner.md)の記事の「リソースプランナーのリソースの予算計上」の節を参照してください。

  ビジネスケースのリソース予算計上エリアでのリソース予算計上について詳しくは、[ビジネスケースのリソース予算計上](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)を参照してください。

* 上記の計算の&#x200B;**担当業務の 1 時間あたりのコスト率**&#x200B;は、プロジェクトの各担当業務に関連付けられたコストを指します。\
  担当業務の作成と管理およびコスト率との関連付けについて詳しくは、[担当業務の作成と管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)を参照してください。

>[!NOTE]
>
>Workfront は、プロジェクトの通貨を使用してすべてのコスト情報を計算します。リソースプランナーでリソースに予算計上時間数を指定した場合、プロジェクト通貨を変更するオプションは無効になります。\
>プロジェクトの通貨の変更について詳しくは、[プロジェクトの通貨の変更](../../../manage-work/projects/project-finances/change-project-currency.md)を参照してください。

## ユーザーの予算計上労力コストの概要

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Update the following section in the Create a Business Case article, as well, when you update it here.)</p>
-->

>[!IMPORTANT]
>
>ユーザーの予算計上労力コストは、プロジェクトの予算計上労力コストに影響しません。プロジェクトでの担当業務の労力コストのみが、プロジェクトのリソースプランナー予算計上労力コストに影響します。
> 
>すべてのユーザーの労力コストの合計は、ユーザーに関連付けられた担当業務のリソースプランナー予算計上労力コストと等しい場合もあれば異なる場合もあります。
>
>リソースプランナーでユーザーの予算計上時間数を見積もる場合、ユーザーに関連付けられたコストは、ユーザーに関連付けられた担当業務のコストになります。ユーザーやそのレートに関連するコストではありません。

ユーザーがプロジェクトの担当業務に関連付けられ、その時間数がリソースプランナーで予算計上されている場合、その予算計上労力コストは、Workfront での表示場所に応じて、次の名前で表示されます。

* [!UICONTROL **予算計上労力コスト**]：ビジネスケースのリソース予算計上エリアでのそれぞれの役割下。

  ![](assets/budgeted-labor-cost-for-users-in-business-case-highlighted-350x73.png)

* [!UICONTROL **BDG**]：プロジェクトおよび役割ビューで情報をコスト別に表示する場合のリソースプランナー。

  ![](assets/budgeted-labor-cost-for-users-in-rp-project-view-cost--highlighted-350x115.png)

次の要件を満たす場合、ユーザーは、ビジネスケースのリソース予算計上エリアで、それぞれの役割の下またはリソースプランナーに表示されます。

* プロジェクト上の担当業務の 1 つに関連付けられている。
* リソースプランナーで予算計上時間数が指定されている。
* プロファイルで 1 時間当たりのコスト率が関連付けられている。

  1 時間当たりのコスト率とユーザーとの関連付けの詳細については、[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

* ユーザーは、プロジェクトに関連付けられたリソースプールの 1 つに属しています。

ユーザーの予算計上労力コストは、次の式で計算されます。

`User Budgeted Labor Cost = Budgeted hours for the user on the project * Cost per Hour rate of the user`

## プロジェクトの予算計上労力コストの検索

ビジネスケースのリソース予算計上エリアまたはリソースプランナーに反映された予算計上リソースは、Workfront の次のエリアに次の名前で表示されます。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>予算計上労力コストの表示名</strong></td> 
     <td><strong>Workfront のエリア</strong></td> 
    </tr> 
    <tr> 
     <td>予算計上労力コスト</td> 
     <td>ビジネスケースのリソース予算計上エリア</td> 
    </tr> 
    <tr> 
     <td>予算計上コスト</td> 
     <td><p>稼働率レポートのコストビュー</p><p>詳しくは、<a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">稼働率情報の表示</a>を参照してください。</p></td> 
    </tr> 
    <tr> 
     <td>BDG </td> 
     <td>リソースプランナープロジェクトビューまたは役割ビュー（コスト別）</td> 
    </tr> 
    <tr> 
     <td>リソースプランナーのプロジェクト予算計上労力コスト</td> 
     <td> <p>プロジェクトレポート</p> <p>プロジェクト（財務データ）レポート</p> <p>タスクレポート</p> <p>イシューレポート</p> <p>予算計上時間数レポート</p> <p>レポートの作成について詳しくは、<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">カスタムレポートの作成</a>を参照してください。</p> </td> 
    </tr> 
   </tbody> 
  </table>

>[!NOTE]
>
>Adobe Workfront シナリオプランナーを使用してプロジェクトリソースの予算を計上する場合、ビジネスケースのリソース予算計上領域の予算計上労力コストは、プロジェクトにリンクされているイニシアチブの人件費と同じになります。シナリオプランナーは、新しい Adobe Workfront エクスペリエンスでのみ使用でき、追加のライセンスが必要です。Workfront シナリオプランナーについて詳しくは、[シナリオプランナーの概要](../../../scenario-planner/scenario-planner-overview.md)を参照してください。シナリオプランナーを使用したリソースの予算作成について詳しくは、[シナリオプランナーを使用したビジネスケースのリソースの予算作成](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md)を参照してください。

## プロジェクトの予算時間を検索する

<!--
(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)
-->

予算計上時間数は、プロジェクトの予算労力コスト（またはリソースプランナーの予算コスト）の値に影響を与えます。

プロジェクトの予算労力コストは、プロジェクトの作業を完了するために割り当てられた担当業務に関連するコストと、各役割が作業を完了するために必要になる推定時間数（予算計上時間数）です。

次の表に示すフィールドで、Workfront の予算計上時間数を表示できます。

>[!NOTE]
>
>Workfront の「予算計上時間数」に関する他の明記では、Workfront から削除および非推奨の機能を使用して予算計上された時間数を指します。これらは、表示のみのフィールドで、現在のリソース予算計上ツールを使用する際に、現在の情報では更新されません。

ビジネスケースまたはリソースプランナーのリソース予算計上エリアで予算計上された時間は、Workfront の次のエリアに次の名前で表示されます。

* **時間**：ビジネスケースのリソース予算計上エリア
* **BDG**：時間単位で表示されたリソースプランナー
* **予算計上時間数**：稼動率レポートの時間数表示
詳しくは、[リソース稼動率情報を表示](../../../resource-mgmt/resource-utilization/view-utilization-information.md)を参照してください。
* **予算計上時間数**：予算計上時間数レポート

  予算計上時間数レポートの予算計上時間数オブジェクトは、非推奨であるリソース管理ツールに関連する情報を参照します。このレポートの「予算時間」フィールドのみが、プロジェクトのビジネスケースのリソースプランナーまたはリソース予算計上エリアで予算計上された時間数を参照します。

  レポートの作成について詳しくは、**カスタムレポートの作成**&#x200B;を参照してください。
* **リソースプランナーの予算計上時間数**：次のレポート内：

   * プロジェクトレポート
   * プロジェクト（財務データ）レポート
   * タスクレポート
   * イシューレポート
   * 予算計上時間数レポート
