---
content-type: api
navigation-topic: api-navigation-topic
title: API を使用したファイルのアップロード
description: API を使用したファイルのアップロード
author: Becky
feature: Workfront API
role: Developer
exl-id: 4e0b73b6-0d6d-4971-a87a-dfec85fb031a
TQID: https://experienceleague.adobe.com/Yd7byYJ1pYDXwdKvINXh4fKy-pWoEiNMj345jr1HHNs
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: b58ad82f-df6b-4b01-81a3-3a02ab9567a0
role_v2: id: ff6a42d2-313e-452e-93a6-792e4fad9ff8
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 176
ht-degree: 93%

---

# API を使用したファイルのアップロード

WorkFront API を Postman などの API ツールと併用、または単純な cURL コマンドと併用してファイルをアップロードできます。

ドキュメントのアップロードについては、WorkFront の [POST 動作](/help/quicksilver/wf-api/general/api-basics.md#post-behavior)にある&#x200B;**ドキュメントのアップロード**&#x200B;の手順を参照してください。 また、cURL リクエストに対しても、この同じ手順を使用できます。

**API ツールを使用してファイルをアップロードする場合、以下のガイドラインに従います。**

* API ツールオプションを使用して、ファイルをアップロードします。 リクエスト画面には&#x200B;**ファイルを選択** ボタンが表示されることがよくあります。

* POST HTTP メソッドを使用して、ファイルのアップロードをリクエストします。

* リクエストの結果、そのハンドルの値を含む応答が返されます。

* ハンドル値、オブジェクトタイプ、および JSON ペイロード内の objID の GUID 値を使用して、後続の呼び出しを行います。 これは、次の例に示すように、ファイルのオブジェクトを作成するためのものです。

```
{
"name": "TestPDF",
"handle": "7af257e64aba4a22c33ccdfc40bbb87",
"docObjCode": "PROJ",
"objID": "0398450f8345980843445534354",
"currentVersion": {"version": "1", "fileName" : "TestPDF"},
}
```

応答でオブジェクトの ID を受け取る必要があります。

詳しくは、使用している特定の API ツールのヘルプを参照してください。
