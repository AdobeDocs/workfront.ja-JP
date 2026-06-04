---
content-type: tips-tricks-troubleshooting
product-area: timesheets
navigation-topic: tips-tricks-and-troubleshooting-timesheets
title: レートが変更された際に財務の再計算アクションが履歴時間に影響するのを防ぐ
description: ユーザーまたは担当業務の時間別コストを更新する必要がありますが（増加や他の状況が原因で）、この変更により、以前にプロジェクトにログオンした時間に影響を与えたくない、もしくは過去の時間の一部にのみ影響を与えたいと思っています。
author: Lisa
feature: Timesheets
exl-id: 29d3124b-cf7a-4a47-95c4-cd5379489810
TQID: https://experienceleague.adobe.com/TBeLp0FaUmlRk2uk5SdCqntrUWeAAVucox6Dyx5M0Uw
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 188
ht-degree: 100%

---

# レートが変更された際に財務の再計算アクションが履歴時間に影響するのを防ぐ

## 問題

ユーザーまたは担当業務の時間別コストを更新する必要がありますが（増加や他の状況が原因で）、この変更により、以前にプロジェクトにログオンした時間に影響を与えたくない、もしくは過去の時間の一部にのみ影響を与えたいと思っています。

## ソリューション

変更しない時間をプロジェクトの請求記録に追加し、請求記録のステータスを「請求済み」に設定します。  このロックは古いレートでロックされており、財務の再計算アクションでは無視されます。  請求済み請求記録に属さない時間は、新しいレートで計算されます。 詳しくは、[プロジェクトの財務を再計算](../../manage-work/projects/project-finances/recalculate-project-finances.md)を参照してください。
