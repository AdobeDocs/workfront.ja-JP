---
content-type: overview
product-area: resource-management
navigation-topic: the-workload-balancer
title: ワークロードバランサーの概要
description: プロジェクトマネージャは、プロジェクトでの作業を計画し、タスクを作成した後、ワークロードバランサーを使用して、この作業をチーム内のユーザーに割り当てることができます。
author: Alina
feature: Resource Management
exl-id: 9398bd04-9df7-4b77-8361-fdb5bdce6829
source-git-commit: b3ec7af8032e077736df1f48a9a4990b8c11922f
workflow-type: tm+mt
source-wordcount: '1147'
ht-degree: 0%

---

# ワークロードバランサーの概要

<!--
<p>(NOTE: this is linked from the UI for the Workload Balancer page. DO NOT CHANGE TITLE OR LINK) </p>
-->

プロジェクトマネージャは、プロジェクトでの作業を計画し、タスクを作成した後、ワークロードバランサーを使用してこの作業をユーザーに割り当てることができます。

>[!IMPORTANT]
>
>ワークロードバランサーを使用して、実際の作業（タスクと問題）をユーザーに割り当てることができます。
>
>プロジェクトのジョブ・ロール割当てを高いレベルで見積もるには、ワークロード・バランサではなく、リソース・プランナを使用する必要があります。 リソース・プランナの詳細は、 [リソースプランナーの概要](../../resource-mgmt/resource-planning/get-started-resource-planner.md).

この記事では、ワークロードバランサーの一般的な目的と、プロジェクトとリソースを設定して正常に使用する方法に関するベストプラクティスを説明します。

ワークロードバランサーのビデオチュートリアルを確認するには、 [WorkfrontTutorials](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html) ページに貼り付けます。 左側のメニューで、 **リソースの管理** > **ワークロードバランサー** チュートリアルを選択します。

## ワークロード・バランサの検索

<!--
<p>(NOTE: This will be taken out when all we will have is one tool - should be replaced by a blurb that says you can add this tool anywhere, in any custom tab, etc (long term dev promise)) </p>
-->

リソースをスケジュールする場合は、次の領域でワークロードバランサーを使用することをお勧めします。

* システムレベルで、[ リソース ] 領域で。
* プロジェクトレベルで、プロジェクトのワークロードバランサーセクションに配置します。
* チームレベルで、チームの [ ワークロードバランサー ] セクションに表示されます。

