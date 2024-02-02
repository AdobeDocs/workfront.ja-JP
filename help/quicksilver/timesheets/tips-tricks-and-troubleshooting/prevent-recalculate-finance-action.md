---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: レートが変更された際に財務の再計算アクションが履歴時間に影響するのを防ぐ
description: ユーザーまたは担当業務の時間別コストを更新する必要がありますが（増加や他の状況が原因で）、この変更により、以前にプロジェクトにログオンした時間に影響を与えたくない、もしくは過去の時間の一部にのみ影響を与えたいと思っています。
author: Alina
feature: Timesheets
exl-id: 29d3124b-cf7a-4a47-95c4-cd5379489810
source-git-commit: 7786d899841cb82cc4d3832fb083c6e2bda2e197
workflow-type: ht
source-wordcount: '188'
ht-degree: 100%

---

# レートが変更された際に財務の再計算アクションが履歴時間に影響するのを防ぐ

## 問題

ユーザーまたは担当業務の時間別コストを更新する必要がありますが（増加や他の状況が原因で）、この変更により、以前にプロジェクトにログオンした時間に影響を与えたくない、もしくは過去の時間の一部にのみ影響を与えたいと思っています。

## ソリューション

変更しない時間をプロジェクトの請求記録に追加し、請求記録のステータスを「請求済み」に設定します。このロックは古いレートでロックされており、財務の再計算アクションでは無視されます。請求済み請求記録に属さない時間は、新しいレートで計算されます。詳しくは、[プロジェクトの財務を再計算](../../manage-work/projects/project-finances/recalculate-project-finances.md)を参照してください。
