---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: アップロード後にドキュメント名が変更され、無効な文字が含まれています
description: 特定のドキュメントを配達確認に変換できません。
author: Courtney
source-git-commit: a01c2e42dad1a7c00ac73fcaeb1202c56238a8bb
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 31%

---


# アップロード後にドキュメント名が変更され、無効な文字が含まれています

## 問題

特定のドキュメントを配達確認に変換できません。

## 原因

Workfront にアップロードされるファイルの名前には、特定の文字を含めることができません。ファイル名に `! # % * \ | ' " / ? < > { } [ ]` のいずれかの文字が含まれている場合、その文字はファイルのアップロード時にファイル名から削除されます。

最初のアップロード後にドキュメント名を更新して無効な文字を含めた場合、配達確認の生成は失敗します。

## ソリューション

ドキュメント名から無効な文字を削除します。

1. ドキュメントを選択し、「 **ドキュメントの詳細**.
1. ドキュメント名をクリックして無効な文字を削除し、Enter キーを押します。

   無効な文字： `! # % * \ | ' " / ? < > { } [ ]`

   ![](assets/doc-name.png)

1. ページを更新し、配達確認を生成します。