---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: スケジュールパフォーマンスインデックスの計算 (SPI)
description: SPI(Schedule Performance Index) は、計画済スケジュールと実際のスケジュールとの関係を表します。
author: Alina
feature: Work Management
exl-id: 38259774-f22b-4b69-9e22-5b541118a7de
source-git-commit: a55041ad5a6cd41cd11ec3ade27bf5227ae0ac47
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 1%

---

# スケジュールパフォーマンスインデックスの計算 (SPI)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

SPI(Schedule Performance Index) は、計画済スケジュールと実際のスケジュールとの関係を表します。 Adobe Workfrontは、プロジェクトとタスクのレベルで SPI を計算します。 プロジェクトマネージャーは、この指標をレビューして、現在、タスクまたはプロジェクトがスケジュールを前倒ししているかどうかを特定します。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトおよび財務データへのアクセスの表示</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>財務を表示する権限を持つプロジェクトに対する表示権限以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## スケジュールパフォーマンスインデックス (SPI) の概要

* [SPI 値に表示される内容](#what-the-spi-value-shows)
* [Workfrontによる SPI の計算方法](#how-workfront-calculates-spi)

### SPI 値に表示される内容 {#what-the-spi-value-shows}

プロジェクト管理者は、SPI 値が 1 の場合、プロジェクトが計画中または予定通りであることを意味します。  1 より大きい値は、プロジェクトがスケジュールより早いことを示し、1 より小さい値は、プロジェクトがスケジュールより遅れていることを示します。  1 からの偏差が大きいほど、プランからの偏差が大きくなります。

| **SPI 値** | **「予定通り」の表示** |
|---|---|
| 1 | 計画またはスケジュールに従って |
| > 1 （1 より大きい） | 予定より前 |
| &lt; 1 （1 未満） | スケジュール遅れ |

{style=&quot;table-layout:auto&quot;}

### Workfrontによる SPI の計算方法  {#how-workfront-calculates-spi}

Workfrontは次の式で SPI を計算します。

```
SPI = (Total Planned Hours x % Complete) / Planned Hours Scheduled to Date*
```

*&#42;予定時間の予定日= 0 の場合、SPI = 1*.

計画時間スケジュール：日付は、計算を実行する時点で計算されます。 現在の日付に予定されている計画時間数が表示されます。 財務データを正確に変更した場合は、自動的に再計算できます。 この値を示すフィールドがWorkfrontにありません。

例えば、1 つのタスクを持つプロジェクトがあり、タスクに 10 時間の予定と 10 日間の期間がある場合、5 日目の予定時間スケジュールは 5 となります。 

## プロジェクトまたはタスクで SPI を検索する

1. SPI を表示するプロジェクトまたはタスクに移動します。
1. プロジェクトとタスクのどちらで SPI を表示するかに応じて、次のいずれかの操作を行います。

   1. クリック **プロジェクトの詳細** 左のパネルで、 **金融** 領域

   1. クリック **タスクの詳細** 左のパネルで、 **金融** 領域

      ![](assets/spi-on-project-nwe.png)

1. 次を検索： **CPI/SPI/CSI** フィールドに入力します。
