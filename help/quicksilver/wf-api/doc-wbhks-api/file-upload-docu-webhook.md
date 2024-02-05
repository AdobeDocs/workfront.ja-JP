---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: ドキュメント Web フックを介したファイルのアップロード
description: ドキュメント Web フックを介したファイルのアップロード
author: Becky
feature: Workfront API
role: Developer
exl-id: 2c5727ee-bf8f-4664-a9b1-c5da356d94f5
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '264'
ht-degree: 100%

---


# ドキュメント Web フックを介したファイルのアップロード

ファイルをドキュメントストレージプロバイダーにアップロードするプロセスは、2 つの異なる API エンドポイントを必要とする 2 段階の手順です。Adobe Workfront は、/uploadInit を呼び出して、アップロードプロセスを開始します。このエンドポイントはドキュメント ID を返します。この ID は、ドキュメントのバイトデータをアップロードする際に /upload に渡されます。基盤となるドキュメントストレージシステムによっては、長さ 0 のドキュメントを作成し、後でドキュメントの内容を更新する必要がある場合があります。

ドキュメント ID とドキュメントバージョン ID を使用して、Workfront から追加の情報を取得できる機能が、この仕様のバージョン 1.1 に追加されました。

**例：**&#x200B;ドキュメント管理システムがドキュメントに関する追加情報を必要とする場合、web フックの実装コードは、ドキュメント ID を使用して、Workfront の RESTful API でその情報を取得できます。このような情報は、ドキュメントのカスタムデータフィールドから取得するのが優れたプラクティスです。また、情報にはタスク、イシューまたはプロジェクトを含めます。

## POST メソッド

**URL**

POST /uploadInit

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
   <td>Web フックプロバイダーで参照される親フォルダー ID。</td> 
  </tr> 
  <tr> 
   <td>filename </td> 
   <td>ドキュメントの名前</td> 
  </tr> 
  <tr> 
   <td>documentId</td> 
   <td> <p>Workfront ドキュメント ID（バージョン 1.1 で追加）</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td>documentVersionId</td> 
   <td>Workfront ドキュメントのバージョン ID（バージョン 1.1 で追加）</td> 
  </tr> 
 </tbody> 
</table>

## 応答

/metadata エンドポイントで定義した、ファイルのメタデータです。プロバイダーが使用するドキュメント ID が含まれます。

**例：**

```
https://www.acme.com/api/uploadInit?parentId=12345&filename=new-file.png&documentId=511ea6e000023edb38d2effb2f4e6e3b&documentVersionId=511ea6e000023edb38d2e ffb2f4e6e3b
```

## PUT メソッド

Web フックプロバイダーにドキュメントのバイトデータをアップロードします。

**URL**

PUT /upload

## クエリパラメーター

| 名前  | 説明 |
|---|---|
| id  | 前半で作成されたドキュメント ID。 |


**リクエスト本文**

ドキュメントの Raw コンテンツのバイトデータです。

**応答**

```
{
result: "success"
}
```

または

```
{
result: "fail"
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
