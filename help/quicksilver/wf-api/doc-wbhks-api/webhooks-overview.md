---
content-type: api;overview
product-area: documents
navigation-topic: documents-webhooks-api
title: ウェブフックの概要
description: ウェブフックの概要
author: John
feature: Workfront API
exl-id: 30a3d0cb-51dc-4770-88be-36d8bf232b98
source-git-commit: a62ae524f922326811423cd17d0656920b7cc9d3
workflow-type: tm+mt
source-wordcount: '193'
ht-degree: 0%

---


# ウェブフックの概要

Adobe Workfront Document Webhook は、Workfrontが外部ドキュメントプロバイダーに対して承認済みの API 呼び出しをおこなう API エンドポイントのセットを定義します。 これにより、誰でも任意のドキュメントストレージプロバイダー用のミドルウェアプラグインを作成できます。

![](assets/mceclip0-350x262.png)

Webhook ベースの統合のユーザーエクスペリエンスは、Google Drive、Box、Dropboxなどの既存のドキュメント統合のユーザーエクスペリエンスと似ています。 例えば、Workfrontユーザーは次の操作を実行できます。

* 外部ドキュメントプロバイダーのフォルダー構造に移動する
* ファイルを検索
* ファイルをWorkfrontにリンク
* 外部ドキュメントプロバイダーにファイルをアップロード
* ドキュメントのサムネールを表示

**参照実装**

新しい Web フック実装の開発をすぐに開始できるように、Workfrontでは参照実装を提供しています。 これを行うコードは、で確認できます。 [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app) . この実装は Java ベースで、Workfrontはネットワークファイルシステム上でドキュメントに接続できます。 

## バージョン

* バージョン 1.0（リリース日 — 2015 年 5 月）:初期仕様

* バージョン 1.1（リリース日 — 2015 年 6 月） /uploadInit の更新 — documentId と documentVersionId の追加

* バージョン 1.2（リリース日 — 2015 年 10 月）:/createFolder を追加しました

* 今後のバージョン（リリース日 — 未定）:

   * /delete を追加しました
   * /rename を追加しました。
   * /serviceInfo を追加しました。
   * /customAction を追加しました。
   * /search にページネーションと parentId を追加
