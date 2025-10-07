---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2017.3 ベータ版最終リリースアクティビティ
description: このページでは、2017.3 ベータ版最終リリースでプレビュー環境で最近利用可能となったすべての変更について説明します。このページの機能は、2017年9月12日（PT）にプレビュー環境で使用できるようになりました。2017年11月初旬に、実稼動環境で利用可能になる予定です。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 880828f4-3908-4ef0-ab1f-774f8dee72b6
source-git-commit: f5044d457ebf203269e8007075e98ba4c136660f
workflow-type: tm+mt
source-wordcount: '3791'
ht-degree: 100%

---

# 2017.3 ベータ版最終リリースアクティビティ

このページでは、2017.3 ベータ版最終リリースでプレビュー環境で最近利用可能となったすべての変更について説明します。このページの機能は、2017年9月12日（PT）にプレビュー環境で使用できるようになりました。2017年11月初旬に、実稼動環境で利用可能になる予定です。

>[!IMPORTANT]
>
>このページで説明する機能は、実稼動環境で使用可能になる前に変更される場合があります。

2017年3月に行われたすべての変更のリストについては、[2017.3 リリースアクティビティの概要](../../../../product-announcements/product-releases/quarterly-release-archive/2017.3-release-activity/2017-3-release-activity-overview.md)を参照してください。

2017.3 ベータ版最終リリースには、Workfront 管理者およびその他のユーザー向けの機能強化が含まれています。

**管理者向け**

