---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 共有列のデータがダッシュボードレポートに表示されない
description: レポートが複数列のダッシュボードレイアウトに配置されている場合、共有列のデータは表示されませんが、単一列のレイアウトには表示されます。改行も上書きされます。
author: Courtney
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
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

レポートで使用するビューにアクセスし、テキストモードを開きます。（詳しくは、[&#x200B; テキストモードを使用したビューの編集 &#x200B;](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md) を参照してください）。共有/結合列で使用されている列を含む、レポートのすべての列に、次のラベルを付けます

```
shortview=true
```

.レポートの列は、ダッシュボードに正しく表示されます。
