---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: プロジェクトとイニシアチブ間でのリソース割り当て調整の概要
description: プロジェクトとイニシアチブ間でのリソース割り当て調整の概要
author: Alina
feature: Workfront Scenario Planner
exl-id: 82cd9641-1213-436c-935a-2f04a0425e9c
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: ht
source-wordcount: '554'
ht-degree: 100%

---

# プロジェクトとイニシアチブ間でのリソース割り当て調整の概要

>[!IMPORTANT]
>
>プロジェクトのイニシアチブ情報を表示するには、組織は [!DNL Adobe Workfront Scenario Planner] の追加ライセンスを購入する必要があります。[!DNL Workfront Scenario Planner] の取得について詳しくは、[シナリオプランナーを使用する際に必要なアクセス権](../scenario-planner/access-needed-to-use-sp.md)を参照してください。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: two more articles were added to split content from here according to where the reconciling can happen) </p>
-->

プロジェクトとイニシアチブを接続して、戦略計画と実際の作業を同期させることができます。戦略計画とイニシアチブを [!DNL Scenario Planner] で概説し、プロジェクトで実際の作業を計画すると、プロジェクトとイニシアチブの両方でリソースが一致するようになるので、割り当ての超過と不足を避けられます。

## 前提条件

開始する前に以下が必要です。

* プロジェクトに接続されたイニシアチブがある [!DNL Scenario Planner] のプラン
* イニシアチブに必要な担当業務の割り当て。
* 予定時間数があり、次のいずれかに割り当てられたプロジェクトのタスクまたはイシュー

   * 担当業務
   * 担当業務に関連付けられたユーザー

## プロジェクトとイニシアチブの接続

>[!NOTE]
>
>組織が [!DNL Workfront Scenario Planner] の追加のライセンスを購入している場合にのみ、イニシアチブを作成してプロジェクトに接続できます。

次のいずれかの操作を行うことで、プロジェクトとイニシアチブを接続することができます。

* 新しいイニシアチブとしてのプランへのプロジェクトのインポート

  詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) でのプランへのプロジェクトのインポートを参照してください。

* プロジェクトへのイニシアチブの公開

  詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) でのイニシアチブの公開によるプロジェクトの更新または作成を参照してください。

両方のプロセスによって、プロジェクトと対応するイニシアチブとの間に接続が作成されます。接続後、リソースの割り当てを比較し、それらが一致していることを確認することで、リソースの割り当てを管理できます。

## リンクされたプロジェクトとイニシアチブでのリソースの調整に関する考慮事項

>[!NOTE]
>
>組織が [!DNL Workfront Scenario Planner] の追加のライセンスを購入した場合にのみ、イニシアチブを表示し、プロジェクトに接続し、プロジェクトに対するリソースの割り当てを表示できます。

* プロジェクト上の作業項目にユーザー、チーム、担当業務を割り当てたり、担当業務をイニシアチブに割り当てたりできます。つまり、プロジェクトとイニシアチブ間で調整できるのは担当業務のみとなります。

  >[!TIP]
  >
  >プロジェクトでのユーザーの時間とイニシアチブでの役割の割り当てを一致させるには、ユーザーを担当業務に関連付ける必要があります。

* プロジェクトの次のエリアで、リンクされたプロジェクトに対するイニシアチブの担当業務の割り当てを表示できます。

   * プロジェクトの「[!UICONTROL プロジェクト詳細]」エリアの [!DNL Scenario Planner] のセクション詳しくは、次の記事を参照してください。

      * [ [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md) でのイニシアチブの公開によるプロジェクトの更新または作成
      * [プロジェクトの[!UICONTROL 概要]エリアでの情報の管理](../manage-work/projects/manage-projects/understand-project-overview-area.md)

     >[!TIP]
     >
     >プロジェクトとイニシアチブの担当業務の情報は、[!UICONTROL プロジェクト詳細]の [!DNL Scenario Planner] のセクションに表示されません。

   * 次のエリアにある「[!UICONTROL 役割割り当て]」パネル

      * プロジェクトの[!UICONTROL ワークロードバランサー]

        [!UICONTROL ワークロードバランサー]内のイニシアチブとリンク済みプロジェクト間の役割割り当てを表示および調整する方法について詳しくは、[[!UICONTROL ワークロードバランサー]](../scenario-planner/show-role-allocation-workload-balancer.md)内のプロジェクトおよびイニシアチブに対する役割割り当ての表示を参照してください。

      * [!UICONTROL タスク]セクション

        「[!UICONTROL タスク]」セクション内のイニシアチブとリンク済みプロジェクト間の役割割り当てを調整する方法について詳しくは、[タスクリスト内のプロジェクトとイニシアチブの役割割り当ての表示](../scenario-planner/show-role-allocation-task-list-nwe.md)を参照してください。

     >[!TIP]
     >
     >プロジェクトとイニシアチブの担当業務に関する情報は、「[!UICONTROL 役割割り当て]」パネルに表示されます。

* リンクされたイニシアチブのプロジェクトに対する担当業務の割り当ては表示できません。詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md) のプランへのプロジェクトのインポートを参照してください。

  <!--
  <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
  (NOTE: this might change - project job role visibility into initiative)
  </MadCap:conditionalText>
  -->