ワークロード・バランサの検索の詳細は、 [ワークロード・バランサの検索](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## ワークロードバランサーのメリット

ワークロード・バランサを使用する際は、次のメリットを考慮してください。

<!--
<p> Add about the what-if scenarios as a benefit when they become available </p>
-->

* リソースの割り当て超過と過剰な使用率の明確なビジュアルマッピングにアクセスし、すべての関係者に対して透過的です。
* 人々の管理者として、あなたは燃え尽きからあなたの人々を守り、より良い焦点、品質、エンゲージメントを持って最善の仕事を行う権限を与えることができます。 チーム間での作業の完全な活用、サイロ化の解除、および連携の可能化を実現できます。
* タスクまたは問題のレベルで作業を割り当てる場合、ユーザーのビジー状態を表示できません。 ワークロード・バランサを使用する場合、どのユーザーがワークロードに使用可能かを表示して、タスクまたは問題を時間通りに完了できます。 これには、休暇およびスケジュールの例外の詳細が含まれます。

  詳しくは、 [ワークロードバランサーでの作業割り当ての概要](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md).

  また、作業項目を一括で割り当てて、複数のプロジェクトに一度に大量の作業項目を配布しやすくすることもできます。 詳しくは、 [ワークロードバランサーを使用して作業を一括で割り当てる](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md).

* 経営陣は、組織内の人々の活用方法に対する透明性を高め、タイムリーなスタッフの意思決定を行うことができます。
* チームメンバーは、常に同僚が何に取り組んでいるかを見ることができるので、より良いコラボレーションのメリットを得ることができます。 ワークロード・バランサでリソースを表示または管理するために必要なアクセスの詳細は、 [ワークロードバランサーでリソースを管理するために必要なアクセス](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
* カスタムタブにリンクを埋め込んで、リソース領域にアクセスできないユーザーとリソースを共有します。 詳しくは、 [リンクとのワークロードバランサーの共有](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md)
* グローバル、プロジェクト、またはチームレベルで、役割に応じて、1 つのビューで担当者のワークロードと需要を視覚化および管理します。 プロジェクトを管理する場合、これには、プロジェクトのリソース割り当てだけでなく、Adobe Workfront Scenario Planner からのリソース割り当ての視覚化も含まれます。 担当者マネージャは、Workfrontシナリオプランナーを使用して、組織全体のジョブスキルを管理します。 シナリオプランナーは、新しいAdobe Workfrontエクスペリエンスでのみ使用できます。

  >[!NOTE]
  >
  >  シナリオ・プランナには、追加のライセンスが必要です。 Workfront Scenario Planner の詳細は、 [シナリオプランナーの概要](../../scenario-planner/scenario-planner-overview.md).


## ワークロードバランサーの使用に関するベストプラクティス

ワークロードバランサーを使用してリソースのスケジュールを開始する前に、プロジェクトの計画、ユーザーの構成、およびフィルタの使用に関する次のベストプラクティスを実行することをお勧めします。

* [ワークロードバランサーに情報を表示する際のベストプラクティス](#best-practices-for-displaying-information-in-the-workload-balancer)
* [ユーザーの設定のベストプラクティス](#best-practices-for-setting-up-users)
* [タスクと問題の設定に関するベストプラクティス](#best-practices-for-setting-up-tasks-and-issues)

### ワークロードバランサーに情報を表示する際のベストプラクティス {#best-practices-for-displaying-information-in-the-workload-balancer}

未割り当ての作業項目と割り当てられた作業項目の両方について、自分に関連する情報のみを表示できるように、フィルターを使用することをお勧めします。

ワークロード・バランサでのフィルタの作成と使用の詳細は、 [ワークロードバランサーの情報のフィルタリング](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

### ユーザーの設定のベストプラクティス

* 他のユーザーの作業をスケジュールするユーザーは、作業のためのリソースをスケジュールするための正しいアクセス権と権限が必要です。

  ワークロードバランサーでリソースのワークロードを管理するために必要なアクセスの詳細は、 [ワークロードバランサーでリソースを管理するために必要なアクセス](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).

* 管理するワークロードのユーザーは、可用性とスキルに関する情報が正確になるように、次の基準を満たす必要があります。

   * スケジュールとジョブの役割がプロファイルに関連付けられている。
   * スケジュールおよびジョブロールのユーザーへの関連付けの詳細は、 [ユーザーを追加](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)
   * ユーザーがスケジュールに関連付けられていない場合、リソース管理のために、Workfrontシステムのデフォルトスケジュールがデフォルトでユーザーに関連付けられます。
   * スケジュールの例外をスケジュール内で更新します。\
     スケジュールの作成について詳しくは、 [スケジュールの作成](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)

   * プロファイルの「休暇」カレンダーを更新してもらう。\
     ユーザーのタイムオフカレンダーの更新について詳しくは、 [個人の休日を設定](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md).

     <!--   
     <div data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <p>(NOTE: Add another bullet for Costs, when this becomes available:</p>   
     <p>If you want to budget your resources by Cost, you must associate Job Roles with Cost/ Hr. rates. The cost associated with Job Roles assigned to users in your Resource Pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project.For more information about associating job roles with rates, see the article Creating and Managing Job Roles in the new Adobe Workfront experience.For more information about calculating Budgeted Labor Cost, see the article Calculating Budgeted Labor Cost in the new Adobe Workfront experience.For more information about calculating Budgeted Cost, see the article Calculating Budgeted Cost in .) </p>   
     </div>   
     -->

* Workfront管理者は、Workfrontによるユーザーの可用性の計算方法を決定する必要があります。 ユーザーは、Workfrontでシステムのデフォルトスケジュールを使用するか、ユーザーのスケジュールを使用して、ユーザーが作業できる時間を計算するかを決定できます。 詳しくは、 [リソース管理環境設定の指定](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md).

### タスクと問題の設定に関するベストプラクティス {#best-practices-for-setting-up-tasks-and-issues}

ワークロードバランサーでユーザーに作業を割り当てる前に、次のタスクと問題の設定が存在することを確認します。

* 親タスクは、ユーザーや役割には割り当てられません。 ワークロードバランサーには表示されません。
* タスクとタスクには、計画時間の値が 0 より大きい値が設定されます。

* タスクとタスクの期間には 0 より大きい値が設定されます。
* 問題の計画日は、プロジェクトのタイムライン内に表示されます。

## ワークロードバランサーの使用を開始する前に

* ワークロードバランサーを使用して、組織内のユーザーに作業を割り当て、日次の割り当てを管理できます。

  この記事では、次の操作を実行するために、ワークロードバランサーをナビゲートする方法について説明します。 [ワークロード・バランサのナビゲート](../workload-balancer/navigate-the-workload-balancer.md).

  次の記事では、作業の割り当て方法とユーザー割り当ての管理方法について説明します。

   * [ワークロードバランサーでの作業割り当ての概要](../workload-balancer/assign-work-in-workload-balancer.md).
   * [ワークロードバランサーでのユーザー割り当ての管理](../workload-balancer/manage-user-allocations-workload-balancer.md).

* ワークロードバランサーは、Workfrontの複数の異なる領域に配置できます。 ワークロード・バランサの場所の詳細は、 [ワークロード・バランサの検索](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## ワークロードバランサーの使用に必要なアクセス

Workfrontでワークロードバランサーを表示および使用するには、特定のプロジェクトに対する正しいWorkfrontアクセス権と権限が必要です。 ワークロードバランサーの使用に必要なアクセスの詳細については、この記事を参照してください [ワークロードバランサーでリソースを管理するために必要なアクセス](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md).
