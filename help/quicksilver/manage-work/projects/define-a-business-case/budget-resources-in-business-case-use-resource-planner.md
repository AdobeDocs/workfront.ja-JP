---
navigation-topic: business-case-and-scorecards
title: リソース・プランナを使用したビジネス・ケースの予算リソース
description: 生産資源計画の一環として、プロジェクト・レベルの生産資源計画担当を使用して、ビジネス・ケースの構築時に、プロジェクトでの作業の完了に必要な役割を予算できます。
author: Alina
feature: Work Management
exl-id: 51ebb940-111c-442f-a8a6-287a04d2db68
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1249'
ht-degree: 0%

---

# リソース・プランナを使用したビジネス・ケースの予算リソース

生産資源計画の一環として、プロジェクト・レベルの生産資源計画担当を使用して、ビジネス・ケースの構築時に、プロジェクトでの作業の完了に必要な役割を予算できます。

ビジネスケースの作成について詳しくは、 [プロジェクトのビジネスケースの作成](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>プロジェクト・レベルの生産資源プランナに入力した情報は、システム・レベルの生産資源プランナにも表示されます。 逆も同じです。 リソース・プランナの詳細は、 [リソースプランナーの概要](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

また、Adobe Workfront Scenario Planner を使用して、ビジネス事例内のリソースを予算化することもできます。 詳しくは、 [シナリオ・プランナを使用したビジネス・ケースの予算生産資源](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfrontプラン</a>*</td> 
   <td> <p>Pro 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfrontライセンスの概要</a>*</td> 
   <td> <p>レビュー以上</p> <p>重要：リソース予算情報を変更するには、プランライセンスが必要です。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>次へのアクセスを編集します。 </p> 
    <ul> 
     <li> <p>プロジェクト</p> </li> 
     <li> <p>リソース管理</p> </li> 
     <li> <p>財務データ</p> </li> 
    </ul> <p>予算リソースに必要なアクセスについては、 <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Adobe Workfrontの予算リソースに必要なアクセス</a>.</p> <p>注意：まだアクセス権がない場合は、Adobe Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

開始する前に、次の操作を行う必要があります。

* Adobe Workfrontでのリソース計画に関するすべての前提条件を満たします。 詳しくは、 [リソースプランナーの概要](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* リソースプールをプロジェクトに関連付けます。

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:(you must have tasks assigned to job roles and users on the project - this is optional because the users and their roles come from the pools))</p>
  -->

   >[!NOTE]
   ビジネスケースの問題に割り当てられたリソースを予算できません。 予算は、システムレベルのリソースプランナーで作成できます。 リソース・プランナの詳細は、 [リソースプランナーの概要](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* これは前提条件ではありませんが、プロジェクトのタスクに対して「予定時間」を指定することをお勧めします。 これにより、タスクの完了に必要な作業量を把握し、リソースの予算を作成してタスクを完了するのに必要な時間を決定するのに役立ちます。 タスクと計画時間の関連付けについては、 [タスクを編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## ビジネス事例のプロジェクトおよび予算リソースへの資源プールの適用

>[!IMPORTANT]
15 年間のリソース予算を作成できます。 期間が 15 年を超えるプロジェクトのリソースを予算する場合、予算設定情報が正確でない可能性があります。

資源プールのないプロジェクトに対して、ビジネス・ケースで資源プールと予算プロジェクトの資源を適用する手順は、次のとおりです。

1. リソースを予算するプロジェクトに移動します。
1. クリック **ビジネス事例** をクリックします。
1. （条件付き）会社がWorkfront Scenario Planner のライセンスを持っていない場合、 **リソース予算の編集** 内 **リソース予算設定** 」セクションを開き、手順 5 に進みます。

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">(NOTE: ensure it stays right - this is 5 instead of 6 because step 2 won't print for nwe)</p>
   -->

1. （オプションおよび条件付き）プロジェクト情報がシナリオ・プランナのイニシアチブから発行された場合は、次のいずれかを実行します。

   * でリソースプランナーを選択 **プロジェクトの予算労務費の計算に使用する時間を選択します** 「 」フィールドで、「 **「> 生産資源予算の編集」を選択します。**.

      ![](assets/business-case-rp-selected-with-choose-button-350x120.png)

   * プロジェクトの予算リソースに対して「シナリオ・プランナ」が選択された場合は、 **変更** > **リソース予算の編集**.

      ![](assets/business-case-sp-selected-change-option-to-switch-to-rp-highlighted-350x88.png)
   プロジェクトの予算時間を使用して、プロジェクトの予算人件費を計算します。

   シナリオプランナーは、新しいAdobe Workfrontエクスペリエンスでのみ使用でき、追加のライセンスが必要です。 Workfront Scenario Planner の詳細は、 [シナリオプランナーの概要](../../../scenario-planner/scenario-planner-overview.md).

   >[!NOTE]
   プロジェクトの作業を開始する際に、リソースプランナーとシナリオプランナーのどちらを使用するかを決定することをお勧めします。 プロジェクトの期間中にこの 2 つを頻繁に切り替えると、プロジェクトのリソースを予算する際に不整合が生じる場合があります。

1. 内 **リソースプールを選択** フィールドに、1 つまたは複数を指定します **リソースプール**.

   アクティブなユーザーが入力されたリソースプールのみを指定する必要があります。

   >[!TIP]
   プロジェクトが既に資源プールに関連付けられている場合、資源プランナはデフォルトで表示されます。 プロジェクトにさらに資源プールを追加するには、プロジェクトを編集します。 プロジェクトの編集について詳しくは、 [プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md).

1. クリック **適用**.

   選択したプロジェクトに対して、リソースプランナーが表示されます。

   デフォルトでは、このプロジェクトに関連付けられた最初の 20 のジョブロールが、アルファベット順に「リソース予算設定」セクションに表示されます。 

   リソース・プランナの詳細は、 [リソースプランナーの概要](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   ![BC_resource_budgeting_area.png](assets/bc-resource-budgeting-area-350x276.png)

1. （オプションおよび条件付き）ジョブの役割を展開して、関連付けられているユーザーを表示します。

   >[!NOTE]
   アクティブなユーザーは、次の条件を満たす場合にのみ、関連付けられたジョブの役割の下に表示されます。
   * プロジェクトのリソースプールの 1 つに属しています。
   * 予算時間が割り当てられています。
   * これらは、プロジェクトのジョブの役割の 1 つに関連付けられています。


    

1. クリック **今日** 今日の時間枠に戻る
1. （オプション）「 **週**, **月** または **四半期** 異なる時間枠でプロジェクトの情報を表示する。
1. （オプション） **時間** ドロップダウンメニューで、 **時間**,**FTE**&#x200B;または **コスト** をクリックして、リソース・プランナでの情報の表示方法を変更します。 デフォルトでは時間が表示されます。

1. （オプション）「 **書き出し** をクリックして、Resource Planner を Excel ファイルにエクスポートします。

   >[!NOTE]
   一度に 12 個までの期間のデータをエクスポートできます。

1. （オプション） **全画面表示** アイコン ![full_screen_RP_in_BC.png](assets/full-screen-rp-in-bc.png) をクリックして、リソースプランナーをフルスクリーンモードで表示します。

1. を更新します。 **BDG** 次のいずれかの操作を行って、ユーザー、役割またはプロジェクトの時間、工数または原価の値を含む（予算時間）フィールド。

   * 役割、ユーザー、プロジェクトの時間、工数、コストの値を手動で見積もります。

      または

   * 次をクリック： **オプション** プロジェクトまたはジョブの役割のアイコンをクリックし、役割、ユーザーまたはプロジェクトの時間を自動的に予算するオプションを選択します。
   リソース・プランナのプロジェクト・ビューでの予算編成の詳細は、 [「プロジェクト」ビューと「ロール」ビューを使用する、リソースプランナーの予算リソース](../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   >[!NOTE]
   プロジェクトのタイムラインに関係なく、「生産資源予算」領域に表示される任意の期間の生産資源の予算時間、工数または原価を指定できます。 たとえば、プロジェクトのタイムライン（計画時間と関連付けられている）でリソースが使用できない可能性があるが、別の時間で使用できる場合は、計画時間がゼロの時間枠に予算を割り当てます。

1. （オプション）予算に基づく時間、工数、コストを別の期間に移動できるかどうかを把握するには、 **オプション** アイコン、 **予算作成日の調整**.

   予算日付の調整の詳細については、 [リソース・プランナで予算作成日を調整](../../../resource-mgmt/resource-planning/adjust-budgeting-dates.md).

1. 「**保存**」をクリックします。

   「時間当たりの原価率」がジョブの役割に関連付けられている場合は、「生産資源予算」領域で生産資源を予算作成すると、 **予算労務費** プロジェクトの 予算労務費は、ビジネス・ケースの「生産資源予算設定」領域とビジネス・ケース要約に表示されます。

   >[!TIP]
   コストは、ビジネスケースにプロジェクトの通貨で表示されます。

   ビジネス・ケースで指定された予算情報は、リソース・プランナにも表示されます。
