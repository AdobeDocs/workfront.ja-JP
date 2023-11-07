---
content-type: api
navigation-topic: api-navigation-topic
title: API を使用したファイルのアップロード
description: API を使用したファイルのアップロード
author: Becky
feature: Workfront API
role: Developer
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
source-git-commit: 3e339e2bfb26e101f0305c05f620a21541394993
workflow-type: tm+mt
source-wordcount: '176'
ht-degree: 0%

---

# API を使用したファイルのアップロード

Postmanなどの API ツールを使用したWorkfront API や、単純な cURL コマンドを使用してファイルをアップロードできます。

ドキュメントをアップロードするには、 **ドキュメントのアップロード** Workfront [投稿の動作](/help/quicksilver/wf-api/general/api-basics.md#post-behavior). また、cURL リクエストに対しても、これらの同じ手順を使用できます。

**API ツールを使用してファイルをアップロードする場合は、次のガイドラインに従います。**

* API ツールオプションを使用して、ファイルをアップロードします。 多くの場合、 **ファイルを選択** ボタンをクリックします。

* POSTHTTP メソッドを使用して、ファイルのアップロードをリクエストします。

* リクエストの結果、そのハンドルの値を含む応答が返されます。

* 後続の呼び出しをおこなうには、JSON ペイロードの objID の handle 値、オブジェクトタイプ、GUID 値を使用します。 これは、次の例に示すように、ファイルのオブジェクトを作成するためのものです。

```
}
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "v1.0", "fileName" : "TestPDF"},
}
```

応答内のオブジェクトの ID を受け取る必要があります。

詳しくは、使用している特定の API ツールのヘルプを参照してください。
