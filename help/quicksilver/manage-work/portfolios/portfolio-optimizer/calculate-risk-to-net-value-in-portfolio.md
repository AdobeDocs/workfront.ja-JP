---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: ポートフォリオ内の純価値に対するリスクを計算
description: ポートフォリオオプティマイザーでは、[!UICONTROL 純価値に対するリスク]指標が、ポートフォリオオプティマイザーに表示されるすべてのプロジェクトによって提供される純価値を考慮して、潜在的なリスクを測定します。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
TQID: https://experienceleague.adobe.com/mClkaUv0y-Y9wiqg4oJivWYtmJDuKG701nOr5TU5rCA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
subfeature_v2: id: c10f2e93-7a58-4212-aa24-684c265ebe76id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 178
ht-degree: 52%

---

# ポートフォリオ内の[!UICONTROL 純価値に対するリスク]の計算

[!UICONTROL Portfolio Optimizer]では、[!UICONTROL 純価値へのリスク ]指標は、[!UICONTROL Portfolio Optimizer]に表示されているすべてのプロジェクトによって提供される[!UICONTROL 純価値]を考慮して、潜在的なリスクを測定します。

ポートフォリオ内で最も効率を高めるには、[!UICONTROL  リスク ]指標が低く、[!UICONTROL 正味値]指標が高いことを確認します。

[!UICONTROL リスク]および[!UICONTROL 純価値]指標は、相互にどのように関係しているかという観点から表現されます。

[!DNL Adobe Workfront] は次の式を使用して [!UICONTROL リスク]および[!UICONTROL 純価値] 指標を計算します。

* [!UICONTROL リスク]指標は次の数式で計算されます。

  ```
  Risk indicator = Risk / (Risk + Net Value)
  ```

* [!DNL Net Value] 指標は、次の数式で計算されます。

  ```
  Net Value indicator = 1 - Risk / (Risk + Net Value)
  ```

  または

  ```
  Net Value indicator = Net Value / (Risk + Net Value)
  ```

>[!NOTE]
>
>[!UICONTROL 純価値に対するリスク ]指標は、[!UICONTROL Portfolio Optimizer]に表示されるプロジェクトに基づいて計算され、ポートフォリオに関連付けられているすべてのプロジェクトに基づいていません。
