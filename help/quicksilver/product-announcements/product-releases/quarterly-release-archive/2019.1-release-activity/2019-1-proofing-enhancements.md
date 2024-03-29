---
content-type: release-notes
navigation-topic: 2019-1-release-activity
title: 2019.1 プルーフ機能の強化
description: ここでは、2019.1 リリースに含まれるすべてのプルーフ機能の強化について説明します。この機能は実稼動環境で使用できるようになっています。
author: Luke
feature: Product Announcements, Workfront Proof
recommendations: noDisplay, noCatalog
exl-id: 6b9b847c-dfb5-4285-b8fc-72f33c6a54d0
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '879'
ht-degree: 100%

---

# 2019.1 プルーフ機能の強化

ここでは、2019.1 リリースに含まれるすべてのプルーフ機能の強化について説明します。この機能は実稼動環境で使用できるようになっています。

2019.1 でのすべての変更のリストについては、[2019.1 リリースアクティビティの概要](../../../../product-announcements/product-releases/quarterly-release-archive/2019.1-release-activity/2019-1-release-activity-overview.md)を参照してください。

## 管理者向け

* [プルーフを開く受信者以外のユーザーに対する既定のプルーフの役割の設定](#configure-default-proofing-role-for-non-recipients-who-open-a-proof)

## すべてのユーザー

* [Web プルーフビューアでのインタラクティブコンテンツのプルーフ](#proof-interactive-content-in-the-web-proofing-viewer)
* [プルーフビューアでのコメントのデフォルトの並べ替え順が、最も古いものから並ぶようになりました](#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest)
* [ビデオの範囲に関連付けられたプルーフビューアでのコメントのレビュー機能の強化](#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video)
* [プルーフ通知またはプルーフビューアからドキュメントの詳細へのリンク](#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer)
* [プルーフビューアでのメール通知の変更](#change-your-email-notifications-in-the-proofing-viewer)
* [デスクトッププルーフビューアでの背景色の変更](#change-the-background-color-in-the-desktop-proofing-viewer)
* [デスクトッププルーフビューアでのプルーフからキャッシュされたブラウザデータの消去](#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer)

## プルーフを開く受信者以外のユーザーに対する既定のプルーフの役割の設定 {#configure-default-proofing-role-for-non-recipients-who-open-a-proof}

Workfront 管理者は、プルーフのワークフローで受信者が指定されていないが、Workfront オブジェクト（プロジェクト、タスクまたは問題など）を介してプルーフにアクセスできるユーザーに対して、デフォルトのプルーフの役割を設定できるようになりました。

以前は、ユーザーとゲストがワークフローに追加されずにプルーフにアクセスできた場合、デフォルトのプルーフの役割はレビュアーでした。

この機能は、Workfront で作成されたプルーフにのみ適用され、Workfront Proof には適用されません。

## Web プルーフビューアでのインタラクティブコンテンツのプルーフ {#proof-interactive-content-in-the-web-proofing-viewer}

組織のセキュリティポリシーでスタンドアロンのデスクトッププルーフビューアアプリの使用が許可されていない場合、Workfront 管理者は web プルーフビューアでインタラクティブコンテンツを有効にできます。プルーフを作成する前に、コンテンツを ZIP ファイルにバンドルする必要があります。

詳しくは、記事を参照してください。

ビデオ

## プルーフビューアでのコメントのデフォルトの並べ替え順が、最も古いものから並ぶようになりました  {#default-sorting-order-for-comments-in-the-proofing-viewer-is-now-oldest-to-latest}

プルーフビューアでは、プルーフに対するコメントのデフォルトの並べ替え順が、口頭での会話と同様に、最も古いものから順番に並ぶようになりました。

以前は、デフォルトの並べ替え順は最も新しいものから並んでいました。

別の並べ替えオプションを選択すると、他のプルーフを開いたときにも選択したオプションが記憶されています。

詳しくは、記事の該当する節を参照してください。

## ビデオの範囲に関連付けられたプルーフビューアでのコメントのレビュー機能の強化 {#enhanced-reviewing-for-comments-in-the-proofing-viewer-associated-with-a-range-of-video}

プルーフビューアで、ビデオフッテージの範囲に関連するコメントを確認する際に、「再生」をクリックすると、フッテージの範囲全体を表示できます。範囲の終わりに達すると、再生が一時停止します。コメントは開いたままなので、現在の作業中の場所がわからなくなってしまうことはありません。

以前は、ビデオフッテージの範囲のコメントを開いた場合、「再生」をクリックする前に、コメントに表示されるフレーム番号を見つけて、範囲の先頭を手動で見つける必要がありました。そうしないと、ビデオタイムライン内で最後にクリックした場所でプルーフビューアが再生を開始し、範囲の最後で一時停止しませんでした。また、「再生」をクリックするとコメントが折りたたまれるために、どのコメントをレビューしているかがわからなくなってしまうことがありました。

ビデオのプルーフのレビューについて詳しくは、次を参照してください。

ビデオ

## プルーフ通知またはプルーフビューアからドキュメントの詳細へのリンク {#link-to-document-details-from-a-proof-notification-or-the-proofing-viewer}

プルーフのレビューを促すメールを受信する際、またはプルーフビューアでプルーフを確認する際に、プルーフのドキュメントの詳細ページにすばやくアクセスできるようになりました。このページでは、プルーフに関連付けられた Workfront オブジェクト（タスク、プロジェクトまたは問題など）を表示できます。これは、プルーフで実行する必要がある作業を理解するのに役立つコンテキストを提供します。

この機能は、システムに追加した新規ユーザーに対してのみ機能する場合があります。この問題は一時的なものです。

詳しくは、記事を参照してください。

ビデオ

## プルーフビューアでのメール通知の変更 {#change-your-email-notifications-in-the-proofing-viewer}

すべてのプルーフレビュアーが、プルーフに対してどのプルーフ通知を受け取るかを指定できるようになりました。これは、外部の関係者と協力する際に特に重要です。

以前は、プルーフ所有者またはトラフィックマネージャーのみが、プルーフに追加したレビュアーに対するプルーフのメールアラートを設定できました。外部の共同作業者は、Workfront に対する必要なアクセス権と適切な権限レベルを持っていなかったので、プルーフに関して受け取るメールアラートを制御できませんでした。

これらの設定は、Workfront で設定できるメールアラート設定とは別のものです。

詳しくは、[プルーフのコメントおよび決定に関する通知の管理](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md)を参照してください。

ビデオ

## デスクトッププルーフビューアでの背景色の変更 {#change-the-background-color-in-the-desktop-proofing-viewer}

デスクトッププルーフビューアの背景色をデフォルトの黒に近い色から白に変更できるようになりました。これにより、透明な背景でプルーフコンテンツを見やすくなります。

詳しくは、[プルーフビューア設定の指定](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md)を参照してください。

ビデオ

## デスクトッププルーフビューアでのプルーフからキャッシュされたブラウザデータの消去 {#clear-cached-browser-data-from-a-proof-in-the-desktop-proofing-viewer}

ブラウザーの Cookie とキャッシュの設定がポップアップなどのコンテンツをブロックするように設定されている場合、このブロック動作はデスクトッププルーフビューアでも発生する可能性があり、レビュアーはプルーフのポップアップコンテンツを閲覧したりコメントしたりできません。

今回のリリースで、プルーフと共に保存されるブラウザーのキャッシュデータを消去できるようになったので、すべてのコンテンツをデスクトッププルーフビューアに表示し、レビュアーが表示してコメントできます。

詳しくは、[プルーフビューア設定の指定](../../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/configure-proofing-viewer-settings.md)を参照してください。

ビデオ
