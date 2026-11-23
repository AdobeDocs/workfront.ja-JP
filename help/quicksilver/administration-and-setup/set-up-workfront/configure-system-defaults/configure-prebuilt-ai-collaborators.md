---
user-type: administrator
product-area: system-administration;setup
title: 事前定義済みのAI共同作業者の設定
description: Adobe Workfront管理者は、ユーザーがタスクやイシューに割り当てることができる作業担当者として、受注コーディネーターなどのAdobeから事前構築済みのAI共同作業者を設定できます。
author: Becky
feature: System Setup and Administration
role: Admin
source-git-commit: 71c1855166c2f950509cc8b7dc63792eabb6de16
workflow-type: tm+mt
source-wordcount: '416'
ht-degree: 13%
---
# 事前定義済みのAI共同作業者の設定

<span class="preview">このページの情報は、まだ一般に提供されていない機能を指します。 すべてのユーザーのプレビュー環境でのみ使用できます。 リリースからプレビューの後、高速リリースを有効にしたお客様は、同じ機能を毎月実稼動環境でも使用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

## 概要

事前定義済みのAI共同作業者は、Adobeの既製の作業エージェントで、欠落している情報のリクエストの確認など、特定の作業を行うように設定されています。 Adobe Native Work Agentsとして利用できるため、外部プラットフォームでエージェントを設定したり、外部プラットフォームの資格情報を提供したりする必要はありません。

作業エージェントを設定する際に、エージェントのソースとして事前定義済みの共同作業者を選択します。 次に、作業エージェントに名前を付け、アクセスレベルを設定し、実行できるアクションを選択します。 ユーザーは、設定された作業エージェントを、他の作業エージェントを割り当てるのと同じ方法で、タスクまたはイシューに割り当てます。 ユーザーは、エージェントが事前に構築された共同作業者であることを知る必要はありません。

Work Agentsおよびその他のAI コラボレーターの種類について詳しくは、[AI コラボレーターの設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] パッケージ</td> 
   <td><p>Select、Prime、またはUltimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>[!UICONTROL Standard]</p></td> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>[!UICONTROL システム管理者]またはグループ管理者</td> 
  </tr> 
  </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

Adobe CX Coworkerを有効にする必要があります。 詳しくは、[WorkfrontでのCX Enterprise Coworkerの概要](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md)を参照してください。

## 事前定義済みAI コラボレーターの設定

Work Agentを設定する際に、事前構築済みのAI Collaboratorを設定します。 **エージェントのオリジンを選択**&#x200B;領域で、**Adobe Native**&#x200B;を選択し、次のリストから使用する事前定義済みの共同作業者を選択します。

完全な手順については、[WorkfrontでのWork Agentの設定](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-work-agent-in-workfront)を参照してください。

共同作業者を設定した後、ユーザーはそれをタスクまたはイシューに割り当てることができます。 詳しくは、[作業担当者の使用](/help/quicksilver/manage-work/tasks/assign-tasks/use-task-collaborators.md)を参照してください。

## 利用可能な事前定義済みのAI共同作業者

### CX Enterprise Coworker {#cx-enterprise-coworker}

Adobe Agent Orchestratorを活用したCX Enterprise Coworkerエージェント。

詳しくは、[WorkfrontでのCX Enterprise Coworkerの概要](/help/quicksilver/workfront-basics/coworker-in-workfront/coworker-overview.md)を参照してください。

### 受注コーディネーター {#intake-coordinator}

受注コーディネーターは、欠落、不明確、または一貫性のない情報について、リクエストの詳細、カスタムフォーム、添付ファイルをチェックします。 フィードバックを投稿したり、ユーザーの承認にもとづいて変更を加えたりします。

<!--
### Context Carrier {#context-carrier}

The Context Carrier keeps brief information flowing downstream so that context doesn't get scattered. It helps campaign managers and project managers keep the project team current without writing reports.

Requirements: A Workfront project and a Workfront Planning project must be connected to a Planning record. The Context Carrier must be triggered to run.

Steps to be added.

### Production Specialist {#production-specialist}

The Production Specialist produces images in every size you need, so designers don't have to resize them manually.

Requirement: Users must assign the Production Specialist to a task or issue.

Steps to be added.

### Version Comparer {#version-comparer}

The Version Comparer compares versions of a document so project teams can move content faster instead of spotting differences by hand.

Requirement: The document must have more than one version.

Steps to be added.

### Metadata Manager {#metadata-manager}

The Metadata Manager helps marketing teams find, tag, and label documents while work is in progress instead of later in the process.

Requirement: The Metadata Manager is available when you upload a document. Users must trigger it from the toolbar.

Steps to be added.

### Resource PTO Detector {#resource-pto-detector}

The Resource PTO Detector helps project teams make sure delivery isn't affected by time off, by identifying tasks assigned to people who are out of office.

Requirements: Tasks must be assigned, and PTO must be logged in Workfront.

Steps to be added.

### Campaign Summarizer {#campaign-summarizer}

Description and steps to be added.
-->
