---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 ベータ版 4 リリースアクティビティ
description: このページでは、2018.2 Beta 4 リリースによりプレビュー環境で最近利用可能になったすべての変更について説明します。この機能は、2018年5月17日（PT）にプレビュー環境で使用できるようになります。2018年7月に、実稼動環境で利用可能になる予定です。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 4b54b9e6-d1bf-4802-9d6c-9c3d3b6a6583
source-git-commit: b18a7835c6de131c125b77c6688057638c62fa4a
workflow-type: tm+mt
source-wordcount: '1705'
ht-degree: 100%

---

# 2018.2 ベータ版 4 リリースアクティビティ

このページでは、2018.2 Beta 4 リリースによりプレビュー環境で最近利用可能になったすべての変更について説明します。この機能は、2018年5月17日（PT）にプレビュー環境で使用できるようになります。2018年7月に、実稼動環境で利用可能になる予定です。

>[!IMPORTANT]
>
>このページで説明する機能は、実稼動環境で使用可能になる前に変更される場合があります。

2018.2 で行われたすべての変更のリストについては、[2018.2 リリースアクティビティの概要](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md) を参照してください。

2018.2 Beta 4 リリースには、Workfront 管理者およびその他のユーザー向けの機能強化が含まれています。

**管理者向け**

* [システム設定：外部ページのセッション情報](#system-setting-session-information-in-external-pages)

**すべてのユーザー向け**

* [かんばんボードでの進行中の作業（WIP）の上限の機能強化](#work-in-progress-wip-limit-enhancements-on-the-kanban-board)
* [アジャイルチームのステータスを設定するためのインターフェイスの改善](#improved-interface-for-configuring-statuses-for-an-agile-team)
* [ホームエリアの作業リスト（左側のパネル）のアップデート](#updated-work-list-left-panel-in-the-home-area)
* [インタラクティブ（リッチメディア）コンテンツのプルーフ用の新しいデスクトッププルーフビューア](#new-desktop-proofing-viewer-for-proofing-interactive-rich-media-content)
* [リソースプランナーへのユーザービューの書き出し](#export-the-user-view-in-the-resource-planner)
* [Google Team Drives のサポート](#support-for-google-team-drives)
* [ガントチャートの新しい書き出し制限](#new-export-limit-for-the-gantt-chart)
* [Internet Explorer または Safari の使用時に、「クリップボードから貼り付け」オプションが淡色表示に](#paste-from-clipboard-option-now-displays-as-dimmed-when-using-internet-explorer-or-safari)
* [Android 向けの新しいベータ版環境と新機能](#new-beta-environment-for-android-along-with-new-features)
* [イベント登録メッセージのフィルターの例](#examples-of-filters-for-event-subscriptions-messages)

## かんばんボードでの進行中の作業（WIP）の上限の機能強化 {#work-in-progress-wip-limit-enhancements-on-the-kanban-board}

### かんばんボードの各列で進行中の作業（WIP）の上限を設定

かんばんボードの各列で進行中の作業（WIP）の上限を設定できるようになりました。 

この変更が行われる前は、かんばんボードのすべての列に適用される WIP の上限を 1 つだけ設定できました。 

詳しくは、[かんばんの設定](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md)記事の、[進行中の作業（WIP）の上限の設定](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md#configur4)の節を参照してください。

### かんばんボードから直接進行中の作業（WIP）の上限を更新

チームに対する編集権限を持つチームメンバーは、かんばんボードから直接 WIP の上限を更新できるようになりました。

この変更が行われる前は、チーム設定エリアからのみ WIP の上限を更新できました。

詳しくは、該当する記事を参照してください。

## アジャイルチームのステータスを設定するためのインターフェイスの改善 {#improved-interface-for-configuring-statuses-for-an-agile-team}

アジャイルチームのステータスを設定するためのインターフェイスが、次の改善を加えて更新されました。

* 新しいルックアンドフィール
* ドラッグ＆ドロップでステータス列を並べ替え

詳しくは、次の記事を参照してください。

* [かんばんの設定](../../../../agile/get-started-with-agile-in-workfront/configure-kanban.md)
* [スクラムの設定](../../../../agile/get-started-with-agile-in-workfront/configure-scrum.md)

## ホームエリアの作業リスト（左側のパネル）のアップデート {#updated-work-list-left-panel-in-the-home-area}

ホームエリアの作業リストには、次の改善点が含まれています。

* 未読の項目が太字と青い点で目立つようになりました。

  ホームエリア以外で閲覧された項目は、ホームエリアで未読と表示されます。

  詳しくは、[ホームエリアの作業リストに項目を表示](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)を参照してください。

* イシューが、その横に表示されるイシューアイコンで区別されるようになりました。
* 承認が、承認タイプによって区別され、承認のタイプが表示されるようになりました。可能な承認の種類は、タスク、プロジェクト、イシュー、アクセス、ドキュメント、タイムシート、プルーフです。

  この変更以前は、承認は「承認」という単語でのみ区別されていました。

* 項目は、開始する準備ができているかどうかで識別されるようになりました。選択可能なオプションは、「開始準備完了」、「準備未完了」、「作業中」です。

  承認は常に開始できる状態なので、この情報は承認用に表示されません。

* 項目にドキュメントが添付されるたびに、項目名の下にドキュメントアイコンが表示されます。
* 作業リスト内のグループを折りたたんだり展開したりして、表示される情報をより適切に制御できるようになりました。グループは、「遅延」、「プロジェクト」、「日付」、「完了」です。

  デフォルトでは、今週セクションが展開され、その他のグループはすべて折りたたまれています。

* 「予定完了日」または「コミット日」で項目を並び替えるかどうかを選択します。
* 各グループ内の項目数が、グループ化タイトルの横に括弧で囲んで表示されるようになりました。

  この数は、「完了」グループには使用できません。

  詳しくは、[ホームエリアの作業リストでの項目の表示](../../../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md)を参照してください。

* 作業リストのサイズをドラッグ＆ドロップで変更。作業リストのサイズを変更して、画面の半分まで使用できます。設定したサイズは、次回ホームにアクセスしたときにも保持されます。

  この変更以前は、作業リストのサイズは変更できませんでした。

* リクエストの場合、リクエストを行ったユーザーのユーザーアバターが「[Approver_name] に承認を求められています」というテキストと共に表示されるようになりました。
* 新しい個人用タスクを作成する際に、「タスク」ボタンに「個人用」というラベルが付くようになりました。

  詳しくは、[ホームエリアからの作業アイテムの作成](../../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md)の[ホームエリアからの作業アイテムの作成](../../../../workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md)を参照してください。

* 遅延項目は、予定完了日から 1 時間たってから遅延として示されます。

ホームエリアの詳細については、[ホームエリアの使用](../../../../workfront-basics/using-home/using-the-home-area/use-the-home-area.md)を参照してください。

## インタラクティブ（リッチメディア）コンテンツのプルーフ用の新しいデスクトッププルーフビューア {#new-desktop-proofing-viewer-for-proofing-interactive-rich-media-content}

新しいデスクトッププルーフビューアでは、インタラクティブコンテンツのプルーフが可能です。従来のプルーフビューアや、ブラウザーで実行される新しいプルーフビューアとは異なり、デスクトッププルーフビューアは、ワークステーションで実行されるアプリケーションです。

新しいデスクトッププルーフビューアより前のバージョンでは、インタラクティブコンテンツのプルーフは従来のプルーフビューアでのみ行うことができました。 

デスクトッププルーフビューアには、従来のプルーフビューアに対して次の機能強化が含まれています。

* セキュリティで保護されていない（HTTP）サイトのレビュー

  従来のプルーフビューアでは、セキュリティで保護された（HTTPS）サイトのみを確認できました

* iFrame で保護されたサイト（iFrame 内での表示を保護されたサイト）をレビューします。

  従来のプルーフビューアでは、iFrame 内での表示を保護されたサイトのレビューをサポートしていませんでした。

* 様々なデバイス向けに事前に設定された解像度でコンテンツを表示します。例えば、様々な標準のデスクトップ解像度や、iPhone 8 などの個々のデバイスでコンテンツがどのように表示されるかを確認できます。 

デスクトッププルーフビューアのダウンロード、インストール、使用について詳しくは、次を参照してください。

デスクトッププルーフビューアと web プルーフビューアの比較情報については、[web プルーフビューアとデスクトッププルーフビューアの違いの概要](../../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md)を参照してください。

## リソースプランナーへのユーザービューの書き出し {#export-the-user-view-in-the-resource-planner}

パフォーマンス上の問題に対処するために、ユーザービューで表示する際に、リソースプランナーからのデータの書き出しを一時的に無効にしていました。このリリースでは、ユーザービューでリソースプランナーを表示する際に、データの書き出しを再び有効にしています。

Excel へのリソースプランナーデータの書き出しの詳細については、[リソースプランナーのナビゲーションの概要](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md)の「書き出しオプション」の節を参照してください。

リソースプランナーの現在のベータプログラムに参加するには、[リソースプランナーのパフォーマンス Beta](https://experienceleaguecommunities.adobe.com/t5/workfront/ct-p/workfront?profile.language=ja) を参照してください。

## システム設定：外部ページのセッション情報 {#system-setting-session-information-in-external-pages}

Workfront 管理者は、外部ページの作成時にセッション情報（セッション ID など）の使用を制限できるようになりました。

この変更が行われる前は、外部ページを作成できるユーザーは、他のサイトを Workfront ダッシュボードに埋め込む際に、任意のセッション情報を使用できました。 

Workfront でのシステム環境設定の設定について詳しくは、[システムセキュリティの環境設定の指定](../../../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)を参照してください。

## Google Team Drive のサポート {#support-for-google-team-drives}

Workfront から Google Team Drive 上のドキュメントまたはフォルダーをリンクできるようになりました。

この機能強化が行われる前は、Google My Drive 上にあるドキュメントまたはフォルダーのみをリンクすることができました。

様々なアプリケーションから Workfront へのドキュメントおよびフォルダーのリンクについて詳しくは、[外部アプリケーションからのドキュメントのリンク](../../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)を参照してください。

## ガントチャートの新しい書き出し制限 {#new-export-limit-for-the-gantt-chart}

ガントチャートで最大 500 件のタスクを書き出せるようになりました。

以前は、最大 250 件のタスクのみを書き出すことができました。

詳しくは、[ガントチャートの PDF への書き出し](../../../../manage-work/gantt-chart/use-the-gantt-chart/export-gantt-chart-to-pdf.md)を参照してください。

## Internet Explorer または Safari を使用する場合、「クリップボードから貼り付け」オプションが淡色表示 {#paste-from-clipboard-option-now-displays-as-dimmed-when-using-internet-explorer-or-safari}

Internet Explorer または Safari ブラウザーを使用する場合、「クリップボードから貼り付け」オプションが淡色表示になり、この機能では Chrome および Firefox ブラウザーのみがサポートされていることを説明するツールヒントが表示されます。

この変更以前は、Internet Explorer または Safari を使用している場合、このオプションは表示されませんでした。 

クリップボードから画像を貼り付ける方法について詳しくは、[クリップボードからの画像の貼り付け](../../../../documents/managing-documents/paste-image-clipboard.md)を参照してください。

## Android 向けの新しいベータ環境と新機能 {#new-beta-environment-for-android-along-with-new-features}

ベータ版テスターに新規登録すると、一般公開される前にチームが取り組んでいるモバイルアプリの最新の機能を体験できるようになりました。この環境は、現在、Workfront モバイルアプリで Android のデバイスのみでサポートされています。

Workfront モバイルアプリのベータ版テスターに登録する方法について詳しくは、次を参照してください。

モバイルアプリのベータ版では、次の機能強化が行われました。

* 新しいアカウントページ

  アカウント情報の表示、モバイル設定の管理、フィードバックの送信またはアカウントページからログアウトができるようになりました。

  この改善以前は、モバイルアプリでアカウント情報を表示できず、Workfront のメインメニューから設定にアクセスしたり、フィードバックを送信したり、ログアウトしていました。

* 新しいナビゲーション下部パネル

  画面の下部に、モバイルアプリのすべてのエリアが起動される、より目立つナビゲーションバーが表示されるようになりました。

  この改善以前は、Workfront のメインメニューに機能のエリアは表示されていました。Workfront のメインメニューが削除され、新しい下部ナビゲーションバーに置き換えられました。

  新しいナビゲーションバーの設定について詳しくは、次の記事のモバイルアプリの設定の節を参照してください。

* 新しい通知リストビュー

  通知リストのルックアンドフィールが改善され、通知の種類、未読か開封済みかをリスト内の通知を簡単に区別できます。

* 検索ボックスは、より目立つ位置に移動されました。

* より効率的な新しいログインエクスペリエンスに。

* 新しいチュートリアルエクスペリエンス

  新しいチュートリアルは、ユーザーが初めてログインする際に、簡単にアプリをガイドするために利用できるようになりました。このエクスペリエンス以前は、ユーザーが特定の機能エリアにアクセスした場合にのみチュートリアルが起動されるようになっていました。

## イベント登録メッセージのフィルターの例 {#examples-of-filters-for-event-subscriptions-messages}

組織に関連するメッセージのみを受け取るイベント登録をフィルタリングする方法を示すために、コードスニペットの例を使用して、エンドポイントに到達するイベントのフローをフィルタリングできます。フィルタリングの例の表示について詳しくは、[イベント登録メッセージのフィルタリング](../../../../wf-api/api/filter-event-sub-messages.md)を参照してください。
