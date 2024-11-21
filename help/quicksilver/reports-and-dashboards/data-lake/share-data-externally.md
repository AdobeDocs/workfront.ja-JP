---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Connect への接続の確立
description: Workfront Data Connect を使用すると、組織のWorkfront データをビジネスインテリジェンスツールで使用したり、外部データウェアハウスに保存したりできます。
author: Nolan
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: 7b50876f1be16473704eddeb3157dacfacd96e90
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 9%

---

# Workfront Data Connect への接続の確立

Workfront Data Connect を使用すると、組織のWorkfront データをビジネスインテリジェンスツールで使用したり、外部データウェアハウスに保存したりできます。

Data Connect Data Lake を外部Snowflakeと接続するには、まず「製品のリーダーアカウントまたは接続の作成 [ の説明に従って接続を作成する必要があり ](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md) す。 次に、以下の [許可リスト許可リストに加えるへの IP の追加 ](#add-ips-to-the-allowlist) で説明するように、必要な IP をページに追加する必要があります。

ほとんどの製品では、接続を確立するために、データレイクに関する次の情報が必要です。

| フィールド名 | 値 |
|---------------|-------------|
| サーバー | `https://` 部分を除いた接続用の URL （Workfront*の **Data Connect** ページにあります） |
| ポート | `443` |
| データベース | `WORKFRONT` |
| ウェアハウス | `READER_WH` |
| スキーマ | `WF` |
| 役割 | `READER_ROLE` |
| ユーザー名 | 接続の作成時に選択したユーザー名（Workfront*の **Data Connect** ページにあります） |
| パスワード | 初回Snowflakeログイン時に選択したパスワード* |

*Snowflakeを含む **Data Connect** ページの見つけ方については、[Create a reader account or connection for connection](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md) を参照してください。

>[!IMPORTANT]
>
>IP許可リストに 1 つのエントリが追加されると、その他の IP アドレスはすべて許可されなくなります。 ツールを使用する前に、ビジュアライゼーションツールの作成と読み取りの両方で必要な IP アドレスをすべて入力してあることを確認します。 そうでない場合、無効な資格情報に関してエラーが発生する可能性があります。
>
>許可リストに IP アドレスが含まれていなくても、BI ツールへの接続に問題がある場合は、BI ツールのプロキシサーバー設定を確認します。

## アクセス要件

+++ 展開すると、アクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>次のプランに含まれる：</p>
    <ul>
        <li>Ultimate</li> 
    </ul>    
   <p>次のプランのアドオンとして購入できます。</p> 
    <ul>
        <li>選択</li> 
        <li>Prime</li>
    </ul> 
    <p>Workfront Data Connect は、従来のWorkfront プランでは使用できません。</p> 
   </td> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p></td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 許可リストに IP を追加

1. Adobe Workfrontの右上隅にある **[!UICONTROL メインメニュー]** アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon.png) をクリックするか、可能な場合は）右上隅にある **[!UICONTROL メインメニュー]** アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックしてから、**設定** をクリックします。

1. 左側のパネルで、**システム**/**データ接続** をクリックします。

1. 「**許可されている IP**」タブをクリックし、「**許可リストに IP アドレスを追加**」ボタンをクリックします。

1. 許可リストに加える **IP アドレスの説明** に IP アドレスの名前を入力し、**IP アドレス** で使用するツールの IP アドレス（または CIDR ブロック）を入力してから、「**IP を追加**」をクリックします。

   ![IP アドレスの追加 ](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## 許可リストから IP アドレスを削除する

1. Adobe Workfrontの右上隅にある **[!UICONTROL メインメニュー]** アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon.png) をクリックするか、可能な場合は）右上隅にある **[!UICONTROL メインメニュー]** アイコン ![ メインメニュー ](/help/_includes/assets/main-menu-icon-left-nav.png) をクリックしてから、**設定** をクリックします。

1. 左側のパネルで、**システム**/**データ接続** をクリックします。

1. 「**許可されている IP**」タブをクリックし、削除する IP アドレスの右側にあるごみ箱アイコン ![ 削除アイコン ](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) をクリックします。

1. 表示されるウィンドウで、チェックボックスをオンにして「**削除**」をクリックします。

## ビジネスインテリジェンスツールとのデータの共有

以下に、一般的なビジネスインテリジェンスツールの一覧を示します。データレイクへの接続について詳しくは、ドキュメントサイトを参照してください。

* Tableau
* Power BI
* ドモ
* SAP HANA

## 外部データウェアハウスへのデータの保存

以下に、一般的なデータウェアハウスの数を示します。データレイクへの接続について詳しくは、ドキュメントサイトを参照してください。

* Databricks
* AWS Redshift
