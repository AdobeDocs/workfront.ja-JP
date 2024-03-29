---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.3 ベータ 2 リリースアクティビティ
description: このページでは、2018.3 ベータ 2 リリースでのプレビュー環境で利用可能となった最新の変更点について説明します。この機能は、2018年8月1日（PT）にプレビュー環境で利用できるようになります。ベータ 2 でリリースされるプルーフの機能強化は、7月18日水曜日（PT）にプレビュー環境で利用できるようになります。2018年11月に、実稼動環境で利用可能になる予定です。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 97945661-e97d-43c8-b564-624c4388de2f
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '908'
ht-degree: 100%

---

# 2018.3 ベータ 2 リリースアクティビティ

このページでは、2018.3 ベータ 2 リリースでのプレビュー環境で利用可能となった最新の変更点について説明します。この機能は、2018年8月1日（PT）にプレビュー環境で利用できるようになります。ベータ 2 でリリースされるプルーフの機能強化は、7月18日水曜日（PT）にプレビュー環境で利用できるようになります。2018年11月に、実稼動環境で利用可能になる予定です。

>[!NOTE]
>
>このページで説明する機能は、実稼動環境で使用可能になる前に変更される場合があります。

2018.3 で行われたすべての変更のリストについては、[2018.3 リリースアクティビティの概要](../../../../product-announcements/product-releases/quarterly-release-archive/2018.3-release-activity/2018-3-release-activity-overview.md)を参照してください。

2018.3 ベータ 2 リリースには、Workfront 管理者およびその他のユーザー向けの機能強化が含まれています。

**管理者向け**

