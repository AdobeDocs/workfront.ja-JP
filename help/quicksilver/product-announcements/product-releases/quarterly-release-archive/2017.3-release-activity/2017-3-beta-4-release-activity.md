---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.3 ベータ版 4 リリースアクティビティ
description: このページでは、2017.3 ベータ版 4 リリースでプレビュー環境に最近利用可能となったすべての変更について説明します。このページの機能は、2017年9月25日（PT）の週にプレビュー環境で使用できるようになりました。2017年11月初旬に、実稼動環境で利用可能になる予定です。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: d6bb889c-a057-453f-8f80-761cfb1ad4a1
source-git-commit: 6405c01c8b1d842a4175f9caa18a7ed31316a3a1
workflow-type: tm+mt
source-wordcount: '1676'
ht-degree: 98%

---

# 2017.3 ベータ版 4 リリースアクティビティ

このページでは、2017.3 ベータ版 4 リリースでプレビュー環境に最近利用可能となったすべての変更について説明します。このページの機能は、2017年9月25日（PT）の週にプレビュー環境で使用できるようになりました。2017年11月初旬に、実稼動環境で利用可能になる予定です。

>[!IMPORTANT]
>
>このページで説明する機能は、実稼動環境で使用可能になる前に変更される場合があります。

2017年3月に行われたすべての変更のリストについては、[2017.3 リリースアクティビティの概要](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md)を参照してください。

2017.3 ベータ版 4 リリースには、Workfront 管理者およびその他のユーザー向けの機能強化が含まれています。

**管理者向け**

