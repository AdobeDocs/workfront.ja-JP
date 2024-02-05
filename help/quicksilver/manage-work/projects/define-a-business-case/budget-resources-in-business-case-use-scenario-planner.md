---
navigation-topic: business-case-and-scorecards
title: シナリオプランナーを使用してビジネスケースのリソースの予算を立てる
description: リソース計画の一環として、ビジネスケースを構築するときに、Adobe Workfront Scenario Planner を使用して、プロジェクトの作業を完了するために必要な担当業務の予算を立てることができます。
author: Alina
feature: Work Management
exl-id: d5f3e348-dc7d-4265-a5ce-8eef152db410
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: ht
source-wordcount: '927'
ht-degree: 100%

---

# シナリオプランナーを使用してビジネスケースのリソースの予算を立てる

リソース計画の一環として、ビジネスケースを構築するときに、Adobe Workfront Scenario Planner を使用して、プロジェクトの作業を完了するために必要な担当業務の予算を立てることができます。

ビジネスケースの作成について詳しくは、[プロジェクトのビジネスケースの作成](../../../manage-work/projects/define-a-business-case/create-business-case.md)を参照してください。

>[!TIP]
>
>システムレベルのシナリオプランナーで入力したプロジェクトにリンクされているイニシアチブの担当業務情報は、イニシアチブを発行する際に、プロジェクトのビジネスケースのリソース予算計上エリアに表示されます。シナリオプランナーは、新しい Adobe Workfront エクスペリエンスでのみ使用でき、追加のライセンスが必要です。Workfront Scenario Planner の詳細については、[シナリオプランナーの概要](../../../scenario-planner/scenario-planner-overview.md)を参照してください。

また、リソースプランナーを使用して、ビジネスケース内のリソースの予算を立てることもできます。詳しくは、以下を参照してください。

* [ビジネスケースでのリソースの予算計上](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)
  <!--* [Budget resources by project in the Resource Planner](../../../resource-mgmt/resource-planning/budget-by-project-resource-planner-d.md)-->

>[!NOTE]
>
>プロジェクトの作業を開始する際に、リソースプランナーとシナリオプランナーのどちらを使用するかを決定することをお勧めします。プロジェクトの期間中にこの 2 つを頻繁に切り替えると、プロジェクトのリソースを予算計上する方法に一貫性がなくなる可能性があります。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>ビジネス以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td> <p>この記事で説明する機能にアクセスするには、Adobe Workfront シナリオプランナーの追加ライセンスを購入する必要があります。</p> <p>Workfront Scenario Planner の取得について詳しくは、<a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Scenario Planner を使用するために必要なアクセス</a>を参照してください。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>以下の項目についてアクセス権を編集します。 </p> 
    <ul> 
     <li> <p>プロジェクト</p> </li> 
     <li> <p>財務データ</p> </li> 
     <li> <p>シナリオプランナー </p> </li> 
    </ul> <p>リソースの予算を立てるのに必要なアクセスについては、<a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Adobe Workfront の予算リソースに必要なアクセス</a>を参照してください。</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する権限を管理</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

## 前提条件

始める前に、以下を行う必要があります。

* シナリオプランナーを使用して計画を作成します。

  詳しくは、[シナリオプランナーでのプランの作成と編集](../../../scenario-planner/create-and-edit-plans.md)を参照してください。

* プランにイニシアチブを作成し、プロジェクトにリンクします。

  イニシアチブに必要な担当業務情報を指定し、リンクされたプロジェクトをこの情報で更新します。

  詳しくは、次の記事を参照してください。

   * [シナリオプランナーでのイニシアチブの作成と編集](../../../scenario-planner/create-and-edit-initiatives.md)
   * [Scenario Planner のプランにプロジェクトを読み込む](../../../scenario-planner/import-projects-to-plans.md)
   * [シナリオプランナーでイニシアチブを公開して、プロジェクトを更新または作成する](../../../scenario-planner/publish-scenarios-update-projects.md)

* これらは前提条件ではありませんが、次もお勧めします。

   * プロジェクト上のタスクを、シナリオプランナーで予算計上された担当業務に割り当てます。
   * プロジェクトのタスクの予定時間数を示す。

     これは、タスクが完了するのに必要な作業量を把握するのに役立ちます。これは、リソースがタスクを完了するために予算を作成する時間を決定するのに役立ちます。

     タスクと予定時間数の関連付けについては、[タスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md)を参照してください。

## イニシアチブにリンクされたプロジェクトに対してシナリオプランナーを使用するビジネスケースのリソースの予算を計上

>[!IMPORTANT]
>
>リソースは 15 年の期間にわたって予算計上できます。期間が 15 年を超えるプロジェクトのリソースを予算計上すると、計上する情報が正確でなくなる可能性があります。
<!--
><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>(is this still accurate for the Scenario Planner?)>
></MadCap:conditionalText>>
>-->

1. 予算計上するプロジェクトにリソースを移動します。

   >[!TIP]
   >
   >これは、リンクされたイニシアチブが少なくとも 1 回発行されたシナリオプランナーのイニシアチブにリンクされたプロジェクトです。

1. 左パネルで「**ビジネスケース**」をクリックします
1. （条件付き）**リソース予算計上**&#x200B;セクションで、次のいずれかの操作を行います。

   * シナリオプランナーから情報を公開したばかりの場合は、リソース予算計上エリアの「**プロジェクトの予算人件費の計算に使用する時間を選択**」フィールドでシナリオプランナーを選択し、「**選択**」をクリックします。

     ![](assets/business-case-sp-selected-with-choose-button-350x121.png)

   * プロジェクトの予算リソースに対して、リソースプランナーが以前に選択されていた場合は、**変更**／**シナリオプランナ**／**選択**&#x200B;をクリックします。

     ![](assets/business-case-rp-selected-change-option-to-switch-to-sp-highlighted-350x37.png)

     Workfront は、リンクされたイニシアティブから必要な担当業務時間を使用して、プロジェクトの予算労務費と予算時間を計算します。これは推奨されるオプションです。コストは、ビジネスケースにプロジェクトの通貨で表示されます。

     プロジェクトをコピーし、予算時間を新規プロジェクトにコピーする場合、シナリオプランナーを使用して予算された時間は新規プロジェクトにコピーされません。リソースプランナーで予算計上された時間のみがコピーされます。詳しくは、[プロジェクトのコピー](../manage-projects/copy-project.md)を参照してください。

     >[!IMPORTANT]
     >
     >シナリオプランナーを使用してプロジェクトのリソースを予算計上すると、Workfront の次のエリアに予算計上労力コストが表示されます。
     >
     >   
     >   
     >* ビジネスケースのリソース予算計上エリア
     >* プロジェクトにリンクされたイニシアチブの人件費としてのシステムレベルのシナリオプランナ。詳しくは、[シナリオプランナーでイニシアチブを作成および編集](../../../scenario-planner/create-and-edit-initiatives.md)を参照してください。
     >   
     >

1. （オプション）「**シナリオプランナーで表示**」をクリックし、プロジェクトにリンクされたイニシアチブを含むプランを開きます。新しいブラウザータブでシナリオプランナーが開きます。
1. （オプション）イニシアチブの情報を更新します。詳しくは、[シナリオプランナーでイニシアチブを作成および編集](../../../scenario-planner/create-and-edit-initiatives.md)を参照してください。

   >[!NOTE]
   >
   >更新するプロジェクトのリソース予算計上エリアに変更があるたびに、イニシアチブを発行する必要があります。
