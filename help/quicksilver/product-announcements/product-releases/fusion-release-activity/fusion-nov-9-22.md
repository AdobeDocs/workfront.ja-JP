---
product-previous: workfront-fusion
content-type: release-notes
product-area: workfront-integrations
navigation-topic: fusion-release-activity
title: 「Workfront Fusion リリースアクティビティ： 2022 年 11 月 8 日の週」
description: このページでは、2022 年 11 月 8 日の週にAdobe Workfront Fusion でおこなわれたすべての機能強化について説明します。
author: Luke
feature: Product Announcements, Workfront Fusion
recommendations: noDisplay, noCatalog
hidefromtoc: true
exl-id: 802db851-39bb-4f40-8a66-ecb8c8b3ced6
source-git-commit: 76deb76c66e8f8a7dea721378591ae035b8d42e7
workflow-type: tm+mt
source-wordcount: '227'
ht-degree: 0%

---

# Workfront Fusion リリースアクティビティ： 2022 年 11 月 8 日の週

**Webhook キューの最適化**

Fusion の Webhook キューは、このリリースで最適化されました。 Web フックを受け入れるサービスは、キューや他のプロセスとは別のものになりました。 この変更により、Fusion で Webhook キューをより迅速かつ一貫性のある速度で処理できるようになりました。

この変更の実装時に、キューに入れられた Webhook イベントに対して予想されるログ処理時間をより深く理解できました。 Fusion の Webhook ビューアページは 1 分以内にする必要があります。

現在キューに入れられている Webhook イベントを確認するには、左のナビゲーションで Webhook に移動します。 分子に数字が入ったトラックのアイコンは、そのウェブフックのキューイベントを示します。 トラックアイコンをクリックして、キュー内のイベントを表示します。

![](assets/fusion-webhook-queue-1866x567.png)


**未使用のウェブフックは、非アクティブ化または削除されます**

Workfront Fusion での未使用のウェブフックの処理方法をいくつか変更しました。 次のいずれかに該当する場合、wWebhook は自動的に無効化されます。

* Webhook は 5 日以上どのシナリオにも接続されていません。
* Webhook は、非アクティブなシナリオ（30 日以上非アクティブであったシナリオ）でのみ使用されます。

非アクティブ化された Web フックは、シナリオに接続されておらず、30 日以上非アクティブ状態にある場合、自動的に削除され、登録解除されます。
