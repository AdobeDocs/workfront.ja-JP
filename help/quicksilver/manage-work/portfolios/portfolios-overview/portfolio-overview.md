---
content-type: overview
product-area: portfolios
navigation-topic: portfolios-overview
title: Portfolio手法について
description: ポートフォリオは、統一された特性を持つプロジェクトのコレクションです。これらのプロジェクトは通常、同じリソース、予算または時間枠を得るために競い合うことになります。ポートフォリオに追加する前に、ポートフォリオをプログラムに分割し、プロジェクトをプログラムに関連付けることができます。
author: Alina
feature: Work Management, Strategic Planning
exl-id: b340501e-1190-415e-aa96-5aad177c4b7b
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '587'
ht-degree: 70%

---

# ポートフォリオの方法論について

<!-- Audited: 1/2024 -->

Portfolioとは、特定のビジネス目標を達成するために、プロジェクトの優先順位付けと管理を行うプロセスです。

PPMに関する一般的な情報については、[Portfolio Managementの概要](/help/quicksilver/manage-work/portfolios/portfolios-overview/portfolio-managament-overview.md)を参照してください。

Adobe Workfrontでは、ポートフォリオとは、統一性のあるプロジェクトの集まりのことです。 これらのプロジェクトは通常、同じリソース、予算または時間枠を得るために競い合うことになります。ポートフォリオに追加する前に、ポートフォリオをプログラムに分割し、プロジェクトをプログラムに関連付けることができます。

ポートフォリオとプログラムを使用すると、プロジェクトを整理できます。プロジェクトを整理すると、類似のプロジェクトを比較することができ、どこにリソースを使うのが最適かを判断できるようになります。

プログラムの使用について詳しくは、[プログラムの作成](../../../manage-work/portfolios/create-and-manage-programs/create-program.md)を参照してください。

この資料には、Workfrontのポートフォリオに関する一般的な情報が含まれています。

## ポートフォリオの作成に必要なアクセス権

<!--leave the table uncollapsed as this article is about access-->

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] パッケージ</td> 
   <td> <p>Workfront Prime以降</p>
   <p>Workflow Prime以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>ポートフォリオへの[!UICONTROL Edit]アクセス権</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ポートフォリオの作成者は、デフォルトで、そのポートフォリオに対する管理権限があります。</p> 
   <p>ポートフォリオを編集またはプロジェクトを追加するための権限を管理します</p>
   <p>ポートフォリオに対する権限を表示して、Workfrontで表示する</p>
    </td> 
  </tr> 
 </tbody> 
</table>

* 詳しくは、[Workfront ドキュメント ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>New: Any</p>
   <p>Current:[!UICONTROL Business] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>New: [!UICONTROL Standard]</p>
   <p>Current:[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Portfolios</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>After you create a portfolio, you have Manage permissions to it, by default</p> 
   <p>Manage permissions to edit a portfolio or add projects to it</p>
   <p>View permissions to a portfolio to view it in Workfront</p>
    </td> 
  </tr> 
 </tbody> 
</table>
-->

## [!DNL Adobe Workfront] ポートフォリオ手法について

[!DNL Workfront] では、ポートフォリオにプロジェクトを追加して、ポートフォリオを作成および整理できます。

ポートフォリオを効率的に整理するには、次の手順に従うことをお勧めします。

1. プロジェクトのビジネスケースを作成し、そのプロジェクトをポートフォリオに関連付けます。

   組織に価値をもたらす効率的なポートフォリオを作成するには、まずプロジェクトリクエストを作成し、そこで後にポートフォリオに追加する各プロジェクトのビジネスケースを定義する必要があります。

   [!UICONTROL ビジネスケース]には、次の情報が含まれます。

   * プロジェクトに関する一般情報（説明、ポートフォリオ、プログラムの割り当て、プロジェクト所有者およびスポンサー）
   * プロジェクトの目的または目標
   * 推定所要コスト
   * 労力コストのリソース予算
   * 整合性スコア
   * リスク評価

   [!UICONTROL ビジネスケース]について詳しくは、[プロジェクトのビジネスケースの作成](../../../manage-work/projects/define-a-business-case/create-business-case.md)を参照してください。

   ビジネスケースを構築しながら、プロジェクトをポートフォリオに関連付けることができます。 プロジェクトに関連付ける前に、ポートフォリオを作成する必要があります。 詳しくは、[ ポートフォリオの作成](/help/quicksilver/manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md)を参照してください

   ビジネスケースの構築中に収集した詳細は、[!UICONTROL portfolio optimizer]および[!UICONTROL  リソースプランナー]で使用され、プロジェクトの選択における管理に役立ちます。
1. リソースプールとプロジェクトを関連付け、ビジネスケースを構築します。

   ポートフォリオは、通常、リソースプールに対応するように構成されます。ポートフォリオ内のプログラムは、リソースプールとも整合させます。同じポートフォリオ内のプロジェクトは通常同じリソースを奪い合うので、この相関関係により、すべてのリソース計画がポートフォリオの目的に沿うようになります。

   詳しくは、[ リソースプールの作成](/help/quicksilver/resource-mgmt/resource-planning/resource-pools/create-resource-pools.md)を参照してください。

1. [!UICONTROL ビジネスケース]をポートフォリオマネージャーから承認してもらいます。

   詳しくは、[ ビジネスケースの承認](/help/quicksilver/manage-work/projects/define-a-business-case/approve-business-case.md)を参照してください。
1. [!UICONTROL ポートフォリオオプティマイザー]で、ポートフォリオ内のプロジェクトのパフォーマンスを管理します。

   ポートフォリオマネージャーは、ポートフォリオダッシュボードを使用して、ポートフォリオ内の財務パフォーマンスを追跡できます。このダッシュボードはポートフォリオのヘッダーに表示されます。

   ポートフォリオの財務フィールドについて詳しくは、[ポートフォリオオプティマイザーの概要](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)の[ポートフォリオオプティマイザーの財務フィールドについて](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md#financial-fieds-subsection)の節を参照してください。
