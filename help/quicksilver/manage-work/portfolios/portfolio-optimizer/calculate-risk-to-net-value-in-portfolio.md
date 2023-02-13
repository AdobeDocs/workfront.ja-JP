---
product-area: portfolios
navigation-topic: portfolio-optimizer
title: ポートフォリオ内の純価値に対するリスクを計算
description: Portfolio・オプティマイザで、 [!UICONTROL 純価値に対するリスク] 指標は、Potential Risk を測定します。Potential Optimizer に表示されるすべてのプロジェクトで提供される純値を考慮に入れます。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 9e86f6eb-dd82-4731-aebb-ce8da1df5614
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '178'
ht-degree: 0%

---

# 次を計算： [!UICONTROL 純価値に対するリスク] ポートフォリオ内

内 [!UICONTROL Portfolio最適化]、 [!UICONTROL 純価値に対するリスク] 指標は、 [!UICONTROL 正味値] が [!UICONTROL Portfolio最適化]. 

ポートフォリオ内で最も効率的なを実現するには、 [!UICONTROL リスク] 指標が低く、 [!UICONTROL 正味値] インジケータが高い。 

この [!UICONTROL リスク] および [!UICONTROL 正味値] 指標は、相互にどのように関係しているかという観点から表現されます。

[!DNL Adobe Workfront] は [!UICONTROL リスク] および [!UICONTROL 正味値] 次の式を使用する指標：

* この [!UICONTROL リスク] 指標は次の数式で計算されます。

   ```
   Risk indicator = Risk / (Risk + Net Value)
   ```

* この [!DNL Net Value] 指標は、次の数式で計算されます。

   ```
   Net Value indicator = 1 - Risk / (Risk + Net Value)
   ```

   または

   ```
   Net Value indicator = Net Value / (Risk + Net Value)
   ```

>[!NOTE]
>
>この [!UICONTROL 純価値に対するリスク] 指標は、 [!UICONTROL Portfolio最適化]（ポートフォリオに関連付けられているすべてのプロジェクトに対して）ではなく、 
