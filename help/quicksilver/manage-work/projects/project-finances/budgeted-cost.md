---
content-type: reference
product-area: projects
navigation-topic: financials
title: 予算コストの計算
description: 稼働率レポートを使用した予算計上コスト追跡プロジェクトの進捗の計算
author: Alina
feature: Work Management
exl-id: e96fe38f-58c2-4938-9d2d-81d1109123fa
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '394'
ht-degree: 100%

---

# 予算コストの計算

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked from "Tracking Project Progress with a Utilization Report"</p>
<p>Keep the structure of this article similar to Calculating Budgeted Labor Cost)</p>
</div>
-->

プロジェクトの予算計上コストは、プロジェクトの計画時に見積もられた、プロジェクトに関連する合計コストです。

## プロジェクトの予算計上コストの概要

プロジェクトの予算計上コストは手動で変更できません。Adobe Workfront は、次の式を使用して予算計上コストを計算します。

`Budgeted Cost = Resource Planner Budgeted Labor Cost + Budgeted Expenses Cost + Fixed Cost of the project`

* 上記の計算での&#x200B;**リソースプランナーの予算計上労力コスト**&#x200B;は、プロジェクトの担当業務に関連付けられたコストです。

  プロジェクトの予算計上労力コストは、ビジネスケースまたはリソースプランナーのリソース予算計上エリアで追跡できます。

  >[!TIP]
  >
  >  ビジネスケースでのプロジェクトの予算計上労力コストは、レポートおよびリストで、リソースプランナーの予算計上労力コストとして表示されます。

  予算計上労力コストの計算について詳しくは、[プロジェクトの予算計上労力コストと予算計上時間数について](../../../manage-work/projects/project-finances/budgeted-labor-cost.md)を参照してください。

* 上記の計算での&#x200B;**予算計上費用コスト**&#x200B;は、ビジネスケースの費用エリアまたはプロジェクトの「費用」タブで計算される、プロジェクトの費用に関連付けられた予定コストです。\
  プロジェクトの費用について詳しくは、[プロジェクト費用の管理](../../../manage-work/projects/project-finances/manage-project-expenses.md)の記事を参照してください。

* 上記の計算の&#x200B;**固定コスト**&#x200B;は、プロジェクトの詳細セクションの財務エリアで定義されている、プロジェクトのコストに関連する固定金額です。\
  プロジェクトの「財務」サブタブについて詳しくは、[プロジェクトの財務エリアでの情報管理](../../../manage-work/projects/project-finances/manage-project-finance-area.md)の記事を参照してください。

>[!NOTE]
>
>Workfront は、プロジェクトの通貨を使用してすべてのコスト情報を計算します。リソースプランナーでリソースに予算計上時間数を指定した場合、プロジェクト通貨を変更するオプションは無効になります。
>
>プロジェクトの通貨の変更について詳しくは、[プロジェクトの通貨の変更](../../../manage-work/projects/project-finances/change-project-currency.md)を参照してください。

## プロジェクトの予算コストの検索

ビジネスケースのリソース予算計上エリアまたはリソースプランナーに反映された予算計上リソースは、Workfront の次のエリアに次の名前で表示されます。

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>予算計上コストの表示名</strong></td> 
     <td><strong>Workfront のエリア</strong></td> 
    </tr> 
    <tr> 
     <td>予算計上コスト</td> 
     <td> <p>ビジネスケースの概要</p> <p> <img src="assets/business-case-summary-qs-350x453.png" style="width: 350;height: 453;"> </p> </td> 
    </tr> 
    <tr> 
     <td>コスト</td> 
     <td> <p>ポートフォリオオプティマイザー</p> <p>ヒント：すべてのプロジェクトの予算計上コスト値の合計は、ポートフォリオの予算計上コストです。</p> </td> 
    </tr> 
    <tr> 
     <td>プロジェクト予算計上コスト</td> 
     <td> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (NOTE: this was removed with flash)</p>
      --> <p>プロジェクトレポート</p> <p>プロジェクト（財務データ）レポート</p> <p>タスクレポート</p> <p>イシューレポート</p> <p>予算計上時間数レポート</p> <p>レポートの作成について詳しくは、<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">カスタムレポートの作成</a>の記事を参照してください。</p> </td> 
    </tr> 
   </tbody> 
  </table>
