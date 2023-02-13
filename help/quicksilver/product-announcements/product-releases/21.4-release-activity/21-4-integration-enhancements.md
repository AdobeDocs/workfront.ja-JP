---
title: 21.4 統合の強化
description: 21.4 統合の強化
author: Luke
draft: Probably
feature: Product Announcements, Workfront Integrations and Apps
exl-id: d3e2342e-1c44-49c2-90bc-9fd77fbb2db8
source-git-commit: 665732453b33b49421108791a560ab84d51280b9
workflow-type: tm+mt
source-wordcount: '358'
ht-degree: 0%

---

# 21.4 統合の強化

このページでは、プレビュー環境の 21.4 リリースでおこなわれた統合の機能強化について説明します。 これらの機能強化は、2021 年 10 月 4 日の週に実稼動環境で利用可能になる予定です。

21.4 リリースで利用可能なすべての変更点の一覧については、 [21.4 リリースの概要](../../../product-announcements/product-releases/21.4-release-activity/21.4-release-overview.md).

## ドキュメントをDropboxビジネス

使用可能なドキュメント統合としてDropboxビジネスを追加しました。 これで、Workfront内から直接、Dropboxビジネスに保存したドキュメントにアクセスできます。

Dropboxビジネスでは、共有ドキュメントをリンクし、共有フォルダにドキュメントをアップロードできます。 Dropbox(Dropboxビジネスではない ) を使用すると、ドキュメントの所有者のみがWorkfrontでドキュメントを表示できます。

Workfront管理者が組織に対してこの統合を有効にできます。

詳しくは、 [外部アプリケーションからドキュメントをリンク](../../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

Workfront管理者がこのオプションを有効にする方法について詳しくは、 [ドキュメント統合の設定](../../../administration-and-setup/configure-integrations/configure-document-integrations.md).

## WorkfrontのSlackの更新

WorkfrontでのSlack統合に関して、次の更新が表示されるようになりました。

* Workfront forSlackは、新しい外観と操作性を備えています。
* これで、WorkfrontにリアルタイムでSlack通知が届きます。

   例えば、タスクに割り当てられている場合は、割り当てられるとすぐに通知を受け取ります。 以前は、通知がSlackに表示されるまでに遅延が生じる可能性がありました。

この更新では、Workfrontを認証統合のために再認証する必要があります。 統合の認証について詳しくは、 [Adobe WorkfrontをSlack用に設定](../../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

Slack通知について詳しくは、 Workfront [Adobe Workfront通知をSlackで受信](../../../workfront-integrations-and-apps/using-workfront-with-slack/receive-workfront-notifications-in-slack.md).

## Adobe Workfront統合に同意する場合のアカウントアクセスの詳細をより明確に示す

Adobe Workfront統合の同意画面が更新されました。 これで、統合がアクセスできる特定のアクションおよび領域を表示できるので、統合またはアプリケーションがアクセスできるようにする内容をより深く理解できます。

この新しい同意画面は、OAuth 2.0 を使用するAdobe Workfront統合に適用されます。

特定の統合について詳しくは、統合のドキュメントを参照してください。

## 統合に API キー認証は不要になりました

Workfront統合は、最近、セキュリティと操作性を高めるために OAuth2 を使用し始めています。 この移行の一環として、Workfrontでは、統合認証に API キーを必要としなくなりました。
