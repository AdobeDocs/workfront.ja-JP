---
content-type: api
navigation-topic: general-api
title: イベント登録のベストプラクティス
description: イベント登録のベストプラクティス
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
TQID: https://experienceleague.adobe.com/uT7erlnJR5-h-KKGQiuztzZKBtwtEvWQ8U-EUgN4TG4
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 356
ht-degree: 86%

---

# イベント登録のベストプラクティス

サービスを正しく設定し、イベント登録を作成してこれらのメッセージ配信をトリガーすると、Adobe Workfront イベント登録メッセージが Workfront から自動的に送信されます。 イベント登録の適切な設定について詳しくは、[イベント登録の配信要件](../../wf-api/general/setup-event-sub-endpoint.md)を


イベント登録を効果的に作成するのに役立つ、いくつかのベストプラクティスを以下に示します。

## リクエスト本文の必須フィールドをすべて入力する

リクエスト本文のすべての必須フィールドが API に提供されていることを確認します。 必要なすべてのリクエスト属性について詳しくは、[Event Subscription API](../../wf-api/general/event-subs-api.md) を参照してください。

## 余分な本文フィールドを含めない

リクエストに余分な本文フィールドを含めないでください。含めると、API で登録を作成できなくなります。

## イベント登録の過負荷の回避

イベント登録サービスは、すべてのユーザーに信頼性の高いイベント配信を提供するように設計されています。 これを確実にするために、すべてのユーザーに対してサービス品質の問題を引き起こす可能性がある 1 人のユーザーによる過剰なイベント生成を防ぐ対策が講じられています。 その結果、短期間に多すぎるイベントを高率で生成するユーザーの場合、サンドボックス化やイベント配信の遅延が発生する可能性があります。

## 猶予期間内のテストの完了

100 件のメッセージの猶予期間内に、すべての登録テストを実施するようにします。 この猶予期間について詳しくは、[FAQ - イベント登録](../../wf-api/general/event-subs-faq.md)を参照してください。

## 標準イベント登録メッセージ配信要件の満たす

登録エンドポイントが、標準イベント登録メッセージ配信要件に準拠していることを確認します。 これらの要件について詳しくは、[イベント登録の配信要件](../../wf-api/general/setup-event-sub-endpoint.md)を参照してください。

## グローバル地域ごとの IP アドレス許可リスト

ファイアウォール経由でイベント登録ペイロードを受け取るには、グローバル地域ごとに IP アドレスを許可リストに加える必要があります。 詳しくは、[Event Subscription API](../../wf-api/general/event-subs-api.md) を参照してください。

## 適切なアクセスレベルと認証を持っている

イベント登録を作成、クエリ、または削除するには、Workfront ユーザーが次の条件を満たす必要があります。

* **システム管理者のアクセス レベル**
詳しくは、[&#x200B; ユーザーに完全な管理アクセス権を付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)または[特定の領域へのユーザーの管理アクセス権を付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)を参照してください。

* 組織でAdobe IMS（Identity Management System）を使用している場合は、`X-User-Token` ヘッダーに渡されたIMS ユーザートークンを含めます。
