---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: ドキュメントウェブフックを介したファイルのアップロード
description: ドキュメントウェブフックを介したファイルのアップロード
author: Becky
feature: Workfront API
exl-id: 2c5727ee-bf8f-4664-a9b1-c5da356d94f5
source-git-commit: f050c8b95145552c9ed67b549608c16115000606
workflow-type: tm+mt
source-wordcount: '261'
ht-degree: 3%

---


# ドキュメントウェブフックを介したファイルのアップロード

ファイルをドキュメントストレージプロバイダーにアップロードするプロセスは、2 つの異なる API エンドポイントを必要とする 2 つの手順で構成されます。 Adobe Workfrontは、 /uploadInit を呼び出して、アップロードプロセスを開始します。 このエンドポイントはドキュメント ID を返し、ドキュメントのバイトをアップロードする際に/upload に渡されます。 基になるドキュメントストレージシステムによっては、長さ 0 のドキュメントを作成してから、後でドキュメントの内容を更新する必要が生じる場合があります。

この仕様のバージョン 1.1 に追加されたドキュメント ID とドキュメントバージョン ID を使用して、Workfrontから追加の情報を取得できます。

**例：** ドキュメント管理システムがドキュメントに関する追加の情報を必要とする場合、Webhook 実装コードは、Workfrontの RESTful API を使用して、ドキュメント ID を使用してその情報を取得できます。 ベストプラクティスとして、この情報は、ドキュメント上のカスタムデータフィールドから取得され、タスク、問題、またはプロジェクトが含まれている場合があります。

## POST法

**URL**

POST/uploadInit

### クエリパラメーター

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名前 </th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>parentId </td> 
   <td>Webhook プロバイダーによって参照される親フォルダー ID。</td> 
  </tr> 
  <tr> 
   <td>filename </td> 
   <td>ドキュメントの名前</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>Workfrontドキュメント ID （バージョン 1.1 で追加）</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId </td> 
   <td>Workfrontドキュメントのバージョン ID（バージョン 1.1 で追加） </td> 
  </tr> 
 </tbody> 
</table>

## 応答

ファイルのメタデータ（/metadata エンドポイントで定義）。 プロバイダーが使用するドキュメント ID が含まれます。

**例:**

```
https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&documentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b
```

## PUT法

Webhook プロバイダーにドキュメントのバイトをアップロードします。

**URL**

PUT/upload

## クエリパラメーター

| 名前  | 説明 |
|---|---|
| id  |  作成されたドキュメント ID。 |


**リクエスト本文**

ドキュメントの生の内容のバイト。

**応答**

```
{
result: “success”
}
```

または

```
{
result: “fail”
}
```

**例**

`https://www.acme.com/api/upload?id=1234 [document bytes included in update stream]`

応答

```
{
result:"success"
}
```
