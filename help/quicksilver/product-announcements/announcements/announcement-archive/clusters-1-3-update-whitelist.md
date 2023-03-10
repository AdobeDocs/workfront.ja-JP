---
content-type: reference
navigation-topic: announcements
title: クラスター 1、2、3 のお客様は、Adobe Workfrontサービスのブロックを防ぐた許可リストめに、すべての IP ブロックを更新する必要があります
description: コアインフラストラクチャを強化し改善するため、近日中に、Clusters 01、02 および 03 上のAdobe Workfrontのお客様をAWSパブリッククラウドに移行します。
author: Luke
feature: Product Announcements
exl-id: 77d43206-1db7-4075-a063-043f8c9f75ed
source-git-commit: 1bc7334423c567ef5f7fd9bcbc28de267e035c0a
workflow-type: tm+mt
source-wordcount: '301'
ht-degree: 4%

---

# クラスター 1、2、3 のお客様は、Adobe Workfrontサービスのブロックを防ぐた許可リストめに、すべての IP ブロックを更新する必要があります

コアインフラストラクチャを強化し改善するため、近日中に、Clusters 01、02 および 03 上のAdobe Workfrontのお客様をAWSパブリッククラウドに移行します。

この変更の一環として、Workfrontサービスのブロックを防ぐため許可リストに、次の IP を IP ブロックに追加する必要があります。

SSO および POP の場合：

* 34.215.145.168
* 54.69.155.48
* 35.160.44.226
* 34.213.96.218
* 3.16.210.22
* 3.16.229.153
* 18.224.117.99
* 3.18.123.153
* 3.211.159.196
* 3.85.255.45
* 3.210.78.197
* 3.211.23.183

メールの場合：

* 54.240.60.174
* 54.240.60.175

IP ブロ許可リストックが 2019 年 5 月 13 日までに更新されていることを確認してください。 詳しくは、 [ファイアウォールの設定を許可リスト行う](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

お客様にとってより信頼性が高く堅牢なエクスペリエンスを提供するために、Workfrontの継続的なサポートにご協力いただき、ありがとうございます。

その他のご質問がある場合は、experience.workfront.com をご覧になるか、844.306.4357（米国）または+44.1256.274200(EMEA) にお電話いただき、サポートチームにお問い合わせください。

## FAQ

### なぜWorkfrontはこの変化を起こしているのでしょうか？

Workfrontでは、常にお客様に可能な限り最高のサービスを提供し続けるために、ユーザーエクスペリエンスを向上させる方法を常に検討しています。 この変更により、最高のエクスペリエンスを提供し、既に堅牢なセキュリティモデルを改善できる新しいテクノロジーを利用できるようになりました。

### Workfront管理者として必要なアクションは何ですか？

お客様の IP ブロックの確認や上記の IP の追加に関し許可リストては、社内の IT 部門またはセキュリティ部門に問い合わせてください。

### この変更を行わない場合、組織は何を期待できますか？

サービスを新しい IP に移行すると、Workfrontサービスにアクセスできなくなります。
