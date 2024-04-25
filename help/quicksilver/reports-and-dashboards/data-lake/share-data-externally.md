---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data lake
title: Workfront Data Lake への接続の確立
description: Workfront データレイクを使用すると、組織のWorkfront データを一般的なビジネスインテリジェンスツールで使用したり、外部データウェアハウスに保存したりできます。
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: e5bd25315062ad15ccd3448e008dfe94f1b616da
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 1%

---

# Workfront Data Lake への接続の確立

Workfront データレイクを使用すると、組織のWorkfront データを business intelligence ツールで使用したり、外部データウェアハウスに保存したりできます。

Workfront Data Lake のデータを外部の商品と結び付けるには、の説明に従ってまず必要な IP を許可リストに追加する必要があります [許可リストに IP を追加](#add-ips-to-the-allowlist) 下。 さらに、ほとんどの製品では、接続を確立するためにデータレイクに関する追加情報が必要になります。

| フィールド名 | 値 |
|---------------|-------------|
| サーバー | 接続の URL （を除く） `https://` 部分（見つかった部分） **データアクセス** Workfrontのページ*） |
| ポート | `443` |
| データベース | `WORKFRONT` |
| ウェアハウス | `READER_WH` |
| スキーマ | `WF` |
| 役割 | `READER_ROLE` |
| ユーザー名 | 接続の作成時に選択したユーザー名（に見つかりました） **データアクセス** Workfrontのページ*） |
| パスワード | 初回Snowflakeログイン時に選択したパスワード* |

*詳細は、 **データアクセス** データレイク接続を含んだページ。を参照してください。 [Snowflake用のリーダー（サービス） アカウントを作成します](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>IP許可リストに 1 つのエントリが追加されると、その他の IP アドレスはすべて許可されなくなります。 ツールを使用する前に、ビジュアライゼーションツールの作成と読み取りの両方で必要な IP アドレスをすべて入力してあることを確認します。 そうでない場合、無効な資格情報に関してエラーが発生する可能性があります。

## 許可リストに IP を追加

1. 「」をクリックします **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon.png) Adobe Workfrontの右上隅、または（利用可能な場合は）をクリックし、 **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png) 左上隅のをクリックし、 **設定**.

1. 左側のパネルで、 **システム** > **データアクセス**.

1. 「」をクリック **許可された IP** タブをクリックしてから、 **許可リストに IP アドレスを追加** ボタン。

1. IP アドレスの名前を **IP アドレスの説明** で使用するツールの IP アドレスを入力します **IP アドレス**&#x200B;を選択し、 **許可リストに IP を追加**.

   ![IP アドレスを追加](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## 許可リストから IP アドレスを削除する

1. 「」をクリックします **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon.png) Adobe Workfrontの右上隅、または（利用可能な場合は）をクリックし、 **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png) 左上隅のをクリックし、 **設定**.

1. 左側のパネルで、 **システム** > **データアクセス**.

1. 「」をクリック **許可された IP** タブをクリックしてから、ごみ箱アイコンをクリックします ![アイコンを削除](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) 削除する IP アドレスの右側に表示されます。

1. 表示されるウィンドウで、チェックボックスをオンにして確認し、 **削除**.

## ビジネスインテリジェンスツールとのデータの共有

一般的なビジネスインテリジェンスツールの多くを以下に示します。リンクをクリックすると、サービスのドキュメントサイトに移動し、データレイクへの接続について詳しく確認できます。

* [Tableau](https://help.tableau.com/current/pro/desktop/en-us/basicconnectoverview.htm)
* [Power BI](https://learn.microsoft.com/power-query/connectors/snowflake)
* [ドモ](https://www.domo.com/appstore/connector/snowflake-connector/overview)
* SAP HANA

## 外部データウェアハウスへのデータの保存

以下に、一般的なデータウェアハウスの数を示します。リンクをクリックすると、各サービスのドキュメントサイトが表示され、データレイクへの接続について詳しく確認できます。

* [Databricks](https://docs.databricks.com/en/connect/index.html)
* [AWS Redshift](https://docs.aws.amazon.com/redshift/latest/gsg/federated-query.html)
