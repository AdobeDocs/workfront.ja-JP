---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 ベータ 5 リリースアクティビティ
description: このページでは、2018.2 ベータ 5 リリースでのプレビュー環境で最近行われたすべての変更点について説明します。この機能は、2018年6月1日（PT）にプレビュー環境で使用できるようになります。ベータ 5 でリリースされるプルーフの機能強化は、6月4日月曜日（PT）にプレビュー環境で利用できるようになります。2018年7月に、実稼動環境で利用可能になる予定です。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 0a8602aa-34c8-44d0-a102-9497d106f806
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '3158'
ht-degree: 100%

---

# 2018.2 ベータ 5 リリースアクティビティ

このページでは、2018.2 ベータ 5 リリースでのプレビュー環境で最近行われたすべての変更点について説明します。この機能は、2018年6月1日（PT）にプレビュー環境で使用できるようになります。ベータ 5 でリリースされるプルーフの機能強化は、6月4日月曜日（PT）にプレビュー環境で利用できるようになります。2018年7月に、実稼動環境で利用可能になる予定です。

>[!IMPORTANT]
>
>このページで説明する機能は、実稼動環境で使用可能になる前に変更される場合があります。

2018.2 で行われたすべての変更のリストについては、[2018.2 リリースアクティビティの概要](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md) を参照してください。

2018.2 ベータ 5 リリースには、Workfront 管理者およびその他のユーザー向けの機能強化が含まれています。

**管理者向け**

