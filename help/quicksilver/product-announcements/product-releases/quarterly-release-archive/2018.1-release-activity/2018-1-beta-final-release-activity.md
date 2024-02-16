---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 ベータ版最終リリース（PT）アクティビティ
description: このページでは、2018.1 ベータ版最終リリースのプレビュー環境で最近使用されたすべての変更について説明します。この機能は、2018年1月31日（PT）にプレビュー環境で使用できるようになりました。2018年3月に、実稼動環境で利用できるようになります。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 35bd3604-5452-4b46-afb1-78bc2fbb48ec
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '883'
ht-degree: 100%

---

# 2018.1 ベータ版最終リリース（PT）アクティビティ

このページでは、2018.1 ベータ版最終リリースのプレビュー環境で最近使用されたすべての変更について説明します。この機能は、2018年1月31日（PT）にプレビュー環境で使用できるようになりました。2018年3月に、実稼動環境で利用できるようになります。

>[!IMPORTANT]
>
>このページで説明する機能は、実稼動環境で使用可能になる前に変更される場合があります。

2018年1月に行われたすべての変更のリストについては、[2018.1 リリースアクティビティの概要](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md)を参照してください。

2018.1 ベータ版最終リリースには、Workfront 管理者とその他のユーザーの両方の機能強化が含まれています。

**管理者向け**

* [ユーザースケジュールに基づいて計算するリソースの空き時間とユーザー割り当ての設定](#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule)

**すべてのユーザー向け**

* [モバイルの強化](#mobile-enhancements)
* [Jira 統合](#jira-integration)
* [プルーフビューアー名に更新](#update-to-proofing-viewer-names)
* [実稼動環境からプレビューへの同期時の同期頻度への変更](#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview)
* [リソースプランナーで 2,000 項目制限に達すると、警告メッセージが表示されます](#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner)

## モバイルの機能強化 {#mobile-enhancements}

2018年3月初旬に、モバイルアプリストアに以下の機能が追加されます。

* 新しいナビゲーション：モバイルアプリのホームページのデザインが変更されました。
* Home on Mobile：新しいホーム機能がモバイルアプリでも更新されました。

この新しい機能は、iOS と Android の両方のプラットフォームでサポートされています。

## Jira 統合 {#jira-integration}

Jira 用 Workfront アドオンをインストールして設定することで、Jira のイシューを Workfront のタスクやイシューにリンクできるようになりました。この統合により、プロジェクトマネージャーは Workfront で作業を続け、開発エンジニアは Jira で作業を続け、個々の項目は Workfront と Jira の統合によってリンクされます。

この統合を通じて、次の設定を行うことができます。

* Workfront の割り当てのトリガーを確立して、発生したときに Jira のイシューを自動的に作成します。
* Jira のイシューを Workfront のタスクまたは以前に作成されたイシューに手動でリンクします。
* いずれかのアプリケーションで項目が更新された後、リンクされた項目に対して同期する必要があるフィールドを指定します。

Workfront アドオンは、Jira のオンプレミスバージョンとオンデマンドバージョンの両方で使用できます。アドオンは無料で、2018年3月初めに Atlassian Marketplace でダウンロードできるようになります。

Jira 用 Workfront アドオンのダウンロードリンクなどについて詳しくは、[Workfront を Jira と一緒に使用](https://support.workfront.com/hc/en-us/sections/115001130053)を参照してください。

## プルーフビューアー名に更新 {#update-to-proofing-viewer-names}

Workfront システム全体で、HTML5 ベースのプルーフビューアーおよび Flash ベースのプルーフビューアーの名前が変更されました。以前の名前と更新された名前は次のとおりです。

| **以前の名前** | **更新された名前** |
|---|---|
| HTML5 プルーフビューアー | 新しいプルーフビューアー |
| Flash プルーフビューアー | 従来のプルーフビューアー |

{style="table-layout:auto"}

新しいプルーフビューアーの使用方法について詳しくは、[プルーフビューアーでのプルーフの確認](https://support.workfront.com/hc/en-us/sections/115000275214)を参照してください。

## ユーザースケジュールに基づいて計算するリソースの空き時間とユーザー割り当ての設定 {#configure-resource-availability-and-user-allocations-to-calculate-based-on-the-user-schedule}

>[!NOTE]
>
>23.1 リリースで、リソーススケジュールツールは廃止され、Workfront から削除されました。ワークロードバランサーを使用したリソースのスケジュール設定の詳細は、[ワークロードバランサーの概要](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)を参照してください。

Workfront の管理者は、Workfront がリソースの空き時間とユーザー割り当てをシステムレベルで計算する方法（時間および FTE の空き時間を考慮）を決定できるようになりました。Workfront 管理者は、リソースの空き時間とユーザーの割り当てが、デフォルトのスケジュールまたはユーザーのスケジュールのいずれかを使用して計算されるように設定できます。

この設定は、リソースをスケジュールする際に、以下の状況でのユーザーの空き時間に影響します。

* 「スケジュールエリアで未割り当てのタスクおよびイシューを手動で割り当て」の説明に従って、Workfront がリソースを自動的に割り当てることを許可する場合。

* 「スケジューリングエリアでユーザー割り当てを管理」の説明に従って、割り当て指標を表示する場合。

詳しくは、Workfront がスケジュールエリアでリソース時間と FTE の空き時間を計算する方法を設定を参照してください。

>[!NOTE]
>
>23.1 リリースで、リソーススケジュールツールは廃止され、Workfront から削除されました。ワークロードバランサーを使用したリソースのスケジュール設定について詳しくは、[ワークロードバランサーの概要](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)を参照してください。


## プルーフ実稼動環境からプレビューに同期する場合に、同期頻度へ変更 {#change-to-synchronization-cadence-when-synchronizing-from-the-proofing-production-environment-to-preview}

>[!NOTE]
>
>この変更は2018年2月11日（PT）に発効します。

Workfront Proof の実稼動環境のデータが、毎週 Workfront Proof のプレビュー環境に同期されるようになりました。

この変更以前は、データは Workfront Proof の実稼働環境からプレビュー環境に毎月同期されていましたが、Workfront の実稼働環境のデータは週に 1 回 Workfront のプレビュー環境に同期されていました。この不一致により、Workfront のプレビュー環境でプルーフ機能を使用するときに、数件の同期エラーが発生しました。 

詳しくは、[サンドボックステスト環境のプレビュー - Workfront Proof](../../../../workfront-proof/wp-getstarted/system-information/preview-sandbox.md) を参照してください。

## リソースプランナーで 2,000 項目制限に達すると、警告メッセージが表示されます {#warning-message-displays-when-the-2-000-item-limit-is-reached-in-the-resource-planner}

現在、リソースプランナーのパフォーマンスを向上させるために、より永続的なソリューションに取り組んでおります。このため、リソースプランナーに適用できる各ビューに対して、2,000 項目の制限を導入しました。

* ユーザービューは 2,000 個の割り当てのみを表示
* プロジェクトビューは 2,000 個のプロジェクトのみを表示
* 役割ビューは 2,000 個の役割のみを表示

リソースプランナーが 2,000 個を超える項目を読み込もうとすると、2,000 個の項目のみが表示可能であることを警告する通知が表示されます。

これらの制限とリソースプランナーへの影響に関して詳しくは、[リソースプランナーの表示制限](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)を参照してください。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our beta program for the Resource Planner performance, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref">Resource Planner performance beta </a>.</p>
-->
