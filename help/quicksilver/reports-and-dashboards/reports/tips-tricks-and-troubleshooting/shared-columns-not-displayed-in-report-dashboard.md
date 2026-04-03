---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 共有列のデータがダッシュボードレポートに表示されない
description: レポートが複数列のダッシュボードレイアウトに配置されている場合、共有列のデータは表示されませんが、単一列のレイアウトには表示されます。改行も上書きされます。
author: Courtney
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 83%

---

# 共有列のデータがダッシュボードレポートに表示されない

## 問題

レポートが複数列のダッシュボードレイアウトに配置されている場合、共有列のデータは表示されませんが、単一列のレイアウトには表示されます。改行も上書きされます。

## 原因

ダッシュボードレイアウトに左/右分割または左／中央／右分割が設定されている場合、

```
shortview=true
```

のようにマークされている列のみがレポートのダッシュボードビューに含まれます。

## ソリューション

レポートで使用するビューにアクセスし、テキストモードを開きます。（詳細については、[ テキストモードを使用したビューの編集](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md)を参照してください。）共有/結合された列で使用されている列を含め、レポート内のすべての列に次のラベルを付けます。

```
shortview=true
```

.レポートの列は、ダッシュボードに正しく表示されます。
