---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: コストスケジュール効率指数（CSI）の計算
description: コストスケジュール効率指数（CSI）は、コスト効率指数（CPI）とスケジュール効率指数（SPI）を組み合わせて、コストとスケジュールのバランスを取った 1 つの一般的な指標にする自動計算です。
author: Lisa
feature: Work Management
exl-id: 38a8c5e0-b812-499d-8fe7-a71ddccb3aad
source-git-commit: abf5f21281b05dedfecbe71c6ffbf54ee69e2460
workflow-type: tm+mt
source-wordcount: '331'
ht-degree: 65%

---

# コストスケジュール効率指数（CSI）の計算

<!-- Audited: 6/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.) </p>
-->

## コストスケジュール効率指数（CSI）の概要

コストスケジュール効率指数（CSI）は、コスト効率指数（CPI）とスケジュール効率指数（SPI）を組み合わせて、コストとスケジュールのバランスを取った 1 つの一般的な指標にする自動計算です。これらの値を乗算することで、少ない予算で長期に及ぶスケジュールまたはその逆を 1 つの指標で説明することができます。プロジェクトマネージャーは、これを使用して、プロジェクトの途中でスケジュールを立てるためにコストが犠牲になった場合の、一般的なプロジェクトまたはタスクの正常性を判断できます。

>[!TIP]
>
>Adobe Workfrontは、タスクとプロジェクトの両方に対して CSI を計算しますが、イシューには計算しません。

この指標から得られる情報を活用できるのは、組織に次のシナリオが存在する場合のみです。

* ユーザーが完了した作業の時間を記録しています。 これにより、時間数に基づいて CSI が計算されます。
* ユーザーまたは担当業務には、1 時間当たりのコストの割合が関連付けられています。 これにより、コストに基づいて CSI が計算されます。

## Workfront でのコストスケジュール効率指数（CSI）の計算方法

Workfront では、次の式を使用して、プロジェクトまたはタスクのコスト効率指数（CPI）を計算します。

`CSI = CPI x SPI`

CPI について詳しくは、[コスト効率指数（CPI）の計算](../../../manage-work/projects/project-finances/calculate-cpi.md)の記事を参照してください。

SPI について詳しくは、[スケジュール効率指数（SPI）の計算](../../../manage-work/projects/project-finances/calculate-spi.md)を参照してください。

CSI には次の 3 つの値が考えられます。

* 1 = 全体的に計画どおり
* \>1 = 予算とスケジュールの組み合わせ以内
* &lt;1 = 予算とスケジュールの組み合わせを超過

![CSI](assets/csi-highlighted.png)

## コストスケジュール効率指数（CSI）を見つける

>[!CAUTION]
>
>プロジェクトまたはタスクの CSI 値を確認するには、アクセスレベルで財務データを表示するアクセス権と、プロジェクトまたはタスクを表示する権限が必要です。

CSI は、Workfront の次のエリアに表示されます。

* 「プロジェクト詳細」セクションの財務エリア。
* 「タスクの詳細」セクションの財務エリア。
* プロジェクトまたはタスクのビュー。
* プロジェクトまたはタスクレポート。
