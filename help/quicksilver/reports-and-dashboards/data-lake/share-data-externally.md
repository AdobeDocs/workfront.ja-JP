---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Connect への接続の確立
description: Workfront Data Connectを使用すると、組織のWorkfront データをビジネスインテリジェンスツールで使用したり、外部のデータウェアハウスに保存したりできます。
author: Courtney
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/pPk3qt9-o3QhAajyI4eGhwe0J2tRphXDstrJxmdW8Ww
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 1489
ht-degree: 4%

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

## Microsoft Power BIのAzure IP範囲を検索する

Microsoft Power BIのData Connectへのトラフィックは、1つの固定アドレスからのものではありません。 Microsoftは、IP範囲を大きなJSON ファイル内のCIDR ブロックとして公開します。 このセクションでは、実際に使用する地域のブロックを見つける方法について説明します。

### AzureのIP範囲とサービスタグ用の公式Microsoft ソース

Microsoftは、[Azure IP範囲とサービスタグ – パブリッククラウドのダウンロードページ &#x200B;](https://www.microsoft.com/en-us/download/details.aspx?id=56519)でリストを公開します。 現在のJSON ファイルをダウンロードします（ファイル名は通常`ServiceTags_Public_YYYYMMDD.json`に似ています）。 Microsoftがこのファイルを更新する場合、またはMicrosoftの変更後に接続性の問題が発生する場合は、の許可リストを更新します。

>[!NOTE]
>
>JSON ファイルは非常に大きく、多くの場合、100,000行を超えます。 今期待されているものです。 必要なセクションは小さいです。手作業でファイル全体を読む必要はありません。

### Power BIとPower Query Onlineの比較

トラフィックが実際にPower Query コンポーネントから発生し、Microsoftがサービスタグリストで個別のAzure サービスとして扱う場合、お客様から「Power BI」と報告されることがあります。

| ユーザーが… | JSONでこのサービスタグを探します |
|----------------|---------------------------------------|
| Power BI サービス、Azureでホストされているデータセット、またはクラウドコンテキストのゲートウェイを使用する | `PowerBI` （`PowerBI.EastUS`などのグローバルまたは地域のエントリ） |
| Power Query Online、クラウドデータフローなどのエクスペリエンスを使用する | `PowerQueryOnline` （`PowerQueryOnline.EastUS`などのグローバルまたは地域のエントリ） |

組織で両方のエクスペリエンスを使用している場合は、同じ地域に`PowerBI`と`PowerQueryOnline`の両方からCIDR ブロックを追加します。 1つしか追加しない場合でも、一部のユーザーはブロックされ、他のユーザーは成功する場合があります。

### グローバル集計ではなく、地域タグを選択します

JSON ファイルには、多数の地域を集約し、数百のCIDR ブロックを含むことができる`PowerBI` （および`PowerQueryOnline`と同様）の単一の全地域エントリと、さらに`PowerBI.WestUS`、`PowerBI.WestUS2`、`PowerBI.WestUS3`などの多数の小さな地域エントリが含まれます。 各地域オブジェクトには、その地域の接頭辞（通常は数十行）のみが一覧表示されます。 すべてのAzure リージョンを許可するための文書化された要件がない限り、グローバルエントリを追加することはお勧めしません。 ほとんどのData Connectのお客様の場合、地域エントリが正しいデフォルトになります。 Power BIのテナントとユーザーが実際に実行しているリージョンと、冗長性の小さなバッファーを追加します（例えば、会社が使用するセカンダリ災害復旧リージョン）。

### 地域の選択

ファイル内のMicrosoftのリージョン名は、`EastUS`、`WestEurope`、`GermanyWestCentral`のようになります。 Power BIのキャパシティとユーザーがホストされているリージョンは、オフィスの場所ではなく、リージョンを使用します。ただし、これらのリージョンは頻繁に調整されます。

| シナリオ | 最初に追加すべきもの |
|----------|-------------------|
| 米国の利用状況 | テナントが使用している米国の地域から開始します（例：`EastUS`、`EastUS2`、`WestUS`、`WestUS2`、`WestUS3`、`CentralUS`、`SouthCentralUS`）。 Microsoftの管理者が複数リージョンのホスティングを確認しない限り、米国のすべてのリージョンは必要ありません。 |
| EUまたは英国での使用 | テナントが使用する地域から開始します（例：`WestEurope`、`NorthEurope`、`FranceCentral`、`GermanyWestCentral`、`SwedenCentral`、`UKSouth`）。 追加のMicrosoft リージョンにまたがるユーザーの場合にのみ追加します。 |
| アジア太平洋地域の利用状況 | Power BIまたはAzure管理者が確認したリージョンを追加します（例：`SoutheastAsia`、`EastAsia`、`AustraliaEast`）。 |
| 複数の地域 | 各サービス （`PowerBI`と`PowerQueryOnline`）に対して、両方の地域タグのセット （EUと米国など）を追加します（両方を使用している場合）。 |
| 不明な地域 | Microsoft 365またはPower BI管理者に、Power BI リソースをホストするAzure リージョンを尋ねるか、Power BI管理者のテナント設定を確認します。 テスト用に素早くブロックを解除する必要がある場合は、既知の地域ペア （例：`EastUS`と`WestUS`）を1つ追加して監視し、確認したらリストを絞り込みます。 |

### IP範囲を見つけて許可リストに追加する

MicrosoftからIP範囲を収集し、Workfront許可リストに追加するには：

1. [Azure IP範囲とサービスタグ – パブリッククラウドのダウンロードページ &#x200B;](https://www.microsoft.com/en-us/download/details.aspx?id=56519)を開き、サービスタグ JSON ファイルをダウンロードし、ローカルに保存します（例：`Downloads\ServiceTags_Public_YYYYMMDD.json`）。

1. Visual Studio Codeなど、大きなJSONを適切に処理する任意のエディターでファイルを開きます。

1. エディターの検索機能（`Ctrl+F` Windows版または`Cmd+F` macOS版）を使用して、`"name"` フィールドが`PowerBI.EastUS`や`PowerQueryOnline.WestEurope`などのサービスタグに等しいJSON オブジェクトを検索します。 便利な検索：

   * `"name": "PowerBI.WestUS"` – 米国Power BI西部にジャンプします。
   * `"name": "PowerQueryOnline.WestUS"` — West US Power Query Onlineに移動します。
   * `PowerBI.` – すべてのPower BI地域タグを一覧表示してから、リージョン名に絞り込みます。

1. 一致する各オブジェクトの下で、`addressPrefixes`という名前の配列を見つけます。 その配列内の各文字列はCIDR ブロックです（例：`20.59.79.96/27`またはIPv6 プレフィックス）。 許可リストに加える価値は、次のとおりです。

1. この記事の「[IPを許可リストに追加](#add-ips-to-the-allowlist)」の説明に従って、各CIDRをアドビの組織に追加します。 環境がルールをキャッシュする場合は、数分だけポリシーの反映を許可します。

1. Power BIまたはPower Query Onlineから、Data Connectに対して小さなテストクエリを実行して、接続を検証します。 失敗した場合は、おおよその時間を取得し、拒否が欠落している範囲に一致するかどうかをネットワークチームに尋ねます。 共通のギャップである`PowerBI`のみが追加されたときに`PowerQueryOnline`を見逃したかどうかを再確認します。

例えば、Microsoftの管理者が、Power BIのワークロードでWest US、West US 2、West US 3が使用され、ユーザーがPower BIとPower Query Onlineの両方を使用していることを確認した場合、それぞれ`PowerBI.WestUS`、`PowerBI.WestUS2`、`PowerBI.WestUS3`および一致する`PowerQueryOnline.<Region>`の6つのオブジェクトを開き、6つすべてから`addressPrefixes`をコピーします。

### JSON構造参照

各サービスタグブロックは、概念的には次のようになります。 実際のファイルには、より多くのメタデータが含まれます。

```json
{
  "name": "PowerBI.WestUS2",
  "id": "PowerBI.WestUS2",
  "properties": {
    "region": "westus2",
    "systemService": "PowerBI",
    "addressPrefixes": [
      "203.0.113.0/24",
      "2001:db8::/32"
    ],
    "networkFeatures": ["API", "NSG", "UDR", "FW"]
  }
}
```

`addressPrefixes`配列には、Workfrontに追加するCIDR ブロックが含まれています。 その他のフィールドはAzureのネットワークシナリオ用で、ここでは適用されません。

### 「許可リストに加える」を維持する

* Microsoftは、IP範囲を経時的に変更します。 Microsoftが更新されたJSON ファイルを公開する場合、特に接続性インシデントの後は、定期的に更新または比較します。
* 環境でIPv6からSnowflakeへのIPv6がサポートされており、MicrosoftでIPv6のプレフィックスが一覧表示されている場合は、セキュリティポリシーでIPv6が許可されている場合に含めます。 それ以外は、ネットワークチームと調整してください。

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
