---
content-type: release-notes
navigation-topic: 2020-1-release-activity
title: 2020.1 その他の機能強化
description: このページでは、2020.1 リリースでの Workfront の一般エリアに対するすべての機能強化について説明します。 これらの機能強化は、現在、プレビュー環境で使用でき、2020年3月下旬または 4月上旬に本番環境で使用できるようになる予定です。
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: a716590c-c833-458a-a138-9bc0723e5896
TQID: https://experienceleague.adobe.com/I5djuVv0ixHspF6afQaa5-jTkl0uXl26VlKf8BXqhO4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: b8ea32d4-f1fe-4c71-8871-afe5a702a009
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 433
ht-degree: 100%

---

# 2020.1 その他の機能強化

このページでは、2020.1 リリースでの Workfront の一般エリアに対するすべての機能強化について説明します。 これらの機能強化は、現在、プレビュー環境で使用でき、2020年3月下旬または 4月上旬に本番環境で使用できるようになる予定です。

2020.1 リリースで使用可能なすべての変更点の一覧については、[2020.1 リリースの概要](../../../product-announcements/product-releases/2020.1-release-activity/2020-1-release-overview.md)を参照してください。

## 許可リストにプルーフを追加する必要のある変更

>[!NOTE]
>
>この機能は 2020.1 リリースから削除されました。 後日ご利用いただけるようになります。

プルーフドメインは from proofhq.com から workfront.com に変更されています。

ファイアウォールやメールサーバーで特定のベンダーへのみアクセスできるように設定されている場合は、次の URL を許可リストに追加する必要があります。これにより、組織のユーザーがブラウザープルーフビューアとデスクトッププルーフビューアの両方で Workfront 内のプルーフを表示できるようになります。

&#42;.workfront.com

&#42;proofhq.com URL も引き続き必要です。

許可リストの更新について詳しくは、[ファイアウォールの許可リストの設定](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)を参照してください。

>[!NOTE]
>
>この更新は、Workfront 内のプルーフにのみ適用されます。Workfront Proof アプリケーションをスタンドアロンで使用する場合は適用されません。

## Chrome との互換性を維持するために Workfront クッキーの動作を更新しました

今後の Google Chrome の更新（Chrome v80）との互換性を維持するために、Workfront のプラットフォームを更新し、リクエストに応じてクッキーが適切に送信されるようにしました。

この Chrome の更新により、SameSite クッキー属性のデフォルト値が変更になります。 Google Chrome を更新後に Workfront インスタンスがどのように動作するかをテストするには、Chrome でフラグを調整し、次のオプションを有効にします。

* 「デフォルトのクッキーによる SameSite」
* 「SameSite を使用しないクッキーは安全でなければならない」

## Workfront のコメントを Jira に同期しました

Workfront の Jira との統合により、Workfront のコメントを Jira のネイティブなコメントストリームに同期できるようになりました。

以前は、Jira から Workfront にコメントを同期できましたが、Workfront から Jira にコメントを同期することはできませんでした。

詳しくは、[Adobe Workfront の Jira 向け設定](../../../workfront-integrations-and-apps/use-workfront-with-jira/configure-workfront-for-jira.md)を参照してください。

## Flash ポートフォリオオプティマイザーが削除されました

すべてのお客様を対象に、Workfront Classic 環境から、新しいポートフォリオオプティマイザーと従来の（Flash ベースの）ポートフォリオオプティマイザーを切り替える機能を削除しました。 従来のポートフォリオオプティマイザーの機能は廃止し、新しいツールでこれまでと同じ機能を提供しています。

ポートフォリオオプティマイザーについて詳しくは、 https://experience.workfront.com/s/article/Understanding-the-Portfolio-Optimizer-356650079 を参照してください。

Workfront での Flash ベースツールの廃止について詳しくは、[Adobe Workfront の Flash ベースのツールの置換](../../../product-announcements/announcements/announcement-archive/replace-flash-tools.md)を参照してください。
