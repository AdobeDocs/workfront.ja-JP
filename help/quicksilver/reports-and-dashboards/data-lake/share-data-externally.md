---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Lake への接続の確立
description: Workfront データレイクを使用すると、組織のWorkfront データを一般的なビジネスインテリジェンスツールで使用したり、外部データウェアハウスに保存したりできます。
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: 16809b2d1801dd7aa4ab1f452e4687601fc1ac59
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 1%

---

# Workfront Data Connect への接続の確立

Workfront Data Connect を使用すると、組織のWorkfront データをビジネスインテリジェンスツールで使用したり、外部データウェアハウスに保存したりできます。

Data Connect Data Lake を外部許可リスト許可リストに加えるに接続するには、以下の [Add IPs to the](#add-ips-to-the-allowlist) で説明されているように、最初に必要な IP を製品に追加する必要があります。 さらに、ほとんどの製品では、接続を確立するためにデータレイクに関する追加情報が必要になります。

| フィールド名 | 値 |
|---------------|-------------|
| サーバー | `https://` 部分を除いた接続用の URL （Workfront*の **データアクセス** ページにあります） |
| ポート | `443` |
| データベース | `WORKFRONT` |
| ウェアハウス | `READER_WH` |
| スキーマ | `WF` |
| 役割 | `READER_ROLE` |
| ユーザー名 | 接続時に選択したユーザー名（Workfront*の **データアクセス** ページで確認できます） |
| パスワード | 初回Snowflakeログイン時に選択したパスワード* |

*Data ConnectSnowflakeを含む **データアクセス** ページの場所については、[ 接続用のリーダー（サービス）アカウントの作成 ](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md) を参照してください。

>[!IMPORTANT]
>
>IP許可リストに 1 つのエントリが追加されると、その他の IP アドレスはすべて許可されなくなります。 ツールを使用する前に、ビジュアライゼーションツールの作成と読み取りの両方で必要な IP アドレスをすべて入力してあることを確認します。 そうでない場合、無効な資格情報に関してエラーが発生する可能性があります。
>
>許可リストに IP アドレスが含まれていなくても、BI ツールへの接続に問題がある場合は、BI ツールのプロキシサーバー設定を確認します。

## 許可リストに IP を追加

1. Adobe Workfrontの右上隅にある **[!UICONTROL メインメニュー]** アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon.png) をクリックするか、可能な場合は）右上隅にある **[!UICONTROL メインメニュー]** アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックしてから、**設定** をクリックします。

1. 左側のパネルで、**システム**/**データアクセス** をクリックします。

1. 「**許可されている IP**」タブをクリックし、「**許可リストに IP アドレスを追加**」ボタンをクリックします。

1. 許可リストに加える **IP アドレスの説明** に IP アドレスの名前を入力し、**IP アドレス** で使用するツールの IP アドレス（または CIDR ブロック）を入力してから、「**IP を追加**」をクリックします。

   ![IP アドレスの追加 ](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## 許可リストから IP アドレスを削除する

1. Adobe Workfrontの右上隅にある **[!UICONTROL メインメニュー]** アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon.png) をクリックするか、可能な場合は）右上隅にある **[!UICONTROL メインメニュー]** アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックしてから、**設定** をクリックします。

1. 左側のパネルで、**システム**/**データアクセス** をクリックします。

1. 「**許可されている IP**」タブをクリックし、削除する IP アドレスの右側にあるごみ箱アイコン ![ 削除アイコン ](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) をクリックします。

1. 表示されるウィンドウで、チェックボックスをオンにして「**削除**」をクリックします。

## ビジネスインテリジェンスツールとのデータの共有

一般的なビジネスインテリジェンスツールの多くを以下に示します。リンクをクリックすると、サービスのドキュメントサイトに移動し、データレイクへの接続について詳しく確認できます。

* [Tableau](https://help.tableau.com/current/pro/desktop/en-us/basicconnectoverview.htm)
* [Power BI](https://learn.microsoft.com/power-query/connectors/snowflake)
* [ ドモ ](https://www.domo.com/appstore/connector/snowflake-connector/overview)
* SAP HANA

## 外部データウェアハウスへのデータの保存

以下に、一般的なデータウェアハウスの数を示します。リンクをクリックすると、各サービスのドキュメントサイトが表示され、データレイクへの接続について詳しく確認できます。

* [Databricks](https://docs.databricks.com/en/connect/index.html)
* [AWS Redshift](https://docs.aws.amazon.com/redshift/latest/gsg/federated-query.html)
