---
content-type: reference
navigation-topic: announcements
title: クラスター 1、2、3 のお客様は、Adobe Workfront サービスのブロックを防ぐために、許可リストの IP ブロックを更新する必要があります。
description: コアインフラストラクチャを強化し改善するには、近日中に、Clusters 01、02 および 03 上の Adobe Workfront のお客様を AWS パブリッククラウドに移行します。
author: Luke
feature: Product Announcements
exl-id: 77d43206-1db7-4075-a063-043f8c9f75ed
TQID: https://experienceleague.adobe.com/I6EiM5bD37m-gC5wyB3DBaOscSTMX-18BpjogM1LcgU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 303
ht-degree: 100%

---

# クラスター 1、2、3 のお客様は、Adobe Workfront サービスのブロックを防ぐために、許可リストの IP ブロックを更新する必要があります。

コアインフラストラクチャを強化し改善するには、近日中に、Clusters 01、02 および 03 上の Adobe Workfront のお客様を AWS パブリッククラウドに移行します。

この変更の一環として、Workfront サービスのブロックを防ぐために、次の IP を許可リストの IP ブロックに追加する必要があります。

SSO および POP の場合は、次のとおりです。

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

メールの場合は、次のとおりです。

* 54.240.60.174
* 54.240.60.175

許可リスト IP ブロックが 2019年5月13日（PT）までに更新されていることを確認してください。 詳しくは、[ファイアウォールの許可リストの設定](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)を参照してください。

お客様にとってより信頼性が高く堅牢なエクスペリエンスを提供するために、Workfront の継続的なサポートにご協力いただき、ありがとうございます。

その他のご質問がございましたら、experience.workfront.com にアクセスするか、844.306.4357（米国）または +44.1256.274200（EMEA）にお電話ください。

## よくある質問

### なぜ Workfront はこの変更を行っているのですか？

Workfront では、お客様に一貫した最高のサービスを提供することを目的に、ユーザーエクスペリエンスの向上方法を常に検討しています。 この変更により、最高のエクスペリエンスを提供し、既に堅牢なセキュリティモデルを改善できる新しいテクノロジーを利用できるようになりました。

### Workfront 管理者としてどのようなアクションが必要ですか？

お客様の許可リスト IP ブロックの確認や上記の IP の追加について詳しくは、社内の IT 部門またはセキュリティ部門にお問い合わせください。

### この変更を行わない場合、組織でどのような影響があると予測されますか？

サービスを新しい IP に移行すると、Workfront サービスにアクセスできなくなります。
