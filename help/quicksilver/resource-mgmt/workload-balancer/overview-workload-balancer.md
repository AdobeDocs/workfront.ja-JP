---
content-type: overview
product-area: resource-management
navigation-topic: the-workload-balancer
title: ワークロードバランサーの概要
description: プロジェクトマネージャーがタスクを作成することでプロジェクトの作業を計画し、リソース管理者がリソースプランナーでプロジェクトに担当業務のリソースを割り当てたら、プロジェクト所有者とチームマネージャーはワークロードバランサーを使用して作業アイテムをユーザーに割り当てることができます。
author: Lisa
feature: Resource Management
exl-id: 9398bd04-9df7-4b77-8361-fdb5bdce6829
source-git-commit: 233e61c011cc87f49d0d4082a20b7790104c96c8
workflow-type: tm+mt
source-wordcount: '1176'
ht-degree: 96%

---

# ワークロードバランサーの概要

<!--
<p>(NOTE: this is linked from the UI for the Workload Balancer page. DO NOT CHANGE TITLE OR LINK) </p>
-->

プロジェクトマネージャーがタスクを作成することでプロジェクトの作業を計画し、リソース管理者がリソースプランナーでプロジェクトに担当業務のリソースを割り当てたら、プロジェクト所有者とチームマネージャーはワークロードバランサーを使用して作業アイテムをユーザーに割り当てることができます。

>[!IMPORTANT]
>
>ワークロードバランサーを使用して、実際の作業（タスクとイシュー）をユーザーに割り当てることができます。
>
>プロジェクトの担当業務割当てを高いレベルで見積もるには、ワークロードバランサーではなく、リソースプランナーを使用する必要があります。リソースプランナーについて詳しくは、[リソースプランナーの概要](../../resource-mgmt/resource-planning/get-started-resource-planner.md)を参照してください。

この記事では、ワークロードバランサーの一般的な目的と、うまく使用できるようにプロジェクトとリソースを設定する方法に関するベストプラクティスを説明します。

