---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Workfront Data Connectのプライベートリストの登録
description: Snowflakeのプライベートリストを登録して、Workfront Data Connect データを組織のSnowflake アカウントと直接共有します。
author: Courtney
feature: Reports and Dashboards
exl-id:
last-update: 2026-09-15T00:00:00.000Z
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: ed31fce397f9e99e7049d4f55eaca94f43dfcf5c
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 3%
---
# Workfront Data Connectのプライベートリストの登録

非公開リストを登録することで、Workfront Data Connect データを組織のSnowflake アカウントと直接共有できます。 この連携方法は、Snowflakeのプライベートリスト機能を使用して、データを公開することなく、組織間で安全にデータを共有し、地域やホスティングプラットフォームをまたいで機能します。

プライベートリストは、Workfront データをエンタープライズデータウェアハウス内の他のデータと結合する場合に便利です。 データは独自のSnowflakeアカウントに格納されるため、他のデータと組み合わせてクエリすることができます。

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

リストを受け入れ、データベースを作成する権限を持つSnowflake アカウントと、Workfront Data Connectの使用権限も必要です。

## プライベートリストのシェア

プライベートリストでは、次のアクセス権を持ちます。

* Workfrontオブジェクトのデータビューは100を超えています。 各ビューについて詳しくは、[Workfront Data Connect データディクショナリ ](/help/quicksilver/reports-and-dashboards/data-lake/data-dictionary.md)を参照してください。
* データ接続データパイプラインに配信された各変更トランザクションを含む`*_event` データビュー。
* データ拡張可能なオブジェクトのカスタムデータ値。 例については、[Workfront Data Connect クエリの例](/help/quicksilver/reports-and-dashboards/data-lake/basic-query-examples.md)のカスタムデータクエリの例を参照してください。

## リーダーアカウント接続との違い

プライベートリストは、リーダーアカウント接続とは異なるビューのセットを共有し、データは異なるスケジュールで届きます。 次の違いを考慮に入れてください。

