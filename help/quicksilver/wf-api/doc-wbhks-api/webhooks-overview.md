---
content-type: api;overview
product-area: documents
navigation-topic: documents-webhooks-api
title: ウェブフックの概要
description: ウェブフックの概要
author: Becky
feature: Workfront API
exl-id: 30a3d0cb-51dc-4770-88be-36d8bf232b98
source-git-commit: eb738fa8cadaafb0332c5c78a3816d5c346c33b2
workflow-type: tm+mt
source-wordcount: '209'
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

新しい Web フック実装の開発をすぐに開始できるように、Workfrontでは参照実装の例を提供しています。 これらの例は、次の場所にあります。 [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). 例は Java ベースで、Workfrontがネットワークファイルシステム上でドキュメントに接続できるようにします。 

>[!NOTE]
>
>GitHub のリソースは例に過ぎず、実装を実行できません。

## バージョン

* バージョン 1.0（リリース日 — 2015 年 5 月）：初期仕様

* バージョン 1.1（リリース日 — 2015 年 6 月）。 /uploadInit の更新 — documentId と documentVersionId の追加

* バージョン 1.2（リリース日 — 2015 年 10 月）: /createFolder を追加しました。

* 今後のバージョン（リリース日 — 未定）:

   * /delete を追加しました
   * /rename を追加しました。
   * /serviceInfo を追加しました。
   * /customAction を追加しました。
   * /search にページネーションと parentId を追加
