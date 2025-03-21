---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Tableau Desktop は接続を確立できません
description: Tableau Desktop をデータ接続に接続しようとすると、エラーが発生します。
author: Courtney
feature: Reports and Dashboards
source-git-commit: e8b1d553ac4761e2b6eae79ae384956105939d90
workflow-type: tm+mt
source-wordcount: '252'
ht-degree: 1%

---


# Tableau Desktop は接続を確立できません

## 問題

Tableau Desktop をデータ接続に接続しようとすると、次のエラーが表示されます。

`Cannot load data into PowerBI. Receiving an HY000 [Microsoft][Snowflake] (25) message`

## 原因

このエラーは、ローカルマシンのプロキシ設定により、データ接続からデータが読み込まれないことが原因です。

Data Connect はサードパーティのSnowflake クラウドサービスを通じて提供されます。 Tableau では、Snowflakeとの通信にネットワークを開放する必要があります。

## ソリューション

この問題を解決するには、次の手順を試してください。

* **セキュリティツールを無効にしてトラブルシューティングを行う**: Zscaler や Cisco などのセキュリティツールをオフにして、接続の問題が解決するかどうかを確認します。 接続の問題が解決した場合は、セキュリティ ツールが最新バージョンにアップグレードされていることを確認し、Data Connect （Snowflake）の IP アドレスを社内ネットワーク チームと VPN許可リストに追加します。

* **ファイアウォールに IP アドレスを追加**: 許可リスト設定で Data Connect が使用する IP アドレスが許可されていることを確認します。 コマンド `SYSTEM$ALLOWLIST()` を使用して IP アドレスを取得し、VPN に許可リストに加えるします。

* **ファイアウォールおよびプロキシ設定の確認**：ネットワーク上のファイアウォールまたはプロキシ設定がSnowflakeのエンドポイントへのアクセスをブロックしているかどうかを確認します。 場合によっては、ネットワーク管理者に問い合わせて、必要なSnowflakeの IP アドレスとポートを会社の許可リストに追加する必要があります。

* **回避策オプション**:Tableau のデータSourceペインではなく、ワークシート画面からエクストラクトを作成します。 接続は失われず、抽出プロセスが完了します。

