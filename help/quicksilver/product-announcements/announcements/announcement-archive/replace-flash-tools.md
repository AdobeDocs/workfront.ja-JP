---
title: Adobe Workfront における Flash ベースのツールの置き換え
description: Adobe Workfront における Flash ベースのツールの置き換え
author: Luke
draft: Probably
feature: Product Announcements
exl-id: a0ca824d-aab8-4da2-97ed-0913a7f76d55
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '2702'
ht-degree: 99%

---

# Adobe Workfront における Flash ベースのツールの置き換え

Adobe Workfront Classic から、すべての Flash ベースのツールを削除しました。

現在の標準に基づく代替ツールが、Workfront で利用できるようになりました。これらの変更は、アドビが発表した Flash 製品のサポート終了に合わせて行われます。

## 重要な日付

Workfront のすべての Flash ベースのツールを削除する際には、次の日付が重要です。

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>July 1, 2020</strong>: All Flash-based tools will be removed from all Workfront products for those customers who are not using them currently. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">All customers who are currently using the Flash-based tools will continue to have access after this date. If you are still using these products, report all blocking issues or concerns that you see which prevent you from fully transitioning all your users to the new replacement tools by this date. Work with your account manager or our support team to report these concerns. </p>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about contacting our support team, see <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>. </p>
  -->

* **2020年11月19日（PT）**：すべての Flash ベースのツールが、すべての Workfront 製品から削除されました。

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  We recommend that you start using the new tools and retire the Flash tools before then, to increase the security of your instance. We will also gradually disable the tools that have not been used for at least 3 months. If you would like us to disable the Flash tools before November, you can contact
  <a href="../../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">Contact Customer Support</a>.
  </MadCap:conditionalText>
  -->

## レガシー Flash ベースのツール

以下の節で示すツールは、Workfront システムから削除され、新しいソリューションに置き換えられました。

