---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: スケジュール効率指数（SPI）の計算
description: スケジュール効率指数（SPI）は、予定されたスケジュールと実際のスケジュールとの関係を表します。
author: Lisa
feature: Work Management
exl-id: 38259774-f22b-4b69-9e22-5b541118a7de
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 65%

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

### SPI 値の表示内容 {#what-the-spi-value-shows}

プロジェクトマネージャーは、SPI の値が 1 の場合、プロジェクトが計画中またはスケジュール通りであることを意味することを理解しています。  1 より大きい値はプロジェクトがスケジュールより進んでいることを示し、1 より小さい値はプロジェクトがスケジュールより遅れていることを意味します。  1 からの偏差が大きいほど、プランからの偏差が大きくなります。

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

予定時間数スケジュール累計は、計算を実行する分に計算されます。 現在の日付に予定されている予定時間数が表示されます。 財務データを正確に変更すると、自動的に再計算されます。 Workfrontには、この値を示すフィールドはありません。

例えば、1 つのタスクを含むプロジェクトがあり、そのタスクに 10 の予定時間と 10 日間の期間がある場合、5 日目のスケジュール終了日の予定時間数は 5 です。

## プロジェクトまたはタスクでの SPI の確認

1. SPI を確認するプロジェクトまたはタスクに移動します。
1. プロジェクトとタスクのどちらの SPI を確認するかに応じて、次のいずれかを行います。

   1. 左パネルで「**プロジェクト詳細**」をクリックして、**財務**&#x200B;エリアを表示します。

   1. 左パネルで「**タスクの詳細**」をクリックして、**財務**&#x200B;エリアを表示します。

      ![ プロジェクトの SPI](assets/spi-on-project-nwe.png)

1. 「**CPI/SPI/CSI**」フィールドの値を確認します。
