---
content-type: api
navigation-topic: api-navigation-topic
title: JSONP のサポートの終了
description: JSONP のサポートの終了
author: Becky
feature: Workfront API
exl-id: 681336c2-2f41-4746-8cba-be077f556742
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '203'
ht-degree: 0%

---

# JSONP のサポートの終了

JSONP（パディング付き JavaScript）は既知のセキュリティ脆弱性を備えた古い標準なので、Adobe Workfrontは 2018 年 11 月以降 JSONP をサポートしなくなります。 この決定は、Workfrontプラットフォームを最新化するためのより大規模なイニシアチブをサポートします。

JSONP は、クロスオリジンまたはクロスサイトのリクエストを実行できる標準です。 Workfrontの多くのお客様およびパートナーは、統合の一環として、JSONP を使用し、独自のドメイン上のシステムからWorkfrontにアクセスします。 JSONP を使用すると、Workfront以外のドメインからのリクエストをWorkfrontアプリケーションで処理できます。

Workfront統合の一部として JSONP を使用している場合は、 CORS（クロスオリジンリソース共有）標準を使用するように統合を更新する必要があります。 この更新では、次の操作をおこなう必要があります。

1. クロスオリジンリクエストをアドビのWorkfrontに対しておこなうために使用されているドメインを持つよう、アドビのアドビサポートチームにリクエストを送信し許可リストます。

   ドメインを CORS 用にWorkfrontに追加するに許可リストは、カスタマーサポート (844-306-HELP(4357)) に問い合わせるか、オンラインでサポートチケットを送信してください。

   >[!NOTE]
   >
   >CORS 用のドメインの許可リストへの追加は、2018 年 8 月 1 日以前に JSONP を使用していたお客様のみサポートされます。


1. CORS を使用するために、統合コードを変更します。