代替ツールの詳細について詳しくは、この記事の[レガシー Flash ベースのツールとその代替](#legacy-flash-based-tools-and-their-replacements)を参照してください。

### リソース管理

* ユーザーエリアの「レガシーリソースプランニング」タブと、タブに含まれるすべてのツール（以下を含む）。

   * リソース予算マネージャー
   * キャパシティプランナー
   * リソース見積り
   * リソースグリッド\
     詳しくは、[Adobe Workfront でのリソースプランニング](../../../resource-mgmt/resource-planning/resource-planning-overview.md)を参照してください。

* プロジェクトのビジネスケースのレガシーリソースの予測エリア

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  is displayed in view-only mode
  </MadCap:conditionalText>
  -->

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  For more information, see
  <a href="../../../resource-mgmt/resource-mgmt-overview/migrate-resource-estimates-to-budgeting.md" class="MCXref xref">Migrate from Legacy Resource Estimates to Resource Budgeting </a>
  </MadCap:conditionalText>
  -->

  。

* プロジェクトの「人材の配置」タブの「リソースグリッド」サブタブ
* プロジェクトの「人材の配置」タブの「スケジュール」サブタブにある「新しいスケジュールエリアを使用」オプションで、レガシースケジューリングエリアまたはチームビルダーが削除されます。この場合、スケジュールタイムラインがデフォルトで表示されるようになりました。
* ユーザープロファイルの下の「配分」タブ

### レポート

次のレポート機能とレポートが削除されました。

* 次のレポート機能が削除されました。

   * ユーザーレポートの「リソースグリッド」オプション
   * プロジェクトまたはタスクレポートの「レガシーガント」オプション\
     詳しくは、[ガントチャートで情報を表示](../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md)を参照してください。

* 削除されたレポート：

   * レガシーリソースプールレポート
   * リソースの予測レポート

  >[!NOTE]
  >
  >レポートまたは API（レガシーリソースプール、レガシー予算計上コスト、レガシーコスト、レガシー予算計上時間、レガシー予算計上労力コストなど）を使用してアクセスしたすべてのレガシーフィールドは、様々なレポートに表示されますが、新しい情報は入力されません。

### 従来のガント

* プロジェクトとタスクのリストからのすべてのレガシーガントビュー、およびレポートとレポートのオプション
* ポートフォリオとプログラムの「レガシーガント」サブタブ
* テンプレートのテンプレートタスクのリストの「レガシーガント」サブタブ、テンプレートタスクの「サブタスク」タブのレガシーガントビュー、およびテンプレートタスクレポートのレガシーガントビュー

### プルーフ

レガシープルーフビューアは、ほとんどの顧客に対して新しい web プルーフビューアおよびデスクトッププルーフビューアに置き換えられ、2020年11月にすべての顧客に対して削除されました。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">With the 2018.2 release, the Legacy proofing viewer was removed as the default viewer.</p>
-->

詳しくは、次のリソースを参照してください。

* [Web プルーフビューアーでのプルーフのレビュー](../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proofs-in-wpv.md)
* [デスクトッププルーフビューアーでのプルーフのレビュー](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/review-proofs-in-desktop-proofing-viewer.md)

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="../../../workfront-proof/wp-work-proofsfiles/review-proofs-lpv/lpv-removed-2018.md" class="MCXref xref">Legacy proofing viewer removed in 2018.3</a> </li>
  -->

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Additional features to be removed</h3>
<ul>
<li>The Legacy Portfolio Optimizer<br>For more information, see <a href="../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md" class="MCXref xref">Portfolio Optimizer overview</a>.<br></li>
<li>The Legacy financial fields in the Business Case of the project and the Portfolio Optimizer</li>
<li>The dialog boxes used when sharing reports, calendars, and documents no longer rely on Flash-based technology</li>
</ul>
</div>
-->

## レガシー Flash ベースのツールとその代替 {#legacy-flash-based-tools-and-their-replacements}

特に指定しない場合を除き、次の表に示すように、すべてのレガシー機能は新しい機能に置き換えられています。

>[!CAUTION]
>
>レガシー Flash ベースのツールは、すべての環境から削除されました。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>レガシーツール</strong> </p> </th> 
   <th> <p><strong>新しいツール</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p><strong>レガシーリソースプール</strong> </p> <p>レガシーリソースプールは、プロジェクトを完了するために、一度に必要となる担当業務のグループまたはコレクションでした。レガシーリソースプールには、次のような多くの欠点があります。</p> 
    <ul> 
     <li> ユーザーを 1 つのレガシーリソースプールに関連付けることはできますが、これはレポート目的でのみ使用されていました。レガシーリソースプールは抽象的な担当業務エンティティで動作していたので、ユーザーのスケジュールの例外と休暇は考慮されず、リソースの空き時間に関するデータが不正確になることがありました。 </li> 
    </ul> 
    <ul> 
     <li>プロジェクトごとに指定できるレガシーリソースプールは 1 つだけでした。その結果、複数のレガシーリソースプールは、互いに独立して動作する個別のグループのフローのみをサポートし、リソースを共有することはありませんでした。それ以外の場合はすべて、システム内のすべてのリソースを含むレガシーリソースプールを 1 つ保持することが推奨されました。これにより、大量のプロジェクトとデータでパフォーマンスの問題が発生しました。</li> 
    </ul> </td> 
   <td> <p><strong>リソースプール</strong> </p> <p>新しいリソースプールは、プロジェクトの完了に同時に必要なユーザーのコレクションです。また、Workfront は、専門のユーザーに個別に作業を割り当てる必要がある場合があることも認識しています。このため、担当業務の代わりにユーザーの予算を設定できるようになりました。 </p> レガシーリソースプールと比較した場合のリソースプールの利点は次のとおりです。 
    <ul>
     <li>リソースプールはユーザーに基づいているので、ユーザーと役割の空き時間の計算では、そのユーザーの休暇およびスケジュールの例外が既に考慮されています。これにより、正確で最新のデータが得られ、予算を正しく決定し、プロジェクトの進行中に変更が発生する可能性を最小限に抑えることができます。</li>
     <li>Workfront では、リソースの空き時間とデータの正確性をより制御できるようになったので、複数のリソースプールをプロジェクトに関連付けることができます。複数のプロジェクトで同時に使用できる複数のスキルを持っている場合、1 人のユーザーが複数のリソースプールに所属することもできます。 </li>
    </ul><p>このようなデータの制御により、使用可能な予算を配分するためのすべてのリソースを含む 1 つのリソースプールを使用する必要がなくなりました。実際には、これはお勧めしません。代わりに、リソースプールを多様化し、関連するリソースプールのみをプロジェクトに関連付けることをお勧めします。</p><p> リソースプールについて詳しくは、<a href="../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md" class="MCXref xref">リソースプールの概要</a>を参照してください。</p></td> 
  </tr> 
  <tr> 
   <td> <p><strong>リソース予算マネージャー</strong> </p> <p>リソース予算マネージャーを使用して、複数のリソースプールにわたる担当業務リソースの空き時間を指定できました。ただし、レガシーリソースプールの欠点により、この機能はほとんど使用されませんでした。使用すると、予算をより正確に設定するために、ユーザーは担当業務の空き時間を手動で入力する必要がありました。スケジュールの例外とユーザーの休暇は考慮されませんでした。</p> </td> 
   <td> <p>リソースプール内のユーザーに基づいて空き時間が自動的に計算されるため、リソース予算マネージャーは不要になりました。このツールは、空き時間の計算に関するすべての手動作業とともに削除されました。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>リソース見積り</strong> </p> <p>各レガシーリソースプールの「リソースの見積もり」タブは、1 つのレガシーリソースプールのコンテキストでのみ、リソース予算マネージャーと同じ目的を果たしました。このツールには、不正確なデータと空き時間の手動入力という、リソース予算マネージャーやレガシーリソースプールと同じ制限がありました。 </p> </td> 
   <td> <p>ユーザーの空き時間を自動的に計算することにより、リソースの見積もりは廃止され、削除されました。</p> <p>このツールは、プロジェクトのビジネスケースのレガシーリソースプールとレガシーリソース見積もりでは削除されます。 <!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
       The Legacy Resource Estimates area on the Business Case of the project remains there in View-only mode at this time. 
      </MadCap:conditionalText>
     --></p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>キャパシティプランナー</strong> </p> <p>キャパシティプランナーは、リソースの空き時間に応じてレガシーリソースプール内のリソースを予算化し、プロジェクトを優先順位付けする Workfront のツールでした。キャパシティプランナーの情報を提供したリソース見積もりとリソース予算マネージャーのデータが不完全な場合、プロジェクトの優先順位付けは、ユーザーの空き時間に対して再確認する必要がありました。</p> <p>システム内のすべての担当業務を含む単一のレガシーリソースプールを使用するシナリオが最も一般的でした。これにより、キャパシティプランナーが多数のプロジェクトを読み込もうとすると、パフォーマンスの問題が発生しました。</p> </td> 
   <td> <p><strong>リソースプランナーのプロジェクトビュー</strong> </p> <p>リソースプランナーのプロジェクトベースビューでは、レガシーキャパシティプランナーで行っていた方法と同様に、リソースの予算を設定し、プロジェクトの優先順位を付けることができます。レガシーツールとは異なり、より多くのデータがサポートされるようになり、ユーザーの休暇とスケジュールの例外の両方を考慮することで、利用可能な情報がより正確になります。</p> <p>利用可能な情報、予定済みの情報、および予算済みの情報が一目でわかるため、リソース管理者は、作業を行うのに十分な人材がいるかどうか、プロジェクト計画が当初の予算見積もりを超えているかどうかを確認できます。</p> <p> リソースプランナーでのプロジェクトビューの使用について詳しくは、<a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">リソースプランナーの概要</a>参照してください。</p> <p><strong>シナリオプランナー</strong> </p> <p>長期的なキャパシティ計画、what-if シナリオのモデリングと優先順位付けについては、Workfront のシナリオプランナーも導入されました。 </p> <p>シナリオプランナーは、新しい Adobe Workfront エクスペリエンスでのみ使用でき、追加のライセンスが必要です。Workfront のシナリオプランナーについて詳しくは、<a href="../../../scenario-planner/scenario-planner-overview.md" class="MCXref xref">シナリオプランナーの概要</a>を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>レガシーリソース見積もり（ビジネスケース）</strong> </p> <p>ビジネスケースのレガシーリソース見積もりエリアを使用して、プロジェクト計画の一環として一定の労働時間とコストの予算を立て、リソースを要求できます。このビューでは、リソースの空き時間がまったく表示されなかったため、その結果、リソースのリクエストが概算になり、プロジェクト作業が拒否される可能性が高くなりました。</p> </td> 
   <td> <p><strong>リソース予算計上（ビジネスケース）</strong> </p> <p>ビジネスケースの下の「リソース予算計上」セクションでは、リソースプランナーの機能をビジネスケースに提供し、ユーザーと役割の空き時間を表示し、ユーザーレベルで予算を作成できます。 </p> <p> ビジネスケースのリソース予算計上エリアについて詳しくは、<a href="../../../manage-work/projects/define-a-business-case/areas-of-business-case.md" class="MCXref xref">ビジネスケースのエリアの概要</a>を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>リソースの見積もりレポート</strong> </p> <p>リソース管理にレガシーツールを使用すると、ビジネスケースから予算および予定時間数についてレポートできました。これにより、特定の期間における各担当業務の予算および予定作業の合計を示すマトリックスレポートを作成できました。このレポートは編集できず、レポートの結果に基づいてリソースの予算を変更できませんでした。 </p> </td> 
   <td> <p><strong>稼動率レポート</strong> </p> <p>組み込みの稼動率レポートには、計画済み、予算済み、および実績時間、コスト、および収益が並べて表示されます。 </p> <p>稼動率レポートの使用について詳しくは、<a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md" class="MCXref xref">リソース稼動率情報を表示</a>を参照してください。 </p> 
    <div> 
     <p><strong>レポート可能な予算計上時間</strong> </p> 
     <p>予算計上時間のレポートを作成して、リソースプランナーで予算に設定された時間をレポートフォームでレビューします。 </p> 
     <p>予算計上時間について詳しくは、<a href="../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md" class="MCXref xref">Adobe Workfront の用語集</a>を参照してください。</p> 
     <p>レポートの作成について詳しくは、<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">カスタムレポートを作成</a>を参照してください。</p> 
    </div> <p><strong>リソースプランナーの役割ビュー</strong> </p> <p>レガシーリソース管理ツールのビジネスケースの予算計上時間数と予定時間数を、新しいネイティブビュー（ソースプランナーの役割ベースのビュー）で利用できるようになりました。このビューでは、利用可能な時間数、予定時間数、予算計上時間数の情報を一目で確認し、すべての予算計上を一元的に管理および変更できます。これにより、上位の担当業務を計画する際、より適切に意思決定を行うことができます。 </p> <p> リソースプランナーの役割ビューでのリソースを計上について詳しくは、<a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">リソースプランナーの概要</a>の<a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using2" class="MCXref xref">プロジェクトビューと役割ビューを使用してリソースを計上</a>の節を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>リソースグリッド</strong> </p> <p>リソースグリッドを使用すると、プロジェクトが完了に向かって進むにつれて、特定のユーザーの割り当てを確認できます。 </p> <p>例えば、プロジェクトチームの誰が作業を早く終えたか、誰が遅れているか、特定の期間の割り当てが不足または超過しているかを簡単に確認できます。 </p> <p>残念ながら、同じビューの情報に基づいて対処することはできませんでした。割り当て超過の問題を修正するには、アクションの結果を全く表示しない状態でプロジェクトに移動し、そこにある情報を手動で調整する必要がありました。</p> </td> 
   <td> <p>リソースグリッドは、2 つの新しいツールに置き換えられました。リソース計画の段階に応じて、次のツールを使用できます。</p> 
    <ul> 
     <li> <p><strong>分析フェーズの場合：</strong> </p> 
      <ul> 
       <li> <p><strong>ワークロードバランサー</strong>：ワークロードバランサーを使用すると、より詳細なレベルでユーザーのワークロードを表示できます。ワークロードバランサーを使用すると、ワークロード内でタスクを時間通りに完了できるユーザーを確認できます。これには、休暇およびスケジュール例外の詳細が含まれます。 </p> <p>ワークロード・バランサの詳細は、 <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">ワークロードバランサーの概要</a>.</p> </li> 
       <li> <p><strong>リソースプランナーのユーザービュー</strong><strong>：</strong>リソースプランナーのユーザービューを使用すると、ユーザーが割り当てられるプロジェクトをより高いレベルで把握できます。これにより、ユーザーが何に取り組んでいるか、また、特定の期間での割り当ての超過や不足を確認できます。また、リソースプランナーは、ユーザー全体の全体的な割り当ての視覚化と、ログに記録された実際の時間数の表示を提供するので、作業の進行状況を分析するのに役立ちます。 </p> <p>リソースプランナーでのユーザービューの使用について詳しくは、<a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md" class="MCXref xref">リソースプランナーの概要</a>の<a href="../../../resource-mgmt/resource-planning/get-started-resource-planner.md#using" class="MCXref xref">ユーザービューを使用して、使用可能時間、計画時間、実際の時間数または FTE を表示する</a>の節を参照してください。</p> </li> 
      </ul> </li> 
     <li><strong>戦術フェーズの場合：</strong> 
      <ul> 
       <li><strong>ワークロードバランサー</strong>：ワークロードバランサーを使用すると、次の操作を実行できます。 
        <ul>
         <li>作業をユーザーに割り当てます。</li>
         <li>作業アイテムに対するユーザーの割り当てを管理します。 </li>
         <li>担当者領域を参照できない可能性のある他のユーザーと、ワークロードバランサーを共有できます。共有可能なリンク機能を使用して、ワークロードバランサーへのリンクを共有し、カスタムダッシュボードに埋め込みます。これらのダッシュボードを共有すると、「ユーザーを表示」へのアクセス権を持つすべてのユーザーがこれらのダッシュボードを表示できます。</li>
        </ul><p>ワークロードバランサーは、担当者領域で使用できます。 </p><p>ワークロード・バランサの詳細は、 <a href="../../../resource-mgmt/workload-balancer/overview-workload-balancer.md" class="MCXref xref">ワークロードバランサーの概要</a>.</p></li> 
      </ul> <!--
       <ul data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
        <li><strong>The Resource Scheduling Areas</strong><strong>:</strong> When assigning your resources to the actual work that must be completed, use the Resource Scheduling areas in the People or Team areas, or at the project level. These areas allow you to visualize and manage the users' workload by day and rectify any problems from one view using the following actions: 
         <ul>
          <li> manual dragging and dropping of tasks to the correct assignee </li>
          <li> automatic assigning of tasks </li>
          <li> bulk swapping assignments </li>
          <li><p>adjusting Planned Hours according to the true availability of users. </p></li>
         </ul><p>These actions provide even more control over managing workload. </p><p> For information about managing user assignments and allocations in the Resource Scheduling areas, see <a href="../../../resource-mgmt/resource-scheduling/get-started-resource-scheduling.md" class="MCXref xref">Get started with Resource Scheduling</a>.</p><p>With this new functionality, the Resource Grid is replaced by the User View of the Resource Planner and the Resource Scheduling areas in the following areas of the application: </p>
         <ul>
          <li>People - the Resource Grid is eliminated along with the Legacy Resource Planning tab.</li>
          <li>Project - the Scheduling area under the Staffing tab of the project is available to Work and Plan license users. They do not have to have Manage access to the project to view this area. </li>
          <li>Reporting - the ability to view User reports in the Resource Grid view is removed. Instead, there is an option to share a URL for the User View of the Resource Planner and embed it in custom dashboards, providing visibility into user utilization to virtually anyone in the system. Any users with access to View users are able to view these dashboards when you share them. </li>
          <li>User - the Allocation tab is eliminated as the same information can be accessed in the User View of the Resource Planner.</li>
         </ul></li> 
       </ul>
      --> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>従来のガントチャート、タスクリスト</strong> </p> <p> タスクリストの従来のガントチャートを使用すると、ユーザーは、データベースに変更を加えることなく、プロジェクトのタイムラインを視覚的に確認し、what-if シナリオ計画を実行できます。従来のガントチャートは Flash テクノロジーに基づいていたことにより、セキュリティリスクが生じていました。 </p> </td> 
   <td> <p><strong>ガントチャート、</strong> <strong>タスクリスト</strong></p> <p> 新しい HTML ベースのガントチャートは、従来のガントチャートと同じ目的で機能します。ユーザーは、タスクリストツールバーの「手動保存」オプションを変更すると、データベースに変更をコミットせずに、プロジェクトのタイムラインを視覚化し、what-if シナリオ計画を実行できます。 </p> <p>新しいガントチャートは、「自動保存」オプションを使用するとインタラクティブになり、変更の発生時に自動的に保存する場合に使用できます。 </p> <p>新しいタスクリストガントチャートは、最新のテクノロジーに基づいて構築され、信頼性があります。この新しいガントチャートはタスクリストに直接配置され、タスクリストでの作業中にタブを切り替えたりビューを変更したりすることなく、簡単にアクセスできます。 </p> <p>新しいガントチャートは前のチャートと同じ機能を提供しますが、従来のガントチャートと比較すると、機能にいくつかの違いがあります。 </p> <p> テンプレートのテンプレートタスクのリストの「従来のガント」サブタブ、テンプレートタスクの「サブタスク」タブの従来のガントビュー、およびテンプレートタスクレポートの従来のガントチャートも、HTML ベースのガントチャートに置き換えられました。 </p> <p>従来のガントチャートを主にシンプルな表示とクイック編集で使用し、実際のチャートを使用しない場合は、新しい「タイムライン計画」オプションを使用すると、主要な計画フィールドを素早く変更できます。タスクリストツールバーから、「自動保存」の代わりに「タイムライン計画」を選択できます。</p> <p>「タイムライン計画」オプションを使用してタスクリストを保存する方法について詳しくは、<a href="../../../manage-work/tasks/manage-tasks/edit-tasks-in-a-list.md" class="MCXref xref">リスト内のタスクの編集</a>の記事の「タイムライン計画オプションを選択した場合にタスクリストの変更を手動で保存」の節を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>プロジェクトリストの従来のガントチャート</strong> </p> <p>プロジェクトリストの従来のガントチャートを使用すると、ユーザーはプロジェクトとそのタスクを 1 つのビューで表示できます。プロジェクトリストのコンテキストを離れることなく、ユーザーはプロジェクト内のタスクの詳細やプロジェクト間の依存関係を確認できます。プロジェクトリストの従来のガントチャートは Flash テクノロジーに基づいていたことにより、セキュリティリスクが生じていました。 </p> </td> 
   <td> <p><strong>ガントチャート、プロジェクトリスト</strong> </p> <p>HTML ベースのガントチャートは、従来のガントチャートと同じ目的で機能します。ユーザーは、プロジェクトとそのタスクを 1 つのビューで表示して、プロジェクトやタスク間の依存関係を視覚的に識別できます。プロジェクトリストのガントチャートは、プロジェクトリストに直接表示されます。新しいガントチャートは最新のインターフェイスを備え、最新のテクノロジーに基づいて構築されています。</p> <p>プロジェクトリストのガントチャートについて詳しくは、<a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">ガントチャートで情報を表示</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>レポート、カレンダー、ドキュメントの共有ダイアログボックス</strong> </p> <p>レポート、カレンダー、ドキュメントを共有する場合、使用されたダイアログボックスは Flash の技術に基づいていました。</p> </td> 
   <td> <p>Workfront でレポート、カレンダー、ドキュメントを共有する際のエクスペリエンスは変更されていません。ただし、エクスペリエンスは Flash に依存しなくなりました。</p> <p>これらの項目の共有について詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">オブジェクトに対する共有権限の概要</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>従来のプルーフビューア</strong> </p> <p>従来のプルーフビューアは、静的プルーフ、ビデオプルーフ、インタラクティブなプルーフ機能を提供する web ベースのプルーフビューアでした。</p> </td> 
   <td> <p><strong>Web プルーフビューアおよびデスクトッププルーフビューア</strong> </p> <p>Web プルーフビューアには、静的プルーフおよびビデオプルーフ用のプルーフ機能が用意されています。</p> <p>デスクトッププルーフビューアには、静的プルーフおよびビデオプルーフを完全にサポートするだけでなく、インタラクティブなプルーフ用のプルーフ機能も用意されています。</p> <p>この SWF ファイル形式は、主要なプロバイダーではサポートされなくなり、プルーフ用に HTML5 バナーに置き換えられました。 </p> <p>使用可能なプルーフビューアの違いについて詳しくは、<a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">web プルーフビューアとデスクトッププルーフビューアの違いの概要</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>
