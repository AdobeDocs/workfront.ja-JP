---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: HTTP／その他のモジュール
description: ' [!DNL Adobe Workfront Fusion]  HTTP アプリは、Hypertext Transfer Protocol（HTTP）で通信するための様々なモジュールを提供します。HTTP は、World Wide Web のためのデータ通信基盤です。このモジュールを使用すると、web のページやファイルをダウンロードしたり、web フックや API エンドポイントを呼び出したりできます。'
author: Becky
feature: Workfront Fusion
exl-id: ff2cd098-d1d7-43a3-9f00-15e0f6e92332
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: ht
source-wordcount: '427'
ht-degree: 100%

---

# HTTP／その他のモジュール

>[!NOTE]
>
>[!UICONTROL Adobe Workfront Fusion] には、[!UICONTROL Adobe Workfront]ライセンスに加えて [!UICONTROL Adobe Workfront Fusion]ライセンスが必要です。

[!UICONTROL HTTP][!DNL Adobe Workfront Fusion] アプリは、Hypertext Transfer Protocol（HTTP）で通信するための様々なモジュールを提供します。HTTP は、World Wide Web のためのデータ通信基盤です。このモジュールを使用すると、web のページやファイルをダウンロードしたり、web フックや API エンドポイントを呼び出したりできます。

モジュールの適切な選択は、アクセスするリソースが使用する認証 / 承認メカニズムによって異なります。次に、モジュールの例を示します。

* リクエストの作成：ユニバーサルモジュールは、主にどのタイプの認証 / 承認をも使用しないリソースを対象としています。
* 基本認証リクエストの作成：[!DNL HTTP] 基本認証（BA）を使用するリソース向け
* OAuth 2.0 リクエストの作成：OAuth 2.0 承認プロトコルを使用するリソース向け
* クライアント証明書認証リクエストの作成：クライアントサイドの証明書を必要とする認証プロトコルを使用しているリソース向け。
* API キー認証リクエストの作成：認証に API キーを使用しているリソース向け

## リクエストモジュール

特定のリクエストモジュールの手順については、次の記事を参照してください。

* [[!UICONTROL HTTP]／[!UICONTROL リクエストの作成]モジュール](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-request.md)
* [[!UICONTROL HTTP]／[!UICONTROL 基本認証リクエストの作成]モジュール](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-basic-auth-request.md)
* [[!UICONTROL HTTP]／[!UICONTROL OAuth 2.0 リクエストの作成]モジュール](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md)
* [[!UICONTROL HTTP]／[!UICONTROL クライアント証明書認証リクエストの作成]モジュール](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-a-client-cert-auth-request.md)
* [[!UICONTROL HTTP]／[!UICONTROL API キー認証リクエストの作成]](../../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-api-key-auth-request.md)

## その他のアクションモジュール

* [[!UICONTROL ファイルの取得]](#get-a-file)
* [[!UICONTROL ターゲット URL の解決]](#resolve-a-target-url)

### [!UICONTROL ファイルの取得]

このアクションモジュールでは、指定した URL からファイルをダウンロードします。ファイルがダウンロードされたら、シナリオ内の他のモジュールを使用して、ファイルをさらに処理（ファイルデータをマッピング）できます。

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
   <td> <p>[!DNL bit.ly] URL などの解決する URL を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method] </td> 
   <td> <p>[!UICONTROL HEAD] メソッドと [!UICONTROL GET] メソッドのどちらを使用するかを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

## イテレータモジュール

### [!UICONTROL ヘッダーの取得]

このモジュールは、指定された HTTP モジュールの各ヘッダー（名前と値）を個別のバンドルで返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td> <p> ヘッダーの取得元のモジュールを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

## JSON Web トークン（JWT）の生成

組み込みの関数のヘルプを使用して JWT トークンを生成できます。

ヘッダー:

![](assets/jwt-header-350x19.png)

コピーおよび貼り付けのコード：

```
{{replace(replace(replace(base64("{""alg"":""HS256"",""typ"":""JWT""}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

ペイロード：

![](assets/jwt-payload-350x17.png)

コピーおよび貼り付けのコード：

```
{{replace(replace(replace(base64("{""iss"":""key"",""exp"":" + (timestamp + 60) + "}"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```

トークン：

![](assets/jwt-token-350x15.png)

コピーおよび貼り付けのコード：

```
{{1.value}}.{{2.value}}.{{replace(replace(replace(sha256(1.value + "." + 2.value; "base64"; "secret"); "/=/g"; emptystring); "/\+/g"; "-"); "/\//g"; "_")}}
```
