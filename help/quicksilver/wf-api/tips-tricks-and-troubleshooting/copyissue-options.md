---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: OPTASK copyIssue のオプション設定
description: copyIssue エンドポイントで想定される整数値の説明です。
author: Becky
feature: Workfront API
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
source-git-commit: 93a67b3dbd59f188dad6b060ec93c3f137c981b2
workflow-type: tm+mt
source-wordcount: '117'
ht-degree: 6%

---

# OPTASK copyIssue のオプション設定


copyIssue API 呼び出しのプロパティの 1 つは、 `options`. このフィールドには整数が必要です。

次のいずれかのオプションを含めるには、一致する整数を入力します。 複数のオプションを含めるには、一致する整数の合計を入力します。

| オプション | value* |
|---|---|
| 割り当てをクリア | 2 |
| 進行状況をクリア | 4 |
| ドキュメントを消去 | 128 |
| 更新をクリア | 65536 |
| 権限をクリア | 524288 |
| カスタムデータをクリア | 1048576 |

*すべての値は 2 の乗です。

例:

* 問題をコピーする際に進行状況をクリアするには、 `options` 値 `4`.

* 進行状況とドキュメントの両方をクリアするには、 `options` 値 `132`.

   進行状況の消去= 4

   ドキュメントの消去= 128

   4 + 128 = 132
