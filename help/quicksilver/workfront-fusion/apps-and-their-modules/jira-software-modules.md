---
title: Jira Software モジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Jira] ソフトウェアを使用し、複数のサードパーティのアプリケーションやサービスに接続します。
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 6437fe98-2c2b-4b49-97e2-f94b23da93fd
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2085'
ht-degree: 1%

---

# [!DNL Jira Software] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Jira Software]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

シナリオの作成手順については、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

モジュールについて詳しくは、 [のモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

<!-- Bob Fix this compared to original -->

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td>
  <td> <p>[!UICONTROL Pro] 以降</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] がある場合 [!DNL Adobe Workfront] プラン（組織で購入する必要がある） [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。 [!DNL Workfront Fusion] は、[!UICONTROL Ultimate] に含まれています [!DNL Workfront] プラン</p>
   <p>または</p>
   <p>従来の製品要件：組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 前提条件

使用する [!DNL Jira] モジュールには [!DNL Jira] アカウント

## 接続 [!DNL Jira Software] から [!DNL Workfront Fusion]

接続方法は、 [!DNL Jira Cloud] または [!DNL Jira Server].

* [接続 [!DNL Jira Cloud] Workfront Fusion](#connect-jira-cloud-to-workfront-fusion)
* [接続 [!DNL Jira Server] から [!DNL Workfront Fusion]](#connect-jira-server-to-workfront-fusion)

### 接続 [!DNL Jira Cloud] から [!DNL Workfront Fusion]

接続 [!DNL Jira Cloud] から [!DNL Workfront Fusion]

接続するには [!DNL Jira Software] から [!DNL Workfront Fusion]を使用する場合は、API トークンを作成し、サービス URL とユーザー名と共にを [!UICONTROL 接続の作成] ～に入る [!DNL Workfront Fusion].

#### での API トークンの作成 [!DNL Jira]

1. に移動します。 [https://id.atlassian.com/manage/api-tokens](https://id.atlassian.com/manage/api-tokens) をクリックし、ログインします。
1. クリック **[!UICONTROL API トークンを作成]**.
1. トークンの名前を入力します（例： ）。 *Workfront Fusion*.
1. を使用してトークンをコピーします。 **[!UICONTROL クリップボードにコピー]** 」ボタンをクリックします。

   >[!IMPORTANT]
   >
   >このダイアログを閉じた後は、トークンを再度表示することはできません。
1. 生成されたトークンを安全な場所に保存します。
1. 続行 [の設定 [!DNL Jira] の API トークン [!DNL Workfront Fusion]](#configure-the-jira-api-token-in-workfront-fusion).

#### の設定 [!DNL Jira] の API トークン [!DNL Workfront Fusion]

1. In [!DNL Workfront Fusion]、 [!DNL Jira] モジュールをシナリオに追加して、 **[!UICONTROL 接続の作成]** ボックス
1. 次の情報を指定します。

   * **[!UICONTROL サービス URL]**
   * **[!UICONTROL ユーザー名]**
   * **[!UICONTROL API トークン]:** これは、 [での API トークンの作成 [!DNL Jira]](#create-an-api-token-in-jira) 」の節を参照してください。

1. クリック [!UICONTROL 続行] 接続を作成し、モジュールに戻ります。

### 接続 [!DNL Jira Server] から [!DNL Workfront Fusion]

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Becky: Find out and document how to find these things</p>
-->

次の間の接続を許可するには： [!DNL Workfront Fusion] および [!DNL Jira Server]の場合は、消費者キー、秘密鍵、サービス URL が必要です。 場合によっては、 [!DNL Jira] 管理者を参照してください。

* [の公開鍵と秘密鍵を生成 [!DNL Jira] 接続](#generate-public-and-private-keys-for-your-jira-connection)
* [でクライアントアプリをコンシューマーとして設定する [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)
* [への接続の作成 [!DNL Jira] のサーバーまたは Jira データセンター [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### の公開鍵と秘密鍵を生成 [!DNL Jira] 接続

の秘密鍵を取得するには [!DNL Workfront Fusion Jira] 接続する場合は、公開鍵と秘密鍵を生成する必要があります。

1. ターミナルで、次を実行します。 `openssl` コマンド

   * `openssl genrsa -out jira_privatekey.pem 1024`

     このコマンドは、1024 ビットの秘密鍵を生成します。

   * `openssl req -newkey rsa:1024 -x509 -key jira_privatekey.pem -out jira_publickey.cer -days 365`

     このコマンドは X509 証明書を作成します。

   * `openssl pkcs8 -topk8 -nocrypt -in jira_privatekey.pem -out jira_privatekey.pcks8`

     このコマンドは、秘密鍵（PKCS8 形式）を `jira_privatekey.pcks8`
ファイル。

   * `openssl x509 -pubkey -noout -in jira_publickey.cer  > jira_publickey.pem`

     このコマンドは、証明書から `jira_publickey.pem` ファイル。

     >[!NOTE]
     >
     >Windows を使用している場合は、公開鍵を `jira_publickey.pem` ファイルを手動で作成：
     >
     >1. ターミナルで、次のコマンドを実行します。
     >   
     >   `openssl x509 -pubkey -noout -in jira_publickey.cer`
     >   
     >1. ターミナル出力 ( `-------BEGIN PUBLIC KEY--------` および `-------END PUBLIC KEY--------`
     >   
     >1. ターミナル出力を、 `jira_publickey.pem`.


1. 続行 [でクライアントアプリをコンシューマーとして設定する [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira)

#### でクライアントアプリをコンシューマーとして設定する [!DNL Jira]

1. にログインします。 [!DNL Jira] インスタンス。
1. 左側のナビゲーションパネルで、 **[!UICONTROL [!DNL Jira]設定]** ![](assets/jira-settings-icon.png) > **[!UICONTROL アプリ]**> **[!UICONTROL アプリリンク]**.
1. 内 **[!UICONTROL リンクするアプリケーションの URL を入力]** フィールドに入力

   ```
   https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1
   ```

1. クリック **[!UICONTROL 新しいリンクを作成]**. 「入力した URL から応答が受信されませんでした」というエラーメッセージを無視します。
1. 内 **[!UICONTROL アプリのリンク]** ウィンドウで、 **[!UICONTROL 消費者キー]** および **[!UICONTROL 共有暗号鍵]** フィールド。

   これらのフィールドの値を選択できます。

1. 次の値をコピー： **[!UICONTROL 消費者キー]** および **[!UICONTROL 共有暗号鍵]** フィールドを安全な場所に設定します。

   これらの値は、後で設定プロセスで必要になります。

1. 「 URL 」フィールドに次のように入力します。

   | フィールド | 説明 |
   |---|---|
   | [!UICONTROL リクエストトークン URL] | `<Jira base url>/plugins/servlet/oauth/request-token` |
   | [!UICONTROL 認証 URL] | `<Jira base url>/plugins/servlet/oauth/authorize` |
   | [!UICONTROL トークン URL にアクセス] | `<Jira base url>/plugins/servlet/oauth/access-token` |

1. を選択します。 **[!UICONTROL 受信リンクを作成]** チェックボックス。
1. クリック **[!UICONTROL 続行]**.
1. 内 **[!UICONTROL アプリをリンク]** ウィンドウで、次のフィールドに入力します。

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 消費者キー ]</p> </td> 
      <td> 安全な場所にコピーした消費者キーを貼り付けます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 消費者名 ]</td> 
      <td>任意の名前を入力します。 この名前は、参照用です。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 公開鍵 ]</td> 
      <td>公開鍵を <code>[!DNL jira_publickey.pem]</code> ファイル。</td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **[!UICONTROL 続行]**.
1. 続行 [への接続の作成 [!DNL Jira Server] または [!DNL Jira Data Center] in [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### への接続の作成 [!DNL Jira Server] または [!DNL Jira Data Center] in [!DNL Workfront Fusion]

>[!NOTE]
>
>以下を使用： [!DNL Jira Server] 接続するアプリ [!DNL Jira Server] または [!DNL Jira Data Center].
1. 任意の [!DNL Jira Server] モジュール [!DNL Workfront Fusion]をクリックし、 **[!UICONTROL 追加]** の横 [!UICONTROL 接続] フィールドに入力します。
1. 内 [!UICONTROL 接続の作成] パネルで、次のフィールドに入力します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 接続名 ]</p> </td> 
      <td> <p>接続名を入力</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 消費者キー ]</td> 
      <td>安全な場所 ( <a href="#configure-the-client-app-as-a-consumer-in-jira" class="MCXref xref">でクライアントアプリをコンシューマーとして設定する [!DNL Jira]</a></td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Private Key]</td> 
      <td>秘密鍵に、 <code>[!DNL jira_privatekey.pcks8]</code> で作成したファイル <a href="#generate-public-and-private-keys-for-your-jira-connection" class="MCXref xref">の公開鍵と秘密鍵を生成 [!DNL Jira] 接続</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Service URL]</td> 
      <td>を入力します。 [!DNL Jira] インスタンス URL。 </td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **[!UICONTROL 続行]** 接続を作成し、モジュールに戻ります。

## [!DNL Jira Software] モジュールとそのフィールド

設定時に [!DNL Jira Software] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Jira Software] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [トリガー](#triggers)
* [アクション](#actions)
* [検索](#searches)

### トリガー

#### [!UICONTROL レコードの監視]

このトリガーモジュールは、レコードが追加、更新または削除されたときにシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>レコードの監視に使用する Webhook を選択します。 </p> <p>新しい Webhook を追加するには：</p> 
    <ol> 
     <li value="1">クリック <strong>[!UICONTROL 追加 ]</strong></li> 
     <li value="2">ウェブフックの名前を入力します。</li> 
     <li value="3"> <p>Webhook に使用する接続を選択します。 </p> <p>接続方法 [!DNL Jira Software] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">接続 [!DNL Jira Software] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </li> 
     <li value="4"> <p>ソフトウェアで監視するレコードの種類を選択します。</p> 
      <ul> 
       <li>[!UICONTROL コメント ] </li> 
       <li>[!UICONTROL の問題 ]</li> 
       <li>[!UICONTROL プロジェクト ] </li> 
       <li>[!UICONTROL Sprint]</li> 
      </ul> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL スプリントに問題を追加]](#add-issue-to-sprint)
* [[!UICONTROL カスタム API 呼び出し]](#custom-api-call)
* [[!UICONTROL レコードの作成]](#create-a-record)
* [[!UICONTROL レコードの削除]](#delete-a-record)
* [[!UICONTROL 添付ファイルのダウンロード]](#download-an-attachment)
* [[!UICONTROL レコードを読み取る]](#read-a-record)
* [[!UICONTROL レコードの更新]](#update-a-record)

#### [!UICONTROL スプリントに問題を追加]

このアクションモジュールは、スプリントに 1 つ以上の問題を追加します。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Jira Software] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">接続 [!DNL Jira Software] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sprint ID]</td> 
   <td>イシューを追加するスプリントのスプリント ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 問題 ID またはキー ]</td> 
   <td>スプリントに追加する各イシューのイシュー ID またはキーを追加します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードの作成]

このアクションモジュールは、Jira に新しいレコードを作成します。

このモジュールは、レコードに関連付けられた標準フィールドと、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Jira Software] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">接続 [!DNL Jira Software] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>モジュールで作成するレコードのタイプを選択します。 レコードタイプを選択すると、そのレコードタイプに固有の他のフィールドがモジュールに表示されます。</p> 
    <ul> 
     <li>[!UICONTROL 添付ファイル ]</li> 
     <li>[!UICONTROL コメント ]</li> 
     <li>[!UICONTROL の問題 ]</li> 
     <li>[!UICONTROL プロジェクト ]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カスタム API 呼び出し]

このアクションモジュールを使用すると、 [!DNL Jira Software] API これにより、他のユーザーが達成できないデータフローの自動化を作成できます [!DNL Jira Software] モジュール。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Jira Software] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">接続 [!DNL Jira Software] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>相対パスを入力<code>&lt;Instance URL>/rest/api/2/ </code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メソッド ]</td> 
   td&gt; <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] によって、認証ヘッダーが追加されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しのクエリを追加します。</p> <p>例： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文のコンテンツを追加します。</p> <p>メモ:  <p>条件文 ( <code>if</code> JSON で、条件文の外側に引用符を置きます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードの削除]

このアクションモジュールは、特定のレコードを削除します。

レコードの ID を指定します。

このモジュールは、レコードと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Jira Software] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">接続 [!DNL Jira Software] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>モジュールで削除するレコードのタイプを選択します。 </p> 
    <ul> 
     <li>[!UICONTROL 添付ファイル ]</li> 
     <li>[!UICONTROL コメント ]</li> 
     <li>[!UICONTROL の問題 ]</li> 
     <li>[!UICONTROL プロジェクト ]</li> 
     <li>[!UICONTROL Sprint] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID またはキー ]</td> 
   <td>削除するレコードの ID またはキーを入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 添付ファイルのダウンロード]

このアクションモジュールは、特定の添付ファイルをダウンロードします。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Jira Software] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">接続 [!DNL Jira Software] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>ダウンロードする添付ファイルの ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを読み取る]

このアクションモジュールは、 [!DNL Jira Software].

レコードの ID を指定します。

このモジュールは、レコードに関連付けられた標準フィールドと、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Jira Software] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">接続 [!DNL Jira Software] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>タイプを選択 [!DNL Jira] を記録します。</p> 
    <ul> 
     <li>[!UICONTROL 添付ファイル ]</li> 
     <li>[!UICONTROL の問題 ]</li> 
     <li>[!UICONTROL プロジェクト ]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL ユーザー ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td>受信する出力を選択します。 出力オプションは、「[!UICONTROL レコードタイプ ]」フィールドで選択したレコードのタイプに基づいて使用できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>一意の [!DNL Jira Software] モジュールが読み取るレコードの ID。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードの更新]

このアクションモジュールは、問題やプロジェクトなどの既存のレコードを更新します。

レコードの ID を指定します。

このモジュールは、レコードと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Jira Software] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">接続 [!DNL Jira Software] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>モジュールで更新するレコードのタイプを選択します。 レコードタイプを選択すると、そのレコードタイプに固有の他のフィールドがモジュールに表示されます。</p> 
    <ul> 
     <li>[!UICONTROL コメント ]</li> 
     <li>[!UICONTROL の問題 ]</li> 
     <li>[!UICONTROL プロジェクト ]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL 移行の問題 ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID またはキー ]</td> 
   <td>更新するレコードの ID またはキーを入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

