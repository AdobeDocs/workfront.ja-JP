---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: スケジュール効率指数（SPI）の計算
description: スケジュール効率指数（SPI）は、予定されたスケジュールと実際のスケジュールとの関係を表します。
author: Lisa
feature: Work Management
exl-id: 38259774-f22b-4b69-9e22-5b541118a7de
TQID: https://experienceleague.adobe.com/WfZDTGfYIcngo8a3MQAh-Z7jnKm4nnBppV8hYSweygo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 398
ht-degree: 62%

---

# スケジュール効率指数（SPI）の計算

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

スケジュール効率指数（SPI）は、予定されたスケジュールと実際のスケジュールとの関係を表します。 Adobe Workfront では、プロジェクトレベルおよびタスクレベルで SPI を計算します。 プロジェクトマネージャーは、この指標をレビューして、タスクやプロジェクトが現在スケジュールより進んでいるか遅れているかを追跡します。

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
   <p>明るいまたはそれ以上</p>
   <p>レビュー以上</p></td>  
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>プロジェクトおよび財務データへのアクセス権を表示</td> 
  </tr> 
  <tr> 
   <td>オブジェクト権限</td> 
   <td>一般財務を表示する権限を持つプロジェクトに対する表示以上の権限</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## スケジュール効率指数（SPI）の概要

* [SPI 値で示される内容](#what-the-spi-value-shows)
* [Workfront による SPI の計算方法](#how-workfront-calculates-spi)

### SPI値の表示 {#what-the-spi-value-shows}

プロジェクトマネージャーは、SPI値が1であるということは、プロジェクトが計画通りに進んでいるか、スケジュール通りに進んでいることを意味します。  1より大きい値は、プロジェクトがスケジュールより前に進んでいることを示し、1より小さい値は、プロジェクトがスケジュールより遅れていることを示します。  1 からの偏差が大きいほど、プランからの偏差が大きくなります。

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

予定時間数スケジュール日は、計算を実行した分に計算されます。 現在の日付に対して計画された予定時間数が表示されます。 財務データを正確に変更すると、自動的に再計算されます。 Workfrontには、この値を示すフィールドはありません。

例えば、1つのタスクを含むプロジェクトがあり、そのタスクに10の予定時間と10日間の期間がある場合、5日目の予定時間数スケジュールは5です。

## プロジェクトまたはタスクでの SPI の確認

1. SPI を確認するプロジェクトまたはタスクに移動します。
1. プロジェクトとタスクのどちらの SPI を確認するかに応じて、次のいずれかを行います。

   1. 左パネルで「**プロジェクト詳細**」をクリックして、**財務**&#x200B;エリアを表示します。

   1. 左パネルで「**タスクの詳細**」をクリックして、**財務**&#x200B;エリアを表示します。

      プロジェクト ![&#128279;](assets/spi-on-project-nwe.png)のSPI

1. 「**CPI/SPI/CSI**」フィールドの値を確認します。
