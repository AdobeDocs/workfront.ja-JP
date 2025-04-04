---
content-type: api;faq
navigation-topic: general-api
title: FAQ - イベント登録
description: FAQ - イベント登録
author: Becky
feature: Workfront API
role: Developer
exl-id: a6120939-5d76-4f46-a304-125de6b22502
source-git-commit: 074f78e27d2ab1cb1d1b8216f14557b91d9afd00
workflow-type: tm+mt
source-wordcount: '973'
ht-degree: 94%

---

# FAQ - イベント登録

<!--
{{highlighted-preview}}
-->

以下は、イベント登録に関してよくある質問です。

## 購読とは何ですか？

購読とは、Adobe Workfront イベントを照合し、顧客の HTTP エンドポイントに配信するために使用される一連のデータです。このリソースは、次の 4 つの主要な属性で構成されています。

* customer_id
* obj_code
* obj_id
* url

また、登録には、独自の一意の ID や作成日など、他の属性も含めることができますが、上記の属性は主にイベントを照合し顧客に配信するために使用されます。

## エンドポイントに送信されるイベントを、イベントペイロード内の特定の条件に基づいて選択できますか？

イベント登録フィルターを使用すると、イベント登録を指定した条件で並べ替えることができます。エンドポイントで使用する必要のあるメッセージの数が大幅に減る場合があるので、イベント登録にフィルターを適用することをお勧めします。詳しくは、[イベント登録のフィルタリング](../../wf-api/general/event-subs-api.md#event)を参照してください。

## API が 409 競合応答コードを返すのはなぜですか？

イベント登録を作成しようとして、応答コード 409 が競合した場合、作成しようとした登録は重複しています。Workfront では、重複する登録の作成は許可されていません。

## メッセージがエンドポイントに配信されない場合、どのように対処する必要がありますか？

次のシナリオを確認し、推奨される解決策を使用します。

* **url** フィールドで定義されている登録エンドポイントが、200 番台の HTTP 応答コードを返すことを確認します。このコードが返されない場合は、Workfront サポートに問い合わせるか、[イベント登録の配信要件](../../wf-api/general/setup-event-sub-endpoint.md)を参照してください。

* イベント配信リクエストが完了する前にタイムアウトになる場合があります。エンドポイントが一貫して 5 秒以内に応答することを確認します。これは、HTTP リクエストがイベント登録メッセージを配信する際のデフォルトのタイムアウト設定です。エンドポイントが 5 秒以内に応答しない場合は、Workfront サポートに問い合わせるか、[イベント登録の配信要件](../../wf-api/general/setup-event-sub-endpoint.md)を参照してください。
* イベントは、想定どおりには生成されない場合があります。イベントが発生する方法やタイミングについて、憶測や決めつけを行わないようにしてください。例えば、あなたはタスクでドキュメントを更新すると、タスクの更新イベントが生成されると考えるかもしれません。ですがこの場合、代わりに、ドキュメントの作成イベントまたはドキュメントの更新イベントが生成されます。
* 登録が意図したとおりに設定されない場合があります。あなたは様々な環境でイベント登録を作成して、他の Workfront データと同様にイベント登録が転送されることを期待します。ですが、イベント登録データは、他の環境にコピーまたは昇格するように設定されていません。正しい環境に API リクエストを発行していること、およびその環境の登録が意図どおりに設定されていることを確認してください。
* 必要な Workfront IP アドレスがファイアウォールの許可リストに追加されていないので、ペイロードを受け取れませんでした。イベント登録イベントは、一部の IP アドレスからのみ送信されます。宛先ネットワークに、Workfront イベント登録からペイロードを受け取るのに必要な IP 例外がすべて含まれていることを確認してください。
* ペイロードが 1 MB を超えたので、受信されませんでした。 イベント購読メッセージまたはオブジェクトは 1 MB 以下にする必要があります。

## メッセージがエンドポイントに到達するまでに、極端に長い時間がかかるのはなぜですか？

次のシナリオの一部が原因となっている場合があります。

* システム内で大きな操作（一括更新など）を実行すると、大量のメッセージが一度にキューに入れられ、処理に時間がかかる場合があります。
* 大きなプロジェクトで長時間実行される計算やタイムラインの計算が原因で、イベント登録に対するメッセージの公開で処理が遅れる場合があります。
* 登録が無効になっている場合があります。

   * 100 通分の猶予期間の後、特定の URL（1 つ以上の登録に関連付けられている場合があります）が 1 回につき 70% 以上失敗した場合、または 2000 回連続で配信に失敗した場合、同じ URL の登録に一致するすべてのメッセージの配信は試行されません。代わりに、これらのメッセージは、再試行のためのキューに即座に格納されます。

     URL が無効になってから 10 分ごとに、次のメッセージの配信が試行され、処理を求めます。そのメッセージが成功した場合は、その URL を再度有効にし、その後、一致する登録をすべて有効にします。そのメッセージの送信に失敗した場合は、その 10 分のタイマーがリセットされ、タイマーの期限が切れた後にもう一度配信を試行します。

     この動作は、一貫性のない配信または遅延した配信と受け取られる可能性がありますが、単にイベント登録メッセージの処理方法に関するポリシーに従っているにすぎません。

   * 次のいずれかの条件を満たす場合、イベント登録 URL にはハードな無効化が行われます。

      * 登録 URL は、配信に 7 日間失敗し、過去 72 時間に少なくとも 2,000 回連続で配信の試行に失敗しました。
      * 登録 URL が 50,000 回連続で配信に失敗しました。

## Event Subscription API を呼び出そうとすると、500 応答ステータスが返された場合は、どうすればよいですか？

Workfront サポートにお問い合わせください。サポートへの問い合わせ方法については、[カスタマーサポートへの問い合わせ](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)を参照してください。

## Workfront イベント登録では、様々な種類の認証を使用できますか？

ベアラートークンを使用する任意の認証を使用できます。登録の **authToken** フィールドは、**URL** フィールドで指定された URL で認証するのに使用される OAuth2 ベアラートークンを表す文字列です。理論的には、宛先エンドポイントがエンコーディングの処理方法（**utf-8** を認識している限り、このトークン値は 255 文字未満であれば何でも構いません。

## Workfront イベント登録からイベントのペイロードを受け取るまで、どれくらいかかりますか？

一般的に、ログに記録されるデータ変更から 5 秒未満でイベント購読のイベント配信要求を受け取ることが想定されます。平均的に、web フック通知は、データが変更されてから 1 秒未満で受信されます。ただし、サービスは大量のメッセージを受信するので、長くかかる場合があります。

## 追加のリソース

* **API ドキュメント**：[Event Subscription API](../../wf-api/general/event-subs-api.md)

* **ベストプラクティス**：[イベント登録のベストプラクティス](../../wf-api/general/event-sub-best-practice.md)

* **イベント登録ペイロードをトリガーするフィールド**：[イベント登録リソースフィールド](../../wf-api/api/event-sub-resource-fields.md)

* **イベント登録の再試行について**：[イベント登録の再試行](../../wf-api/api/event-sub-retries.md)

* **Workfront 用のファイアウォールの設定**：[ファイアウォールの許可リストの設定](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)
