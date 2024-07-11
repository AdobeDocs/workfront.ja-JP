---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Adobe Authenticator モジュール
description: Adobe Authenticator モジュールを使用すると、1 回の接続で、API を使用して任意のAdobe製品に接続できます。
author: Becky
feature: Workfront Fusion
exl-id: 74c943fb-37ad-4d91-8af7-9808ba69992e
source-git-commit: 443bdb5caee4b8a7ba9df95b0befff27b7aaabc2
workflow-type: tm+mt
source-wordcount: '993'
ht-degree: 34%

---

# Adobe Authenticator モジュール

Adobe Authenticator モジュールを使用すると、1 回の接続で、任意のAdobeAPI に接続できます。 これにより、まだ専用の Fusion コネクタがないAdobe製品に、より簡単に接続できます。

HTTP モジュールより有利な点は、専用のアプリのように接続を作成できることです。

使用可能なAdobeAPI のリストについては、を参照してください。 [ADOBEAPI](https://developer.adobe.com/apis). 割り当てられている API のみを使用できる場合があります。

## アクセス要件

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] プラン*</td>
      <td>
        <p>新規：任意</p><p>または</p><p>現在：[!UICONTROL Pro] 以上</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td>
      <td>
        <p>新規：標準</p><p>または</p><p>現在：[!UICONTROL 計画 ]、[!UICONTROL 作業 ]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス</td>
      <td>
   <p>現在の Fusion ライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件</p>
   <p>または</p>
   <p>従来の Fusion ライセンス要件：[!UICONTROL [!DNL Workfront Fusion] 作業の自動化と統合のために ] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">製品</td>
      <td>
   <p>新しいWorkfront プラン：[!UICONTROL Select] または [!UICONTROL Prime] がある場合 [!DNL Adobe Workfront] 計画してください。組織による購入が必要です。 [!DNL Adobe Workfront Fusion] も [!DNL Adobe Workfront] ：この記事で説明されている機能を使用します。 [!DNL Workfront Fusion] は、[!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>現在のWorkfront プラン：ご購入が必要です [!DNL Adobe Workfront Fusion] も [!DNL Adobe Workfront] ：この記事で説明されている機能を使用します。</p>
   </td>
    </tr>
  </tbody>
</table>

## 前提条件

* モジュールの接続先となるAdobe製品へのアクセス権が必要です。
* Adobe Developer Consoleにアクセスできる必要があります。
* Adobe Developer Consoleに、モジュールの接続先となる API を含むプロジェクトがある必要があります。 実行できる操作：

   * API を使用して新しいプロジェクトを作成します。

     または
   * API を既存のプロジェクトに追加します。

  Adobe Developer Consoleを使用した API のプロジェクトへの追加について詳しくは、 [プロジェクトの作成](https://developer.adobe.com/dep/guides/dev-console/create-project/) Adobeドキュメント

## 接続の作成

Adobe Authenticator接続は、Adobe Developer Console上の 1 つのプロジェクトに接続します。 複数のAdobeAPI に同じコネクションを使用するには、API を同じプロジェクトに追加して、そのプロジェクトへのコネクションを作成します。

個別のプロジェクトに対して個別の接続を作成できますが、接続を使用して、その接続で指定されたプロジェクトにない API にアクセスすることはできません。

>[!IMPORTANT]
>
>Adobe Authenticator コネクタでは、OAuth サーバー間接続を使用するか、サービスアカウント（JWT）接続を使用するかを選択できます。 Adobeでは、JWT 資格情報を廃止しました。この資格情報は 2025 年 1 月 1 日（PT）以降、機能しなくなります。 **したがって、OAuth 接続を作成することを強くお勧めします。**
>
>これらのタイプの接続の詳細については、を参照してください [サーバーからサーバーへの認証](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/) Adobeドキュメントの

接続を作成するには：

1. 任意の Adobe Authenticator モジュールで、接続フィールドの横にある「**追加**」をクリックします。
1. 次のフィールドに入力します。

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL Connection type]</td>
        <td>
          <p>OAuth サーバー間接続を作成するか、サービスアカウント（JWT）接続を作成するかを選択します。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Connection name]</td>
        <td>
          <p>この接続の名前を入力します。</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>[!DNL Adobe] クライアント ID を入力します。これは、[!DNL Adobe Developer Console] の [!UICONTROL Credentials details] セクションで確認できます。
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>[!DNL Adobe] クライアントの秘密鍵を入力します。これは、[!DNL Adobe Developer Console] の [!UICONTROL Credentials details] セクションで確認できます。
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Scopes]</td>
        <td>OAuth 接続を選択した場合は、この接続に必要なスコープを入力します。</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Technical account ID]</td>
        <td>[!DNL Adobe] テクニカルアカウント ID を入力します。これは、[!DNL Adobe Developer Console] の [!UICONTROL Credentials details] セクションで確認できます。
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Organization ID]</td>
        <td>JWT 接続を選択した場合は、 [!DNL Adobe] 組織 ID。 これは、[!DNL Adobe Developer Console] の [!UICONTROL Credentials details] セクションで確認できます。
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Meta Scopes]</td>
        <td>JWT 接続を選択した場合、この接続に必要なメタ範囲を入力します。 </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Private key]</td>
        <td>
          <p>JWT 接続を選択した場合は、で資格情報が作成されたときに生成された秘密鍵を [!DNL Adobe Developer Console]. </p>
          <p>秘密鍵または証明書を抽出するには：</p>
          <ol>
            <li value="1">
              <p><b>[!UICONTROL Extract]</b> をクリックします。</p>
            </li>
            <li value="2">
              <p>抽出するファイルのタイプを選択します。</p>
            </li>
            <li value="3">
              <p>秘密鍵または証明書を含むファイルを選択します。</p>
            </li>
            <li value="4">
              <p>ファイルのパスワードを入力します。</p>
            </li>
            <li value="5">
              <p><b>[!UICONTROL Save]</b> をクリックしてファイルを抽出し、接続設定に戻ります。</p>
            </li>
          </ol>
        </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL ベース URL]</td>
        <td>この認証を許可するベース URL を追加する必要があります。 シナリオの後半で「カスタム API 呼び出しを行う」モジュールを使用する場合、選択した URL への相対パスを追加します。 ここに URL を入力すると、カスタム API 呼び出しを行うモジュールが何に接続できるかを制御でき、セキュリティが強化されます。<p>認証システムに追加するベース URL ごとに、 <b>項目を追加</b> そして、ベース URL を入力します。</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Authentication URL]</td>
        <td>標準のAdobe IMS認証 URL を使用する場合は、これを空白のままにします。 <code>https://ims-na1.adobelogin.com</code>. 認証にAdobe IMSを使用しない場合は、認証に使用する URL を入力します。</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Environment]</td>
        <td>実稼動環境と非実稼動環境のどちらに接続するかを選択します。</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Type]</td>
        <td>サービスアカウントと個人アカウントのどちらに接続するかを選択します。</td>
      </tr>
    </tbody>
    </table>

