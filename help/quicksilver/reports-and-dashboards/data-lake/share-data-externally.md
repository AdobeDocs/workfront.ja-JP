---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Connect への接続の確立
description: Workfront Data Connectを使用すると、組織のWorkfront データをビジネスインテリジェンスツールで使用したり、外部のデータウェアハウスに保存したりできます。
author: Courtney
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 10%

---

# Workfront Data Connect への接続の確立

Workfront Data Connectを使用すると、組織のWorkfront データをビジネスインテリジェンスツールで使用したり、外部のデータウェアハウスに保存したりできます。

Data Connect データレイクを外部製品に接続するには、まず、[Snowflakeのリーダーアカウントまたは接続の作成](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)の説明に従って、接続を作成する必要があります。 次に、必要なIPを許可リストに追加する必要があります。詳細については、以下の「[IPを許可リストに追加](#add-ips-to-the-allowlist)」を参照してください。

多くの製品では、接続を確立するために、データレイクに関する次の情報が必要です。

| フィールド名 | 値 |
|---------------|-------------|
| サーバー | `https://`部分を含まない接続のURL （**Data Connect** Workfront*） |
| ポート | `443` |
| データベース | `WORKFRONT` |
| ウェアハウス | `READER_WH` |
| スキーマ | `WF` |
| 役割 | `READER_ROLE` |
| ユーザー名 | 接続の作成時に選択されたユーザー名（Workfrontの&#x200B;**Data Connect** ページにあります*） |
| パスワード | Snowflakeの初回起動時に選択したパスワード* |

* 接続を含む&#x200B;**Data Connect** ページの検索場所については、[Snowflakeのリーダーアカウントまたは接続の作成](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md)を参照してください。

>[!IMPORTANT]
>
>1つのエントリがIP アドレスに追加されると、他のすべてのIP アドレスは許可されなくなります。 ビジュアライゼーションツールを使用する前に、ビジュアライゼーションツールの構築と読み取りの両方に必要なすべてのIP アドレスを入力していることを確認してください。 そうでない場合は、無効な資格情報に関するエラーが発生する可能性があります。
>
>お使いのBI ツールにIP アドレスが含まれていないにもかかわらず、BI ツールへの接続に問題がある場合は、BI ツールのプロキシサーバー設定を確認してください。

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
   <td> <p>あなたはWorkfrontの管理者でなければなりません</p></td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 「IP」を許可リストに追加する

1. Adobe Workfrontの右上隅にある&#x200B;**[!UICONTROL Main Menu]** アイコン ![Main Menu](/help/_includes/assets/main-menu-icon.png)をクリックするか（使用可能な場合）、左上隅にある&#x200B;**[!UICONTROL Main Menu]** アイコン ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png)をクリックしてから、**Setup**&#x200B;をクリックします。

1. 左側のパネルで、**システム**/**データ接続**&#x200B;をクリックします。

1. 「**許可されたIP**」タブをクリックし、「**IP アドレスを契約許可リストに追加**」ボタンをクリックします。

1. 「**IP アドレスの説明**」にIP アドレスの名前を入力し、**IP アドレス**&#x200B;で使用するツールのIP アドレス（またはCIDR ブロック）を入力してから、**IP アドレスの追加**&#x200B;をクリックします。

   ![IP アドレスを追加](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## 「IP アドレス」を許可リストから削除する

1. Adobe Workfrontの右上隅にある&#x200B;**[!UICONTROL Main Menu]** アイコン ![Main Menu](/help/_includes/assets/main-menu-icon.png)をクリックするか（使用可能な場合）、左上隅にある&#x200B;**[!UICONTROL Main Menu]** アイコン ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png)をクリックしてから、**Setup**&#x200B;をクリックします。

1. 左側のパネルで、**システム**/**データ接続**&#x200B;をクリックします。

1. **許可されたIP** タブをクリックし、削除するIP アドレスの右側にあるゴミ箱アイコン ![削除アイコン &#x200B;](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png)をクリックします。

1. 表示されるウィンドウで、チェックボックスをオンにして確認し、**削除**&#x200B;をクリックします。

## ビジネスインテリジェンスツールとデータを共有

一般的なビジネスインテリジェンスツールの多くを以下に示します。データレイクへの接続について詳しくは、そのドキュメントサイトを参照してください。

* Tableau
* Power BI
* ドモ
* SAP HANA

## 外部データウェアハウスにデータを保存する

一般的なデータウェアハウスの多くを以下に示します。データレイクへの接続について詳しくは、同社のドキュメントサイトを参照してください。

* Databricks
* AWS Redshift
