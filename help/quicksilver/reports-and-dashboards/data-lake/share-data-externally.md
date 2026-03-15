---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Connect への接続の確立
description: Workfront Data Connectを使用すると、組織のWorkfrontデータをビジネスインテリジェンスツールで使用したり、外部のデータウェアハウスに保存したりできます。
author: Courtney
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 10%

---

# Workfront Data Connect への接続の確立

Workfront Data Connectを使用すると、組織のWorkfrontデータをビジネスインテリジェンスツールで使用したり、外部のデータウェアハウスに保存したりできます。

Data Connect data Lakeを外部Snowflakeと接続するには、最初に[製品のリーダーアカウントまたは接続を作成する](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)の説明に従って接続を作成する必要があります。 次に、以下の[許可リストへのIPの追加](#add-ips-to-the-allowlist)の説明に従って、許可リストに必要なIPを追加する必要があります。

ほとんどの製品では、接続を確立するために、データレイクに関する次の情報が必要です。

| フィールド名 | 値 |
|---------------|-------------|
| サーバー | `https://`部分を除いた接続のURL (**Data Connect**&#x200B;ページのWorkfront*で見つかりました) |
| ポート | `443` |
| データベース | `WORKFRONT` |
| ウェアハウス | `READER_WH` |
| スキーマ | `WF` |
| 役割 | `READER_ROLE` |
| ユーザー名 | 接続時に選択したユーザー名(**Data Connect**&#x200B;ページのWorkfront*にあります) |
| パスワード | 最初のSnowflakeログイン時に選択されたパスワード* |

*Snowflakeを含む&#x200B;**Data Connect**&#x200B;ページの場所については、[Create a reader account or connection for connection](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)を参照してください。

>[!IMPORTANT]
>
>1つのエントリがIP許可リストに追加されると、他のすべてのIPアドレスは許可されなくなります。 視覚化ツールを使用する前に、視覚化ツールの構築エクスペリエンスと読み取りエクスペリエンスの両方に必要なすべてのIPアドレスを入力するようにしてください。 そうでない場合、無効な資格情報に関するエラーが発生する可能性があります。
>
>許可リストにIPアドレスが含まれていないにもかかわらず、BIツールへの接続に問題がある場合は、BIツールのプロキシサーバーの設定を確認します。

## アクセス要件

+++ 展開してアクセス要件を表示します。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td><p>Ultimate</p>
    <p>ワークフロー Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
   <p>標準</p>
   <p>プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfrontの管理者権限が必要です</p></td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 許可リストへのIPの追加

1. Adobe Workfrontの右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;のアイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックします。または（使用可能な場合）、左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;のアイコン![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)をクリックし、「**設定**」をクリックします。

1. 左側のパネルで、**システム**/**データ接続**&#x200B;をクリックします。

1. 「**許可されたIP**」タブをクリックしてから、「**許可リストにIPアドレスを追加**」ボタンをクリックします。

1. **IPアドレスの説明**&#x200B;にIPアドレスの名前を入力し、**IPアドレス**&#x200B;で使用するツールのIPアドレス（またはCIDRブロック）を入力して、[**許可リストにIPを追加**]をクリックします。

   ![IPアドレスの追加](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## 許可リストからIPアドレスを削除する

1. Adobe Workfrontの右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;のアイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックします。または（使用可能な場合）、左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;のアイコン![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)をクリックし、「**設定**」をクリックします。

1. 左側のパネルで、**システム**/**データ接続**&#x200B;をクリックします。

1. 「**許可されたIP**」タブをクリックしてから、削除するIPアドレスの右側にあるゴミ箱アイコン![削除アイコン](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png)をクリックします。

1. 表示されるウィンドウで、確認するボックスをオンにし、[**削除**]をクリックします。

## ビジネスインテリジェンスツールとのデータ共有

一般的なビジネスインテリジェンスツールのリストを以下に示します。データレイクへの接続について詳しくは、それぞれのドキュメントサイトを参照してください。

* Tableau
* Power BI
* Domo
* SAP HANA

## 外部データウェアハウスにデータを格納する

一般的なデータウェアハウスのリストを以下に示します。データレイクへの接続の詳細については、それぞれのドキュメントサイトを参照してください。

* Databricks
* AWS Redshift
