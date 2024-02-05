---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: OPTASK copyIssue のオプション設定
description: copyIssue エンドポイントで想定されている整数値の説明です。
author: Becky
feature: Workfront API
role: Developer
exl-id: a2b8ef01-1c14-47a5-8b0a-550b17b526ff
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '122'
ht-degree: 100%

---

# OPTASK copyIssue のオプション設定


copyIssue API 呼び出しのプロパティの 1 つは、`options` という名前のフィールドです。このフィールドに想定されているのは整数です。

以下のいずれかのオプションを含めるには、一致する整数を入力します。複数のオプションを含めるには、一致する整数の合計を入力します。

| オプション | 値* |
|---|---|
| 割り当てのクリア | 2 |
| 進行状況のクリア | 4 |
| ドキュメントのクリア | 128 |
| 更新のクリア | 65536 |
| 許可のクリア | 524288 |
| カスタムデータ | 1048576 |

*値はすべて 2 の累乗です。

例：

* イシューをコピーする際に進行状況をクリアするには、`options` の値として `4` を入力します。

* 進行状況とドキュメントの両方をクリアするには、`options` の値として `132` を入力します。

  進行状況のクリア = 4

  ドキュメントのクリア = 128

  4 + 128 = 132
