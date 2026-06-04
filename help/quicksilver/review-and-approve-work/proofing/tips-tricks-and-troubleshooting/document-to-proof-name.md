---
content-type: tips-tricks-troubleshooting
product-area: documents
navigation-topic: tips-tricks-and-troubleshooting-proofing-within-workfront
title: アップロード後にドキュメント名が変更され、無効な文字が含まれています
description: 特定の文書をプルーフに変換することはできません。
author: Courtney
exl-id: 7771deb5-cf9f-4a32-a444-b701bec1619e
TQID: https://experienceleague.adobe.com/bE5iUIG7rFpIIa3zXt-5pO0sgfbEO-3QDVFVLwkayIo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 135
ht-degree: 45%

---

# アップロード後にドキュメント名が変更され、無効な文字が含まれています

## 問題

特定の文書をプルーフに変換することはできません。

## 原因

Workfront にアップロードされるファイルの名前には、特定の文字を含めることができません。 ファイル名に `! # % * \ | ' " / ? < > { } [ ]` のいずれかの文字が含まれている場合、その文字はファイルのアップロード時にファイル名から削除されます。

最初のアップロード後にドキュメント名が無効な文字を含むように更新された場合、プルーフの生成は失敗します。

## ソリューション

文書名から無効な文字を削除します。

1. ドキュメントを選択し、**ドキュメントの詳細**&#x200B;をクリックします。
1. 文書名をクリックして無効な文字を削除し、Enter キーを押します。

   無効な文字：`! # % * \ | ' " / ? < > { } [ ]`

   ![&#x200B; ドキュメント名](assets/doc-name.png)

1. ページを更新し、プルーフを生成します。