* [設定エリアの新しいリソース管理環境設定エリア](#new-resource-management-preferences-area-in-the-setup-area)

**すべてのユーザー向け**

* [タスクを複製](#duplicate-tasks)
* [リソースのスケジュール時に割り当てを自動化](#automate-assignments-when-scheduling-resources)
* [リソースのスケジュール時に複数のタスク割り当ての変更](#modify-assignments-for-multiple-tasks-when-scheduling-resources)
* [リソースプランナーへの FTE 分配の適用](#apply-fte-distribution-to-the-resource-planner)
* [ユーザー設定の「担当業務」セクションに含まれる FTE 空き時間の割合](#job-role-section-for-user-settings-includes-percentage-of-fte-availability)
* [プロジェクトにおける稼働率レポートのフィルターの保存と管理](#save-and-manage-filters-in-the-utilization-report-on-a-project)
* [稼動率レポートの追加のフィルタリングオプション](#additional-filtering-options-in-the-utilization-report)
* [プログラムまたはポートフォリオ別の稼働率レポートの表示](#view-the-utilization-report-by-program-or-portfolio)
* [元のイシュー情報をプロジェクトおよびタスクレポートに表示](#show-original-issue-information-in-project-and-task-reports)
* [更新ストリームのフィルターシステムの更新がオブジェクト間で保持](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [Workfront 内のアクティブなプルーフステージのレポート](#report-on-active-proof-stages-within-workfront)
* [Workfront 内でのユーザーへのカスタム Workfront Proof プロファイル権限の割り当て](#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront)
* [イベント登録への時間リソースの追加](#hour-resource-added-to-event-subscriptions)

## タスクを複製 {#duplicate-tasks}

プロジェクト内のタスクやタスクのセットをすばやく複製できるようになりました。このアクションにより、元のタスクと同じタスクが作成されます。複製プロセス中に、新しく作成したタスクに変更を加えることができる追加オプションはありません。 

この変更以前は、新しいプロジェクトまたは既存のプロジェクトにタスクをコピーし、コピー時に情報を変更することができました。

タスクの複製について詳しくは、[タスクのコピーと複製](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)を参照してください。

## リソースのスケジュール時に割り当てを自動化 {#automate-assignments-when-scheduling-resources}

>[!NOTE]
>
>23.1 リリースで、リソーススケジュールツールは廃止され、Workfront から削除されました。ワークロードバランサーを使用したリソースのスケジュール設定について詳しくは、[ワークロードバランサーの概要](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)を参照してください。

Workfront で、複数のプロジェクトのリソースをスケジュールする場合（「スケジュール」タブから）または単一のプロジェクトのリソースをスケジュールする場合（「人材の配置」タブから）、未割り当てタスクとイシューの割り当てを自動的に提案できるようになりました。

Workfront は、稼動可能なユーザー全体の現在の作業割り当てを分析し、まだ割り当てられていないタスクやイシューに対して、インテリジェントで論理的な割り当てを提案します。割り当てを最終決定する前に、提案された割り当てまたは既存の割り当てを変更できます。

詳しくは、「スケジュールエリアでの未割り当てタスクおよびイシューの手動割り当て」を参照してください。

## リソースのスケジュール時に複数のタスク割り当ての変更 {#modify-assignments-for-multiple-tasks-when-scheduling-resources}

リソースを（「スケジュール」タブまたは「人材の配置」タブから）スケジュールする際にユーザーを一括で割り当て、交替、割り当て解除する場合、1 つ以上のプロジェクト内で、指定した特定のタスク（すべてのサブタスクと関連するイシューを含む）の割り当てを変更できます。

この変更以前は、プロジェクト全体でタスクとイシューに対する割り当てを変更できていました（プロジェクト内で特定のタスクを指定することはできませんでした）。

詳しくは、「スケジュールエリアでの未割り当てタスクおよびイシューの手動割り当て」を参照してください。

## リソースプランナーへの FTE 分配の適用 {#apply-fte-distribution-to-the-resource-planner}

>[!NOTE]
>
>この機能は現在、すべてのクラスターのプレビューで使用できるわけではありません。

複数の役割を持つユーザーの場合、各役割の FTE 使用可能時間の割合に基づいて、ユーザーの役割ごとに正確な空き時間数を表示できるようになりました。

例えば、ユーザーのスケジュールが 1 か月で 100 時間の作業が可能で、プライマリ役割の FTE 空き時間の割合が 75％、その他の役割の FTE 空き時間の割合が 25％である場合、リソースプランナーでは、プライマリ役割の空き時間が 75 時間、その他の役割の空き時間が 25 時間のユーザーがリストされます。

この変更以前は、リソースプランナーに表示されるユーザーの名前はプライマリ役割に対してのみ表示され、スケジュールに基づくユーザーの完全な稼働率（100 時間）はプライマリ役割にのみ関連付けられていました。ユーザーのその他の役割は、ユーザーがその役割のタスクに割り当てられ、その他の役割のユーザーの利用可能時間数がゼロである場合にのみ、リソースプランナーに表示されます。

リソースプランナーのユーザーおよび役割に対する利用可能時間数および FTE 使用可能時間を計算する方法について詳しくは、[リソースプランナーのユーザーと役割に対する時間と FTE の計算の概要](../../../../resource-mgmt/resource-planning/calculate-hours-fte-for-users-roles-resource-planner.md)を参照してください。

## ユーザー設定の「担当業務」セクションに含まれる FTE 空き時間の割合 {#job-role-section-for-user-settings-includes-percentage-of-fte-availability}

>[!NOTE]
>
>この機能は現在、すべてのクラスターのプレビューで使用できるわけではありません。

ユーザープロファイルを更新する際に、ユーザーに担当業務を追加し、それぞれの担当業務に割り当てる FTE の割合を定義できるようになりました。

この変更以前は、ユーザーが関連付けられている担当業務のいずれにも、特定の FTE 量を割り当てることができませんでした。

ユーザーの担当業務の FTE の空き時間の割合の更新について詳しくは、[ユーザーのプロファイルの編集](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)または[個人設定を行う](../../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)を参照してください。

## 設定エリアの新しいリソース管理環境設定エリア {#new-resource-management-preferences-area-in-the-setup-area}

これで設定に、リソース管理という新しいエリアが追加されました。このエリアでは、リソースプランナーでのユーザーの空き時間の計算方法を指定できる設定を導入しました。以下の方法で計算できます。

* 手動：ユーザーの個々の FTE に加えて、システムのデフォルトスケジュールを使用して、リソースプランナーでユーザーの空き時間を決定します。ユーザーのスケジュールは無視されます。
* 自動：ユーザーのスケジュールは、リソースプランナーでユーザーの空き時間を決定するために使用されます。FTE の空き時間は、ユーザーのスケジュールとデフォルトのスケジュールに基づいて計算されます。ユーザーの FTE の値は無視されます。 

システムのリソース管理の環境設定の指定について詳しくは、[リソース管理の環境設定を指定](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/configure-resource-mgmt-preferences.md)を参照してください。

## プロジェクトの稼働率レポートでフィルターを保存および管理 {#save-and-manage-filters-in-the-utilization-report-on-a-project}

これで、稼働率レポートで作成したフィルターを保存できます。また、保存済みフィルターの名前変更、保存済みフィルターの複製、保存済みフィルターの削除、保存済みフィルターの変更を行うことができます。

以前は、稼働率レポートをフィルタリングするたびに、個別の「フィルター」オプションを指定する必要がありました。

稼働率レポートでフィルターを保存および管理する方法について詳しくは、[リソース稼働率レポートの概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)にある[リソース稼働率レポートの概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)を参照してください。

## 稼働率レポートの追加の「フィルタリング」オプション {#additional-filtering-options-in-the-utilization-report}

稼働率レポートを実行すると、以前使用可能であったタスク、イシューフ、役割のフィールドに加えて、フィルターを作成する際に、ポートフォリオ、プログラム、プロジェクトの新規フィルタリングフィールドを使用できるようになりました。

この変更以前は、新規フィルター規則を追加することで、ポートフォリオ、プログラム、プロジェクトでのみフィルタリングできました。

詳しくは、[リソース稼働率レポートの概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)の[リソース稼働率レポートの概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)を参照してください。

## プログラムまたはポートフォリオ別の稼働率レポートの表示 {#view-the-utilization-report-by-program-or-portfolio}

プログラムまたはポートフォリオ別に稼働率レポートを表示できるようになりました。これにより、複数のプロジェクトからの情報を 1 つの稼働率レポート内で表示できます。

この変更を容易にするために、Workfront のレポートエリア内と、個々のプロジェクト内の両方で、「稼働率」タブを使用できるようになりました。

この変更以前は、稼働率レポートはプロジェクト内でのみアクセスできました。

詳しくは、[リソース稼働率レポートの概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)を参照してください。

## 元のイシュー情報をプロジェクトおよびタスクレポートに表示 {#show-original-issue-information-in-project-and-task-reports}

>[!NOTE]
>
>この機能は現在、すべてのクラスターのプレビューで使用できるわけではありません。

イシューを変換して作成されたプロジェクトやタスクのプロジェクトやタスクレポートで、元のイシューに関する以下の情報を確認できるようになりました。

* 元のイシューのエントリ日
* 元のイシュー名
* 元のイシューの発信元の ID

この情報は、テキストモードでカスタムビューを作成することにより、タスク、プロジェクトレポートやリストに表示できます。

この変更以前は、この情報をレポートできませんでした。

元のイシューから情報を取得するカスタムテキストモードのビューの作成について詳しくは、[&#x200B; 表示：タスクまたはプロジェクトリストに元のイシューの情報を表示する &#x200B;](../../../../reports-and-dashboards/reports/custom-view-filter-grouping-samples/view-display-original-issue-info-task-project-list.md) を参照してください。

## 更新ストリーム内のフィルターシステムの更新が、オブジェクト間で保持されるようになりました {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

>[!NOTE]
>
>この機能は、ベータ 4 のプレビュー環境ではリリースされませんでした。10月前半にプレビューで公開される予定です。

フィルターシステムの更新オプションは、Workfront サイト全体のオブジェクトにわたって永続的に使用できるようになりました。これにより、システム更新を非表示にして、1 つのオブジェクトの更新ストリーム内のユーザーコメントのみを表示し、他のオブジェクトを参照するときにその設定を維持できます。

この変更以前は、Workfront サイトを参照する際、オブジェクトごとにシステムアップデートを除外することを選択する必要がありました。

詳しくは、[作業の更新](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)を参照してください。

## Workfront 内のアクティブなプルーフステージのレポート {#report-on-active-proof-stages-within-workfront}

Workfront 内でドキュメントのバージョンレポートを作成する際に、「アクティブなプルーフステージ」という列が追加されました。この列では、レポートのそれぞれのドキュメントバージョンで、現在アクティブなプルーフステージを表示できます。ステージの名前は、「アクティブなプルーフステージ」列に表示されます。ドキュメントのバージョンで現在アクティブなステージがない場合、列は空白になります。

ビューとレポートで使用可能なフィールドについて詳しくは、[Adobe Workfront の用語集](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)を参照してください。

## Workfront 内でのユーザーへのカスタム Workfront Proof プロファイル権限の割り当て {#assign-custom-workfront-proof-permission-profiles-to-users-within-workfront}

Workfront でユーザーに対してプルーフ機能を有効にする際に、カスタムの Workfront Proof 権限プロファイルを割り当てられるようになりました。 

この変更以前は、利用可能な権限プロファイルはスーパーバイザー、マネージャー、管理者のみでした。

## イベント登録への時間リソースの追加 {#hour-resource-added-to-event-subscriptions}

新しい時間のリソースを使用して、イベント登録を作成し、請求アプリケーションを Workfront と同期させることができるようになりました。

イベント登録について詳しくは、[Event Subscription API](../../../../wf-api/general/event-subs-api.md) を参照してください。
