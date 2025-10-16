---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: スケジュール効率指数（SPI）の計算
description: スケジュール効率指数（SPI）は、予定されたスケジュールと実際のスケジュールとの関係を表します。
author: Lisa
feature: Work Management
exl-id: 38259774-f22b-4b69-9e22-5b541118a7de
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 94%

---

# スケジュール効率指数（SPI）の計算

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

スケジュール効率指数（SPI）は、予定されたスケジュールと実際のスケジュールとの関係を表します。Adobe Workfront では、プロジェクトレベルおよびタスクレベルで SPI を計算します。プロジェクトマネージャーは、この指標をレビューして、タスクやプロジェクトが現在スケジュールより進んでいるか遅れているかを追跡します。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td>
   <p>ライト以上</p>
   <p>レビュー以上</p></td>  
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>プロジェクトおよび財務データへのアクセス権を表示</td> 
  </tr> 
  <tr> 
   <td>オブジェクト権限</td> 
   <td>財務情報を表示する権限を持つプロジェクトに対する表示以上の権限</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

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

      ![&#x200B; プロジェクトの SPI](assets/spi-on-project-nwe.png)

1. 「**CPI/SPI/CSI**」フィールドの値を確認します。
