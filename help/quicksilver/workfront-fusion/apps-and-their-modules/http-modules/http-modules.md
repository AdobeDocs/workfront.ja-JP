---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: HTTP &gt;その他のモジュール
description: この [!DNL Adobe Workfront Fusion] HTTP アプリは、Hypertext Transfer Protocol(HTTP) プロトコルに基づく通信用の様々なモジュールを提供します。 HTTP は、World Wide Web のデータ通信の基盤です。 モジュールを使用して、Web ページやファイルをダウンロードしたり、Web フックや API エンドポイントを呼び出したりできます。
author: Becky
feature: Workfront Fusion
exl-id: ff2cd098-d1d7-43a3-9f00-15e0f6e92332
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '427'
ht-degree: 0%

---

# HTTP > その他のモジュール

>[!NOTE]
>
>[!UICONTROL Adobe Workfront Fusion] にはが必要です [!UICONTROL Adobe Workfront Fusion] に加えてライセンス [!UICONTROL Adobe Workfront] ライセンス。

この [!DNL Adobe Workfront Fusion] [!UICONTROL HTTP] app は、ハイパーテキスト転送プロトコル (HTTP) プロトコルに基づく通信用の様々なモジュールを提供します。 HTTP は、World Wide Web のデータ通信の基盤です。 モジュールを使用して、Web ページやファイルをダウンロードしたり、Web フックや API エンドポイントを呼び出したりできます。

モジュールの適切な選択は、アクセスするリソースが使用する認証/承認メカニズムによって異なります。 次に、モジュールの例を示します。

* リクエストを行う：ユニバーサルモジュールは、主にどの種類の認証/承認を使用しないリソースを対象としています
* 基本認証要求の作成：を使用するリソース用 [!DNL HTTP] 基本認証 (BA)
* OAuth 2.0 リクエストを作成します。OAuth 2.0 認証プロトコルを使用するリソースの場合
* クライアント証明書認証要求を作成する：クライアント側の証明書を必要とする認証プロトコルを使用するリソースの場合。
* API キー認証リクエストを作成します。認証に API キーを使用するリソースに関する情報を含む )。

## リクエストモジュール

特定のリクエストモジュールの手順については、次の記事を参照してください。

* [[!UICONTROL HTTP] >[!UICONTROL リクエストを実行] モジュール](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL 基本認証リクエストの作成] モジュール](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-basic-auth-request.md)
* [[!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 リクエストを作成] モジュール](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL クライアント証明書認証要求の作成] モジュール](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-client-cert-auth-request.md)
* [[!UICONTROL HTTP] >[!UICONTROL API キー認証リクエストの作成]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-api-key-auth-request.md)

## その他のアクションモジュール

* [[!UICONTROL ファイルの取得]](#get-a-file)
* [[!UICONTROL ターゲット URL の解決]](#resolve-a-target-url)

### [!UICONTROL ファイルの取得]

このアクションモジュールは、指定した URL からファイルをダウンロードします。 ファイルがダウンロードされたら、シナリオ内の他のモジュールを使用して、ファイルをさらに処理（ファイルデータをマッピング）できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>ダウンロードするファイルの URL を入力またはマッピングします。 </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL ターゲット URL の解決]

このアクションモジュールは、HTTP リダイレクトの連鎖を解決し、ターゲット URL を返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL] </td> 
   <td> <p>解決する URL を入力またはマッピングします。例： [!DNL bit.ly] URL。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メソッド ] </td> 
   <td> <p>[!UICONTROLHEAD] メソッドと [!UICONTROLGET] メソッドのどちらを使用するかを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 反復子モジュール

### [!UICONTROL ヘッダーの取得]

このモジュールは、指定された HTTP モジュールの各ヘッダー（名前と値）を別々のバンドルで返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースモジュール ]</td> 
   <td> <p> ヘッダーを取得するモジュールを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

## JSON Web トークン (JWT) の生成

次の組み込み関数を使用して JWT トークンを生成できます。

ヘッダー:

![](assets/jwt-header-350x19.png)

コピー&amp;ペーストのコード：

```
{{replace(replace(replace(base64("{""alg"":""HS256"",""typ"":""JWT""}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

ペイロード：

![](assets/jwt-payload-350x17.png)

コピー&amp;ペーストのコード：

```
{{replace(replace(replace(base64("{""iss"":""key"",""exp"":" + (timestamp + 60) + "}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

トークン：

![](assets/jwt-token-350x15.png)

コピー&amp;ペーストのコード：

```
{{1.value}}.{{2.value}}.{{replace(replace(replace(sha256(1.value + "." + 2.value; "base64"; "secret"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```
