---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Adobe Authenticatorモジュール
description: Adobe Authenticatorモジュールを使用すれば、1 回の接続で、API を使用して任意のAdobe製品に接続できます。
author: Becky
feature: Workfront Fusion
source-git-commit: 61a579c19228381d0aa06de3db5217614999731b
workflow-type: tm+mt
source-wordcount: '882'
ht-degree: 34%

---

# Adobe Authenticatorモジュール

Adobe Authenticatorモジュールを使用すると、1 つの接続を使用して任意のAdobeAPI に接続できます。 これにより、まだ専用の Fusion コネクタを持たないAdobe製品に簡単に接続できます。

HTTP モジュールの利点は、専用アプリと同様に接続を作成できる点です。

使用可能なAdobeAPI のリストについては、 [AdobeAPI](https://developer.adobe.com/apis). 割り当て先の API のみを使用できます。

## アクセス要件

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] プラン</td>
      <td>
        <p>新規：任意</p><p>または</p><p>現在： [!UICONTROL Pro] 以降</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td>
      <td>
        <p>新規：標準</p><p>または</p><p>現在： [!UICONTROL プラン ]、[!UICONTROL 作業 ]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス</td>
      <td>
   <p>現在の Fusion ライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来の Fusion ライセンス要件： [!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">製品</td>
      <td>
   <p>新しいWorkfrontプラン： [!UICONTROL Select] または [!UICONTROL Prime] をお持ちの場合 [!DNL Adobe Workfront] プラン（組織で購入する必要がある） [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。 [!DNL Workfront Fusion] は、[!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>現在のWorkfrontプラン：組織が購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</p>
   </td>
    </tr>
  </tbody>
</table>

## 前提条件

* モジュールを接続するAdobe製品にアクセスできる必要があります。
* Adobe Developerコンソールにアクセスできる必要があります。
* Adobe Developerコンソール上に、モジュールが接続する API を含むプロジェクトが必要です。 実行できる操作：

   * API を使用して新しいプロジェクトを作成します。

     または
   * 既存のプロジェクトに API を追加します。

  Adobe Developer Console で API を作成またはプロジェクトに追加する方法について詳しくは、 [プロジェクトの作成](https://developer.adobe.com/dep/guides/dev-console/create-project/) (Adobeドキュメント )

## 接続の作成

Adobe Authenticator接続は、Adobe Developerコンソールの単一のプロジェクトに接続します。 複数のAdobeAPI で同じ接続を使用するには、同じプロジェクトに API を追加し、そのプロジェクトへの接続を作成します。

別々のプロジェクトに対して別々の接続を作成することはできますが、接続を使用して、その接続で指定されたプロジェクト上にない API にアクセスすることはできません。

>[!IMPORTANT]
>
>Adobe Authenticatorコネクタを使用する場合は、OAuth サーバー間接続と、サービスアカウント (JWT) 接続のどちらを使用するかを選択できます。 Adobeで非推奨となった JWT 資格情報は、2025 年 1 月 1 日以降に機能しなくなります。 **したがって、OAuth 接続を作成することを強くお勧めします。**
>
>これらのタイプの接続について詳しくは、 [サーバー間認証](https://developer.adobe.com/developer-console/docs/guides/authentication/ServerToServerAuthentication/) (Adobeドキュメント )

接続を作成するには：

1. 任意のAdobe Authenticatorモジュールで、 **追加** 「接続」フィールドの横に表示されます。
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
          <p>OAuth サーバー間接続とサービスアカウント (JWT) 接続のどちらを作成するかを選択します。</p>
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
        <td>JWT 接続を選択した場合は、この接続に必要なメタスコープを入力します。 </td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Private key]</td>
        <td>
          <p>JWT 接続を選択した場合は、 [!DNL Adobe Developer Console]. </p>
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
        <td role="rowheader">[!UICONTROL 環境 ]</td>
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

### カスタム API 呼び出しを実行

このアクションモジュールを使用すると、任意のAdobeAPI を呼び出すことができます。

>[!TIP]
>
>接続先の API の URL 全体を入力する必要があります。 このモジュールは相対 URL を受け付けません。

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
     <td>Adobe Authenticatorモジュールへの接続を作成する手順については、 <a href="#create-a-connection" class="MCXref xref" >接続の作成</a> 」を参照してください。</td>
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

