---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: ポートフォリオ内の純価値に対するリスクを計算
description: ポートフォリオオプティマイザーでは、[!UICONTROL 純価値に対するリスク]指標が、ポートフォリオオプティマイザーに表示されるすべてのプロジェクトによって提供される純価値を考慮して、潜在的なリスクを測定します。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 52%

---

# ポートフォリオ内の[!UICONTROL 純価値に対するリスク]の計算

[!UICONTROL Portfolio Optimizer] では、[!UICONTROL  純価に対するリスク ] 指標は、[!UICONTROL Portfolio Optimizer] に表示されるすべてのプロジェクトから提供される [!UICONTROL  純価 ] を考慮して潜在的なリスクを測定します。

ポートフォリオ内で最も効率を高めるには、[!UICONTROL  リスク ] インジケーターが低く、[!UICONTROL  純価 ] インジケーターが高くなるようにしたいと考えています。

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
>[!UICONTROL  純価値に対するリスク ] インジケーターは、ポートフォリオに関連付けられたすべてのプロジェクトではなく、[!UICONTROL Portfolio Optimizer] に表示されるプロジェクトに基づいて計算されます。
