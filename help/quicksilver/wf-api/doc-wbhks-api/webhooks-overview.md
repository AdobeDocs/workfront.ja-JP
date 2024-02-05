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
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '209'
ht-degree: 74%

---


# Web フックの概要

Adobe Workfront のドキュメント Web フックは、Workfront が外部ドキュメントプロバイダーに対して認可された API 呼び出しを行う API エンドポイントのセットを定義します。これにより、誰でも任意のドキュメントストレージプロバイダー用のミドルウェアプラグインを作成できます。

![](assets/mceclip0-350x262.png)

Web フックベースの統合のユーザーエクスペリエンスは、Google Drive、Box、Dropboxなどの既存のドキュメント統合のユーザーエクスペリエンスに似ています。例えば、Workfront ユーザーは以下のアクションを実行できます。

* 外部ドキュメントプロバイダーのフォルダー構造をナビゲート
* ファイルを検索
* ファイルを Workfront にリンク
* 外部ドキュメントプロバイダーにファイルをアップロード
* ドキュメントのサムネールを表示

**参照実装**

新しい Web フック実装の開発をすぐに開始できるように、Workfrontでは参照実装の例を提供しています。 これらの例は、次の場所にあります。 [https://github.com/Workfront/webhooks-app](https://github.com/Workfront/webhooks-app). 例は Java ベースで、Workfrontがネットワークファイルシステム上でドキュメントに接続できるようにします。 

>[!NOTE]
>
>GitHub のリソースは例に過ぎず、実装を実行できません。

## バージョン

* バージョン 1.0（リリース日 - 2015年5月）：初期仕様

* バージョン 1.1（リリース日 - 2015年6月）。/uploadInit の更新 - documentId と documentVersionId の追加

* バージョン 1.2（リリース日 - 2015年10月）：/createFolder を追加

* 今後のバージョン（リリース日 - 未定）:

   * /delete を追加
   * /rename を追加
   * /serviceInfo を追加
   * /customAction を追加
   * /search にページネーションと parentId を追加
