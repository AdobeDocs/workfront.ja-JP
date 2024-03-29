---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.2 ベータ版 1 リリースアクティビティ
description: このページでは、2017.2 ベータ 1 リリースに関してプレビュー環境で使用できるすべての変更について説明します。このページの機能は、2017年5月10日（PT）にプレビュー環境で使用できるようになりました。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 99812ed3-a300-478e-973f-b957382d934b
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1380'
ht-degree: 100%

---

# 2017.2 ベータ版 1 リリースアクティビティ

このページでは、2017.2 ベータ 1 リリースに関してプレビュー環境で使用できるすべての変更について説明します。このページの機能は、2017年5月10日（PT）にプレビュー環境で使用できるようになりました。

>[!IMPORTANT]
>
>このページで説明する機能は、実稼動環境で使用可能になる前に変更される場合があります。

2017.2 ベータ 1 リリースには、Workfront 管理者およびその他のユーザー向けの機能強化が含まれています。

**管理者向け：**

* [ドキュメントを復元](#restore-documents)
* [リリース情報を含む新しいプレビューバナー](#new-preview-banner-with-release-information)
* [API 7 の可用性](#api-7-availability)

**すべてのユーザー向け：**

* [タスクとイシューに登録](#subscribe-to-tasks-and-issues)
* [リソーススケジュールの改善](#resource-scheduling-improvements)
* [プルーフを比較](#compare-proofs)
* [ユーザーとプロジェクトのリソースプールの新しいフィールド](#new-field-for-resource-pools-for-users-and-projects)
* [ダッシュボードリストのルックアンドフィールを更新](#updated-look-and-feel-in-the-dashboard-list)
* [Workfront から承認機能を削除](#removing-the-endorsements-functionality-in-workfront)
* [ドラッグアンドドロップでリスト内の列を並べ替えます（機能は削除されています）](#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed)

## ドキュメントを復元する {#restore-documents}

Workfront 管理者は、過去 30 日以内に削除された個々のドキュメントを復元できるようになりました。 

この変更以前は、Workfront 管理者は、プロジェクト、タスク、およびイシュー（削除されたプロジェクト、タスク、またはイシューとともに削除されたドキュメントを含む）のみを復元できました。

詳しくは、[削除された項目を復元](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)を参照してください。

## リリース情報を含む新しいプレビューバナー {#new-preview-banner-with-release-information}

プレビューサンドボックス環境の上部にある青いバナーに、プレビュー環境のリリース名とバージョン番号が表示されるようになりました。リリースの名前をクリックすると、ヘルプサイトの記事が表示され、現在のプレビューリリースの詳細を確認できます。プレビューサンドボックス環境について詳しくは、[Adobe Workfront プレビューサンドボックス環境](../../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md)を参照してください。

## API 7 の可用性 {#api-7-availability}

API 7 がリリースされ、新しいオブジェクトと更新されたオブジェクトが含まれます。

詳しくは、[API バージョン 7 の新機能](../../../../wf-api/api/new-api-version-7.md)を参照してください。

## タスクとイシューに登録する {#subscribe-to-tasks-and-issues}

Workfront は、自分が割り当てられている項目、または自分が所有している項目に関する通知を送信します。

現在のリリース以降、自分に割り当てられていないが、自分の作業に影響を与える可能性のある項目をフォローする場合は、その項目に登録できます。

少なくとも表示する権限を持つイシューやタスクを登録できます。登録するイシューまたはタスクに新しいコメントが追加されると、そのコメントに関する通知がメールで送信されます。

イシューとタスクの登録について詳しくは、[Adobe Workfront の項目を登録](../../../../workfront-basics/using-notifications/subscribe-to-items-in-workfront.md)を参照してください

## リソーススケジュールの改善 {#resource-scheduling-improvements}

>[!NOTE]
>
>23.1 リリースで、リソーススケジュールツールは廃止され、Workfront から削除されました。ワークロードバランサーを使用したリソースのスケジュール設定について詳しくは、[ワークロードバランサーの概要](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)を参照してください。

リソースをスケジュールする際に、次の改善が行われました。

* [リソーススケジュールタイムラインの項目を 1 つのビューで表示](#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view)
* [スケジュールタイムラインのタスクとイシューに表示するプロジェクト名を設定](#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline)
* [親タスクをスケジュールタイムラインに表示するかどうかを設定](#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline)
* [スケジュールタイムラインですべてのタスクとイシューを容易に展開または折りたたむ](#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline)
* [スクロール時に、役割とユーザー情報がスケジュールタイムラインの先頭に残る](#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling)

### リソーススケジュールタイムラインの項目を 1 つのビューで表示する {#view-more-items-on-the-resource-scheduling-timeline-in-a-single-view}

自分がリソースマネージャーであるチームまたはプロジェクトのリソースをスケジュールする際に、タスクとイシューがスケジュールタイムライン上で消費する垂直方向のスペースが少なくなりました。これにより、1 つのビューでより多くのタスクとイシューを表示できます。

各タスクにプロジェクト名を表示し、スケジューリングタイムラインにイシューを表示することにした場合、各タスクとイシューの垂直方向のスペースが展開され、タスクやイシューが 1 つのビューに表示される数が少なくなります。

リソースのスケジュール設定について詳しくは、「リソースのスケジュール設定の概要」を参照してください。

### スケジュールタイムラインでタスクとイシューに表示するプロジェクト名を設定する {#configure-the-project-name-to-display-on-tasks-and-issues-on-the-scheduling-timeline}

自分がリソースマネージャーであるチームまたはプロジェクトのリソースをスケジュールする際に、スケジュールタイムライン上の各タスクおよびイシューに表示するプロジェクト名を設定できるようになりました。これにより、ユーザーはスケジュールタイムラインを表示して、タスクまたはイシューが存在するプロジェクトの名前をすばやく確認できます。

詳しくは、「リソーススケジュールの基本を学ぶ」を参照してください。

### 親タスクをスケジュールタイムラインに表示するかどうかを設定する {#configure-whether-parent-tasks-are-displayed-on-the-scheduling-timeline}

自分がリソースマネージャーであるプロジェクトのリソースをスケジュールする際に、プロジェクトの概要完了モードオプションが手動に設定されている場合、親タスクをスケジュールタイムラインに表示するかどうかを設定できるようになりました。

この変更以前は、プロジェクトの概要完了モードが手動に設定されている場合、親タスクは常にスケジューリングタイムラインに表示されました。 

プロジェクトの概要完了モードが自動に設定されている場合、親タスクはスケジューリングタイムラインに表示できません。このエクスペリエンスは変更されていません。

詳しくは、「リソーススケジュールの基本を学ぶ」を参照してください。

### スケジュールタイムラインですべてのタスクとイシューを容易に展開または折りたたむ {#more-easily-expand-or-collapse-all-tasks-and-issues-on-the-scheduling-timeline}

新しいリンクを使用して、スケジュールタイムライン上のすべてのタスクやイシューをより容易に折りたたむことができます。

詳しくは、「リソーススケジュールの基本を学ぶ」を参照してください。

### スクロール時に、役割とユーザー情報がスケジュールタイムラインの先頭に残る {#role-and-user-information-remains-at-the-top-of-the-scheduling-timeline-when-scrolling}

スケジュールタイムラインを下にスクロールして追加情報を表示する場合、役割名とユーザー名がスケジュールタイムラインのユーザーと役割エリアの先頭に残るので、タスクとイシューが関連付けられているユーザーと役割をより簡単に確認できるようになりました。

この変更以前は、役割名とユーザー名が現在のビューの外にスクロールアウトしていました。

リソースのスケジュール設定について詳しくは、「リソースのスケジュール設定の概要」を参照してください。

## プルーフの比較 {#compare-proofs}

プロジェクト、タスク、イシュー、ポートフォリオの「ドキュメント」タブ内またはグローバルナビゲーションバーのメインのドキュメントエリア内など、1 つのドキュメントリスト内で 2 つのドキュメントプルーフを比較できるようになりました。 

2 つのプルーフはレビューと承認ツール内に表示され、各ドキュメントを並べて表示し、比較しながらプルーフを行うことができます。

詳しくは、[プルーフの比較](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/compare-proofs.md)を参照してください。

## ユーザーとプロジェクトのリソースプールの新しいフィールド {#new-field-for-resource-pools-for-users-and-projects}

R1.5 リリースでは、プレビュー環境でのリソース計画に関する新しい機能が導入されました。この機能を使用すると、新しいリソースプール（ユーザーのコレクション）を作成できます。

これらのリソースプールをユーザーだけでなくプロジェクトにも関連付けることができるようになりました。プロジェクトとユーザーオブジェクトに「リソースプール」という新しいフィールドが表示されます。

新しいリソースプールと、それらをプロジェクトおよびユーザーに関連付ける方法について詳しくは、[リソースプールの概要](../../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)を参照してください。

## ダッシュボードリストのルックアンドフィールのアップデート {#updated-look-and-feel-in-the-dashboard-list}

ダッシュボードのリストを表示する際のルックアンドフィールがより近代的で拡張性が高くなりました。

この機能は、以前は早期アクセスに登録したユーザーのみが利用できました。これはプレビュー環境のすべてのユーザーが使用できるようになりました。2017.2 リリースの実稼動環境のすべてのユーザーが利用できるようになります。 

ダッシュボードについて詳しくは、[ダッシュボードを作成](../../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md)を参照してください。

## Workfront から承認機能を削除 {#removing-the-endorsements-functionality-in-workfront}

更新ストリームに含まれる機能を評価する際、推薦は採用率も使用率も低い機能であることが判明しました。2017.2 では、2017.2 リリース以降、推薦に関する次の機能が Workfront から削除されます（この機能はプレビューでは使用できなくなりました）。

* ユーザープロファイルエリアの「推薦」タブ
* 推薦オブジェクトは、API エクスプローラーから削除されます。現在、「推薦」または「推薦共有」オブジェクトの API レポートを取得している場合、このオブジェクトが削除された後、呼び出しは無効になります。

以下の機能は、引き続き web アプリケーションに存在します。

* この機能の削除前に行われた別のユーザーによるユーザーの推薦は、推薦者の更新ストリームに残ります。 

推薦はレポート可能なオブジェクトではないので、このオブジェクトのレポートに変更はありません。

## ドラッグアンドドロップでリスト内の列を並べ替えます（機能は削除されています） {#reorder-columns-in-any-list-with-drag-and-drop-functionality-is-being-removed}

列を別の場所からドラッグして別の場所にドロップすることでリストの列の順序を変更する機能は、2017.2 リリースで実稼動環境の早期アクセスから削除され、どのユーザーも利用できなくなります。 

この機能について詳しくは、[列の幅と順序を変更](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md)を参照してください。