* [承認設定エリアでのリクエストの取り消しの新しい設定](#new-configuration-for-recalling-requests-in-the-approval-settings-area)
* [デフォルトのプルーフの役割の設定](#configure-default-proof-roles)

**すべてのユーザー向け**

* [ホームエリア（作業エリアのアップデート）](#home-area-updated-my-work-area)

* [ホームエリアをサポートするようにレイアウトテンプレートをアップデートしました](#updated-layout-template-to-support-the-home-area)

* [アジャイルのかんばん](#kanban-for-agile)
* [アジャイルチームのスクラムバックログに問題を含める](#include-issues-on-the-scrum-backlog-for-an-agile-team)
* [スクラムアジャイルストーリーボードに問題を追加](#include-issues-on-the-scrum-agile-story-board)
* [アジャイルチームのバックログへのグループ化とフィルターの適用](#apply-groupings-and-filters-to-the-backlog-for-an-agile-team)
* [プレビュー環境の強化された @ タグ機能の復活](#enhanced-tagging-functionality-returns-in-the-preview-environment)
* [更新ストリーム内のフィルターシステムの更新が、オブジェクト間で保持されるようになりました](#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects)
* [稼働率レポートでのデータの視覚化](#visualize-data-in-the-utilization-report)
* [稼働率レポートのパフォーマンス向上](#utilization-report-performance-improvement)
* [ドキュメントの機能強化：合理化されたインターフェイス](#document-enhancements-streamlined-interface)
* [Workfront 内でのプルーフ機能の強化](#proofing-enhancements-within-workfront)
* [Workfront Proof と Workfront の両方で強化されたプルーフ機能](#proofing-enhancements-within-both-workfront-proof-and-workfront)
* [更新やメールのリッチテキスト書式](#rich-text-formatting-for-updates-and-emails)
* [新しいガントチャートのデザイン変更](#new-gantt-chart-redesign)
* [ビルトインのレポートの説明が更新されました](#built-in-reports-contain-updated-descriptions)
* [書き出されたレポート、リストおよびダッシュボードのブランディング](#branding-in-exported-reports-lists-and-dashboards)
* [タスクのコピー、タスクまたは問題を移動する際の改善点](#improvements-when-copying-tasks-and-moving-tasks-or-issues)
* [リソース予算計上時間数レポートの新しいグループ化：配分日](#new-grouping-for-resource-budgeted-hour-reports-allocation-date)
* [リソースプランナーの機能強化](#resource-planner-improvements)
* [モバイル機能の強化](#mobile-improvements)
* [Workfront と Slack の統合](#workfront-integration-with-slack)
* [Outlook 365 の改善点](#outlook-365-improvements)
* [API の変更点](#api-changes)

## ホームエリア（作業エリアのアップデート） {#home-area-updated-my-work-area}

>[!NOTE]
>
>この機能は、17.3 リリースで実稼動環境にはリリースされません。2018年初めまでプレビュー環境に残ります。

新しいホームエリアは、担当作業エリアで現在使用可能な同じデータに対して、代替の拡張ビューを提供します。ホームエリアは、担当作業エリアにおいて次のようなメリットがあります。

* より合理化された直感的なインターフェイス
* パフォーマンスの向上

次の機能は、担当作業エリアで使用できますが、ホームエリアにはまだ実装されていません。

* 個人用カレンダーを表示
* リッチテキストの書式設定を使用したタスクと問題の更新
* プルーフの承認
* 承認用に送信した作業のリストを表示
* プロジェクトに関するアドホックイシューを作成
* 自分に委任された承認のみを表示

新しいホームエリアの使用について詳しくは、[ホームエリアの使用](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md)を参照してください。

## ホームエリアをサポートするようにレイアウトテンプレートを更新 {#updated-layout-template-to-support-the-home-area}

>[!NOTE]
>
>この機能は、17.3 リリースで実稼動環境にはリリースされません。2018年初めまでプレビュー環境に残ります。

Workfront 管理者は、組織内のユーザーに割り当てられたレイアウトテンプレートを設定することで、ユーザーがホームエリアにアクセスできるかどうかを決定できます。レイアウトテンプレートを割り当てられていないユーザーは、常にホームエリアにアクセスできます。

詳しくは、「レイアウトテンプレートの作成と管理」の「ホームのカスタマイズ」を参照してください。

## アジャイル用のかんばん {#kanban-for-agile}

アジャイルチームは、既にサポートされているスクラムアジャイル方法論に加えて、かんばん方法論を Workfront 内で使用できるようになりました。

Workfront のスクラムアジャイル方法論とかんばんアジャイル方法論は、次の点で異なります。

**Workfront でかんばんを使用するメリット**

* かんばんアジャイルストーリーボードにバックログを表示できます。

  詳細情報は、次を参照してください。

* 完了と見なされるステータスに他のアイテムが移行したときに自動的にかんばんアジャイルストーリーボードに追加されるように、バックログのアイテムを設定できます。

  詳しくは、[かんばんの設定](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md)の[バックログから自動的に追加されるようにストーリーを設定](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur5)を参照してください。

* 進行中の作業 (WIP) の上限がかんばんアジャイルストーリーボードに表示されるように設定できます。

  詳しくは、[かんばんの設定](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md)の[進行中の作業 (WIP) の上限の設定](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4)を参照してください。

**Workfront でスクラムを使用するメリット**

* 一連のストーリーをアジャイルイテレーションに追加し、そのイテレーションのストーリーボードを作成できます。
* スクラムストーリーボードにイシューを追加できます。
* アジャイルチームのバックログにイシューを含めることができます。

  詳しくは、[スクラムの設定](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)の[作業アイテムをイテレーションに追加する際の日付の適用方法の設定](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5)を参照してください。

* サブタスクをスクラムストーリーボードに表示できます。
* バーンダウンチャートを表示して、イテレーション中のストーリーに対する進捗を確認できます。

  詳しくは、[アジャイルバーンダウンチャートの概要](../../../../agile/use-scrum-in-an-agile-team/burndown/burndown-chart-overview.md)を参照してください。

アジャイルチームのかんばんの有効化と設定について詳しくは、[アジャイルチームの作成](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md)の[アジャイル方法論の決定](../../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md#deciding)を参照してください。

## アジャイルチームのスクラムバックログにイシューを含める {#include-issues-on-the-scrum-backlog-for-an-agile-team}

>[!NOTE]
>
>この機能は、2017年11月14日（PT）に実稼動環境から削除されました。デザインを強化し安定性を向上させたうえで、2018年初めにプレビュー環境に再導入される予定です。2018.1 リリースで実稼動環境において使用できるようになります。

スクラムアジャイル方法論を使用する場合、アジャイルチームのバックログにイシューを含めることができるようになりました（かんばん方法論を使用する場合、イシューはアジャイルチームのバックログには表示されません）。イシューを含めるには、既存のスクラムアジャイルチームがこの機能を有効にする必要があります。2017.3 リリース以降に作成されたスクラムアジャイルチームのバックログには、イシューが自動的に含まれます。

この変更以前は、バックログに追加できたのはタスクだけでした。イシューを追加する場合は、イシューを追加する前に、まずイシューをタスクに変換する必要がありました。

バックログのタスク以外にもアクセスできるようになったので、バックログでこれまで使用可能だったカスタムタスクビューはすべてコピーされ、カスタムバックログ作業アイテムビューとしてバックログに追加されます。

バックログのイシューの使用については、[アジャイルバックログの管理](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)を参照してください。

アジャイルスクラムチームのバックログでイシューを使用できるようにする方法については、[スクラムの設定](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)の[作業アイテムをイテレーションに追加する際の日付の適用方法の設定](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur5)を参照してください。

## スクラムアジャイルストーリーボードにイシューを含める {#include-issues-on-the-scrum-agile-story-board}

>[!NOTE]
>
>この機能は、2017年11月14日（PT）に実稼動環境から削除されました。デザインを強化し安定性を向上させたうえで、2018年初めにプレビュー環境に再導入される予定です。2018.1 リリースで実稼動環境において使用できるようになります。

スクラムアジャイル方法論を使用する際に、ストーリーボードにイシューを含めることができるようになりました。

詳しくは、[スクラムの設定](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)の[アジャイルストーリーボードのステータス列の設定](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configur2)を参照してください。

## アジャイルチームのバックログへのグループ化とフィルターの適用 {#apply-groupings-and-filters-to-the-backlog-for-an-agile-team}

>[!NOTE]
>
>この機能は、2017年11月14日（PT）に実稼動環境から削除されました。デザインを強化し安定性を向上させたうえで、2018年初めにプレビュー環境に再導入される予定です。2018.1 リリースで実稼動環境において使用できるようになります。

「グループ化」および「フィルター」オプションがアジャイルバックログで使用できるようになり、グループ別にバックログを整理し、特定のタスクとイシューに対するフィルターを設定できます。

この変更以前は、ビューでアジャイルバックログに適用できるようになっていました。

詳しくは、[アジャイルバックログの管理](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)の[アジャイルバックログの管理](../../../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)を参照してください。

## 更新やメールのリッチテキスト書式 {#rich-text-formatting-for-updates-and-emails}

>[!NOTE]
>
>プレビュー環境内で行った書式設定の変更は、書式未設定の状態に戻る可能性があります。

Workfront オブジェクトに対して行うコメントや更新を書式設定することで、重要な情報を強調できるようになりました。 

リッチテキストツールを使用すると、テキストに書式設定属性を適用したり、箇条書きリストや番号付きリストを作成したり、追加のリソースにハイパーリンクを追加することができます。

更新ストリーム内のコメントに適用された書式設定は、更新メール通知にも表示されます。コメントの書式設定について詳しくは、[作業の更新](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)を参照してください。

## プレビュー環境の強化された @ タグ機能の復活 {#enhanced-tagging-functionality-returns-in-the-preview-environment}

もう一度 @ 記号を使用して、プレビュー環境のすべてのオブジェクトの更新ストリームに他のユーザーにタグを付けることができます。以前は @tagging により、タグ付けされたユーザーの姓名が更新ストリームに配置されていました。現在、拡張された @tagging 機能により、ユーザーの名前（名）のみが表示されます。更新でのユーザーのタグ付けの詳細については、[更新で他のユーザーへのタグ付け](../../../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)を参照してください。

## 更新ストリーム内のフィルターシステムの更新が、オブジェクト間で保持されるようになりました {#filter-system-updates-in-the-update-stream-is-now-persistent-across-objects}

フィルターシステムの更新オプションは、Workfront サイト全体のオブジェクトにわたって永続的に使用できるようになりました。これにより、システム更新を非表示にして、1 つのオブジェクトの更新ストリーム内のユーザーコメントのみを表示し、他のオブジェクトを参照するときにその設定を維持できます。

この変更以前は、Workfront サイトを参照する際、オブジェクトごとにシステムアップデートを除外することを選択する必要がありました。

詳しくは、[作業の更新](../../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)を参照してください。

## 稼働率レポートでのデータの視覚化 {#visualize-data-in-the-utilization-report}

稼働率情報をグラフビューで表示できるようになりました。 

詳しくは、[リソース稼働率レポートの概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)の[リソース稼働率レポートの概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)を参照してください。

## 稼働率レポートのパフォーマンス向上 {#utilization-report-performance-improvement}

>[!NOTE]
>
>この機能は、ベータ版最終リリース後のパッチでリリースされました。

使用率レポートを実行すると、レポートの実行前にフィルターを適用するように求められるようになりました。この変更により、最も適切な情報が稼働率レポートにできるだけ早く生成されるようになります。

稼働率レポートの実行の詳細については、[リソース稼働率レポートの概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)の[リソース稼働率レポートの概要](../../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md)を参照してください。

## ドキュメントの機能強化：合理化されたインターフェイス {#document-enhancements-streamlined-interface}

Workfront にドキュメントを追加するためのユーザーエクスペリエンスが、より合理化され、直感的になりました。これで、ファイルシステムからドキュメントをアップロードしたり、ドキュメントをリクエストしたり、サードパーティのアプリケーション（Google や Dropboxなど）からファイルをリンクしたりできるようになりました。 

以前は、これらのオプションは、ドキュメントを追加ダイアログボックスを起動することで利用できました。 

詳しくは、以下を参照してください。

* [ファイルシステムから Adobe Workfront へのドキュメントの追加](../../../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)
* [ドキュメントのリクエスト](../../../../documents/adding-documents-to-workfront/request-a-document.md)
* [外部アプリケーションからのドキュメントのリンク](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!NOTE]
>
>この変更により、クリップボードから画像またはドキュメントを貼り付けるオプションは使用できなくなりました。

## Workfront 内でのプルーフ機能の強化 {#proofing-enhancements-within-workfront}

* [ユーザーエクスペリエンスの向上と追加機能](#improved-user-experience-and-additional-functionality)
* [プルーフビューアからの直接共有](#share-directly-from-the-proofing-viewer)
* [デフォルトのプルーフの役割の設定](#configure-default-proof-roles)

### ユーザーエクスペリエンスの向上と追加機能 {#improved-user-experience-and-additional-functionality}

Workfront でプルーフを作成する際のユーザーエクスペリエンスが向上したことに加えて、次の追加機能が利用できるようになりました。

* 複数画像を単一プルーフに結合。
* 複数の解像度で web サイトをプルーフ（複数の解像度を個別のプルーフとして作成することも、単一のプルーフに結合することもできます）。
* アップロードプロセス中にファイル名を編集。
* プルーフ作成フォームにカスタムフィールドを含める。
* プルーフメール通知にカスタムメッセージを追加します。
* 追加のプルーフの設定
* URL のプルーフ時のリアルタイムのエラー検証（以前は、エラーが表示されるまでに数分待つ必要がありました）

詳細情報は、以下を参照してください。

>[!NOTE]
>
>自動ワークフローで新しいプルーフを作成する場合、ユーザーをあるステージから別のステージに移動するためのドラッグ＆ドロップはサポートされません。代わりに、あるステップからユーザーを削除し、別のステップに追加します。

*ドラッグ＆ドロップを使用してユーザーをあるステップから別のステップに移動するオプションは、2018.1 リリースで再導入されました。*

### プルーフビューアから直接共有 {#share-directly-from-the-proofing-viewer}

これで、プルーフビューアから直接、特定の Workfront ユーザーと共有できるようになりました。

>[!NOTE]
>
>この機能は、新しいプルーフ（2017.3 リリース以降に作成されたプルーフ）でのみ、また Workfront Proof Premium アカウントと統合されている Workfront インスタンスでのみ使用できます。

この変更が行われる前は、リンクを作成してそのリンクをユーザーと共有することによってのみ共有できました。 

詳しくは、[Adobe Workfront 内でプルーフを共有する](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)の[Adobe Workfront 内でプルーフを共有する](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)を参照してください。

### デフォルトのプルーフの役割の設定 {#configure-default-proof-roles}

Workfront システム内の新しいプルーフに対して、新規ユーザーとゲストユーザーが持つデフォルトのプルーフの役割を設定できるようになりました。 

これは、プルーフを共有するときにユーザーがプルーフに対して割り当てられるデフォルトの役割です。 

## Workfront Proof と Workfront の両方で強化されたプルーフ機能 {#proofing-enhancements-within-both-workfront-proof-and-workfront}

* [HTML5 ビデオプルーフビューアーでの再開とスキップ（キーボードショートカット）](#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts)
* [HTML5 プルーフビューアーの更新](#html5-proofing-viewer-updates)

### HTML5 ビデオプルーフビューアーでの再開とスキップ（キーボードショートカット） {#restart-and-skip-in-html5-video-proofing-viewer-keyboard-shortcuts}

ビデオの HTML5 プルーフビューア内にキーボードショートカットが追加され、ビデオを最初から再開したり、ビデオの最後までスキップしたりできるようになりました。

使用可能なキーボードショートカットについて詳しくは、[Workfront プルーフのプランビューアーのキーボードショートカット](../../../../workfront-proof/wp-work-proofsfiles/review-proofs-wpv/keyboard-shortcuts.md)を参照してください。

### HTML5 プルーフビューアーの更新 {#html5-proofing-viewer-updates}

HTML5 ビューアーは静的プルーフをサポートするようになりました。

この変更が行われる前は、HTML5 ビューアーはビデオプルーフのみをサポートしていました。 

HTML ビューアーには、静的コンテンツをプルーフする際の次の新機能が含まれています。

* 単一ビューで複数のページにマークアップを含む 1 つのコメントを作成

  以前は、これは連続ビューまたは見開きビューの場合にのみ可能でした

* プルーフのサムネイルを介してプルーフを操作

   * レビュー中のプルーフの部分を簡単に識別します。これは、特にユーザーが大きな形式のプルーフ刷りや長い web ページを扱う場合、または詳細を確認するためにより大きなズームレベルが必要な場合に重要です。
   * ズームレベルの変更
   * コンテンツをパン

* 測定ツールでカスタム値を指定
* Workfront プルーフのプルーフビューアーでプルーフ内のテキストに注釈を付ける場合、テキストを太字、斜体、下線を付ける必要があることを示すオプションを含めることができます。

HTML5 ビューアーは、既存の Flash ビューアーで現在利用可能なすべての機能をまだサポートしていません。次の機能は現在利用できませんが、将来のリリースに含まれる予定です。

* リッチメディアファイルのサポート
* 比較モード（ビデオと静的）
* コメントのフィルタリング（ビデオと静的）
* ドキュメント内のハイパーリンクをレビュー（静的）
* 翻訳（ビデオと静的）
* 現在プルーフに取り組んでいるユーザーを表示するプレゼンスインジケーター
* プルーフの共有

HTML5 ビューアーでの静的プルーフについて詳しくは、次を参照してください。

Workfront プルーフの Workfront 管理者は、組織内のユーザーがビデオプルーフ用の新しい HTML5 プルーフビューアーにアクセスできるかどうかを判断できます。

## 新しいガントチャートのデザイン変更 {#new-gantt-chart-redesign}

新しいガントチャートには、次の改善点が含まれています。

* 新しいアイコンとマーカー
* 特定の時間枠をズームインおよびズームアウトする新しいオプション
* グラフのリスト部分の小さいタスクセル
* 設定、印刷、見込日への切り替えのオプションが再設計されました。

ガントチャートのオプションの設定について詳しくは、[ガントチャートでの情報の表示方法を設定する](../../../../manage-work/gantt-chart/use-the-gantt-chart/configure-info-on-gantt-chart.md)を参照してください。

## ビルトインのレポートの説明が更新されました {#built-in-reports-contain-updated-descriptions}

Workfront のシステムレポートの説明を更新し、レポートの種類と含まれるフィールドに関する情報を追加しました。 

この変更以前は、ほとんどのビルトインレポートには説明がないか、非常に限られた説明しかありませんでした。

ビルトインレポートについて詳しくは、[Adobe Workfront ビルトインレポートの使用](../../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)を参照してください。

## 書き出されたレポート、リストおよびダッシュボードのブランディング {#branding-in-exported-reports-lists-and-dashboards}

>[!NOTE]
>
>この機能は現在、プレビュー環境のすべてのクラスターで利用できるわけではありません。

Workfront でブランディングを活用している場合、グローバルナビゲーションバーで使用しているロゴが、Workfront から書き出された .pdf ファイルに含まれます。

次の .pdf ファイルには、書き出されたドキュメントに組織のロゴが含まれます。

* 書き出したリスト
* 書き出しおよび配信されたレポート
* 印刷済みダッシュボード

Workfront からのデータの書き出しに関して詳しくは、[データを書き出し](../../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md)を参照してください。

## タスクのコピー、タスクまたはイシューを移動する際の改善点 {#improvements-when-copying-tasks-and-moving-tasks-or-issues}

タスクのコピーやタスクまたはイシューの移動の方法を改善して、コピーまたは移動したタスクやイシューの親を選択しやすくしました。例えば、タスクをコピーするときに親を選択すると、親子関係を含むタスクの階層を表示したり、多数のタスクを含むプロジェクトで親を検索したりできるようになりました。

この変更以前は、**親を選択**&#x200B;手順には検索フィールドが無く、タスクの階層がタスクリストに表示されませんでした。

タスクのコピーに関して詳しくは、[タスクのコピーと複製](../../../../manage-work/tasks/manage-tasks/copy-and-duplicate-tasks.md)を参照してください。

イシューの移動に関して詳しくは、[イシューを移動](../../../../manage-work/issues/manage-issues/move-issues.md)を参照してください。

## 承認設定エリアでのリコールリクエストの新規設定 {#new-configuration-for-recalling-requests-in-the-approval-settings-area}

システムレベルの承認設定エリアに新しい設定を導入しました。これにより、Workfront 管理者は、最初のステータスが承認保留となっているイシューやリクエストを、ユーザーに取り消すことを許可するかどうかを決定できます。取り消しが許可されている場合は、イシューが削除されます。取り消しが許可されていない場合は、イシューの最初のステータスが承認待ちのときに、「取り消し」ボタンを表示することはできません。

この変更以前は、イシューの取り消しが常に許可されていました。承認が取り消されると、承認が完全にバイパスされ、イシューが最初のステータスに置かれて、承認が添付されませんでした。

承認設定に関して詳しくは、[グローバル承認設定を指定](../../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/establish-approval-settings.md)を参照してください。

>[!NOTE]
>
>この機能がリリースされると、このオプションはデフォルトで無効になります。現在、イシューの取り消しは、すべての組織に対してデフォルトで有効になっています。この機能がリリースされた場合、Workfront の管理者は、Workfront と同様の機能を維持するために、この設定を手動で有効にする必要があります。

## リソース予算計上時間数レポートの新しいグループ化：配分日 {#new-grouping-for-resource-budgeted-hour-reports-allocation-date}

リソース予算計上時間数レポートを作成する場合の、結果を配分日ごとにグループ化する機能が追加されました。

この変更以前は、レポートのビューに「配分日」を表示し、フィルターで使用できましたが、このフィールドをグループ化で使用することはできませんでした。

配分日に関して詳しくは、[Adobe Workfront の用語集](../../../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md)を参照してください。

レポートの作成に関して詳しくは、[カスタムレポートを作成](../../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。

## リソースプランナーの改善点 {#resource-planner-improvements}

* [リソースプランナー：FTE 別のデータを表示](#resource-planner-show-data-by-fte)
* [リソースプランナー：週別および四半期別のデータを表示](#resource-planner-show-data-by-week-and-quarter)
* [リソースプランナー：ユーザー別表示](#resource-planner-view-by-user)
* [リソースプランナー：プロジェクトをドラッグ＆ドロップして優先度を設定](#resource-planner-drag-and-drop-projects-to-establish-priority)
* [リソースプランナー：リソースプランナーのデータを Excel に書き出し](#resource-planner-export-the-data-in-the-resource-planner-to-excel)

### リソースプランナー：FTE 別のデータを表示 {#resource-planner-show-data-by-fte}

リソースプランナーでリソースの割り当てと空き時間を FTE ごとに表示できるようになりました。この変更以前は、値は時間単位でのみ表示できました。

リソースプランナーの使用に関して詳しくは、[リソースプランナーの概要](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)を参照してください。

### リソースプランナー：週別および四半期別のデータを表示 {#resource-planner-show-data-by-week-and-quarter}

リソースプランナーの時間枠間隔を変更して、週または四半期ごとに表示できるようになりました。この変更以前は、リソースの配分と空き時間を、月単位でのみ表示し、計上することができました。

リソースプランナーの使用に関して詳しくは、[リソースプランナーの概要](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)を参照してください。

### リソースプランナー：ユーザー別表示 {#resource-planner-view-by-user}

リソースプランナーの情報をまずユーザーごとに表示し、次にプロジェクト、役割、タスクごとに情報を表示できるようになりました。また、ユーザーに対して、計画時間数と利用可能時間数または FTE との差を表示することもできます。この変更以前は、プロジェクトと役割別にリソースプランナー情報を表示できました。

リソースプランナーの使用に関して詳しくは、[リソースプランナーの概要](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)を参照してください。

### リソースプランナー：プロジェクトをドラッグ＆ドロップして優先度を設定 {#resource-planner-drag-and-drop-projects-to-establish-priority}

目的の優先度の順序でプロジェクトをドラッグ&amp;ドロップできるようになりました。この変更以前は、手動で番号を割り当てることによってのみ、プロジェクトの優先度を確立できました。

リソースプランナーの使用に関して詳しくは、[リソースプランナーの概要](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)を参照してください。

### リソースプランナー：リソースプランナーのデータを Excel に書き出し {#resource-planner-export-the-data-in-the-resource-planner-to-excel}

リソースプランナー内の情報を Excel ファイルに書き出せるようになりました。

リソースプランナーの使用に関して詳しくは、[リソースプランナーの概要](../../../../resource-mgmt/resource-planning/get-started-resource-planner.md)を参照してください。

## モバイルの改善点 {#mobile-improvements}

Workfront モバイルアプリからプロジェクトにアクセスして管理する機能が追加されました。Workfront モバイルアプリを使用して、次の操作を実行できるようになりました。

* プロジェクトのリストへのアクセス
* プロジェクトのタスクとサブタスクのリストへのアクセス
* プロジェクトのイシューリストへアクセス
* プロジェクトへの新しいイシューの記録

この機能は、Workfront モバイルアプリのアップデート時にインストールできます。2017年11月に、Appleと Android の両方のモバイルストアでアップデートを利用できるようになります。

## Workfront と Slack の統合 {#workfront-integration-with-slack}

>[!NOTE]
>
>Slack 統合は現在使用できません。2017年11月に、実稼動環境で使用できるようになります。

Workfront と Slack の新しい統合を開始します。組織が既に Slack をコミュニケーションに使用している場合、Workfront と統合して、Slack のコミュニケーションチャネルを離れることなく、共通の Workfront アクションを実行できるようになりました。次の操作を Slack アカウントから実行できるようになりました。

* Workfront で項目を検索
* 作業および承認リストへのアクセス
* タスクを作成
* イシューを作成
* 自分と共有されているリンクから任意の項目を購読
* 自分と共有されているリンクからタスクやイシューを割り当てる
* 作業の承認
* お気に入りおよび最近使用した項目のリストへアクセス

Slack から Workfront へのアクセスについて詳しくは、[Workfront の Slack での使用](https://support.workfront.com/hc/ja-jp/sections/115000458033)を参照してください。

## Outlook 365 の改善点 {#outlook-365-improvements}

Outlook 365 用 Workfront アドインに対して、次の機能が強化されました。

* Workfront のプロジェクトへのタスクまたはイシューの追加：Outlook 365 アドインを使用して、Workfront でメールをタスクまたはイシューに変換できるようになりました。このプロセスでは、タスクまたはイシューを追加するプロジェクト、担当者および期限日を指定できます。この機能強化以前は、リクエストキューにリクエストを送信するか、Outlook 365 から」作業中」リストに個人のタスクを追加することのみ可能でした。 
* タスク、イシュー、またはリクエストに変換された元のメール内で Workfront オブジェクトへのリンクを保持：Outlook 365 からメールがタスク、イシュー、またはリクエストに変換されると、Outlook 365 は元のメール内で、そのメールから変換されたタスクまたはイシューへのリンクを保持します。この変更以前は、メールがタスクに変換されたか、リクエストとして送信されたかを Outlook で確認することはできませんでした。 

## API の変更点 {#api-changes}

* [API 8 が利用可能](#api-8-now-available)
* [API の削除および廃止されたバージョン](#removed-and-deprecated-versions-of-the-api)
* [2017.3 ベータ版の最終リリースアクティビティ](#updated-message-format-for-event-subscriptions)
* [配信不能メッセージに対するイベント登録再試行](#event-subscription-retries-for-undeliverable-messages)

### API 8 が利用可能 {#api-8-now-available}

Workfront API バージョン 8 が使用できるようになり、Workfront 統合のための新しいリソースと更新されたリソースを提供します。

Workfront API に加えられた変更の一覧については、[API バージョン 8 のアップデート](../../../../wf-api/api/new-api-version-8-updates.md)を参照してください。

### API の削除および廃止されたバージョン {#removed-and-deprecated-versions-of-the-api}

### イベント登録のメッセージ形式のアップデート

Workfront イベント登録 API を含む統合の役に立つ情報を提供するために、リソースに関連する新旧の値を含めることにより、サポートされるリソースのアウトバウンドメッセージの形式を変更しました。失敗を避けるために、[Event Subscription API](../../../../wf-api/general/event-subs-api.md) で説明されているように、Workfront イベント登録 API を使用する統合を新しい形式に更新する必要があります。

### 配信不能メッセージに対するイベント登録再試行 {#event-subscription-retries-for-undeliverable-messages}

Workfront イベント登録フレームワークに、顧客エンドポイントへの配信に失敗したイベントでトリガーされるアウトバウンドメッセージを処理するメカニズムが追加されました。メッセージの配信を確実に継続するために、お客様は、イベント登録からのアウトバウンドメッセージを使用するエンドポイントが正しく設定されていることを確認する必要があります。詳しくは、[イベント登録の再試行](../../../../wf-api/api/event-sub-retries.md)を参照してください。
