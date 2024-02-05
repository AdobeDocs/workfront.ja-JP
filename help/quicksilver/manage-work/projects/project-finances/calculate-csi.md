---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: コストスケジュール効率指数（CSI）の計算
description: コストスケジュール効率指数（CSI）は、コスト効率指数（CPI）とスケジュール効率指数（SPI）を組み合わせて、コストとスケジュールのバランスを取った 1 つの一般的な指標にする自動計算です。
author: Alina
feature: Work Management
exl-id: 38a8c5e0-b812-499d-8fe7-a71ddccb3aad
source-git-commit: 1cf679376517293f0e0f28b461bd9ecab9283035
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 97%

---

# コストスケジュール効率指数（CSI）の計算

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.) </p>
-->

## コストスケジュール効率指数（CSI）の概要

コストスケジュール効率指数（CSI）は、コスト効率指数（CPI）とスケジュール効率指数（SPI）を組み合わせて、コストとスケジュールのバランスを取った 1 つの一般的な指標にする自動計算です。これらの値を乗算することで、少ない予算で長期に及ぶスケジュールまたはその逆を 1 つの指標で説明することができます。プロジェクトマネージャーは、プロジェクト中盤でスケジュールを推進するためにコストが犠牲になっている場合に、この指標を使用して、プロジェクトやタスクの全般的な健全性を判断することができます。

>[!TIP]
>
>Adobe Workfront では、タスクとプロジェクトの両方に対して CSI を計算します。Workfront では、イシューの CSI 値を計算しません。

この指標から提供される情報を活かすことができるのは、組織内の状況が以下の場合のみです。

* ユーザーが、完了した作業の時間を記録している。\
  これにより、時間数に基づいて CSI が計算されます。
* ユーザーまたは担当業務に 1 時間当たりのコスト率が関連付けられている。 

  これにより、コストに基づいて CSI が計算されます。

## Workfront でのコストスケジュール効率指数（CSI）の計算方法

Workfront では、次の式を使用して、プロジェクトまたはタスクのコスト効率指数（CPI）を計算します。

`CSI = CPI x SPI`

CPI について詳しくは、[コスト効率指数（CPI）の計算](../../../manage-work/projects/project-finances/calculate-cpi.md)の記事を参照してください。

SPI について詳しくは、[スケジュール効率指数（SPI）の計算](../../../manage-work/projects/project-finances/calculate-spi.md)を参照してください。

CSI には次の 3 つの値が考えられます。

* 1 =全体的な計画に従う
* \>1 =予算スケジュールの組み合わせの下
* &lt;1 = 予算とスケジュールの組み合わせを超過

![](assets/csi-highlighted.png)

## コストスケジュール効率指数（CSI）を見つける

>[!CAUTION]
>
>プロジェクトまたはタスクの CSI 値を表示するには、アクセスレベルでの財務データの表示アクセス権と、プロジェクトまたはタスクを表示する権限が必要です。

CSI は、Workfront の次のエリアに表示されます。

* 「プロジェクト詳細」セクションの財務エリア。
* 「タスクの詳細」セクションの財務エリア。
* プロジェクトまたはタスクビュー
* プロジェクトまたはタスクレポート
