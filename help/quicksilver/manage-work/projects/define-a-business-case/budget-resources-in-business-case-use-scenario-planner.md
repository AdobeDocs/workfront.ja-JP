---
navigation-topic: business-case-and-scorecards
title: シナリオ・プランナを使用したビジネス・ケースの予算生産資源
description: リソース計画の一環として、Adobe Workfrontシナリオプランナーを使用して、ビジネスケースの構築時に、プロジェクトでの作業の完了に必要な役割を予算できます。
author: Alina
feature: Work Management
exl-id: d5f3e348-dc7d-4265-a5ce-8eef152db410
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 0%

---

# シナリオ・プランナを使用したビジネス・ケースの予算生産資源

リソース計画の一環として、Adobe Workfrontシナリオプランナーを使用して、ビジネスケースの構築時に、プロジェクトでの作業の完了に必要な役割を予算できます。

ビジネスケースの作成について詳しくは、 [プロジェクトのビジネスケースの作成](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>システム・レベルのシナリオ・プランナで入力したプロジェクトにリンクされているイニシアチブの役割情報は、イニシアチブを発行する際に、プロジェクトのビジネス・ケースの「リソース予算設定」領域に表示されます。 シナリオプランナーは、新しいAdobe Workfrontエクスペリエンスでのみ使用でき、追加のライセンスが必要です。 Workfront Scenario Planner の詳細は、 [シナリオプランナーの概要](../../../scenario-planner/scenario-planner-overview.md).

また、リソース・プランナを使用して、ビジネス・ケース内のリソースを予算できます。 詳しくは、次を参照してください。

* [ビジネス事例の予算リソース](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)

<!--* [Budget resources by project in the Resource Planner](../../../resource-mgmt/resource-planning/budget-by-project-resource-planner-d.md)-->

>[!NOTE]
>
>プロジェクトの作業を開始する際に、リソースプランナーとシナリオプランナーのどちらを使用するかを決定することをお勧めします。 プロジェクトの期間中にこの 2 つを頻繁に切り替えると、プロジェクトのリソースを予算する際に不整合が生じる場合があります。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>ビジネス以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td> <p>この記事で説明する機能にアクセスするには、Adobe Workfront Scenario Planner の追加ライセンスを購入する必要があります。</p> <p>Workfront Scenario Planner の取得について詳しくは、 <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">シナリオ・プランナを使用するために必要なアクセス</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>次へのアクセスを編集します。 </p> 
    <ul> 
     <li> <p>プロジェクト</p> </li> 
     <li> <p>財務データ</p> </li> 
     <li> <p>シナリオ プランナ </p> </li> 
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

* シナリオ・プランナを使用してプランを作成します。

   詳しくは、 [シナリオプランナーでのプランの作成と編集](../../../scenario-planner/create-and-edit-plans.md).

* プランにイニシアチブを作成し、プロジェクトにリンクします。

   イニシアチブに必要な役割情報を指定し、リンクされたプロジェクトをこの情報で更新します。

   詳しくは、次の記事を参照してください。

   * [シナリオプランナーでイニシアチブを作成および編集します](../../../scenario-planner/create-and-edit-initiatives.md)
   * [シナリオプランナーのプランにプロジェクトをインポートします](../../../scenario-planner/import-projects-to-plans.md)
   * [シナリオプランナーでイニシアチブを公開して、プロジェクトを更新または作成します](../../../scenario-planner/publish-scenarios-update-projects.md).

* これらは前提条件ではありませんが、次のこともお勧めします。

   * プロジェクト上のタスクを、シナリオ・プランナで予算化されたジョブの役割に割り当てます。
   * プロジェクトのタスクの予定時間数を指定します。

      これは、タスクが完了するのに必要な作業量を把握するのに役立ちます。これは、リソースがタスクを完了するために予算を作成する時間を決定するのに役立ちます。

      タスクと計画時間の関連付けについては、 [タスクを編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## イニシアチブにリンクされたプロジェクトに対してシナリオ・プランナを使用するビジネス・ケースの予算リソース

>[!IMPORTANT]
15 年間のリソース予算を作成できます。 期間が 15 年を超えるプロジェクトのリソースを予算する場合、予算設定情報が正確でない可能性があります。
<!--
><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>(is this still accurate for the Scenario Planner?)>
></MadCap:conditionalText>>
>-->


1. リソースを予算するプロジェクトに移動します。

   >[!TIP]
   これは、リンクされたイニシアチブが少なくとも 1 回発行されたシナリオプランナーのイニシアチブにリンクされたプロジェクトです。

1. クリック **ビジネス事例** をクリックします。
1. （条件付き） **リソース予算設定** セクションで、次のいずれかの操作を行います。

   * シナリオ・プランナから情報を公開した場合は、 **プロジェクトの予算労務費の計算に使用する時間を選択します** 「生産資源予算編成」領域のフィールドで、 **選択**.

      ![](assets/business-case-sp-selected-with-choose-button-350x121.png)

   * プロジェクトの予算リソースに対して、「リソース・プランナ」が以前に選択されていた場合は、 **変更** > **シナリオプランナー** > **選択**.

      ![](assets/business-case-rp-selected-change-option-to-switch-to-sp-highlighted-350x37.png)

      Workfrontは、リンク・イニシアティブから必要な職務ロール時間を使用して、プロジェクトの予算労務費と予算時間を計算します。 これが推奨されるオプションです。 コストは、ビジネスケースにプロジェクトの通貨で表示されます。

      プロジェクトをコピーし、予算時間を新規プロジェクトにコピーする場合、シナリオ・プランナを使用して予算された時間は新規プロジェクトにコピーされません。 リソース・プランナで予算設定された時間のみがコピーされます。 詳しくは、 [プロジェクトのコピー](../manage-projects/copy-project.md).

      >[!IMPORTANT]
      シナリオ・プランナを使用してプロジェクトの生産資源を予算すると、Workfrontの次の領域に予算労務費が表示されます。
      * ビジネス事例のリソース予算領域
      * プロジェクトにリンクされたイニシアチブの「個人原価」としてのシステム・レベルのシナリオ・プランナ。 詳しくは、 [シナリオプランナーでイニシアチブを作成および編集します](../../../scenario-planner/create-and-edit-initiatives.md).


1. （オプション）「 **シナリオプランナーで表示** ：プロジェクトにリンクされたイニシアチブを含むプランを開きます。 これにより、新しいブラウザタブでシナリオプランナーが開きます。
1. （オプション）イニシアチブの情報を更新します。 詳しくは、 [シナリオプランナーでイニシアチブを作成および編集します](../../../scenario-planner/create-and-edit-initiatives.md).

   >[!NOTE]
   プロジェクトの「生産資源予算設定」領域が更新されるたびに、イニシアチブを発行する必要があります。
