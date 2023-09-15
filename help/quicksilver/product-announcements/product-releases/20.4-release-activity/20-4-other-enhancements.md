---
title: 20.4 その他の機能強化
description: 20.4 その他の機能強化
author: Luke
draft: Probably
feature: Product Announcements
exl-id: bd8fcafc-00cc-4025-b2d3-e3a6f12e40fc
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 0%

---

# 20.4 その他の機能強化

このページでは、20.4 リリースでプレビュー環境に対しておこなわれたその他すべての機能強化について説明します。 これらの機能強化は、2020 年 11 月 10 日の週に、実稼動環境で利用可能になる予定です。

20.4 リリースで使用可能なすべての変更点の一覧については、 [20.4 リリースの概要](../../../product-announcements/product-releases/20.4-release-activity/20-4-release-overview.md).

## 管理者向けの新機能：「 Workfront環境を切り替え」オプションが使用可能

より効率的で便利なエクスペリエンスを実現するために、グループ管理者とWorkfront管理者は、Workfront内の任意のページから、ログアウトしなくても様々なWorkfront環境をすばやく切り替えることができるようになりました。

新しいWorkfrontエクスペリエンスでは、「クラシックに切り替え」オプションがメインメニューに表示されます。

Workfront Classic では、グローバルナビゲーションバーの右上隅にあるプロファイル画像をクリックすると表示されるメニューに、「新しいエクスペリエンスに切り替え」オプションが表示されます。

この機能は、 [管理者の基本、第 1 部の学習パス](https://one.workfront.com/s/learningpath3/administrator-fundamentals-in-the-new-workfront-experience-part-2-user-organizat-20Y0z000000bmAXEAY) Workfront・ワンで

## Workfront Proof の暗号化の改善

Workfront Proofing Application のデータインモーション暗号化の強度を向上させるために、いくつかの変更を加えています。 弱い TLS 暗号は 2020 年 11 月 11 日に廃止されます。

Workfrontにアクセスする際は、サポート対象のブラウザーを使用していることを確認してください。 サポートされているブラウザーについて詳しくは、 [Adobe Workfront browser requirements](../../../workfront-basics/workfront-browser-requirements.md).

## 3 つの E メールテンプレートの新しいルックアンドフィール

次の E メールテンプレートは、読みやすさと全体的なエクスペリエンスを改善するために、新しいルックアンドフィールを備えています。

* 新規作業要求
* 割り当てられた依存タスクを開始する準備が整いました
* 先行者へのチームメール通知が完了しました

プレビュー環境でテスト用に電子メールを有効にするには、プレビューでの電子メールの管理の節を参照してください。 [独自の電子メール通知を変更する](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

## チームへの新しい電子メール通知

チーム向けに次の電子メール通知を追加しました。

* チームに割り当てられたタスクの先行タスクが完了しました：タスクの 1 つの先行タスクが完了とマークされると、割り当てられたチームが電子メール通知を受け取ります。
* チームに割り当てられたタスクの先行タスクがすべて完了しました：チームに割り当てられたチームは、完了とマークされた各先行タスクに関する電子メール通知を受け取ります。

詳しくは、 [通知：自分に割り当てられた作業に関する情報](../../../workfront-basics/using-notifications/notifications-information-about-work-assigned-to-me.md).

## 管理者向けの新機能：電子メール通知の強化

これで、1 回のクリックで、セットアップでイベント電子メール通知を有効または無効にできます。 通知名の横にあるオン/オフスイッチをクリックするだけです。

また、最新のスタイル設定により、電子メール通知領域でイベント通知を設定する操作性が向上しました。

電子メール通知の設定について詳しくは、 [システムの全員に対するイベント通知を設定する](../../../administration-and-setup/manage-workfront/emails/configure-event-notifications-for-everyone-in-the-system.md).

この機能は、 [電子メールおよびアプリ内通知の学習パス](https://one.workfront.com/s/learningpath2/email-and-in-app-notifications-in-the-new-workfront-experience-20Y4X000000CaZGUA0) Workfront・ワンで

## イベント購読更新をトリガーする新しい API オブジェクト

ドキュメントがバージョン管理または承認されたときにイベント購読の更新をトリガーするために、documentVersion と proofApproval という 2 つの新しい API オブジェクトが作成され、設定されました。

各オブジェクトに関連付けられているフィールドの完全なリストについては、 [イベント購読リソースフィールド](../../../wf-api/api/event-sub-resource-fields.md).