ワークロードバランサーのビデオチュートリアルを確認するには、[Workfront チュートリアル](https://experienceleague.adobe.com/docs/workfront-learn/tutorials-workfront/home.html?lang=ja)ページに移動します。左側のメニューで、**リソース管理**／**ワークロードバランサー**&#x200B;を選択し、チュートリアルを選択します。

## ワークロードバランサーの使用場所

<!--
<p>(NOTE: This will be taken out when all we will have is one tool - should be replaced by a blurb that says you can add this tool anywhere, in any custom tab, etc (long term dev promise)) </p>
-->

リソースをスケジュールする場合は、次のエリアでワークロードバランサーを使用することをお勧めします。

* リソースエリア（システムレベル）。
* プロジェクトの「ワークロードバランサー」セクション（プロジェクトレベル）。
* チームの「ワークロードバランサー」セクション（チームレベル）。

ワークロードバランサーへのアクセスについて詳しくは、[ワークロードバランサーへのアクセス](../../resource-mgmt/workload-balancer/locate-workload-balancer.md)を参照してください。

## ワークロードバランサーのメリット

ワークロードバランサーを使用する際は、次のメリットを考慮してください。

<!--
<p> Add about the what-if scenarios as a benefit when they become available </p>
-->

* すべての関係者に対して透明性の高い、リソースの配分超過および低稼働率の明確なビジュアルマッピングにアクセスできます。
* 人材のマネージャーとして、従業員をバーンアウトから守り、集中力、品質およびエンゲージメントを向上して、最大限に仕事の成果を生み出せるようにすることができます。すべてのチームで最大限の稼働率の確保、サイロの打破および作業の整合性を実現できます。
* タスクレベルまたはイシューレベルで作業を割り当てると、ユーザーがどの程度忙しいかを把握できません。ワークロードバランサーを使用すると、タスクまたはイシューを時間どおりに完了するためのワークロードの空き時間が、どのユーザーにあるかを確認できます。これには、休暇およびスケジュール例外の詳細が含まれます。

  詳しくは、[ワークロードバランサーでの作業割り当ての概要](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)を参照してください。

  作業アイテムを一括で割り当てることもできるので、複数のプロジェクトに対して一度に多くの作業アイテムを配分しやすくなります。詳しくは、[ワークロードバランサーを使用した作業の一括割り当て](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer-in-bulk.md)を参照してください。

* 経営陣は、組織内の人材がどのように活用されているかを透明化することで、人材配置に関する意思決定をタイムリーに行うことができます。
* チームメンバーは、同僚社員が何に取り組んでいるかをいつでも確認できるので、コラボレーションの向上によるメリットがあります。ワークロードバランサーでのリソースの表示または管理に必要なアクセス権については、[ワークロードバランサーでのリソース管理に必要なアクセス権](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md)を参照してください。
* メインメニューにリソースがないユーザーと共有するには、カスタムタブにリソースへのリンクを埋め込みます。 詳しくは、[ ワークロードバランサーをリンクと共有する ](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md) を参照してください。
* 役割に応じて、グローバルレベル、プロジェクトレベルまたはチームレベルの 1 つのビューでスタッフのワークロードと需要を視覚化および管理します。プロジェクトを管理する場合、これには、プロジェクトのリソース配分だけでなく、Adobe Workfront シナリオプランナからのリソース配分の視覚化も含まれます。管理職は、Workfront シナリオプランナを使用して、組織全体のジョブスキルを管理します。シナリオプランナは、新しい Adobe Workfront エクスペリエンス でのみ使用できます。

  >[!NOTE]
  >
  >  シナリオプランナには、追加のライセンスが必要です。Workfront シナリオプランナについては、[シナリオプランナの概要](../../scenario-planner/scenario-planner-overview.md)を参照してください。


## ワークロードバランサーの使用に関するベストプラクティス

ワークロードバランサーを使用してリソースのスケジュールを開始する前に、プロジェクトの計画、ユーザーの設定およびフィルターの使用に関する次のベストプラクティスをお勧めします。

* [ワークロードバランサーでの情報表示のベストプラクティス](#best-practices-for-displaying-information-in-the-workload-balancer)
* [ユーザー設定のベストプラクティス](#best-practices-for-setting-up-users)
* [タスクおよびイシュー設定のベストプラクティス](#best-practices-for-setting-up-tasks-and-issues)

### ワークロードバランサーでの情報表示のベストプラクティス {#best-practices-for-displaying-information-in-the-workload-balancer}

未割り当ての作業項目と割り当て済みの作業項目の両方について、自分に関連する情報のみを表示できるように、フィルターを使用することをお勧めします。

ワークロードバランサーでのフィルターの作成と使用については、[ワークロードバランサーでの情報のフィルタリング](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)を参照してください。

### ユーザー設定のベストプラクティス

* 他のユーザーの作業をスケジュールするユーザーには、作業のリソースをスケジュールするための的確なアクセス権と権限が必要です。

  ワークロードバランサーでリソースのワークロードを管理する際に必要なアクセス権については、[ワークロードバランサーでのリソース管理に必要なアクセス権](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md)を参照してください。

* 管理するワークロードのユーザーは、ユーザーの空き時間とスキルに関する情報が正確になるように、次の基準を満たす必要があります。

   * スケジュールと担当業務がプロファイルに関連付けられている。

     スケジュールおよび担当業務のユーザーへの関連付けについて詳しくは、[ユーザーの追加](../../administration-and-setup/add-users/create-and-manage-users/add-users.md)を参照してください。
   * ユーザーがスケジュールに関連付けられていない場合、リソース管理のために、Workfront システムのデフォルトスケジュールがデフォルトでユーザーに関連付けられます。
   * スケジュールの例外をスケジュール内で更新します。

     スケジュールの作成について詳しくは、[スケジュールの作成](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)を参照してください。

   * プロファイルの休暇カレンダーを更新します。

     ユーザーの休暇カレンダーの更新について詳しくは、[個人の休暇の設定](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/personal-time-overview.md)を参照してください。

     <!--   
     <div data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     <p>(NOTE: Add another bullet for Costs, when this becomes available:</p>   
     <p>If you want to budget your resources by Cost, you must associate Job Roles with Cost/ Hr. rates. The cost associated with Job Roles assigned to users in your Resource Pools is used to calculate the Budgeted Labor Cost and the Budgeted Cost of the project.For more information about associating job roles with rates, see the article Creating and Managing Job Roles in the new Adobe Workfront experience.For more information about calculating Budgeted Labor Cost, see the article Calculating Budgeted Labor Cost in the new Adobe Workfront experience.For more information about calculating Budgeted Cost, see the article Calculating Budgeted Cost in .) </p>   
     </div>   
     -->

* Workfront 管理者は、Workfront がユーザーの空き時間をどのように計算するかを決定する必要があります。Workfront の設定エリアで、リソース管理の環境設定を調整して、ユーザーが作業できる時間を計算するのに、Workfront でシステムのデフォルトスケジュールを使用するか、ユーザーのスケジュールを使用するかを決定できます。

  詳しくは、[リソース管理の環境設定を設定](../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)を参照してください。

### タスクおよびイシュー設定のベストプラクティス {#best-practices-for-setting-up-tasks-and-issues}

ワークロードバランサーでユーザーに作業を割り当てる前に、次のタスクとイシューの設定があることを確認します。

* 親タスクは、ユーザーや役割には割り当てられません。親タスクはワークロードバランサーに表示されません。
* タスクとイシューには、予定時間数の値が 0 より大きい値が設定されます。

* タスクとイシューの期間には 0 より大きい値が設定されます。
* イシューの予定日は、プロジェクトのタイムライン内に表示されます。

## ワークロードバランサーを使い始める前に

* ワークロードバランサーの使用を開始する前に、次の記事を確認してください。

   * この記事では、ワークロードバランサーを操作し、[ワークロードバランサーの操作](../workload-balancer/navigate-the-workload-balancer.md)アクションを実行する方法を説明します。

   * 次の記事では、作業の割り当て方法とユーザー割り当ての管理方法について説明します。

      * [ワークロードバランサーでの作業割り当ての概要](../workload-balancer/assign-work-in-workload-balancer.md)。
      * [ワークロードバランサーのユーザー割り当てを管理します](../workload-balancer/manage-user-allocations-workload-balancer.md)。

* ワークロードバランサーは、Workfront の複数の異なるエリアにあります。ワークロードバランサーの場所について詳しくは、[ワークロードバランサーの検索](../../resource-mgmt/workload-balancer/locate-workload-balancer.md)を参照してください。

## ワークロードバランサーの使用に必要なアクセス

Workfront でワークロードバランサーを表示および使用するには、正しい Workfront へのアクセスと特定のプロジェクトへの権限が必要です。ワークロードバランサーの使用に必要なアクセスの詳細については、[ワークロードバランサーでリソースを管理するために必要なアクセス](../../resource-mgmt/workload-balancer/access-needed-manage-resources-balancer.md)の記事を参照してください。
