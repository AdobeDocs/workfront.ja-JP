---
content-type: overview
product-area: projects
navigation-topic: financials
title: プロジェクトの財務情報フィールド
description: プロジェクトを管理するには、プロジェクトの財務状況を把握することが重要です。
author: Alina
feature: Work Management
exl-id: a5e69dea-d0aa-47cd-9b59-6199cec56fe4
source-git-commit: fb1c7ade6622db391e0dac54f37603efe9dc0a58
workflow-type: tm+mt
source-wordcount: '594'
ht-degree: 99%

---

# プロジェクトの財務情報フィールド

プロジェクトを管理するには、プロジェクトの財務状況を把握することが重要です。

プロジェクトマネージャーは、一部の財務フィールドを手動で更新できます。その他の財務データは、Adobe Workfront によって自動的に計算されます。

Workfront では、予算、コストおよび収益をキャプチャする多数のフィールドを使用して財務状況を追跡できます。

詳しくは、次の記事も参照してください。

* [Adobe Workfront の用語集](../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)
* [プロジェクトの財政状況：記事インデックス](../../../manage-work/projects/project-finances/project-finances-overview.md)
* [プロジェクトの財務エリアでの情報の管理](../../../manage-work/projects/project-finances/manage-project-finance-area.md)
* [タスクの詳細セクションでのタスクの財政の管理](../../../manage-work/tasks/manage-tasks/task-finances-in-details.md)

## Workfront における財務上の計算方法

Workfront のプロジェクトおよびタスクレベルで、財務フィールドをトラックできます。イシューに関して、限られた財務フィールドを常にトラックできます。

次の表に、Workfront でトラック可能な財務情報およびどのオブジェクトに関する財務情報をトラックできるかを示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>財務フィールド</th> 
   <th>フィールドの説明</th> 
   <th>タスク</th> 
   <th>プロジェクト</th> 
   <th>イシュー</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>時間</td> 
   <td> プロジェクトでの時間の記録について詳しくは、<a href="../../../timesheets/create-and-manage-timesheets/log-time.md" class="MCXref xref">時間の記録</a>を参照してください。 </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td> コスト</td> 
   <td>コストのトラックについて詳しくは、<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストのトラック</a>を参照してください。</td> 
   <td>✔</td> 
   <td>✔</td> 
   <td>✔</td> 
  </tr> 
  <tr> 
   <td>予算</td> 
   <td> <p>プロジェクトの予算について詳しくは、<a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">プロジェクトの財務エリアでの情報管理</a>を参照してください。</p> <p>プロジェクトのリソースの予算について詳しくは、<a href="../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md" class="MCXref xref">ビジネスケースでのリソースの予算</a>を参照してください。</p> </td> 
   <td> </td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>請求記録</td> 
   <td>請求記録の作成について詳しくは、<a href="../../../manage-work/projects/project-finances/create-billing-records.md" class="MCXref xref">請求記録の作成</a>を参照してください。</td> 
   <td> </td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>収益</td> 
   <td> 請求と収益について詳しくは、<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">請求と収益の概要</a>を参照してください。 </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>費用</td> 
   <td>費用管理について詳しくは、<a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">プロジェクト費用の管理</a>を参照してください。</td> 
   <td>✔</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>請求レート</td> 
   <td> <p>ユーザーまたは担当業務の請求レートを設定できます。</p> <p>ユーザーと請求料率の関連付けについて詳しくは、<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">ユーザーのプロファイルの編集</a>を参照してください。</p> <p>担当業務と請求レートの関連付けについて詳しくは、<a href="../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md" class="MCXref xref">担当業務の作成と管理</a>を参照してください。</p> <p>請求レートは、プロジェクトとタスクの収益を計算します。プロジェクトまたは会社に対する担当業務の請求レートを上書きできます。 </p> <p>プロジェクトの請求レートの上書きについて詳しくは、<a href="../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md" class="MCXref xref">担当業務に対する請求レートの上書きとプロジェクトにおける収益の計算の概要</a>を参照してください。</p> <p>会社の請求レートの上書きについて詳しくは、<a href="../../../manage-work/projects/project-finances/override-project-level-with-company-level-billing-rates.md" class="MCXref xref">プロジェクトレベルの請求レートを会社レベルの請求レートで上書き</a>を参照してください。</p> </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>投資回収率（ROI）</td> 
   <td> ROI の計算について詳しくは、<a href="../../../manage-work/projects/project-finances/calculate-roi.md" class="MCXref xref">投資回収率（ROI）を計算</a>を参照してください。 </td> 
   <td> </td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>対純価危険</td> 
   <td>純価に対するリスク計算について詳しくは、<a href="../../../manage-work/portfolios/portfolio-optimizer/calculate-risk-to-net-value-in-portfolio.md" class="MCXref xref">ポートフォリオの純価に対するリスクを計算</a>を参照してください。</td> 
   <td> </td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>パフォーマンスのメトリック</td> 
   <td> <p>パフォーマンスのメトリックは、特定の時点でのプロジェクトやタスクのパフォーマンスを示します。パフォーマンスのメトリックは、Workfront がタスクとプロジェクトに対して自動で実行する計算です。Workfront で計算できるパフォーマンスのメトリックを、以下の行に一覧で示します。パフォーマンスのメトリックの計算は、使用するパフォーマンスインデックスメソッドのタイプに応じて異なります。 </p> <p>お使いのシステムで使用する PIM の選択について詳しくは、<a href="../../../manage-work/projects/project-finances/set-pim.md" class="MCXref xref">パフォーマンスインデックスメソッド（PIM）の設定</a>を参照してください。</p> </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>完成時総コスト見積り（EAC）</td> 
   <td> EAC の計算について詳しくは、<a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">完了時の推定（EAC）を計算</a>を参照してください。 </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>スケジュール効率指数（SPI）</td> 
   <td>SPI の計算について詳しくは、<a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">スケジュール効率指数（SPI）を計算</a>を参照してください。</td> 
   <td>✔</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>コスト効率指数（CPI）</td> 
   <td>CPI の計算について詳しくは、<a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">コスト効率指数（CPI）を計算</a>を参照してください。</td> 
   <td>✔</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>コストスケジュール効率指数（CSI）</td> 
   <td>CSI の計算について詳しくは、<a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">コストスケジュール効率指数（CSI）を計算</a>を参照してください。</td> 
   <td>✔</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>予定作業時間コスト（BCWS、Budgeted Cost of Work Scheduled）</td> 
   <td>パフォーマンス指標。BCWS の計算の詳細については、<a href="../../../manage-work/projects/project-finances/calculate-bcws.md" class="MCXref xref">予定された作業の予算計上コスト（BCWS）の計算</a>を参照してください。 </td> 
   <td>✔</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td>実行された作業の予算計上コスト（BCWP、Budgeted Cost of Work Performed）</td> 
   <td>パフォーマンス指標。BCWP の計算の詳細については、<a href="../../../manage-work/projects/project-finances/calculate-bcwp.md" class="MCXref xref">実行された作業の予算計上コスト（BCWP）の計算</a>を参照してください。</td> 
   <td>✔</td> 
   <td>✔</td> 
   <td> </td> 
  </tr> 
 </tbody> 
</table>

 
