---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 共有列のデータがダッシュボードレポートに表示されない
description: レポートが複数列のダッシュボードレイアウトに配置されている場合、共有列のデータは表示されませんが、単一列のレイアウトには表示されません。 改行も上書きされます。
author: Nolan
feature: Reports and Dashboards
exl-id: b8307182-3ec1-4f16-8427-48ef7a65f969
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '162'
ht-degree: 0%

---

# 共有列のデータがダッシュボードレポートに表示されない

## 問題

レポートが複数列のダッシュボードレイアウトに配置されている場合、共有列のデータは表示されませんが、単一列のレイアウトには表示されません。 改行も上書きされます。

## 原因

としてマークされた列のみ

```
shortview=true
```

ダッシュボードレイアウトで左/右の分割が設定されている場合、または左/中央/右の分割が設定されている場合に、レポートのダッシュボード表示に含まれます。

## 解決策

レポートで使用するビューにアクセスし、テキストモードを開きます。 ( 詳しくは、 [テキストモードを使用したビューの編集](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md).) 共有/結合された列で使用されている列を含め、レポート内のすべての列にラベルを付けます。

```
shortview=true
```

.レポートの列は、ダッシュボードに正しく表示されます。
