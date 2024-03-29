---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.1 ベータ版 3 リリースアクティビティ
description: このページでは、2018.1 ベータ版 3 リリースでプレビュー環境で最近使用されたすべての変更について説明します。この機能は、2018年1月7日（PT）にプレビュー環境で使用できるようになりました。2018 年初頭に、実稼動環境で利用可能になる予定です。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 26bbc4a0-e5ed-4b5f-bfc2-f888362c1d22
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '1850'
ht-degree: 100%

---

# 2018.1 ベータ版 3 リリースアクティビティ

このページでは、2018.1 ベータ版 3 リリースでプレビュー環境で最近使用されたすべての変更について説明します。この機能は、2018年1月7日（PT）にプレビュー環境で使用できるようになりました。2018 年初頭に、実稼動環境で利用可能になる予定です。

>[!IMPORTANT]
>
>このページで説明する機能は、実稼動環境で使用可能になる前に変更される場合があります。

2018年1月に行われたすべての変更のリストについては、[2018.1 リリースアクティビティの概要](../../../../product-announcements/product-releases/quarterly-release-archive/2018.1-release-activity/2018-1-release-activity-overview.md)を参照してください。

2018.1 ベータ版 3 リリースには、Workfront 管理者およびその他のユーザー向けの機能強化が含まれています。

**管理者向け**

