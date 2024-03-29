---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.3 ベータ版 3 リリースアクティビティ
description: 2017.3 リリースは、2017年11月初旬に実稼動環境で利用可能になる予定です。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: dc0cada8-4b9e-40cb-89a5-16f15268b513
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 100%

---

# 2017.3 ベータ版 3 リリースアクティビティ

2017.3 リリースは、2017年11月初旬に実稼動環境で利用可能になる予定です。

>[!IMPORTANT]
>
>このページで説明する機能は、実稼動環境で使用可能になる前に変更される場合があります。

2017年3月に行われたすべての変更のリストについては、[2017.3 リリースアクティビティの概要](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md)を参照してください。

2017.3 ベータ 3 リリースには、すべてのユーザー向けの機能強化が含まれています。

* [グラフの色をカスタマイズ](#customize-chart-colors)
* [プロジェクトをコピーする際の追加オプション](#additional-options-when-copying-projects)
* [リソースプランナーの改善：フィルター](#resource-planner-improvement-filters)
* [リソースプランナーの改善：「設定」エリアにイシュー時間を表示](#resource-planner-improvement-show-issue-hours-in-the-settings-area)
* [カスタム更新およびプレビューサンドボックスの SSO 情報が更新されない](#sso-information-for-the-custom-refresh-and-preview-sandboxes-do-not-refresh)
* [Workfront Proof のブラウザーサポート要件の更新](#updated-browser-support-requirements-for-workfront-proof)

## グラフの色をカスタマイズ {#customize-chart-colors}

グラフの要素の色をカスタマイズできるようになりました。これは、レポート内のすべてのタイプのグラフに適用されます。ガントチャートには適用されません。

この変更前は、Workfront ではすべてのグラフの要素の色がデフォルトで選択されていました。グラフの色のカスタマイズについて詳しくは、[レポートへのグラフの追加](../../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)の「グラフの色のカスタマイズ」の節を参照してください。

## プロジェクトをコピーする際の追加オプション {#additional-options-when-copying-projects}

プロジェクトをコピーする際のオプションが、タスクやイシューのコピー時に使用できるオプションと一致するようになりました。コピー中に、コピー対象のプロジェクトのステータスを変更することもできます。

この更新の前は、コピー中はコピー対象のプロジェクトのステータスを変更できず、プロジェクトのコピー時に使用できるオプションは次の 2 つのみでした。

* タスクとプロジェクトの割り当てを保持
* タスクとプロジェクトの進捗を保持

新しい機能では、以前のオプションは削除され、プロジェクトをコピーする際に次のオプションが追加されました。

* 割り当てのクリア
* 財務情報のクリア
* 進行状況のクリア
* 承認のクリア
* カスタムデータ
* リマインダ通知のクリア
* ドキュメントのクリア
* 費用のクリア
* すべての先行タスクをクリア
* 許可のクリア
* すべて選択

プロジェクトのコピーに関する新機能について詳しくは、[プロジェクトのコピー](../../../../manage-work/projects/manage-projects/copy-project.md)の「プレビュー環境でのプロジェクトのコピー」の節を参照してください。

## リソースプランナーの改善：フィルター {#resource-planner-improvement-filters}

次のオブジェクトを使用して、リソースプランナーに表示される情報をフィルタリングできるようになりました。

* ポートフォリオ
* プロジェクトのステータス
* チーム
* 担当業務
* リソースプール

また、これらのオブジェクトに基づいてカスタムフィルターを追加することもできます。

リソースプランナーの使用について詳しくは、[リソースプランナーの概要](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)を参照してください。

## リソースプランナーの改善：「設定」エリアにイシュー時間を表示 {#resource-planner-improvement-show-issue-hours-in-the-settings-area}

リソースプランナーに新しい「設定」エリアが追加され、リソースプランナーをカスタマイズするための複数のオプションが表示されます。このリリースでは、イシューの予定時間数をリソースプランナーの「予定時間数」列に含める最初のオプションを追加しました。

リソースプランナーの使用について詳しくは、[リソースプランナーの概要](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)を参照してください。

## カスタム更新およびプレビューサンドボックスの SSO 情報は更新されません {#sso-information-for-the-custom-refresh-and-preview-sandboxes-do-not-refresh}

このリリース以降、カスタム更新およびプレビューサンドボックスを更新すると、SSO 情報は実稼動環境からコピーされず、無効にもなりません。この変更が行われる前は、カスタム更新およびプレビューサンドボックスの SSO 情報が無効になり、「なし」に設定されていました。

カスタム更新サンドボックス環境について詳しくは、[Adobe Workfront カスタム更新サンドボックス環境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-custom-refresh-sandbox-environment.md)を参照してください。

プレビューサンドボックス環境について詳しくは、[Adobe Workfront プレビューサンドボックス環境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)を参照してください。

## Workfront Proof のブラウザーサポート要件の更新 {#updated-browser-support-requirements-for-workfront-proof}

Workfront Proof のブラウザーサポート要件が更新されました。詳しくは、[Adobe Workfront のブラウザー要件](../../../../workfront-basics/workfront-browser-requirements.md)を参照してください。