1. 「**[!UICONTROL 続行]**」をクリックして接続を保存し、モジュールに戻ります。

## モジュール

### カスタム API 呼び出しの実行

このアクションモジュールを使用すると、任意のAdobe API を呼び出すことができます。

>[!TIP]
>
>接続先の API の URL 全体を入力する必要があります。 このモジュールは相対 URL を受け付けません。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Adobe Authenticator モジュールへの接続を作成する手順については、次を参照してください <a href="#create-a-connection" class="MCXref xref" >接続の作成</a> この記事の内容です。</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL URL]</p>
      </td>
      <td>
        <p>接続先の API ポイントの URL 全体を入力します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
   <td> <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]</a>での HTTP リクエストメソッドを参照してください。</p> </td> 
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>リクエストのヘッダーを標準 JSON オブジェクトの形式で追加します。</p>
        <p>例： <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion は、認証ヘッダーを自動的に追加します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>リクエストクエリ文字列を入力します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文の内容を追加します。</p> <p>メモ：  <p><code>if</code> などの条件ステートメントを JSON で使用する場合は、条件ステートメントの外側に引用符を挿入します。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
     <tr>
      <td role="rowheader">[!UICONTROL Limit]  </td>
      <td>
        <p>モジュールが 1 回の実行サイクルで返す結果の最大数を入力します。</p>
      </td>
    </tr>
  </tbody>
</table>
