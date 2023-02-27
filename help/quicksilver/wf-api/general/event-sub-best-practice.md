---
content-type: api
navigation-topic: general-api
title: イベント購読のベストプラクティス
description: イベント購読のベストプラクティス
author: Becky
feature: Workfront API
exl-id: 2c6e3567-d5eb-4528-a393-dbf235958ed2
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '269'
ht-degree: 0%

---


# イベント購読のベストプラクティス

サービスを正しく設定し、イベント購読を作成してこれらのメッセージ配信をトリガーすると、Adobe Workfrontイベント購読メッセージがWorkfrontから自動的に送信されます。 イベント購読の適切な設定について詳しくは、 [イベント購読配信要件](../../wf-api/general/setup-event-sub-endpoint.md).


イベント購読を効果的に作成するのに役立つ、いくつかのベストプラクティスを以下に示します。

## すべての必須リクエスト本文フィールドを指定します

すべての必須リクエスト本文フィールドが API に提供されていることを確認します。 必要なすべての要求属性について詳しくは、 [イベント購読 API](../../wf-api/general/event-subs-api.md).

## 追加の本文フィールドを含めない

リクエストに余分な本文フィールドを含めないでください。含めると、API で購読を作成できなくなります。

## 猶予期間内のテストの完了

100 件のメッセージの猶予期間内に、すべての購読テストを実施してみます。 この猶予期間について詳しくは、 [FAQ — イベント購読](../../wf-api/general/event-subs-faq.md).

## 標準イベント購読メッセージ配信要件の満たし

サブスクリプションエンドポイントが、標準イベントサブスクリプションメッセージ配信要件に準拠していることを確認します。 これらの要件について詳しくは、 [イベント購読配信要件](../../wf-api/general/setup-event-sub-endpoint.md).

## グローバル許可リスト地域別の IP アドレスの

ファイアウォールを通じてイベント購読ペイロードを受け取るには、IP アドレスをグローバル地域別にに追加する必要がありま許可リストす。 詳しくは、 [イベント購読 API](../../wf-api/general/event-subs-api.md).

## 適切なアクセスレベルと API キーを持っている

イベント購読を作成、クエリ、または削除するには、Workfrontユーザーが次の条件を満たす必要があります。

* アクセスレベル： **システム管理者**
詳しくは、 [ユーザーに完全な管理アクセス権を付与する](../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md) または [特定の領域に対する管理者アクセス権をユーザーに付与する](../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* API キー

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">To learn more, see .</p>
  -->
