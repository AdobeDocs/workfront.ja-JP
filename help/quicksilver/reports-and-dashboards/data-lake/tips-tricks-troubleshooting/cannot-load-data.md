---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Tableau Desktop は接続を確立できません
description: Tableau DesktopをData Connectに接続しようとすると、エラーが発生します。
author: Courtney
feature: Reports and Dashboards
exl-id: 2a25d99a-a05e-4f60-ae1a-51ee137ad5f3
TQID: https://experienceleague.adobe.com/-V1TT-X0FjMm2PIKDy0JVFkvt-A-a7f8fRbVzGzy1jg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11id: d095671a-1355-40aa-8b5f-06c33c68080b
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 253
ht-degree: 5%

---

# Tableau Desktop は接続を確立できません

## 問題

Tableau DesktopをData Connectに接続しようとすると、次のエラーが表示されます。

`Cannot load data into PowerBI. Receiving an HY000 [Microsoft][Snowflake] (25) message`

## 原因

このエラーは、データ接続からデータを読み込めないローカルマシンのプロキシ設定が原因で発生します。

Data Connectは、サードパーティのSnowflake クラウドサービスを通じて提供されます。 Tableauでは、Snowflakeと通信するためにネットワークをオープンにする必要があります。

## ソリューション

この問題を解決するには、次の手順を実行します。

* **セキュリティツールを無効にしてトラブルシューティングする**: ZscalerやCiscoなどのセキュリティツールをオフにして、接続性の問題が解決するかどうかを確認します。 この問題が解決した場合は、セキュリティ ツールが最新バージョンにアップグレードされていることを確認し、社内ネットワーク チームと共にData Connect （Snowflake） IP アドレスをVPN Connectに許可リストに加えるします。

* **IP アドレスを追加**: ファイアウォールの設定で、Data Connectで使用されるIP アドレスが許可されていることを確認します。 コマンド `SYSTEM$ALLOWLIST()`を使用してIP アドレスを取得します。このIP アドレスはVPNで許可リストに加えるできます。

* **ファイアウォールとプロキシ設定を確認**：ネットワーク上のファイアウォールまたはプロキシ設定がSnowflakeのエンドポイントへのアクセスをブロックしているかどうかを確認します。 必要なSnowflake IP アドレスとポートを会社のネットワーク許可リストに追加するには、ネットワーク管理者に連絡する必要がある場合があります。

* **回避策オプション**: TableauのData Source ペインではなく、ワークシート画面から抽出を作成します。 接続が失われず、抽出プロセスが完了します。
