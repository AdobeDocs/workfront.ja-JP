---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: 「財務の再計算」アクションがレートが変更された際に履歴時間に影響を与えないようにします
description: （増やしや他の状況が原因で）ユーザーまたはジョブの役割の時間別コストを更新する必要がありますが、この変更が、以前にプロジェクトにログオンした時間に影響を与えたり、過去の時間の一部にのみ影響を与えたりしたい場合は、
author: Alina
feature: Timesheets
exl-id: 29d3124b-cf7a-4a47-95c4-cd5379489810
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: tm+mt
source-wordcount: '188'
ht-degree: 0%

---

# 「財務の再計算」アクションがレートが変更された際に履歴時間に影響を与えないようにします

## 問題

（増やしや他の状況が原因で）ユーザーまたはジョブの役割の時間別コストを更新する必要がありますが、この変更が、以前にプロジェクトにログオンした時間に影響を与えたり、過去の時間の一部にのみ影響を与えたりしたい場合は、

## 解決策

変更しない時間をプロジェクトの請求レコードに追加し、請求レコードのステータスを [ 請求 ] に設定します。  このロックは古いレートでロックされ、[ 財政の再計算 ] アクションでは無視されます。  請求済み請求レコードに属さない時間は、新しい料金で計算されます。 詳しくは、 [プロジェクトの財務を再計算](../../manage-work/projects/project-finances/recalculate-project-finances.md).
