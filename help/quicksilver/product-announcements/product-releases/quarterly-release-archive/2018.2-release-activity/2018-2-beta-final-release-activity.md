---
content-type: release-notes
navigation-topic: product-releases-archive
title: 2018.2 最終ベータ版リリースアクティビティ
description: このページでは、2018.2 ベータ版最終リリースでプレビュー環境で最近使用されたすべての変更について説明します。この機能は、2018年6月20日（PT）にプレビュー環境で使用できるようになりました。2018年7月に、実稼動環境で利用可能になる予定です。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: 36001571-bf8c-4fe8-a66b-09d3726f66d3
source-git-commit: f1e463c90641f9221228e335b583cab72762b3bd
workflow-type: tm+mt
source-wordcount: '813'
ht-degree: 98%

---

# 2018.2 最終ベータ版リリースアクティビティ

このページでは、2018.2 ベータ版最終リリースでプレビュー環境で最近使用されたすべての変更について説明します。この機能は、2018年6月20日（PT）にプレビュー環境で使用できるようになりました。2018年7月に、実稼動環境で利用可能になる予定です。

>[!IMPORTANT]
>
>このページで説明する機能は、実稼動環境で使用可能になる前に変更される場合があります。

2018.2 で行われたすべての変更のリストについては、[2018.2 リリースアクティビティの概要](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-release-activity-overview.md) を参照してください。

18.2 実稼動版リリースの時点で、次の新機能がリリースされます。

* [Workfront メール通知に返信するメール配信サービスを指定](#specify-mail-delivery-services-for-replying-to-workfront-email-notifications)
* [ドキュメントへのコメントに関するメール通知を受信](#receive-email-notifications-for-comments-on-documents)
* [システムが追跡する更新からアイコンが除外](#system-tracked-updates-no-longer-contain-an-icon)
* [コメントをタスクに変換するオプションが削除](#option-to-convert-a-comment-to-a-task-was-removed)
* [Workfront for Salesforce](#workfront-for-salesforce)
* [Workfront for Slack の向上](#workfront-for-slack-improvements)
* [モバイルの改善点](#mobile-improvements)

## Workfront メール通知に返信するメール配信サービスを指定する {#specify-mail-delivery-services-for-replying-to-workfront-email-notifications}

Workfront 管理者は、Workfront を設定して、メールの返信を通じてユーザーがオブジェクトにコメントを付けられるようにする際に、メール配信サービスを選択できるようになりました。Workfront は、デフォルトのメールサービスまたは POP メールアカウントを使用するように設定できます。

この更新以前は、Workfront 管理者が各ユーザーに対して POP アカウントを設定する必要がありました。 

POP メールアカウントの設定について詳しくは、以下を参照してください。

デフォルトのメールサービスについて詳しくは、以下を参照してください。

## ドキュメントへのコメントに関するメール通知を受信する {#receive-email-notifications-for-comments-on-documents}

自分が所有するドキュメントに誰かがコメントをしたときにメール通知が届くようになりました。このオプションは、デフォルトで有効になっています。「私のドキュメントに対するコメントが追加されました」通知設定を使用して、メール通知オプションを無効にできます。

この変更以前は、自分が所有するドキュメントに誰かがコメントをしたときに通知が届きませんでした。 

詳しくは、 [独自の電子メール通知を変更する](../../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

>[!NOTE]
>
>この機能が最初にリリースされたとき、ユーザーにはメール通知に加えてアプリ内通知が届きます。自分が所有しているドキュメントに誰かがコメントをしたときに、アプリ内通知が届かなくなりました。 

## システム追跡された更新にアイコンが含まれなくなりました {#system-tracked-updates-no-longer-contain-an-icon}

Workfront システムがオブジェクト（プロジェクト内など）の更新エリアに更新を作成するたびに、その更新には対応するアイコンが含まれなくなります。

この変更以前は、システムの更新には、行われた更新を表すアイコンも含まれていました。

システム更新について詳しくは、[システムで追跡された更新](../../../../administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md)を参照してください。

## コメントをタスクに変換するオプションが削除されました {#option-to-convert-a-comment-to-a-task-was-removed}

コメントをタスクに変換するオプションが削除されました。

以前は、オブジェクトの更新エリアにいるときにコメントをタスクに変換できました。

## Workfront for Salesforce {#workfront-for-salesforce}

Salesforce と Workfront の新しい標準統合がリリースされます。次の操作を実行できます。

* Salesforce の機会が特定のステージに達したとき、新しい製品が機会に追加されたとき、またはアカウントのタイプが更新されたときに、新しい Workfront プロジェクトを自動的に作成します。
* Salesforce の機会またはアカウントから Workfront リクエストを作成します。

この統合は、Workfront Pro 以降のエディションを持つすべてのお客様が無料で利用できます。

Workfront for Salesforce について詳しくは、[Adobe Workfront for Salesforce](../../../../workfront-integrations-and-apps/using-workfront-with-salesforce/workfront-for-salesforce.md) を参照してください。

## Workfront for Slack の向上 {#workfront-for-slack-improvements}

Slack Workfront チャネルで Workfront 通知を受信するように設定できます。

次の Workfront 通知を Slack で配信するように設定することもできます。

* 誰かがコメントまたは更新で自分をタグ付けする場合。
* 新しいタスクまたはイシューに割り当てられた場合。
* 項目の承認がリクエストされた場合。

この改善以前は、Slack で Workfront 通知を受け取ることができませんでした。

Slack での Workfront 通知について詳しくは、[Adobe Workfront 通知を Slack で受信](../../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md)を参照してください。

## モバイルの改善点 {#mobile-improvements}

以下の新機能は、18.2 実稼動版リリースの時点でモバイルストアにリリースされます。

* オブジェクト名のインライン編集

  モバイルアプリで、プロジェクト、タスク、イシューの名前などのフィールドをインライン編集できるようになりました。

* ドキュメントをアップロード

  Workfront モバイルアプリのオブジェクトにドキュメントをアップロードできるようになりました。

* プロフィール画像をアップロードする

  iOS モバイルアプリにプロファイル写真をアップロードできるようになりました。

  この機能は、iOS モバイルアプリでのみ使用できます。

次の機能は、Workfront モバイルアプリの Android ベータ版に既にリリースされており、パブリック Android および iOS モバイルアプリにもリリースされます。iOS プラットフォームのエクスペリエンスには、既にリリースされている Android エクスペリエンスと、次の違いが含まれます。

* iOS の新しい下部ナビゲーションバー

* iOS の新しいチュートリアルエクスペリエンス

これらの機能について詳しくは、およびそれらの機能をデモするビデオを見るには、[2018.2 ベータ 4 リリースアクティビティ](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-beta-4-release-activity.md)および [2018.2 ベータ 5 リリースアクティビティ](../../../../product-announcements/product-releases/quarterly-release-archive/2018.2-release-activity/2018-2-beta-5-release-activity.md)を参照してください。
