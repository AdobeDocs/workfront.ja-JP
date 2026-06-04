---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: コストスケジュール効率指数（CSI）の計算
description: コストスケジュール効率指数（CSI）は、コスト効率指数（CPI）とスケジュール効率指数（SPI）を組み合わせて、コストとスケジュールのバランスを取った 1 つの一般的な指標にする自動計算です。
author: Lisa
feature: Work Management
exl-id: 38a8c5e0-b812-499d-8fe7-a71ddccb3aad
TQID: https://experienceleague.adobe.com/USODdaQOyE-D76BVmLLVUS1WxUMrK6Q05xZU1Xg9Gjc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 332
ht-degree: 71%

---

# コストスケジュール効率指数（CSI）の計算

<!-- Audited: 6/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.) </p>
-->

## コストスケジュール効率指数（CSI）の概要

コストスケジュール効率指数（CSI）は、コスト効率指数（CPI）とスケジュール効率指数（SPI）を組み合わせて、コストとスケジュールのバランスを取った 1 つの一般的な指標にする自動計算です。 これらの値を乗算することで、少ない予算で長期に及ぶスケジュールまたはその逆を 1 つの指標で説明することができます。 プロジェクトマネージャーは、プロジェクト中盤でスケジュールの推進にコストが犠牲になっている場合に、この指標を使用して、プロジェクトやタスクの全般的な健全性を判断できます。

>[!TIP]
>
>Adobe Workfrontでは、タスクとプロジェクトの両方のCSIが計算されますが、問題は計算されません。

この指標によって提供される情報は、組織に次のシナリオが存在する場合にのみ役立ちます。

* ユーザーは完了した作業の時間を記録しています。 これにより、時間数に基づいて CSI が計算されます。
* ユーザーまたは担当業務に関連する時間当たりコスト率があります。 これにより、コストに基づいて CSI が計算されます。

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
>アクセス レベルで財務データを表示するためのアクセス権と、プロジェクトまたはタスクのCSI値を表示するためのプロジェクトまたはタスクを表示するための権限が必要です。

CSI は、Workfront の次のエリアに表示されます。

* 「プロジェクト詳細」セクションの財務エリア。
* 「タスクの詳細」セクションの財務エリア。
* プロジェクトまたはタスクのビュー。
* プロジェクトまたはタスクのレポート：
