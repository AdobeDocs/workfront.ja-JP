---
title: 20.4 その他の機能強化
description: 20.4 その他の機能強化
author: Luke
draft: Probably
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: bd8fcafc-00cc-4025-b2d3-e3a6f12e40fc
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '487'
ht-degree: 95%

---

# 20.4 その他の機能強化

このページでは、20.4 リリースでプレビュー環境に対して行われたその他すべての機能強化について説明します。これらの機能強化は、2020年11月9日（PT）の週に実稼動環境で利用可能になる予定です。

20.4 リリースで利用可能なすべての変更点の一覧については、[20.4 リリースの概要](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md)を参照してください。

## 管理者向けの新機能：「Workfront 環境を切り替え」オプションが使用可能

より効率的で便利なエクスペリエンスを実現するために、グループ管理者と Workfront 管理者は、ログアウトしなくても Workfront 内の任意のページから様々な Workfront 環境をすばやく切り替えることができるようになりました。

新バージョンの Workfront では、「クラシック Workfront に切り替え」オプションがメインメニューに表示されます。

Workfront Classicでは、グローバルナビゲーションバーの右上隅にあるプロファイル画像のクリックで表示されるメニューに、「新バージョンに切り替える」オプションが表示されます。

この機能は、Workfront One の[管理者の基本、第 1 部の学習パス](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY)に含まれるようになりました。

## Workfront Proof の暗号化の改善

Workfront Proof アプリケーションのデータインモーション暗号化の強度を向上させるために、いくつかの変更を加えています。脆弱な TLS 暗号は 2020年11月11日（PT）に廃止されます。

Workfront にアクセスする際は、サポート対象のブラウザーを使用していることを確認してください。サポートされているブラウザーについて詳しくは、[Adobe Workfront のブラウザー要件](../../../workfront-basics/workfront-browser-requirements.md)を参照してください。

## 3 つの メールテンプレートの新しいルックアンドフィール

読みやすさと全体的なエクスペリエンスを改善するために、次のメールテンプレートのルックアンドフィールが新しくなりました

* 新規作業リクエスト
* あなたに割り当てられた先行タスクを開始する準備ができました
* 前任者とのチームメール通知が完了しました

プレビュー環境でテスト用に電子メールを有効にするには、プレビューでの電子メールの管理の節を参照してください。 [独自の電子メール通知を変更する](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## チームへの新しいメール通知

チーム向けに次のメール通知を追加しました。

* チームに割り当てられたタスクの先行タスクが完了しました：割り当てられたチームは、タスクのいずれかの先行タスクが完了としてマークされると、メール通知を受け取ります。
* チームに割り当てられたタスクの先行タスクがすべて完了しました：割り当てられたチームは、完了のマークが付けられた各先行者についてメール通知を受け取ります。

詳しくは、[通知：自分に割り当てられた作業に関する情報](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md)を参照してください。

## 管理者向けの新機能：メール通知の機能強化

これで、1回のクリックで、セットアップでイベントのメール通知を有効または無効にできるようになりました。通知名の横にあるオン／オフスイッチをクリックするだけです。

また、最新のスタイル設定により、メール通知エリアでイベント通知を設定する操作性が向上しました。

メール通知の設定の詳細については、[システム内の全員に対するイベント通知を設定する](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md)を参照してください。

この機能は、Workfront Oneｍ の[メールおよびアプリ内通知の学習パス](https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-20Y4X000000CaZGUA0)に含まれるようになりました。

## イベント登録の更新をトリガーする新しい API オブジェクト

ドキュメントのバージョン管理またはドキュメントが承認されたときにイベント登録の更新をトリガーするために、documentVersion と proofApproval という 2 つの新しい API オブジェクトが作成され、設定されました。

各オブジェクトに関連付けられているフィールドの完全なリストについては、[イベント登録リソースフィールド](../../../wf-api/api/event-sub-resource-fields.md)を参照してください。