* プライベートリストは`*_event` ビューのみを共有します。 `*_current`および`*_daily_history` ビューは、リーダーアカウントを通じて利用できますが、プライベートリストを通じて利用することはできません。 Snowflakeの自分のアカウントで作成できます。 詳しくは、この記事の「[現在および日々の履歴ビューを設定する](#set-up-current-and-daily-history-views)」を参照してください。
* プライベートリストには、リーダーアカウントを通じて利用可能なすべてのビューが含まれない場合があります。 共有されていないビューの例には、Workfront Planning オブジェクト、`MONITORING_DATA_REFRESHES`、`BOOKINGS`、および`CLASSIFIER`があります。 このリストは網羅的ではありません。
* Data Connectは、4時間ごとに変更イベントを読み込みます。 プライベートリストでは、データを表示するために追加のレプリケーション手順が必要なため、データが読み取りアカウントを介して到着するよりも、データが到着するまでに約1時間かかると予想されます。
* データレプリケーションは、01:01、05:01、09:01、13:01、17:01、および21:01 UTCに実行されます。 データは通常、各実行後10分以内に利用できます。
* `MONITORING_DATA_REFRESHES`と`JOB_HISTORY`のビューには、非公開リストを通じてデータが利用可能になる時間が反映されていません。 `JOB_HISTORY` ビューはプライベートリストを通じて共有されますが、失敗したジョブをより迅速に特定するために、リーダーアカウントを通じて読むことをお勧めします。

## 非公開リストを登録

非公開リストを登録するには、まずSnowflake アカウントの詳細を収集し、そのリストをWorkfrontに追加します。

### Snowflake アカウントの詳細の収集

Workfrontでは、Snowflake アカウントの詳細を使用して、アカウントにリストをターゲティングします。 次の詳細を収集します。

* アカウント検索
* アカウント URL
* アカウント組織
* アカウント名

これらの各値は、Snowflakeのアカウントの詳細モーダルから使用できます。

アカウントの詳細を確認するには：

1. Snowflake アカウントにログインしたら、左下隅のユーザーメニューをクリックします。

1. メニューの「**アカウント**」セクションでアカウントを選択します。

1. アカウントの&#x200B;**アカウントの詳細を表示**&#x200B;をクリックします。

1. 上記の各値を記録します。

また、リンクされたWorkfront データにアクセスするデータベースの名前も決めます。 この名前は、リストを登録するときに入力します。

### Workfrontでプライベートリストを追加する

Adobe Workfront インターフェイスを使用してプライベートリストを登録します。

>[!IMPORTANT]
>
>アカウントのロケーターごとに作成できるプライベートリストは1つだけです。

1. Adobe Workfrontの右上隅にある&#x200B;**[!UICONTROL Main Menu]** アイコン ![Main Menu](/help/_includes/assets/main-menu-icon.png)をクリックするか（使用可能な場合）、左上隅にある&#x200B;**[!UICONTROL Main Menu]** アイコン ![Main Menu](/help/_includes/assets/main-menu-icon-left-nav.png)をクリックしてから、**Setup**&#x200B;をクリックします。

1. 左側のパネルで、**システム**/**データ接続**&#x200B;をクリックします。

1. 「**Snowflake connections**」タブをクリックします。

1. 「**プライベートリストを追加**」をクリックします。

1. 必要なデータベース名など、収集したアカウントの詳細をフォームに入力します。

1. 「**プライベートリストを追加**」をクリックします。

### Snowflakeのリストにアクセスします

Snowflake アカウントで、外部データソースとしてプライベートリストへの接続を確立します。 そして、Workfrontのデータを他のデータと組み合わせてクエリすることができます。

## 現在および日次の履歴ビューの設定

リーダーアカウント接続では、各オブジェクトテーブルに対して3つのデータビューが提供されます。

* **現在** — ソースアプリケーションに現在存在するデータの低遅延表現。
* **日別履歴** – 各日のUTC午後11時59分のデータを表します。
* **イベント** – 各変更トランザクションがData Connect データパイプラインに配信されます。

プライベートリストは、イベントビューのみを共有します。 このセクションでは、SQLを使用して、自分のSnowflake アカウントの現在のビュー、日別履歴ビュー、イベントビューを構築できます。

リストに含まれるすべてのイベントビューには、以下のビューロジックに必要なフィールドがあります。 これらの例では、対象のSnowflake アカウントに新しいデータベースとスキーマを作成し、`projects_event` ビューを使用していることを前提としています。 各例では、`<listing_db>`と`<listing_schema>`を独自の値に置き換えます。

>[!TIP]
>
>`select *`は、分析に使用する列のリストに置き換えることをお勧めします。 `select *`を使用し、後でリストのイベントビューに列が追加された場合は、新しい列を有効にするためにビューを再作成する必要があります。

### 現在のビュー

オブジェクトの現在のビューは、Data Connectに保存されている最後の変更イベントレコードです。 最後のレコードが削除済み状態の場合、レコードは現在のビューから省略されます。 すべてのイベントビューは同じ構造です。

```sql
create or replace view projects_current copy grants
as
select *
from <listing_db>.<listing_schema>.projects_event
where end_effective_timestamp = '2300-01-01'::timestamp_ntz
 and nvl(deleted, 0) != 1;
```

現在のビューでは、`deleted`列と`end_effective_timestamp`列は必要ありません。 ビューでは、データが1つの値にフィルタリングされ、レコードが削除されると、レコードが完全に削除されます。

### 日別履歴ビュー

日別履歴ビューでは、特定の日付の23:59:59でアクティブだった変更イベントレコードを特定できるので、レコードの状態を時系列でトレンドできます。 次の例では、各カレンダー日の終わりにプロジェクトレコードの状態を示します。

```sql
create or replace view projects_daily_history copy grants
as
select d.calendardate as
 , p.*
from <listing_db>.<listing_schema>.calendar_dates d
join <listing_db>.<listing_schema>.projects_event p
 on p.begin_effective_timestamp <= d.calendareodtimestamp
and d.calendareodtimestamp < p.end_effective_timestamp
where d.calendareodtimestamp < current_date() - 1
 and nvl(deleted, 0) != 1;
```

### イベントビュー

一貫性を保つために、リストデータベースからイベントビューのコピーを作成し、現在および日々の履歴ビューと同じスキーマに配置することをお勧めします。

```sql
create or replace view projects_event copy grants
as
select *
from <listing_db>.<listing_schema>.projects_event;
```
