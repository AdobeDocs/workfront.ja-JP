---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.3 ベータ版 1 リリースアクティビティ
description: このページでは、2017.3 リリースでプレビュー環境にて最近利用可能となったすべての変更について説明します。このページに記載されている機能は、2017年8月9日（PT）にプレビュー環境で使用できるようになりました。2017年11月初旬に、実稼動環境で利用可能になる予定です。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 33a91c25-98ec-4f08-b444-4e11e05e464b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1426'
ht-degree: 100%

---

# 2017.3 ベータ版 1 リリースアクティビティ

このページでは、2017.3 リリースでプレビュー環境にて最近利用可能となったすべての変更について説明します。このページに記載されている機能は、2017年8月9日（PT）にプレビュー環境で使用できるようになりました。2017年11月初旬に、実稼動環境で利用可能になる予定です。

>[!IMPORTANT]
>
>このページで説明する機能は、実稼動環境で使用可能になる前に変更される場合があります。

2017年3月に行われたすべての変更のリストについては、[2017.3 リリースアクティビティの概要](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md)を参照してください。

2017.3 ベータ版 1 リリースには、Workfront 管理者およびその他のユーザー向けの機能強化が含まれています。

**管理者向け：**

* [時間数の記録時にタスクとイシューの削除を防止](#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged)
* [設定エリアからの「早期アクセス」設定の削除](#removal-of-the-early-access-setting-from-the-setup-area)
* [Workfront のデフォルトメールアドレスの変更](#workfront-default-email-address-change)

**すべてのユーザー向け：**

* [リソーススケジュールの改善](#resource-scheduling-improvements)
* [ワイドスクリーン表示](#widescreen-display)
* [レポートおよびリストの列のサイズ変更と並べ替え](#resize-and-reorder-columns-in-reports-and-lists)
* [タスクやイシューをコピーする際の「カスタムデータをクリア」オプション](#clear-custom-data-option-when-copying-tasks-and-issues)
* [テンプレートからのプロジェクトの直接作成](#create-a-project-directly-from-a-template)
* [登録されたオブジェクトのアプリ内通知](#in-app-notification-for-subscribed-objects)
* [@タグ付けが現在プレビュー環境で使用不可](#tagging-currently-not-available-in-the-preview-environment)。
* [プロジェクトの稼働率レポートにユーザー割り当て情報を含める](#include-user-allocation-information-in-the-utilization-report-on-a-project)

## リソーススケジュールの改善 {#resource-scheduling-improvements}

>[!NOTE]
>
>23.1 リリースで、リソーススケジュールツールは廃止され、Workfront から削除されました。ワークロードバランサーを使用したリソースのスケジュール設定について詳しくは、[ワークロードバランサーの概要](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)を参照してください。

リソースマネージャーとしてチーム、プロジェクトまたは複数のプロジェクトのリソースをスケジュールする際に、リソーススケジュールの以下の機能強化を利用できます。

* [フルスクリーンモードでのスケジュールエリアの表示](#view-scheduling-area-in-full-screen-mode)
* [リソーススケジュールエリアを表示するための日付範囲オプションの追加](#more-date-range-options-for-viewing-the-resource-scheduling-area)
* [スケジュールタイムラインでの見込日の表示](#view-projected-dates-on-the-scheduling-timeline)

### フルスクリーンモードでのスケジュールエリアの表示 {#view-scheduling-area-in-full-screen-mode}

スケジュールタイムラインをフルスクリーンモードで表示して、1 つのビューでより多くの情報を確認できます。 

詳しくは、「リソーススケジュールの基本を学ぶ」を参照してください。

### リソーススケジュールエリアを表示するための日付範囲オプションの追加 {#more-date-range-options-for-viewing-the-resource-scheduling-area}

スケジュールタイムラインを表示する際に、次の日付範囲オプションが追加で表示されます。

* 1 日表示
* 4 週間表示
* 6 週間表示

この変更以前は、1 週間表示、2 週間表示または 3 週間表示のみでスケジュールタイムラインを表示できました。これらの日付範囲は、新しい日付範囲に加えて、引き続き使用できます。

スケジュールタイムラインを 1 日表示で表示すると、ユーザー割り当て（毎日の合計時間数を含む）は表示できません。

詳しくは、「リソーススケジュールの基本を学ぶ」を参照してください。

### スケジュールタイムラインでの見込日の表示 {#view-projected-dates-on-the-scheduling-timeline}

タスクやイシューの予定日ではなく見込日を表示するようにスケジュールタイムラインを設定できるようになりました。 

この変更以前は、スケジュールタイムラインのタスクやイシューには「予定日」のみが表示されていました。

スケジュールタイムラインで見込日を表示する場合、ユーザー割り当て（毎日の合計時間数を含む）は表示できません。

詳しくは、「リソーススケジュールの基本を学ぶ」を参照してください。

## ワイドスクリーンディスプレイ {#widescreen-display}

Workfront で次のオブジェクトのいずれかを表示すると、ブラウザーウィンドウ全体が自動的に入力されます。

* プロジェクト
* タスク
* イシュー
* レポート
* ダッシュボード
* カレンダー

この変更以前は、表示エリアの両側に白いサイドバーが 2 本ありました。これで、ワイドスクリーン表示は、画面の幅とブラウザーウィンドウの幅に合わせて動的に調整されます。

## レポートとリストの列をサイズ変更および並べ替え {#resize-and-reorder-columns-in-reports-and-lists}

レポートを編集しなくても、レポートまたはリスト内の列の並べ替えやサイズ変更ができるようになりました。（この機能は、今年初めの先行アクセス環境の廃止に伴って削除されました。現在は再導入中です）。

ダッシュボードリストやレポートは新しいデータグリッド構造で再設計されているため、この機能は使用できません。その他のすべてのリストでは、今回のリリースでこの機能が有効になります。

列のサイズ変更と並べ替えについて詳しくは、[列の幅と順序を変更](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md)を参照してください。

## タスクとイシューをコピーする際の「カスタムデータをクリア」オプション {#clear-custom-data-option-when-copying-tasks-and-issues}

タスクまたはイシューをコピーする際に、任意のカスタムデータをクリアするオプションを選択できるようになりました。タスクまたはイシューのカスタムデータをクリアする場合、フォームは新しい項目にコピーされますが、フォームのカスタムデータはコピーされません。カスタムデータを消去すると、アイテムに添付されたドキュメントに添付されたカスタムフォームや、タスクの費用に添付されたカスタムフォームにも影響します。

この変更以前は、タスクまたはイシューをコピーしたときに、カスタムフォームに含まれるカスタムデータも新しい項目にコピーされていました。 

タスクのコピーについて詳しくは、[タスクをコピーおよび複製](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)を参照してください。

イシューのコピーについて詳しくは、[イシューをコピー](../../../../manage-work/issues/manage-issues/copy-issues.md)を参照してください。

## プロジェクトをテンプレートから直接作成 {#create-a-project-directly-from-a-template}

これで、テンプレートレベルで、テンプレートからプロジェクトを作成できるようになりました。

この変更以前は、「**テンプレートからの新規プロジェクト**」オプションを使用して、Workfront のプロジェクトエリアにある「プロジェクト」タブでしか、テンプレートからプロジェクトを作成することはできませんでした。

テンプレートからプロジェクトを作成する方法について詳しくは、[テンプレートを使用してプロジェクトを作成](../../../../manage-work/projects/create-projects/create-project-from-template.md)を参照してください。

## 時間が記録されたときにタスクとイシューが削除されるのを防ぐ {#prevent-tasks-and-issues-from-being-deleted-when-hours-are-logged}

時間が記録されたタスクやイシューの削除を許可、または禁止するように Workfront を設定できるようになりました。

この変更以前は、時間が記録されたタスクまたはイシューを削除した場合、時間は、タイムシートと時間の環境設定に応じて、タスクまたはイシューと共に削除されたか、プロジェクトに移動されていました。

タスクの削除について詳しくは、[タスクを削除](../../../../manage-work/tasks/manage-tasks/delete-tasks.md)を参照してください。

イシューの削除について詳しくは、[イシューを削除](../../../../manage-work/issues/manage-issues/delete-issues.md)を参照してください。

タスクおよびイシューの削除に対してシステム設定を有効にする方法について詳しくは、[システム全体のタスクとイシューの環境設定を指定](../../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

## 設定エリアから「先行アクセス」設定を削除 {#removal-of-the-early-access-setting-from-the-setup-area}

Workfront 管理者がユーザーの先行アクセス環境への登録を可能にする設定を削除します。この機能は、2016 年末以降廃止されました。2017 年に先行アクセスに新しい機能はリリースされておらず、その環境に残っていたすべての機能は実稼動環境に移行しました。

この変更以前は、Workfront 管理者が先行アクセス環境にユーザーを追加することができましたが、アクセスする新機能はありませんでした。

## Workfront のデフォルトメールアドレスの変更 {#workfront-default-email-address-change}

Workfront のデフォルトの送信用メールアドレスが、[noreply@attask.com](mailto:noreply@attask.com) から [noreply@my.workfront.com](mailto:noreply@workfront.com) に変更になりました。

現在、Workfront から送信されるメールをフィルタリングしている場合は、新しいデフォルトのアドレスを反映するようにフィルターを変更する必要があります。 

デフォルトのアドレスの変更は、設定済みの Workfront メールアドレスには影響しません。 

詳細情報は、以下を参照してください。

## 登録したオブジェクトのアプリ内通知 {#in-app-notification-for-subscribed-objects}

登録しているプロジェクト、タスク、およびイシューに対してユーザーがコメントを入力すると、アプリ内通知が届きます。アプリ内通知の登録について詳しくは、[アプリ内通知の表示と管理](../../../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md)を参照してください。

Workfront 管理者が有効にした機能に応じて、登録項目に関するメール通知を受け取ることもできます。登録メールのリンクを通じて、項目を簡単に登録解除できます。詳しくは、[Adobe Workfront 通知](../../../../workfront-basics/using-notifications/wf-notifications.md)を参照してください。

この変更が行われる前は、登録項目に関するメール通知が常に届いており、アプリ内通知を受け取るオプションはありませんでした。

登録メールを無効にすることはできますが、登録項目のアプリ内通知を無効にすることはできません。詳しくは、[システムの全員に対するイベント通知の設定](../../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)を参照してください。

項目の登録について詳しくは、[Adobe Workfront で項目に登録](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)を参照してください。

## プレビュー環境で @ タグ機能が現在利用できない {#tagging-currently-not-available-in-the-preview-environment}

リッチテキスト形式機能を更新ストリームに取り込む作業を行っているため、プレビュー環境の次のオブジェクトに関して、更新ストリームで @ 記号を使用して他のユーザーにタグ付けすることが一時的にできなくなります。

* プロジェクト
* タスク
* イシュー
* タイムシート

「**この更新に他者を含める**」アイコンをクリックすることによって他のユーザーにタグを付けることは、引き続き可能です。

詳しくは、[更新時の他のユーザーへのタグ付け](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)を参照してください。

## プロジェクトの稼働率レポートにユーザー割り当て情報を含める {#include-user-allocation-information-in-the-utilization-report-on-a-project}

>[!NOTE]
>
>23.1 リリースで、リソーススケジュールツールは廃止され、Workfront から削除されました。ワークロードバランサーを使用したリソースのスケジュール設定について詳しくは、[ワークロードバランサーの概要](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)を参照してください。

プロジェクトの稼働率レポートで、タスクの期間中に予定時間数が再割り当てされたかどうかが考慮されるようになりました。ユーザーの時間割り当てが変更された場合（「スケジューリングエリアでユーザー割り当てを管理」を参照）、稼働率レポートで選択した日付にタスクの一部しか含まれていないと、稼働率レポートのデータに影響することがあります。

詳しくは、[リソース稼働率レポートの概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)を参照してください。
