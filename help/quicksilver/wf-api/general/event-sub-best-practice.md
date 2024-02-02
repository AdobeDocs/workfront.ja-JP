---
content-type: api
navigation-topic: general-api
title: イベント登録のベストプラクティス
description: イベント登録のベストプラクティス
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: ht
source-wordcount: '269'
ht-degree: 100%

---


# イベント登録のベストプラクティス

サービスを正しく設定し、イベント登録を作成してこれらのメッセージ配信をトリガーすると、Adobe Workfront イベント登録メッセージが Workfront から自動的に送信されます。イベント登録の適切な設定について詳しくは、[イベント登録の配信要件](../../wf-api/general/setup-event-sub-endpoint.md)を


イベント登録を効果的に作成するのに役立つ、いくつかのベストプラクティスを以下に示します。

## リクエスト本文の必須フィールドをすべて入力する

リクエスト本文のすべての必須フィールドが API に提供されていることを確認します。必要なすべてのリクエスト属性について詳しくは、[Event Subscription API](../../wf-api/general/event-subs-api.md) を参照してください。

## 余分な本文フィールドを含めない

リクエストに余分な本文フィールドを含めないでください。含めると、API で登録を作成できなくなります。

## 猶予期間内のテストの完了

100 件のメッセージの猶予期間内に、すべての登録テストを実施するようにします。この猶予期間について詳しくは、[FAQ - イベント登録](../../wf-api/general/event-subs-faq.md)を参照してください。

## 標準イベント登録メッセージ配信要件の満たす

登録エンドポイントが、標準イベント登録メッセージ配信要件に準拠していることを確認します。これらの要件について詳しくは、[イベント登録の配信要件](../../wf-api/general/setup-event-sub-endpoint.md)を参照してください。

## グローバル地域ごとの IP アドレス許可リスト

ファイアウォール経由でイベント登録ペイロードを受け取るには、グローバル地域ごとに IP アドレスを許可リストに加える必要があります。詳しくは、[Event Subscription API](../../wf-api/general/event-subs-api.md) を参照してください。

## 適切なアクセスレベルと API キーを入手する

イベント登録を作成、クエリ、または削除するには、Workfront ユーザーが次の条件を満たす必要があります。

* アクセスレベル：**システム管理者**
詳しくは、[ユーザーに完全な管理アクセス権を付与する](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md)または[特定の領域に対する管理者アクセス権をユーザーに付与する](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)を参照してください。

* API キー

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more, see .</p>
  -->
