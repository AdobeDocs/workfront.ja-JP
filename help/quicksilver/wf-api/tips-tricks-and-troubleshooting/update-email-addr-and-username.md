---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: emailAddr を更新してもユーザー名が更新されない
description: emailAddr を更新しても username が更新されない
author: Becky
feature: Workfront API
role: Developer
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: ht
source-wordcount: '231'
ht-degree: 100%

---


# emailAddr を更新してもユーザー名が更新されない

## 問題

通常は、`emailAddr` と `username` は同じ属性です。したがって、ユーザーの `emailAddr` 属性を変更する場合、`username` 属性は一致させるために自動的に更新されます。

`username` が `emailAddr` と一致しない場合、`emailAddr` を更新しても `username` は自動的に更新されません。これは両方に当てはまり、`emailAddr` は、ユーザーインターフェイスと API を通じて変更されます。

## 原因

不一致は、次のような要因から発生する可能性があります。

* 同期ルールが存在する前に作成されたユーザー。非常に古いユーザーアカウントでは、これらの属性が同期していない可能性があります。

* Workfront の emailAddr で大文字と小文字が区別された時点で、SSO を使用して作成されたユーザー。SSO 自動プロビジョニングオプションでは、ID プロバイダーからのユーザーの属性に基づいて、ユーザーに対して大文字と小文字が区別されるチェックが実行されます。完全に一致するユーザーが存在しない場合、自動プロビジョニングサービスによって新しいユーザーが作成されます。ユーザーが既に存在する場合は、ユーザー名と `emailAddr` の大文字小文字が一致しない可能性がありました。

* `username` 属性を持つユーザーが API を介して直接更新され、`emailAddr` が更新されませんでした。`username` および `emailAddr` が一致しない可能性があります。

## ソリューション

API を使って `username` 属性を `emailAddr` と同じ属性に変更します。属性を同期した後、`emailAddr` を更新すると `username` も一致するように更新されます（「ユーザー名」フィールドが更新に含まれていない場合）。
