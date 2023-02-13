---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: プロジェクトとイニシアチブ間でのリソース割り当て調整の概要
description: プロジェクトとイニシアチブ間でのリソース割り当て調整の概要
author: Alina
feature: Workfront Scenario Planner
exl-id: 82cd9641-1213-436c-935a-2f04a0425e9c
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '548'
ht-degree: 0%

---

# プロジェクトとイニシアチブ間でのリソース割り当て調整の概要

>[!IMPORTANT]
>
>組織は、 [!DNL Adobe Workfront Scenario Planner] プロジェクトのイニシアチブ情報を表示できます。 詳しくは、 [!DNL Workfront Scenario Planner]を参照してください。 [シナリオ・プランナを使用するために必要なアクセス](../scenario-planner/access-needed-to-use-sp.md) .

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: two more articles were added to split content from here according to where the reconciling can happen) </p>
-->

プロジェクトとイニシアチブを結び付けて、戦略計画と実際の作業を確実に同期させることができます。 戦略計画とイニシアチブの概要を [!DNL Scenario Planner] プロジェクトで実際の作業を計画すると、プロジェクトとイニシアチブの両方でリソースが一致するようになり、割り当て超過や過剰な利用を回避できます。

## 前提条件

開始する前に、次の情報が必要です。

* 内のプラン [!DNL Scenario Planner] イニシアチブがプロジェクトに関連付けられている
* イニシアチブに必要なジョブの役割の割り当て。
* 計画時間を持ち、次のいずれかに割り当てられたプロジェクトのタスクまたはタスク。

   * 担当業務
   * ジョブの役割に関連付けられたユーザー

## プロジェクトとイニシアチブの連携

>[!NOTE]
>
>組織がプロジェクトの追加ライセンスを購入している場合にのみ、イニシアチブを作成してプロジェクトに接続できます [!DNL Workfront Scenario Planner].

次のいずれかの操作を行うことで、プロジェクトとイニシアチブを結び付けることができます。

* 新規イニシアチブとしてプロジェクトをプランにインポート

   詳しくは、 [内のプランにプロジェクトをインポート [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* プロジェクトへのイニシアチブの公開

   詳しくは、 [プロジェクトを更新または作成するには、 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) .

両方のプロセスによって、プロジェクトと対応するイニシアチブとの間に接続が作成されます。 接続後、リソースの割り当てを比較し、それらが一致していることを確認することで、リソースの割り当てを管理できます。

## リンクされたプロジェクトとイニシアチブでのリソースの調整に関する考慮事項

>[!NOTE]
>
>組織がプロジェクトの追加ライセンスを購入した場合にのみ、イニシアチブを表示し、プロジェクトに接続し、プロジェクトに対するリソース割り当てを表示できます [!DNL Workfront Scenario Planner].

* プロジェクト上の作業項目にユーザー、チーム、ジョブの役割を割り当てたり、ジョブの役割をイニシアチブに割り当てたりできます。 その結果、プロジェクトとイニシアチブ間でのジョブの役割の紐付けのみが可能になります。

   >[!TIP]
   >
   >プロジェクトでのユーザーの時間を、イニシアチブに対するロール割り当てと紐付けするには、ユーザーをジョブロールに関連付ける必要があります。

* プロジェクトの次の領域で、リンクされたプロジェクトに対するイニシアチブのジョブの役割の割り当てを表示できます。

   * [!DNL Scenario Planner] セクション [!UICONTROL プロジェクトの詳細] 領域を選択します。 詳しくは、次の記事を参照してください。

      * [プロジェクトを更新または作成するには、 [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md)
      * [プロジェクト内の情報の管理 [!UICONTROL 概要] 領域](../manage-work/projects/manage-projects/understand-project-overview-area.md)

      >[!TIP]
      >
      >プロジェクトとイニシアチブの役割情報を [!DNL Scenario Planner] セクション [!UICONTROL プロジェクトの詳細].

   * この [!UICONTROL ロールの配分] パネルは、次の領域にあります。

      * [!DNL Workload Balancer] プロジェクトの

         イニシアチブと、 [!DNL Workload Balancer]を参照してください。 [内のプロジェクトおよびイニシアチブに対する役割割り当てを表示 [!DNL Workload Balancer]](../scenario-planner/show-role-allocation-workload-balancer.md).

      * [!UICONTROL タスク] セクション

         イニシアチブと、 [!UICONTROL タスク] セクション： [タスクリストのプロジェクトおよびイニシアチブのロール割り当てを表示](../scenario-planner/show-role-allocation-task-list-nwe.md).
      >[!TIP]
      >
      >プロジェクトとイニシアチブの役割情報を、 [!UICONTROL ロールの配分] パネル。



* リンクされたイニシアチブのプロジェクトに対するジョブの役割の割り当てを表示できません。 詳しくは、 [内のプランにプロジェクトをインポート [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

   <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this might change - project job role visibility into initiative)
  </MadCap:conditionalText>
  -->
