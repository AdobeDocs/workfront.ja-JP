---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: CSI(Calculate Cost Schedule Performance Index)
description: CSI(Cost Schedule Performance Index) は、CPI(Cost Performance Index) と SPI(Schedule Performance Index) を組み合わせた自動計算で、コストとスケジュールのバランスを取る 1 つの一般的な指標になります。
author: Alina
feature: Work Management
exl-id: 38a8c5e0-b812-499d-8fe7-a71ddccb3aad
source-git-commit: 1cf679376517293f0e0f28b461bd9ecab9283035
workflow-type: tm+mt
source-wordcount: '337'
ht-degree: 0%

---

# CSI(Calculate Cost Schedule Performance Index)

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.) </p>
-->

## CSI(Cost Schedule Performance Index) の概要

CSI(Cost Schedule Performance Index) は、CPI(Cost Performance Index) と SPI(Schedule Performance Index) を組み合わせた自動計算で、コストとスケジュールのバランスを取る 1 つの一般的な指標になります。 これらの値を乗算することで、1 つの指標が低い予算で長期化されたスケジュールを計算したり、その逆を計算したりできます。 プロジェクトマネージャは、この機能を使用して、コストが犠牲になってスケジュール中のプロジェクトを実行する場合に、一般的なプロジェクトまたはタスクの正常性を判断できます。

>[!TIP]
>
>Adobe Workfrontは、タスクとプロジェクトの両方に対して CSI を計算します。 Workfrontは、問題の CSI 値を計算しません。

組織内に次のものが存在する場合にのみ、この指標によって提供される情報のメリットを得ることができます。

* ユーザーが、完了した作業の時間を記録しています。\
  これにより、時間に基づいて CSI が計算されます。
* ユーザーまたはジョブの役割には、時間あたりのコスト率が関連付けられています。 

  これにより、コストに基づいて CSI が計算されます。

## Workfrontが CSI(Cost Schedule Performance Index) を計算する方法

Workfrontは、次の式を使用して、プロジェクトまたはタスクの CSI(Cost Performance Index) を計算します。

`CSI = CPI x SPI`

CPI の詳細については、「 [コスト効果指数 (CPI) の計算](../../../manage-work/projects/project-finances/calculate-cpi.md).

SPI について詳しくは、「 」を参照してください。 [スケジュールパフォーマンスインデックスの計算 (SPI)](../../../manage-work/projects/project-finances/calculate-spi.md).

CSI には次の 3 つの値が考えられます。

* 1 =全体的な計画に従う
* \>1 =予算スケジュールの組み合わせの下
* &lt;1 =予算超過スケジュールの組み合わせ

![](assets/csi-highlighted.png)

## CSI(Cost Schedule Performance Index) を検索します。

>[!CAUTION]
>
>プロジェクトまたはタスクの CSI 値を表示するには、アクセスレベルで財務データの表示へのアクセス権と、プロジェクトまたはタスクを表示する権限が必要です。

CSI は、Workfrontの次の領域で見つけることができます。

* 「プロジェクトの詳細」セクションの財務領域。
* 「タスクの詳細」セクションの財務領域
* プロジェクトまたはタスクビュー
* プロジェクトまたはタスクレポート
