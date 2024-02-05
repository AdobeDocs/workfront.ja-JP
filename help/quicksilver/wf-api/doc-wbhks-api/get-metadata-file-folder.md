---
content-type: api
product-area: documents
navigation-topic: documents-webhooks-api
title: ファイルまたはフォルダーのメタデータを取得
description: ファイルまたはフォルダーのメタデータを取得
author: Becky
feature: Workfront API
role: Developer
exl-id: 7b594df5-c87f-45d4-b84a-cae17171e906
source-git-commit: 14ff8da8137493e805e683e5426ea933f56f8eb8
workflow-type: tm+mt
source-wordcount: '268'
ht-degree: 92%

---


# ファイルまたはフォルダーのメタデータを取得

指定されたファイルまたはフォルダーのメタデータを返します。

**URL**

GET/metadata?id=[ドキュメントまたはフォルダー ID]

## クエリパラメーター

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
   <td>id</td> 
   <td>Web フックプロバイダーで参照される、ファイルまたはフォルダーの ID。Adobe Workfront のドキュメント ID とは異なります。ルートディレクトリのメタデータを取得するには、値「/」を使用します。
   <p>メモ：ID の最大長は 255 文字です。</p></td> 
  </tr> 
 </tbody> 
</table>

 

## 応答

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>名前</th> 
   <th>タイプ </th> 
   <th>説明</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>タイトル</td> 
   <td>文字列</td> 
   <td>ドキュメントまたはフォルダーの名前</td> 
  </tr> 
  <tr> 
   <td>kind </td> 
   <td>文字列</td> 
   <td>この項目がファイルかフォルダーかを指定します（値は「file」か「folder」のどちらか）</td> 
  </tr> 
  <tr> 
   <td>id</td> 
   <td>文字列</td> 
   <td>ファイルまたはフォルダーの ID。</td> 
  </tr> 
  <tr> 
   <td>viewLink</td> 
   <td>文字列</td> 
   <td> <p>ブラウザーウィンドウでドキュメントを表示するためにユーザーが使用する URL パス。この URL は、ドキュメントプロバイダーかネイティブ外部ストレージプロバイダーのどちらかでホストできます。</p> </td> 
  </tr> 
  <tr> 
   <td>downloadLink</td> 
   <td>文字列</td> 
   <td> <p>ブラウザーウィンドウでドキュメントをダウンロードするためにユーザーが使用する URL パス。この URL は、ドキュメントプロバイダーかネイティブ外部ストレージプロバイダーのどちらかでホストできます。</p> </td> 
  </tr> 
  <tr> 
   <td>mimeType</td> 
   <td>文字列</td> 
   <td>ファイルの MIME タイプ（オプション）</td> 
  </tr> 
  <tr> 
   <td>dateModified</td> 
   <td>文字列</td> 
   <td>このファイルが最後に変更された日時（RFC 3339 形式のタイムスタンプ）</td> 
  </tr> 
  <tr> 
   <td>サイズ</td> 
   <td>Long</td> 
   <td>ファイルのサイズ（バイト単位）。（オプション）</td> 
  </tr> 
  <tr> 
   <td>readOnly</td> 
   <td>ブール値</td> 
   <td> このファイルまたはフォルダーが認証済みユーザーに対して読み取り専用かどうかを示します。（オプション） </td> 
  </tr> 
 </tbody> 
</table>

**例：** https://www.acme.com/api/metadata?id=12345
<pre>{<br>title:"My Document",<br>kind:"file"<br>id":"12345",<br>viewLink:"https://www.acme.com/viewDocument?id=12345",<br>downloadLink:"https://www.acme.com/downloadDocument?id=12345",<br>mimeType:"image/png",<br>dateModified:"20140605T17:39:45.251Z",<br>size: "32554694"<br>}</pre>

>[!NOTE]
>
>エラー処理は、すべての API 呼び出しで一貫している必要があります。詳しくは、以降の「エラー処理」の節を参照してください。