* [監査ログを使用してユーザーがトリガーした変更を表示](#view-user-triggered-changes-with-audit-logs)
* [グループ管理者としてライセンス情報を表示](#view-license-information-as-a-group-administrator)

**すべてのユーザー向け**

* [ホームエリアのカレンダー表示](#calendar-view-in-the-home-area)
* [ホームの作業リスト（左側のパネル）の追加更新](#additional-updates-to-the-work-list-left-panel-in-home)
* [自動リソーススケジュール用の担当業務制限を設定](#configure-job-role-limits-for-automated-resource-scheduling)
* [リソースプランナーでのプロジェクトおよび役割表示の改善](#project-and-role-view-improvements-in-the-resource-planner)
* [プロジェクトリストの列幅のサイズ変更](#resize-column-widths-for-project-lists)
* [新規プロジェクトリストのアイコンサポート](#icon-support-for-the-new-project-lists)
* [ドキュメント表示に「大きいサムネール」フィールドを追加](#add-large-thumbnail-field-in-document-views)
* [Excel 書き出し制限の増加](#increase-excel-export-limit)
* [プロジェクトリストのクイックフィルター](#quick-filters-for-project-lists)
* [プロジェクトおよびタスクレポートでイシューのコレクションを参照](#reference-issue-collections-in-project-and-task-reports)
* [Workfront で新しいドキュメントバージョンを追加する際の、より強固な新しいバージョンメニュー](#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront)
* [Android ベータ版モバイルアプリのモバイル機能の改善](#mobile-improvements-in-the-android-beta-mobile-app)
* [プルーフビューアーの機能強化（Workfront および Workfront Proof）](#proofing-viewer-enhancements-workfront-and-workfront-proof)
* [Workfront でのプルーフ強化](#proofing-enhancements-in-workfront)
* [Workfront Proof でのプルーフの機能強化](#proofing-enhancements-in-workfront-proof)

## ホームエリアのカレンダー表示 {#calendar-view-in-the-home-area}

Workfront ホームカレンダービューを使用して、個人の作業タスクとスケジュールを管理できるようになりました。ホームのカレンダービューでは、次の操作を実行できます。

* 自分に割り当てられた Workfront タスクを実行するための独自のスケジュールを設定する
* 期限が近づいているタスク、または期限を過ぎているタスクをすぐに確認する
* 1 週間の割り当て時間数の合計を表示する
* 割り当てられたタスクを更新する

Outlook でカレンダーを使用する場合は、カレンダーを統合して、Outlook イベントをホームのカレンダービューに表示できます。

## ホームの作業リスト（左側のパネル）の追加更新 {#additional-updates-to-the-work-list-left-panel-in-home}

ホームエリアの作業リストで次の機能強化が利用できるようになりました。

* 完了した項目の数が、「フィルター」ドロップダウンメニューの「完了」オプションの横に括弧で囲んで表示されるようになりました。

  以前は、完了した項目の数がフィルターメニューに表示されませんでした。 

* 過去 2 週間の完了した項目が表示されます。

  以前は、過去 3 か月間の完了した項目が表示されていました。

  ホームエリアでの完了作業の表示について詳しくは、[ホームエリアの作業リストに項目を表示する](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)の記事の[ホームエリアの作業リストに項目を表示する](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)を参照してください。

* ホームエリアで項目を選択した際に表示する「期間」フィールドと「割り当て」フィールドを追加。

  以前は「割り当て」フィールドはデフォルトで使用できましたが、削除するともう一度追加することはできませんでした。「期間」フィールドは、以前は追加できませんでした。

  ホームエリアにフィールドを追加する方法について詳しくは、レイアウトテンプレートの作成と管理を参照してください。

ホームエリアの使用方法について詳しくは、[ホームエリアの使用](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md)を参照してください。

## ユーザーがトリガーした変更の監査ログでの表示 {#view-user-triggered-changes-with-audit-logs}

ユーザーがトリガーした変更を Workfront 管理者が追跡するための次の監査ログが作成されました。

* ユーザー監査ログ
* アクセスレベル監査ログ
* グループ監査ログ
* ログイン試行監査ログ

これまでは、システム内の変更を追跡する方法はありませんでした。

詳しくは、[監査ログの表示と書き出し](../../../../administration-and-setup/add-users/create-and-manage-users/view-and-export-audit-logs.md)を参照してください。

## グループ管理者としてライセンス情報を表示 {#view-license-information-as-a-group-administrator}

グループ管理者が管理下のグループのライセンス数を確認するための読み取り専用のライセンスページが作成されました。

この変更以前は、グループ管理者はライセンス情報を確認できませんでした。

詳しくは、[グループ管理者](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md)を参照してください。

## 自動リソーススケジュールを目的とする担当業務制限の設定 {#configure-job-role-limits-for-automated-resource-scheduling}

>[!NOTE]
>
>23.1 リリースで、リソーススケジュールツールは廃止され、Workfront から削除されました。ワークロードバランサーを使用したリソースのスケジュール設定については、[ワークロードバランサーの概要](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)を参照してください。

「自動リソース スケジュール」設定で、担当業務に制限を設けることができるようになりました。これにより、作業を割り当てられる同じ役割のリソースの数を制御できます。

これまでは、特定の担当業務内で作業を割り当てることができるユーザーの数を指定できませんでした。

詳しくは、「スケジュールエリアでの未割り当てタスクおよびイシューの手動割り当て」を参照してください。

## リソースプランナーのプロジェクトビューと役割ビューの改善 {#project-and-role-view-improvements-in-the-resource-planner}

リソースプランナーのプロジェクトビューと役割ビューで、次の改善を実施しました。

* 画面上の情報だけでなく、データベース全体から情報を取り込むようにフィルターを改善しました。
* フルスクリーンモード。
* パフォーマンスを高速化および効率化しました。

   * 表示できるプロジェクト、役割およびユーザーの数に新しく制限を設けました。
   * 遅延読み込みで、プロジェクトと役割の読み込みを速くします。

* リソースプランナーからプロジェクトとユーザーに直接クイックアクセスできます。
* プロジェクトビューでドラッグ＆ドロップ機能を高速化して、プロジェクトを優先付けします。

この改善が行われる前は、リソースプランナーの読み込みが遅く、表示されるデータに不一致が見られるとの報告がありました。上記の改善により、これらの問題は解消されたはずです。

リソースプランナーの新しい制限については、[リソースプランナーの表示制限](../../../../resource-mgmt/resource-planning/resource-planner-display-limitations.md)を参照してください。

<!--
<p dir="ltr" data-mc-conditions="QuicksilverOrClassic.Draft mode">To participate in our current beta program and give us feedback on the functionality of the Resource Planner, see <a href="../../../../product-announcements/betas/resource-planner-performance-beta.md" class="MCXref xref" xrefformat="{para}">Resource Planner performance beta </a></p>
-->

## プロジェクトリストの列幅のサイズ変更 {#resize-column-widths-for-project-lists}

リストの機能の改善が実施されていたので、次のプロジェクトリストで列の幅を変更する機能が一時的に無効になっていました。

* 所有プロジェクト
* 担当プロジェクト
* すべてのプロジェクト

このリリースで、すべてのプロジェクトリストの列のサイズを再び変更できるようになりました。

この機能に追加の改善が加えられました。

列の右の境界線をドラッグしてサイズを変更すると、右隣の列のサイズが変更されずに維持され、リストが広くなります。また、列の境界線を、隣の列の境界線より右側にドラッグすることもできます。

この改善が行われる前は、サイズを変更した列の右隣の列は、画面に収まるように比例的にサイズが変更され、列の境界線を隣の列の右側の境界線を越えてドラッグすることもできませんでした。 

リスト内の列のサイズ変更と並べ替えについては、[列の幅と順序の変更](../../../../reports-and-dashboards/reports/reporting-elements/modify-column-width-order.md)を参照してください。

現行のリスト改善を目的としたベータテストプログラムに参加するには、[新しいリストの詳細。](https://experienceleaguecommunities.adobe.com/t5/workfront/ct-p/workfront?profile.language=ja)を参照してください（ログインが必要です）。

## 新しいプロジェクトリストでのアイコンのサポート {#icon-support-for-the-new-project-lists}

リストの機能の改善が実施されていたので、次のプロジェクトリストでステータスアイコンの表示が一時的に無効になっていました。

* 所有プロジェクト
* 担当プロジェクト
* すべてのプロジェクト

このリリースで、プロジェクトリストのプロジェクトや他のオブジェクトのステータスアイコンを再びプロジェクトリストに表示できるようになりました。

リストでの作業については、[Adobe Workfront のリストの基本を学ぶ](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)を参照してください。

## ドキュメントビューへの「大きなサムネイル」フィールドの追加 {#add-large-thumbnail-field-in-document-views}

リストやレポートのドキュメントビューに、「大きなサムネイル」という新しいフィールドが追加されています。このフィールドをドキュメントビューで選択すると、ドキュメントの 400 ピクセル幅のサムネールがリストやレポートに表示されます。

この変更を行う前は、ドキュメントの 33～66 ピクセル幅のサムネールを表示する「サムネイル」フィールドのみドキュメントビューに追加できました。

リストおよびレポートのフィールドについては、[Adobe Workfront 用語集](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)を参照してください。

## Excel 書き出し上限の引き上げ {#increase-excel-export-limit}

Excel ファイルに書き出すことができる行数の上限が増えました。以下を書き出すことができるようになりました。

* Excel の .xls ファイルの 65,000 行
* Excel の .xlsx ファイルの 100,000 行

新しい上限は、Workfront から以下を書き出す際に適用されます。

* Web インターフェイスからのリストまたはレポート
* API を使用したリストまたはレポート
* スケジュール済みレポートと配信済みレポート

この改善以前は、Excel ファイルに書き出せる行は 50,000 行まででした。

Workfront からのデータの書き出しについては、[データの書き出し](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)を参照してください。

## プロジェクトリストのクイックフィルター {#quick-filters-for-project-lists}

リストにクイックフィルターを適用できるようになりました。

クイックフィルターの目的は、大きなリスト内の重要な項目に直接移動し、それらを迅速にレビュー、更新または他のユーザーと共有できるようにすることです。

現在、クイックフィルターは、次のサブタブにあるプロジェクトリストにのみ使用できます。

* 担当プロジェクト
* 所有プロジェクト
* すべてのプロジェクト

クイックフィルターについて詳しくは、[Adobe Workfront のリストの基本を学ぶ](../../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md)の「リストへのクイックフィルターの適用」の節を参照してください。

## プロジェクトレポートとタスクレポートでのイシューコレクションの参照 {#reference-issue-collections-in-project-and-task-reports}

プロジェクトビューまたはタスクビューとフィルターで、イシューのコレクションを参照できるようになりました。これは、レポートの作成時にテキストモードを使用する場合にのみ可能です。

この改善以前は、プロジェクトビューまたはフィルターでタスクのコレクションのみを参照できました。

レポートでのコレクションの参照方法については、[レポートでのコレクションの参照](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)を参照してください。

テキストモードの使用については、[テキストモードの一般的な使用の概要](../../../../reports-and-dashboards/reports/text-mode/understand-common-uses-text-mode.md)を参照してください。

>[!NOTE]
>
>次のビデオでは、イシューコレクションのサンプルテキストモードが正しくありませんでした。正しいサンプルテキストモードは、[レポートでのコレクションの参照](../../../../reports-and-dashboards/reports/text-mode/reference-collections-report.md)で紹介しています。

## Workfront で新規ドキュメントバージョンを追加する際に使用する新規バージョンメニューの堅牢性の向上 {#new-more-robust-version-menu-when-adding-new-document-versions-in-workfront}

Workfront でドキュメントに新規バージョンを追加する際に、新規バージョンメニューに追加のオプションが含まれるようになり、新規バージョンを追加できる Workfront のすべてのエリアを通して一貫性が保たれるようになりました。

新規ドキュメントバージョンは、Workfront の次のエリアから追加できます。

* 「ドキュメント」タブのその他ドロップダウンメニュー
* ドキュメントの詳細ページのドキュメント アクションメニュー。
* ドキュメントの詳細ページの「すべてのバージョン」タブ。

この変更以前は、「ドキュメント」タブのその他ドロップダウンメニューにのみ、新規バージョンを追加するためのすべてのオプションが含まれていました。

新規バージョンを追加できるすべてのエリアの新規バージョンメニューで、次のオプションが使用できるようになりました。

* プルーフ
* ドキュメントのみ
* 「リンク元」オプション（「Dropboxから」、「Google Driveから」など）
* クリップボードから貼り付け（バージョンを追加する際の新しいオプションです）

詳しくは、[ファイルシステムから Adobe Workfront へのドキュメントの追加](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)の記事の[ファイルシステムから Adobe Workfront へのドキュメントの追加](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)を参照してください。

## Android ベータ版モバイルアプリのモバイル機能の改善 {#mobile-improvements-in-the-android-beta-mobile-app}

このリリース日の後すぐに、次の機能強化がモバイルアプリの Android ベータ版で利用可能になります。

* スワイプアクション

  Workfront モバイルアプリで様々なオブジェクトをスワイプすることで、自発的にタスクに取り組む、タスクを完了する、通知を既読または新規としてマークする、連絡先にテキストメッセージを送信したり電話をかけたりするといったアクティビティを実行できます。

  この機能により、次のエリアが改善されました。

   * 担当作業とホーム
   * 通知
   * 連絡先
   * 承認

* 項目の「詳細」タブを表示する際の新しいルックアンドフィール

  モバイルアプリの Android ベータ版で項目を表示する際のインターフェイスが変更されて、編集、完了またはドキュメントの添付が容易になりました。

* 時間を記録する際の新しいエクスペリエンス

  アクセスしやすくなった「時間を記録」ボタンと、時間数を記録するためのより効率化されたインターフェイスにより、時間の記録が以前よりも迅速かつ簡単になりました。

このリリースでは、Workfront モバイルアプリの Android ベータ版でのみ、これらの機能強化が利用可能です。現在、iOS では利用できません。

ベータ版テスターに新規登録して、Workfront モバイルアプリの Android ベータ版をダウンロードする方法について詳しくは、以下を参照してください。

## プルーフビューアの機能強化（Workfront および Workfront Proof） {#proofing-viewer-enhancements-workfront-and-workfront-proof}

* [概要の印刷ページを更新](#updated-print-summary-page)
* [プルーフビューアからプルーフにユーザーを直接追加](#add-users-to-a-proof-directly-from-the-proofing-viewer)
* [プルーフビューアですべてのマークアップツールを表示](#display-all-markup-tools-in-the-proofing-viewer)
* [プルーフビューアでデフォルトの並べ替えオプションを設定](#configure-default-sorting-options-in-the-proofing-viewer)
* [デスクトッププルーフビューアで Workfront ドキュメント承認を表示](#view-workfront-document-approvals-in-the-desktop-proofing-viewer)
* [新しいタブやウィンドウで開かれるリンクをデスクトッププルーフビューア内で開くように設定](#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer)
* [プルーフビューアのプレゼンスインジケーター](#presence-indicator-in-the-proofing-viewer)
* [コメントをフィルタリングしてインタラクティブ URL プルーフの単一ページをデスクトッププルーフビューアに表示](#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer)
* [静的コンテンツとビデオコンテンツのためのデスクトッププルーフビューア](#desktop-proofing-viewer-for-static-and-video-content)
* [システムへのカスタムデバイスの追加](#add-custom-devices-to-your-system)

### 概要の印刷ページを更新 {#updated-print-summary-page}

概要の印刷ページが更新されて、ルックアンドフィールが新しくなり、機能が向上しました。

詳しくは、[Adobe Workfront 内でのプルーフ概要の印刷](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/print-proof-summary-in-wf.md)を参照してください。

### プルーフビューアからプルーフにユーザーを直接追加 {#add-users-to-a-proof-directly-from-the-proofing-viewer}

Web プルーフビューアとデスクトッププルーフビューアからプルーフにユーザーを直接追加できるようになりました。 

以前は、個々のユーザーをプルーフに追加できませんでした。正確には、パブリック URL または埋め込みコードのみをコピーできました。

詳しくは、[プルーフビューアからのプルーフの共有](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md)の記事の[プルーフへのユーザーの追加によるプルーフの共有](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/share-a-proof-in-proofing-viewer.md#sharing-with-individual-users)を参照してください。

### プルーフビューアですべてのマークアップツールを表示 {#display-all-markup-tools-in-the-proofing-viewer}

メニューを開かなくても常にマークアップツールが表示されるように設定できるようになりました。これにより、ツールの切り替えが速くなります。このように設定すると、マークアップツールは web プルーフビューアとデスクトッププルーフビューアの上部に横に並んで表示されます。

以前は、マークアップツールはドロップダウンメニューでのみ使用可能でした。

このマークアップ設定について詳しくは、[プルーフビューアの設定](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md)を参照してください。

プルーフのレビュー時にマークアップオプションを使用する方法について詳しくは、次の記事を参照してください。

### プルーフビューアでデフォルトの並べ替えオプションを設定 {#configure-default-sorting-options-in-the-proofing-viewer}

プルーフのコメントリスト内で並べ替えオプションを変更すると、web プルーフビューアまたはデスクトッププルーフビューア内で次にプルーフを開いたときに、そのオプションがデフォルトの並べ替えオプションになります。 

詳しくは、次の記事を参照してください。

### Workfront ドキュメントの承認を Desktop のプルーフビューアーで表示 {#view-workfront-document-approvals-in-the-desktop-proofing-viewer}

Workfront ドキュメントの承認を Desktop のプルーフビューアーで行えるようになります。

以前は、Workfront ドキュメントの承認は、web のプルーフビューアーでしか実行できませんでした。 

詳しくは、[プルーフビューアーでプルーフを決定する](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)の記事の[プルーフビューアーでプルーフを決定する](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)を参照してください。

### 新しいタブとウィンドウが Desktop のプルーフビューアー内で開くようにリンクを設定する {#configure-links-that-open-new-tabs-and-windows-to-open-within-the-desktop-proofing-viewer}

Desktop のプルーフビューアーでインタラクティブコンテンツのプルーフを行う際に、Desktop のプルーフビューアーの新しいタブまたは新しいウィンドウでリンクが開くように設定して、プルーフを続行できるようになりました。

以前のプルーフビューアーでは、新しいタブや新しいウィンドウで開いたリンクを確認できませんでした。

詳しくは、[プルーフビューアーの設定](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md)を参照してください。

### プルーフビューアーのプレゼンスインジケーター {#presence-indicator-in-the-proofing-viewer}

Web のプルーフビューアーまたは Desktop のプルーフビューアーでプルーフを確認する際に、そのプルーフを現在閲覧している各ユーザーのアバターがプルーフビューアーの右上隅に表示されるようになりました。

詳しくは、[複数のレビュアーによるプルーフの同時レビュー](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/review-proof-with-multiple-reviewers.md)を参照してください。

### Desktop のプルーフビューアーでコメントをフィルターしてインタラクティブ URL プルーフ用の単一ページを表示 {#filter-comments-to-display-a-single-page-for-interactive-url-proofs-in-the-desktop-proofing-viewer}

Desktop のプルーフビューアーでインタラクティブプルーフの URL をレビューする際に、コメントをフィルタリングして現在のページに対するコメントのみを表示できるようになりました。 

この変更が行われる前は、このオプションは静的プルーフでのみ使用できました。

詳しくは、記事を参照してください。

### 静的コンテンツとビデオコンテンツのための Desktop のプルーフビューアー {#desktop-proofing-viewer-for-static-and-video-content}

Desktop のプルーフビューアーで静的コンテンツとビデオコンテンツがサポートされるようになりました。

以前は、インタラクティブコンテンツのみがサポートされていました。

Desktop のプルーフビューアーで静的なプルーフとビデオのプルーフを開く設定について詳しくは、[プルーフビューアーの設定](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md)を参照してください。

デスクトッププルーフビューアーについて詳しくは、[デスクトッププルーフビューアーでプルーフをレビュー](https://support.workfront.com/hc/en-us/sections/360000686434)を参照してください。

### システムにカスタムデバイスを追加する {#add-custom-devices-to-your-system}

これで、任意のカスタムデバイスをシステムに追加でき、ユーザーがデスクトッププルーフビューアーでプルーフをレビューする際に、インタラクティブなコンテンツをレビューし、特定のデバイスでの表示をシミュレートできます。

この変更以前は、ユーザーは標準の事前設定済みデバイスのリストからのみ選択できました。

カスタムデバイスの追加について詳しくは、

インタラクティブなコンテンツをレビューする際にユーザーがデバイスを選択する方法について詳しくは、[プルーフプルーフビューアーでインタラクティブなプルーフの解像度を変更](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md)を参照してください。

## Workfront でのプルーフの機能強化 {#proofing-enhancements-in-workfront}

* [Workfront から直接プルーフリンクを共有](#share-the-proof-link-directly-from-workfront)
* [Workfront で追加のプルーフデータをレポート](#report-on-additional-proofing-data-in-workfront)
* [Workfront でプルーフの承認の履歴データを表示する](#view-historical-data-for-proof-approvals-in-workfront)

### Workfront から直接プルーフリンクを共有する {#share-the-proof-link-directly-from-workfront}

Workfront 内でプルーフのリンクを生成し、Workfront から直接共有できるようになりました。または、URL をコピーし、別の方法を使用して配布できます。

この変更以前は、Workfront 内でプルーフのリンクをコピーし、別の方法を使用して配布することしかできませんでした。

詳しくは、[Adobe Workfront 内でプルーフを共有](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)の記事の [Adobe Workfront 内でプルーフを共有](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)を参照してください。

>[!NOTE]
>
>現在使用可能な埋め込みリンクは、将来のリリースで削除されます。埋め込みリンクには、引き続き Workfront API 経由でアクセスできます。

### Workfront で追加のプルーフデータをレポートする {#report-on-additional-proofing-data-in-workfront}

ドキュメントのバージョンオブジェクトを含むレポート（ドキュメントのバージョンレポートやプルーフの承認レポートなど）で、追加のプルーフ情報を表示できる複数のフィールドが使用可能になりました。

* プルーフの期限

  プルーフ期限の曜日、日付、時刻、および年を表示します。

* プルーフ決定

  プルーフの決定ステータスを表示します（保留、変更が必要、承認済み）。

* プルーフ名

  プルーフ名を表示します。

* プルーフページ

  プルーフに含まれるページ数を表示します。

* プルーフの進捗状態

  プルーフの進捗ステータスを表示します（送信済み、開封済み、コメント済み、決定済み）。

これらの各フィールドについて詳しくは、[Adobe Workfront の用語集](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)を参照してください。

### Workfront でプルーフの承認の履歴データを表示する {#view-historical-data-for-proof-approvals-in-workfront}

プルーフの承認レポートで、アクティブでなくなったプルーフの承認に関する決定を表示できるフィールドを追加できます。これを行うには、「承認者の決定」フィールドをレポートに追加します。

この変更以前は、プルーフに対する決定が行われると、その決定を Workfront レポートに表示できなくなっていました。

詳しくは、[Adobe Workfront の用語集](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)を参照してください。

## Workfront Proof でのプルーフの機能強化 {#proofing-enhancements-in-workfront-proof}

* [プルーフビューアーから直接新しいバージョンのプルーフを作成（Workfront Proof）](#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof)
* [プルーフビューアーおよびデスクトッププルーフビューアーでの新しいプルーフの詳細リンク（Workfront Proof）](#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof)

### プルーフビューアーから直接新しいバージョンのプルーフを作成（Workfront Proof） {#create-a-new-version-of-a-proof-directly-from-the-proofing-viewer-workfront-proof}

Workfront Proof 内でのプルーフ時に、新しいプルーフビューアーとデスクトップのプルーフビューアーから、新しいバージョンのプルーフを直接作成できるようになりました。

以前は、このオプションはレガシー Flash ビューアー内でのみ使用できました。

詳しくは、[Workfront Proof でプルーフをコピー](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md)の記事の [Workfront Proof でプルーフをコピー](../../../../workfront-proof/wp-work-proofsfiles/create-proofs-and-files/copy-proofs.md)を参照してください。

### プルーフビューアーおよびデスクトッププルーフビューアーでの新しいプルーフの詳細リンク（Workfront Proof） {#new-proof-details-link-in-the-proofing-viewer-and-desktop-proofing-viewer-workfront-proof}

プルーフビューアーでプルーフを表示するときに、Workfront Proof ユーザーは、Workfront Proof 内のプルーフの詳細ページにすぐに移動できるようになりました。

詳しくは、「プルーフの詳細の表示」を参照してください。
