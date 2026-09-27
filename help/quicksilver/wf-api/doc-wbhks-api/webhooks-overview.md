---
content-type: api;overview
product-area: documents
navigation-topic: documents-webhooks-api
title: Web フックの概要
description: Web フックの概要
author: Becky
feature: Workfront API
role: Developer
exl-id: 30a3d0cb-51dc-4770-88be-36d8bf232b98
TQID: 'https://experienceleague.adobe.com/5bBLva-jIjwc953MVjAnwo4y0nABq1N0HGDTIurXk40'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
    internal-label: Integrations
  - id: 682536a8-4872-5ee6-a8a6-8012d713482c
    internal-label: Workfront API
role_v2:
  - id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
    internal-label: Developer
topic_v2:
  - id: b5ce8718-c3af-4fdb-a1a9-fca32f83a87c
    internal-label: Implementation
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '220'
ht-degree: 100%
---
# Web フックの概要

Adobe Workfront のドキュメント Web フックは、Workfront が外部ドキュメントプロバイダーに対して認可された API 呼び出しを行う API エンドポイントのセットを定義します。 これにより、誰でも任意のドキュメントストレージプロバイダー用のミドルウェアプラグインを作成できます。

![Web フック](assets/mceclip0-350x262.png)

Web フックベースの統合のユーザーエクスペリエンスは、Google Drive、Box、Dropboxなどの既存のドキュメント統合のユーザーエクスペリエンスに似ています。 例えば、Workfront ユーザーは以下のアクションを実行できます。

* 外部ドキュメントプロバイダーのフォルダー構造をナビゲート
* ファイルを検索
* ファイルを Workfront にリンク
* 外部ドキュメントプロバイダーにファイルをアップロード
* ドキュメントのサムネールを表示

**参照実装**

新しい web フック実装の開発をすぐに開始できるように、Workfront では参照実装の例を提供しています。 これらの例は、[https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app) にあります。 これらは Java ベースの例で、Workfront からネットワークファイルシステム上のドキュメントに接続できるようにするものです。 

>[!NOTE]
>
>GitHub で公開しているリソースは例に過ぎず、実装を実行することはできません。

## バージョン

* バージョン 1.0（リリース日 - 2015年5月）：初期仕様

* バージョン 1.1（リリース日 - 2015年6月）。 /uploadInit の更新 - documentId と documentVersionId の追加

* バージョン 1.2（リリース日 - 2015年10月）：/createFolder を追加

* 今後のバージョン（リリース日 - 未定）:

  * /delete を追加
  * /rename を追加
  * /serviceInfo を追加
  * /customAction を追加
  * /search にページネーションと parentId を追加
