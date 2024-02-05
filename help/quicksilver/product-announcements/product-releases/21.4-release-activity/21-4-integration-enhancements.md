---
title: 21.4 統合の機能強化
description: 21.4 統合の機能強化
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
recommendations: noDisplay, noCatalog
exl-id: d3e2342e-1c44-49c2-90bc-9fd77fbb2db8
source-git-commit: ccba3a3d7c0cac50dbd29cae677b076811904a91
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 100%

---

# 21.4 統合の機能強化

このページでは、プレビュー環境の 21.4 リリースで行われた統合の機能強化について説明します。これらの機能強化は、2021年10月4日（PT）の週に実稼動環境で利用可能になる予定です。

21.4 リリースで利用可能なすべての変更点の一覧については、[21.4 リリースの概要](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md)を参照してください。

## Dropbox Business からドキュメントをリンク

利用可能なドキュメント統合として Dropbox Business を追加しました。Dropbox Business に保存したドキュメントに Workfront 内から直接アクセスできるようになりました。

Dropbox Business では、共有ドキュメントをリンクしたり、ドキュメントを共有フォルダーにアップロードしたりできます。Dropbox（Dropbox Business ではありません）では、ドキュメントの所有者のみが Workfront でドキュメントを表示できます。

Workfront 管理者は、組織に対してこの統合を有効にすることができます。

詳しくは、[外部アプリケーションからドキュメントをリンク](../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)を参照してください。

Workfront 管理者がこのオプションを有効にする方法について詳しくは、[ドキュメント統合の設定](../../../administration-and-setup/configure-integrations/configure-document-integrations.md)を参照してください。

## Workfront for Slack をアップデート

次の更新が Workfront for Slack 統合に表示されるようになりました。

* Workfront for Slack のルックアンドフィールが新しくなりました。
* Workfront for Slack の通知をリアルタイムで受信できるようになりました。

  例えば、タスクに割り当てられている場合は、割り当てられるとすぐに通知を受け取ります。以前は、通知が Slack に表示されるまでに遅延が生じる可能性がありました。

この更新では、Workfront for Slack を統合するために再認証する必要があります。統合の認証について詳しくは、[Adobe Workfront for Slack を設定](../../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)を参照してください。

Workfront for Slack の通知について詳しくは、[Adobe Workfront の通知を Slack で受信](../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md)を参照してください。

## Adobe Workfront 統合に同意する際のアカウントアクセスの詳細を、より明確に表示

Adobe Workfront 統合の同意画面が更新されました。これで、統合がアクセスできる特定のアクションおよびエリアを表示できるので、統合またはアプリケーションがアクセスできるようにする内容をより深く理解できます。

この新しい同意画面は、OAuth 2.0 を使用する Adobe Workfront 統合に適用されます。

特定の統合について詳しくは、統合のドキュメントを参照してください。

## 統合に API キー認証が不要になりました

最近、Workfront 統合では、セキュリティと使いやすさを向上させるために、OAuth2 の使用が開始されました。この移行の一環として、Workfront では、統合認証に API キーを必要としなくなりました。