* [グループ管理者としてユーザープロファイルのメールアドレスを更新](#update-the-email-address-in-the-user-profile-as-a-group-administrator)

**すべてのユーザー向け**

* [ホームエリアで自分に委任された承認を表示](#view-approvals-delegated-to-me-in-the-home-area)
* [特定の期間のデータをリソースプランナーに書き出し](#export-data-for-a-given-period-in-the-resource-planner)
* [ユーザーの割り当てが超過している場合、日次合計が赤色で表示されるようになりました](#daily-totals-now-display-in-red-when-the-user-is-overallocated)
* [最小化した場合、タスクとイシューはスケジュールタイムラインで非表示になります](#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized)
* [プルーフビューアーでユーザーによるコメントと返信をフィルタリング](#filter-comments-and-replies-by-user-in-the-proofing-viewer)
* [ビデオプルーフのフッテージの範囲に対するコメント](#comment-on-a-range-of-footage-in-a-video-proof)
* [プルーフビューアーでのコメントマークアップ用の新しいポリラインツール](#new-polyline-tool-for-comment-markup-in-the-proofing-viewer)
* [レポート、カレンダー、ドキュメント共有の用の Flash の削除](#flash-removal-for-report-calendar-and-document-sharing)

## グループ管理者としてユーザープロファイルのメールアドレスを更新 {#update-the-email-address-in-the-user-profile-as-a-group-administrator}

管理しているグループに属するユーザーのメールアドレスを更新できるようになりました。 

以前は、他のユーザーのメールアドレスを更新できたのは Workfront 管理者のみでした。 

詳しくは、[グループ管理者](../../../../administration-and-setup/manage-groups/group-roles/group-administrators.md)を参照してください。

## ホームエリアで自分に委任された承認を表示 {#view-approvals-delegated-to-me-in-the-home-area}

ホームエリアを使用して、自分に委任されたプロジェクト、タスクおよびイシューの承認を表示できるようになりました。

この変更以前は、委任された承認は「担当作業」エリアでのみ表示できました。

詳しくは、[承認リクエストの委任](../../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md)を参照してください。

## 特定の期間のデータをリソースプランナーに書き出し {#export-data-for-a-given-period-in-the-resource-planner}

リソースプランナーの情報を書き出す際に新しいウィンドウが表示され、書き出したファイルの特定の期間を選択できるようになりました。

この機能強化が行われるまでは、画面に表示されている情報しか書き出すことができませんでした。

リソースプランナーからのデータの書き出しについて詳しくは、[リソースプランナーのナビゲーションの概要](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md)の記事の[リソースプランナーのナビゲーションの概要](../../../../resource-mgmt/resource-planning/resource-planner-navigation.md)を参照してください。

## ユーザーの割り当てが超過している場合、日次合計が赤色で表示されるようになりました {#daily-totals-now-display-in-red-when-the-user-is-overallocated}

>[!NOTE]
>
>23.1 リリースで、リソーススケジュールツールは廃止され、Workfront から削除されました。ワークロードバランサーを使用したリソースのスケジュール設定について詳しくは、[ワークロードバランサーの概要](../../../../resource-mgmt/workload-balancer/overview-workload-balancer.md)を参照してください。

ユーザーの割り当てが超過している場合、ユーザーが割り当て超過になっている日の日次合計が赤色で表示されるようになりました。このオプションは、スケジュールタイムライン設定で「日次予定時間数の合計を表示」オプションが有効になっている場合にのみ表示されます。この機能強化が行われるまでは、ユーザーが割り当て超過になった日に赤い棒グラフインジケーターで表示されていましたが、日次合計には赤いハイライトが付いていませんでした。

ユーザー割り当てについて詳しくは、「スケジューリングエリアでユーザー割り当てを管理」を参照してください。

## 最小化した場合、タスクとイシューはスケジュールタイムラインで非表示になります {#tasks-and-issues-are-hidden-on-the-scheduling-timeline-when-minimized}

設定で「日次予定時間数の合計を表示」オプションが有効になっている場合、スケジュールタイムラインでタスクやイシューを最小化すると、ユーザーや役割ではタスクやイシューが非表示になります。未割り当て領域のタスクとイシューは、圧縮されたビューで表示されます。

以前は、タスクとイシューを最小化すると、タスクとイシューはユーザーと役割のスケジュールタイムラインに残りますが、圧縮されたビューで表示されていました。

スケジュールタイムラインでのタスクとイシューの最小化について詳しくは、「リソースのスケジュール設定の概要」を参照してください。

## プルーフビューアーでユーザーによるコメントと返信をフィルタリング {#filter-comments-and-replies-by-user-in-the-proofing-viewer}

指定したユーザーによるコメントをフィルタリングする際に、返信を含められるようになりました。これは、クライアントやプロジェクトマネージャーなど、重要なレビュアーが行ったすべてのフィードバックに焦点を当てる場合に便利です。

以前は、ユーザーによるフィルタリングは、指定したレビュアーによって作成（開始）されたコメントのみに限定されていました。

## ビデオプルーフのフッテージの範囲に対するコメント {#comment-on-a-range-of-footage-in-a-video-proof}

ビデオプルーフのフッテージの範囲に対するコメントを作成できます。これは、例えば、フッテージのセグメントを再撮影または削除する必要があることを示す場合に便利です。

以前は、ビデオタイムライン上の 1 点に対してのみコメントを作成できました。

## プルーフビューアーでのコメントマークアップ用の新しいポリラインツール {#new-polyline-tool-for-comment-markup-in-the-proofing-viewer}

これで、プルーフにコメントを追加する際に、ポリラインマークアップを使用してセグメント化された線と図形を描画できるようになりました。開いているセグメント化された線や閉じた形状を作成できます。このツールは、技術画像や建築画像などの、複雑な画像を操作する場合に特に便利です。

以前は、プルーフをマークアップしてコメントを追加する際に、長方形、直線、フリーハンドの線や形状、矢印を描画することができました。

## レポート、カレンダー、ドキュメント共有の用の Flash の削除 {#flash-removal-for-report-calendar-and-document-sharing}

Workfront の以下の共有ダイアログボックスから Flash を削除しました。

* レポート
* カレンダー
* ドキュメント

これらのオブジェクトは以前と同様に共有できますが、エクスペリエンスは Flash に依存しなくなりました。