* [グループ管理者の改善](#group-administrator-improvements)

**すべてのユーザー向け**

* [HTML5 プルーフビューアの改善](#html5-proofing-viewer-improvements)
* [Workfront 内でのプルーフ機能の改善](#proofing-improvements-within-workfront)
* [ホームエリアの改善](#home-area-improvements)
* [アジャイルの改善](#agile-improvements)
* [ガントチャートの向上](#gantt-chart-improvements)
* [リソースプランナーの改善点](#resource-planner-improvements)

## グループ管理者の改善 {#group-administrator-improvements}

* [グループ管理者用に更新されたパスワード UI をリセット](#reset-password-ui-updated-for-group-administrators)
* [グループ管理者用のアクセスレベル設定オプション](#access-level-setup-options-for-group-administrators)
* [グループのタイムシートプロファイルを作成](#create-timesheet-profiles-for-groups)
* [ユーザーの削除された項目をグループ管理者として復元](#recover-deleted-items-for-users-as-a-group-administrator)

### グループ管理者用に更新されたパスワード UI をリセット {#reset-password-ui-updated-for-group-administrators}

グループ管理者は、別のユーザーのパスワードをリセットすると、パスワードを変更する前に、自分のパスワードを入力するよう求められます。UI が更新され、この機能が反映されました。この変更以前は、UI では Workfront 管理者パスワードが必要であることが表示されていました。

他のユーザーのパスワードのリセットについて詳しくは、[ユーザーのプロファイルの編集](../../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

グループ管理者の機能について詳しくは、[グループの作成](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)内の「グループ管理者の機能」の節を参照してください。

### グループ管理者用のアクセスレベル設定オプション {#access-level-setup-options-for-group-administrators}

Workfront の管理者は、グループ管理者が他のユーザーとしてログインできるかどうか、または他のユーザーのパスワードをリセットできるかどうかを制御できるようになりました。アクセスレベルに、このアクセスを有効または無効にする新しい設定を追加しました。この変更以前は、すべてのグループ管理者が他のユーザーとしてログインし、デフォルトで他のユーザーのパスワードをリセットすることが可能でした。この変更は、計画担当者アクセスレベルにのみ影響します。

ユーザーのアクセスレベルの設定について詳しくは、[ユーザーへのアクセス権の付与](../../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)を参照してください。

グループ管理者の機能について詳しくは、[グループの作成](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)内の「グループ管理者の機能」の節を参照してください。

### グループのタイムシートプロファイルを作成 {#create-timesheet-profiles-for-groups}

グループ管理者は、管理しているグループのタイムシートプロファイルを作成し、管理しているグループ、またはこれらのグループのユーザーに関連付けることができます。タイムシートプロファイルは、タイムシートに関連付けられたユーザーに対してタイムシートが自動的に作成されるようにします。

この変更以前は、Workfront 管理者のみがタイムシートプロファイルを作成できました。

タイムシートプロファイルの作成について詳しくは、[タイムシートプロファイルの作成、編集、割り当て](../../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)を参照してください。

グループ管理者の機能について詳しくは、[グループの作成](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)内の「グループ管理者の機能」の節を参照してください。

### ユーザーの削除された項目をグループ管理者として復元 {#recover-deleted-items-for-users-as-a-group-administrator}

プロジェクトがグループ管理者のグループに関連付けられている場合は、プロジェクト、または削除されたタスク、イシュー、またはドキュメントをごみ箱から復元できます。この変更以前は、Workfront 管理者のみがごみ箱から項目を復元できました。

Workfront で削除した項目を復元する方法について詳しくは、[削除した項目の復元](../../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)を参照してください。

グループ管理者の機能について詳しくは、[グループの作成](../../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)内の「グループ管理者の機能」の節を参照してください。

## HTML5 プルーフビューアの改善 {#html5-proofing-viewer-improvements}

* [比較モード](#compare-mode)
* [コメントリストをフィルタリング](#filter-the-comment-list)
* [最初の文字が入力されるとコメントリストを検索する](#comment-list-is-searched-after-the-first-character-is-entered)

### 比較モード {#compare-mode}

静的プルーフおよびビデオプルーフを表示する際に、HTML5 プルーフビューアで比較モードを使用できるようになりました。 

HTML5 プルーフビューアの比較モードは、次の点でレガシープルーフビューアとは異なります。

* 比較モードを起動すると、新しいバージョンが右側に移動し、比較しているバージョンが左側に開きます。

  以前は、新しいバージョンが左側に移動し、比較しているバージョンが右側に開きました。

* プルーフビューアから、直接比較するプルーフのバージョンを選択できます。 
* プルーフビューア内のプルーフの現在のズームレベルと位置は、同時ナビゲーションを開始するときに維持されます。
* 同時ナビゲーションを使用する場合の新しいリセットオプション。
* 比較モードを終了する際に、閉じるプルーフを選択できます。 

  以前は、古いバージョンは常に閉じられていました。

* 様々なルックアンドフィールとユーザビリティの改善。

詳しくは、[プルーフビューアでプルーフを比較](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/compare-proofs.md)を参照してください。

### コメントリストのフィルタリング {#filter-the-comment-list}

コメントリスト内のコメントをフィルタリングできるようになりました。ユーザー、アクション、未読などでフィルタリングできます。

### 最初の文字が入力されるとコメントリストを検索する {#comment-list-is-searched-after-the-first-character-is-entered}

コメントリストを検索する際に、最初の文字を入力すると、リストが自動的にフィルタリングされるようになりました。

この変更以前は、コメントリストをフィルタリングする前に、検索フィールドに少なくとも 3 文字を入力する必要がありました。

詳細情報は、次を参照してください。

## Workfront 内のプルーフ機能の改善 {#proofing-improvements-within-workfront}

* [Workfront Proof から Workfront へリンク](#link-proofs-from-workfront-proof-to-workfront)
* [ドキュメントからプルーフを削除できなくなりました](#can-no-longer-remove-a-proof-from-a-document)
* [プルーフを生成して開く際のルックアンドフィールの更新](#updated-look-and-feel-when-generating-and-opening-proofs)

### Workfront Proof から Workfront にプルーフをリンクする {#link-proofs-from-workfront-proof-to-workfront}

Workfront Proof アカウントに既に存在するドキュメントプルーフを Workfront にリンクできるようになりました。

この変更以前は、Workfront 内の Workfront Proof に既に存在するプルーフにアクセスできませんでした。 

詳しくは、[外部アプリケーションからドキュメントをリンク](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)の[外部アプリケーションからドキュメントをリンク](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)を参照してください。

### ドキュメントからプルーフを削除できなくなりました {#can-no-longer-remove-a-proof-from-a-document}

ドキュメントからプルーフを削除できなくなりました。プルーフを削除するには、ドキュメント全体を削除する必要があります。

この機能強化により、ユーザーがプルーフ済みドキュメントのすべてのバージョンを誤って削除するリスクが軽減されます。 

ドキュメントの削除について詳しくは、[プルーフを削除](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md)の[プルーフを削除](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/remove-archiveg-proof.md)を参照してください。

### プルーフを生成して開く際のルックアンドフィールの更新 {#updated-look-and-feel-when-generating-and-opening-proofs}

プルーフの生成時にアニメーションスピナーが更新されました。

## ホームエリアの改善 {#home-area-improvements}

ホームエリアに次の機能強化が加えられました。

* [ホームエリアからプルーフの承認を表示](#view-proof-approvals-from-the-home-area)
* [ホームエリアでアイテムのレイアウトテンプレートを設定する際にデフォルトのフィールドを表示](#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area)

### ホームエリアからプルーフの承認を表示する {#view-proof-approvals-from-the-home-area}

標準の承認に加えて、ホームエリアでプルーフの承認を表示できるようになりました。

以前は、Workfront の承認を表示できましたが、プルーフの承認を表示できませんでした。 

詳しくは、[ホームエリアを使用](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md)を参照してください。

### ホームエリアでアイテムのレイアウトテンプレートを設定する際にデフォルトのフィールドを表示 {#default-fields-are-displayed-when-configuring-the-layout-template-for-items-in-the-home-area}

以前は、デフォルトのフィールドはレイアウトテンプレートに表示されていませんでした。

詳しくは、「レイアウトテンプレートの作成と管理」を参照してください。

## アジャイルの改善 {#agile-improvements}

* [タスクまたはイシューの詳細ページから直接イテレーションにタスクとイシューを追加](#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page)
* [アジャイルチームのスクラムバックログとストーリーボードにイシューを含める](#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team)
* [アジャイルチームのバックログへのグループ化とフィルターの適用](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team)
* [空白のイテレーションを作成し後で更新](#create-a-blank-iteration-and-update-it-later)
* [イテレーションの作成時に「フォーカス」フィールドと「処理能力」フィールドを事前入力](#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration)

### タスクまたはイシューの詳細ページから直接イテレーションにタスクとイシューを追加する {#add-tasks-and-issues-to-the-iteration-directly-from-the-task-or-issue-details-page}

現在アジャイルチームに割り当てられているタスクやイシューを、タスクやイシューから直接イテレーションに追加できるようになりました。

以前は、バックログからのみイテレーションにタスクを追加できました。 

詳しくは、[イテレーションを作成](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md)の[イテレーションを作](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md)を参照してください。

### アジャイルチームのスクラムバックログとストーリーボードにイシューを含める {#include-issues-on-the-scrum-backlog-and-story-board-for-an-agile-team}

スクラムアジャイル方法論を使用する場合、アジャイルチームのバックログにデフォルトでイシューが含まれるようになりました（かんばん方法論を使用する場合、イシューはアジャイルチームのバックログに表示されません）。

この変更以前は、バックログに追加できたのはタスクだけでした。イシューを追加する場合は、イシューを追加する前に、まずイシューをタスクに変換する必要がありました。

バックログでのイシューの使用については、[アジャイルバックログを管理](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)を参照してください。

### アジャイルチームのバックログへのグループ化とフィルターの適用 {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

「グループ化」および「フィルター」オプションがアジャイルバックログで使用できるようになり、グループ別にバックログを整理し、特定のタスクとイシューに対するフィルターを設定できます。

この変更以前は、ビューでアジャイルバックログに適用できるようになっていました。

詳しくは、[アジャイルバックログを管理](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)の[アジャイルバックログを管理](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)を参照してください。

### 空白のイテレーションを作成し後で更新する {#create-a-blank-iteration-and-update-it-later}

イテレーションを作成するためにタスクやイシューをイテレーションに追加する必要はなくなりました。空白のイテレーションを作成し、後でタスクとイシューを追加できます。

詳しくは、[イテレーションを作成](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md)を参照してください。

### イテレーションの作成時に「フォーカス」フィールドと「処理能力」フィールドを事前入力 {#the-focus-and-capacity-fields-are-pre-populated-when-creating-an-iteration}

これで、イテレーションを作成する際に、チームが過去に作成したすべてのイテレーションの平均値が「焦点」フィールドと「処理能力」フィールドに事前に設定されます。チームが過去のイテレーションを作成していない場合、これらのフィールドは 0 と表示されます。

以前は、これらのフィールドは常に 0 に設定されていました。

詳しくは、[イテレーションを作成](../../../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md)を参照してください。

## ガントチャートの向上 {#gantt-chart-improvements}

* [ガントチャートで編集モードを有効にする](#enable-edit-mode-in-the-gantt-chart)
* [ガントチャートの編集時に先行タスクを削除する](#remove-predecessors-when-editing-the-gantt-chart)

### ガントチャートで編集モードを有効にする {#enable-edit-mode-in-the-gantt-chart}

ガントチャートで編集モードを有効にすると、グラフ内の情報を変更できます。この変更以前は、ガントチャートの情報を編集できませんでした。タスクリスト上のタスク情報のみ編集できました。

ガントチャートの編集について詳しくは、[タスクリストのガントチャートの情報を更新](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md)を参照してください。

### ガントチャートの編集時に先行タスクを削除する {#remove-predecessors-when-editing-the-gantt-chart}

ガントチャートの編集モードを使用して、プロジェクトのガントチャートでタスク間の先行タスク関係を削除できるようになりました。この機能強化以前は、タスクリスト内の先行タスク関係のみ、またはタスクレベルで削除することができました。

ガントチャートの編集について詳しくは、[タスクリストのガントチャートの情報を更新](../../../../manage-work/gantt-chart/use-the-gantt-chart/update-info-task-list-gantt.md)を参照してください。

## リソースプランナーの改善点 {#resource-planner-improvements}

* [リソースプランナーに期間ゼロの予算](#budget-with-zero-duration-in-the-resource-planner)

* [リソースプランナーにコスト別のデータを表示する](#show-data-by-cost-in-the-resource-planner)

### リソースプランナーに期間ゼロの予算 {#budget-with-zero-duration-in-the-resource-planner}

>[!NOTE]
>
>この機能はプレビュー環境から削除され、18.1 リリースでリリースされます。

プロジェクトの期間内または期間外にかかわらず、リソースプランナーでリソースの予算を任意の日付に設定できるようになりました。この機能強化以前は、プロジェクトの期間内の日付に対してのみリソースの予算を設定することができました。

リソースプランナーのリソースの予算設定について詳しくは、[リソースプランナーの概要](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)の「リソースプランナーのリソースの予算設定」の節を参照してください。

### リソースプランナーにコスト別のデータを表示する {#show-data-by-cost-in-the-resource-planner}

時間と FTE の値に加えて、リソースプランナーにコスト別の情報を表示できるようになりました。「プロジェクト別に表示」ビューまたは「役割別に表示」ビューで表示する場合は、リソースプランナーにコストを表示できます。「ユーザー別に表示」ビューでリソースプランナーを表示している場合は、コストを表示できません。

時間、FTE、または原価の値別のリソースプランナーの表示について詳しくは、[リソースプランナーのナビゲーションの概要](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md)を参照してください。
