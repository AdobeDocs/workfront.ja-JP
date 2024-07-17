---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: アップロード後にドキュメント名が変更され、無効な文字が含まれています
description: プルーフに変換できないドキュメントもあります。
author: Courtney
exl-id: 7771deb5-cf9f-4a32-a444-b701bec1619e
source-git-commit: 3e16f69f5b3c2b37093b00841945e6529394fa94
workflow-type: tm+mt
source-wordcount: '133'
ht-degree: 46%

---

# アップロード後にドキュメント名が変更され、無効な文字が含まれています

## 問題

プルーフに変換できないドキュメントもあります。

## 原因

Workfront にアップロードされるファイルの名前には、特定の文字を含めることができません。ファイル名に `! # % * \ | ' " / ? < > { } [ ]` のいずれかの文字が含まれている場合、その文字はファイルのアップロード時にファイル名から削除されます。

最初のアップロードの後に、無効な文字を含むようにドキュメント名が更新されると、プルーフの生成に失敗します。

## ソリューション

ドキュメント名から無効な文字を削除します。

1. ドキュメントを選択し、「**ドキュメントの詳細**」をクリックします。
1. ドキュメント名をクリックして無効な文字を削除し、Enter キーを押します。

   無効な文字：`! # % * \ | ' " / ? < > { } [ ]`

   ![](assets/doc-name.png)

1. ページを更新し、プルーフを生成します。
