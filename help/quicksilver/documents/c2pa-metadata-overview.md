---
product-area: documents
navigation-topic: documents-navigation-topic
title: Adobe WorkfrontのC2PA メタデータ
description: C2PA メタデータとは何か、およびAdobe Workfrontがアップロード、保存、ダウンロードするドキュメント上でC2PA メタデータを保持する方法について説明します。
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 3510218fb179a0852ad22abe2a753ccdb261205a
workflow-type: tm+mt
source-wordcount: 215
ht-degree: 0%

---

# Adobe WorkfrontのC2PA メタデータ

C2PA メタデータは、コンテンツとともに移動する、安全で改ざんされやすい情報です。 生成AI （GenAI）を使用して画像、動画、オーディオファイルを作成または変更する場合、C2PA メタデータはその事実を記録するため、ファイルを受け取る人は誰でもその作成方法を確認できます。

C2PA メタデータは、オープン [C2PA](https://c2pa.org/)標準に基づいています。

## C2PA メタデータに含まれるもの

C2PA メタデータには、次のものが含まれます。

* 生成AI ツールを提供したプロバイダーの名前。
* コンテンツの作成や変更に使用される生成AI システムの名前とバージョン番号。
* コンテンツが作成または変更された日時。
* 一意のID:

C2PAのメタデータには、個人情報（PII）は含まれません。

## WorkfrontによるC2PA メタデータの処理

Adobe Workfrontでは、操作するファイルのメタデータは変更されません。 既にC2PA メタデータを含むファイルをアップロードする場合、ファイルが保存され、Workfrontからダウンロードされる際に、Workfrontはその情報を変更せずに保持します。

メタデータはファイル自体に埋め込まれているため、Workfront ワークフローを通じて変更されずに残ります。そのため、来歴情報はWorkfrontを離れた場合もコンテンツに残ります。
