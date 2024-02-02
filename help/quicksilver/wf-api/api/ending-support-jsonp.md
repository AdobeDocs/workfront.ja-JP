---
content-type: api
navigation-topic: api-navigation-topic
title: JSONP のサポートの終了
description: JSONP のサポートの終了
author: Becky
feature: Workfront API
role: Developer
exl-id: 681336c2-2f41-4746-8cba-be077f556742
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: ht
source-wordcount: '206'
ht-degree: 100%

---

# JSONP のサポートの終了

JSONP（パディング付き JavaScript）は古い標準であり、既知のセキュリティ脆弱性を持っているので、Adobe Workfront では 2018年11月（PT）をもって JSONP のサポートを停止します。この決定は、Workfront プラットフォームを最新化するためのより大規模なイニシアチブをサポートしています。

JSONP は、異なるオリジンまたは異なるサイトからのリクエストを実行できる標準です。Workfront の多くのお客様とパートナーは、統合の一環として JSONP を使用し、独自のドメイン上のシステムから Workfront にアクセスします。JSONP を使用すると、Workfront 以外のドメインからのリクエストを Workfront アプリケーションで処理できます。

Workfront 統合の一部として JSONP を使用している場合は、CORS（クロスオリジンリソース共有）標準を使用するように統合を更新する必要があります。この更新では、次の操作を行う必要があります。

1. Workfront サポートチームにリクエストを送信して、クロスオリジンリクエストの作成に使用されているドメインを許可リストに追加するように依頼します。

   CORS の許可リストにドメインを追加するには、Workfront カスタマーサポート（844-306-HELP（4357））に問い合わせるか、オンラインでサポートチケットを送信してください。

   >[!NOTE]
   >
   >CORS の許可リストにドメインを追加できるのは、2018年8月1日（PT）より前に JSONP を使用していたお客様のみです。


1. CORS を使用するように、統合コードを変更します。
