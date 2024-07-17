---
content-type: api;tips-tricks-troubleshooting
navigation-topic: tips-tricks-and-troubleshooting-workfront-api
title: API エラーメッセージ 400 無効なリクエスト
description: API エラーメッセージ 400 無効なリクエスト
author: Becky
feature: Workfront API
role: Developer
exl-id: ab7c76a9-16ce-41f9-b7af-5943eb2dfdff
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '93'
ht-degree: 100%

---


# API エラー：「リモートサーバーがエラー (400) 無効なリクエストを返しました」

## 問題

API を使用してカスタムフィールドをイシューに読み込もうとすると、次のエラーが発生します。

`The remote server returned an error: (400) Bad Request`

## 原因

このエラーは、キュートピックに関連付けられたカスタムフォームを持たないプロジェクトのカスタムフィールドを API を介して読み込もうとすると発生します。

## ソリューション

正しいカスタムフォームをキュートピックに追加します。

キュートピックの作成について詳しくは、[キュートピックの作成](../../manage-work/requests/create-and-manage-request-queues/create-queue-topics.md)を参照してください。