### 検索

* [[!UICONTROL レコードのリスト]](#list-records)
* [[!UICONTROL レコードの検索]](#search-for-records)

#### [!UICONTROL レコードのリスト]

この検索モジュールは、検索クエリに一致する特定のタイプのすべての項目を取得します

この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Jira Software] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">接続 [!DNL Jira Software] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>モジュールのリストに表示するレコードのタイプを選択します。 レコードタイプを選択すると、そのレコードタイプに固有の他のフィールドがモジュールに表示されます。</p> 
    <ul> 
     <li>[!UICONTROL コメント ]</li> 
     <li>[!UICONTROL の問題 ]</li> 
     <li>[!UICONTROL プロジェクト ]</li> 
     <li>[!UICONTROL Sprint の問題 ]</li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 最大結果数 ]</p> </td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールで取得するレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Offset</td> 
    <td> Enter or map the ID of the first item you want to retrieve details for. This is a way to paginate the records. If you enter the 5000th item as the offset, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL レコードの検索]

この検索モジュールは、 [!DNL Jira Software] 指定した検索クエリに一致する

この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL Jira Software] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">接続 [!DNL Jira Software] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>モジュールで検索するレコードのタイプを選択します。 レコードタイプを選択すると、そのレコードタイプに固有の他のフィールドがモジュールに表示されます。</p> 
    <ul> 
     <li>[!UICONTROL の問題 ]</li> 
     <li> <p>[!UICONTROL JQL (Jira Query Language) による問題 ] </p> <p>JQL について詳しくは、 <a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQLstandsforJiraQuery,projectmanagers%2Candbusinessusers.">JQL</a> アトラシアのヘルプサイトで </p> </li> 
     <li>[!UICONTROL プロジェクト ]</li> 
     <li>[!UICONTROL プロジェクト（発行別）]</li> 
     <li>[!UICONTROL ユーザー ]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
