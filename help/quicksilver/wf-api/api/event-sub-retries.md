---
content-type: api
navigation-topic: api-navigation-topic
title: イベント登録の再試行
description: イベント登録の再試行
author: Becky
feature: Workfront API
role: Developer
exl-id: b698cb60-4cff-4ccc-87d7-74afb5badc49
source-git-commit: 05f8dc8770c185720520fc631e19c75b925a70bf
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 63%

---

# イベント登録の再試行

メッセージ配信システムを実装する場合、安定性、一貫性、優れたユーザーエクスペリエンスを確保するために、いくつかの注意事項があります。メッセージ配信システムの問題点の 1 つとして、メッセージを宛先に正常に到達させること、およびメッセージが届かなかった場合にどのように対処するかを確認することがあります。

一部の統合では、配信の失敗を受け入れてから、メッセージをドロップして次のメッセージに移動する場合があります。その他の統合では、メッセージの配信に失敗したことを無視することはできません。例えば、財務統合はメッセージの配信を試みる場合がありますが、代わりに HTTP ステータスコード 404 を受信します。これは、サーバーがメッセージの配信先のエンドポイントを見つけられなかったことを示します。このような場合、メッセージが欠落しているということは、誰かが時間に対して賃金を支払っていないこと、または組織が契約リソースの予算を超過していることを意味する可能性があります。

## イベントサブスクリプションの再試行のための Adobe Workfront 戦略

顧客は Workfront プラットフォームを日々の知識作業の中核として活用するので、Workfront イベントサブスクリプションフレームワークは、各メッセージの配信を可能な限り確実に試行するメカニズムを提供します。

顧客のエンドポイントへの配信に失敗したイベントトリガーの送信メッセージは、最大 48 時間配信が成功するまで再送信されます。この間、配信が成功するか 11 回の試行が行われるまで、再試行は徐々に高い頻度で行われます。

これらの再試行の数式を次に示します。

`((2^attempt) - 1) * 84800ms`

1 回目の再試行は 1.5 分後に行われ、2 回目はほぼ 5 分後に行われ、11 回目は約 48 時間で行われます。

顧客は、Workfront イベントサブスクリプションからの送信メッセージを消費するエンドポイントが、配信が成功したときに 200 レベルの応答メッセージを Workfront に返すように設定されていることを確認する必要があります。

## 無効な購読ルールと凍結された購読ルール

* 購読 URL が 100 回を超える試行で 70% を超える失敗率を持つ場合、または 2,000 回連続して失敗する場合、**無効** になります
* 購読 URL が 2,000 回以上連続してエラーが発生し、最後の成功が 72 時間以上あった場合、または任意の期間に 50,000 回連続してエラーが発生した場合、購読 URL は **フリーズ** されます。
* **無効** の購読 URL は、引き続き 10 分ごとに配信を試み、配信が成功すると再度有効になります。
* **フリーズ** された購読 URL は、API リクエストを行って手動で有効にしない限り、配信を試みません。




<!--

## Handling Failed Event-Triggered Outbound Messages

The following flowchart shows the strategy for reattempting message deliveries with Workfront Event Subscriptions:

![](assets/event-subscription-circuit-breaker-retries-350x234.png)

The following explanations correspond with the steps depicted in the flowchart:

1. Message fails to be delivered. 
1. Message delivery failure information is logged.

   All failed attempts to deliver a message are logged so that debugging may be performed to determine the root cause of a given failure or series of failures. 

1. URL failures incremented. 
1. Message attempt count is incremented. 
1. Calculate the delay until this message's delivery will be attempted again. 
1. Message is placed onto the message retry queue.

   As shown in the preceding flowchart, the message queue used for processing message delivery retries is a separate queue from the one that processes the initial delivery attempt for each message. This allows the near real-time flow of messages to continue unimpeded by the failure of any subset of messages. 

1. URL circuit status is evaluated. One of the following occurs:

   * If the circuit is open and not allowing deliveries at this time, restart the process at step 5.
   * If the circuit is half-open, this implies that our circuit is currently open, but enough time has passed to allow testing of the URL to see if the problem with delivering to it has been resolved.
   * If the message delivery attempt limits have been reached (48 hours of retrying) then the message is dropped

1. If the URL circuit is closed and allowing deliveries, attempt to deliver the message. If this delivery fails, the message will restart at step 1 

1. If the URL circuit is closed and allowing deliveries, attempt to deliver the message. If this delivery fails, the message will restart at step 1.
   -->
