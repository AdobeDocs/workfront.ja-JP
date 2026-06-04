---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 共有列のデータがダッシュボードレポートに表示されない
description: レポートが複数列のダッシュボードレイアウトに配置されている場合、共有列のデータは表示されませんが、単一列のレイアウトには表示されます。 改行も上書きされます。
author: Courtney
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/OEFlwkdPf98g4-rC1tzaTmmEwb5-BXHx-j8XGrRR8sE
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 162
ht-degree: 83%

---

# 共有列のデータがダッシュボードレポートに表示されない

## 問題

レポートが複数列のダッシュボードレイアウトに配置されている場合、共有列のデータは表示されませんが、単一列のレイアウトには表示されます。 改行も上書きされます。

## 原因

ダッシュボードレイアウトに左/右分割または左／中央／右分割が設定されている場合、

```
shortview=true
```

のようにマークされている列のみがレポートのダッシュボードビューに含まれます。

## ソリューション

レポートで使用するビューにアクセスし、テキストモードを開きます。 （詳しくは、[ テキストモードを使用したビューの編集](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)を参照してください）。 共有/結合された列で使用される列を含め、レポートのすべての列にラベルを付けます。

```
shortview=true
```

. レポートの列は、ダッシュボードに正しく表示されます。
