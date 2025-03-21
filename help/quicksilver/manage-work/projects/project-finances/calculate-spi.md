---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: スケジュール効率指数（SPI）の計算
description: スケジュール効率指数（SPI）は、予定されたスケジュールと実際のスケジュールとの関係を表します。
author: Lisa
feature: Work Management
exl-id: 38259774-f22b-4b69-9e22-5b541118a7de
source-git-commit: b983a780198743a2b87b4b48cf4d6afdf1cee437
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 96%

---

# スケジュール効率指数（SPI）の計算

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

スケジュール効率指数（SPI）は、予定されたスケジュールと実際のスケジュールとの関係を表します。Adobe Workfront では、プロジェクトレベルおよびタスクレベルで SPI を計算します。プロジェクトマネージャーは、この指標をレビューして、タスクやプロジェクトが現在スケジュールより進んでいるか遅れているかを追跡します。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
   <p>新規：ライト以上</p>
   <p>または</p>
   <p>現在：レビュー以上</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>プロジェクトおよび財務データへのアクセス権を表示</td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td>財務情報を表示する権限を持つプロジェクトに対する表示以上の権限</td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## スケジュール効率指数（SPI）の概要

* [SPI 値で示される内容](#what-the-spi-value-shows)
* [Workfront による SPI の計算方法](#how-workfront-calculates-spi)

### SPI 値で示される内容 {#what-the-spi-value-shows}

プロジェクト管理者の理解では、SPI 値が 1 の場合、プロジェクトが計画どおりまたはスケジュールどおりであることを意味します。値が 1 より大きい場合は、プロジェクトがスケジュールより早く進行していることを示し、1 未満の場合は、プロジェクトがスケジュールより遅れていることを示しています。1 との違いが大きいほど、計画からのずれが大きくなります。

| **SPI 値** | **指し示すスケジュール状況** |
|---|---|
| 1 | 計画どおりまたはスケジュールどおり |
| > 1（1 より大きい） | スケジュールより早い |
| &lt; 1（1 未満） | スケジュールより遅い |

{style="table-layout:auto"}

### Workfront による SPI の計算方法  {#how-workfront-calculates-spi}

Workfront では次の式で SPI を計算します。

```
SPI = (Total Planned Hours x % Complete) / Planned Hours Scheduled to Date*
```

*&#42;日付までの予定時間数 = 0 の場合、SPI = 1*。

日付までの予定時間数は、計算を実行した時点で分単位で計算されます。現在の日付までに予定されている予定時間数を示します。財務データを変更して正確にすると、自動的に再計算されます。この値を示すフィールドは Workfront にはありません。

例えば、タスクが 1 つのプロジェクトがあり、そのタスクの予定時間数が 10 時間で期間が 10 日間である場合、5 日目の「日付までの予定時間数」は 5 となります。 

## プロジェクトまたはタスクでの SPI の確認

1. SPI を確認するプロジェクトまたはタスクに移動します。
1. プロジェクトとタスクのどちらの SPI を確認するかに応じて、次のいずれかを行います。

   1. 左パネルで「**プロジェクト詳細**」をクリックして、**財務**&#x200B;エリアを表示します。

   1. 左パネルで「**タスクの詳細**」をクリックして、**財務**&#x200B;エリアを表示します。

      ![ プロジェクトの SPI](assets/spi-on-project-nwe.png)

1. 「**CPI/SPI/CSI**」フィールドの値を確認します。
