---
content-type: api;tips-tricks-troubleshooting
navigation-topic: workfront-api
title: emailAddr に対する更新は、ユーザー名を更新しません
description: emailAddr に対する更新は、ユーザー名を更新しません
author: Becky
feature: Workfront API
exl-id: 2d24d1b8-9504-484f-9cc0-d2f1abd6391a
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '231'
ht-degree: 0%

---


# emailAddr に対する更新は、ユーザー名を更新しません

## 問題

通常、 `emailAddr` および `username` は同じ属性です。 したがって、ユーザーの `emailAddr` 属性 `username` 属性は、に合わせて自動的に更新されます。

次の場合に `username` 一致しない `emailAddr`( `emailAddr` を更新しない `username` 自動的に。 これは両方に当てはまります。 `emailAddr` は、ユーザーインターフェイスと API を通じて変更されます。

## 原因

不一致は、次の方法で生成される場合があります。

* 同期ルールが存在する前に作成されたユーザー。 非常に古いユーザーアカウントでは、これらの属性が同期していない可能性があります。

* Workfrontの emailAddr で大文字と小文字が区別された時点で、SSO を使用して作成されたユーザー。 SSO 自動プロビジョニングオプションでは、ID プロバイダーからのユーザーの属性に基づいて、ユーザーに対して大文字と小文字が区別されるチェックが実行されます。 完全一致が存在しなかった場合、自動プロビジョニングサービスによって新しいユーザーが作成されます。 ユーザーが既に存在する場合、ユーザー名と `emailAddr` 同じ筐体を持つことはなかった

* 次の条件を満たすユーザー `username` 属性が API を介して直接更新され、 `emailAddr` は更新されませんでした。 この `username` および `emailAddr` が一致しない可能性があります。

## 解決策

API を使用して `username` 属性が `emailAddr`. 属性を同期した後、 `emailAddr` は、 `username` 照合する（ユーザー名フィールドが更新に含まれていない場合）
