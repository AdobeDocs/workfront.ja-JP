---
title: Jira ソフトウェアモジュール
description: ' [!DNL Adobe Workfront Fusion]  のシナリオでは、 [!DNL Jira] Software を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。'
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 6437fe98-2c2b-4b49-97e2-f94b23da93fd
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2072'
ht-degree: 100%

---

# [!DNL Jira Software] モジュール

[!DNL Adobe Workfront Fusion] のシナリオでは、[!DNL Jira Software] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。

シナリオの作成手順が必要な場合は、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) でのシナリオの作成を参照してください。

モジュールについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md) のモジュールを参照してください。

<!-- Bob Fix this compared to original -->

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td>
  <td> <p>[!UICONTROL Pro] 以降</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront]を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス ](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください

## 前提条件

[!DNL Jira] モジュールを使用するには、[!DNL Jira] アカウントが必要です。

## [!DNL Jira Software] を [!DNL Workfront Fusion] に接続

接続方法は、[!DNL Jira Cloud] を使用しているか、[!DNL Jira Server] を使用しているかによって決まります。

* [ [!DNL Jira Cloud]  を Workfront Fusion に接続](#connect-jira-cloud-to-workfront-fusion)
* [ [!DNL Jira Server]  を  [!DNL Workfront Fusion] に接続](#connect-jira-server-to-workfront-fusion)

### [!DNL Jira Cloud] を [!DNL Workfront Fusion] に接続

[!DNL Jira Cloud] を [!DNL Workfront Fusion] に接続

[!DNL Jira Software] を [!DNL Workfront Fusion] に接続するには、API トークンを作成し、それをサービス URL とユーザー名とともに [!DNL Workfront Fusion] の「[!UICONTROL 接続の作成]」フィールドに挿入する必要があります。

#### [!DNL Jira] での API トークンの作成

1. [https://id.atlassian.com/manage/api-tokens](https://id.atlassian.com/manage/api-tokens) に移動してログインします。
1. 「**[!UICONTROL API トークンを作成]**」をクリックします。
1. トークンの名前を入力します（例：*Workfront Fusion*）。
1. 「**[!UICONTROL クリップボードにコピー]**」ボタンを使用してトークンをコピーします。

   >[!IMPORTANT]
   >
   >このダイアログを閉じた後は、トークンを再度表示することはできません。
1. 生成されたトークンを安全な場所に保存します。
1. [ [!DNL Workfront Fusion]](#configure-the-jira-api-token-in-workfront-fusion) で [!DNL Jira] API トークンを設定するに進みます。

#### [!DNL Jira][!DNL Workfront Fusion] の API トークンを設定

1. [!DNL Workfront Fusion] で、[!DNL Jira] モジュールをシナリオに追加して、「**[!UICONTROL 接続を作成]**」ボックスを開きます。
1. 次の情報を指定します。

   * **[!UICONTROL サービス URL]**
   * **[!UICONTROL ユーザー名]**
   * **[!UICONTROL API トークン]：** これは、この記事の [ [!DNL Jira]](#create-an-api-token-in-jira) での API トークンの作成の節で作成した API トークンです。

1. 「[!UICONTROL 続行]」をクリックして接続を作成し、モジュールに戻ります。

### [!DNL Jira Server] を [!DNL Workfront Fusion] に接続

<!--
<p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Becky: Find out and document how to find these things</p>
-->

[!DNL Workfront Fusion] と [!DNL Jira Server] の間の接続を承認するには、コンシューマキー、プライベートキー、サービス URL が必要です。この情報については、[!DNL Jira] 管理者への問い合わせが必要になる場合があります。

* [ [!DNL Jira]  接続の公開キーと秘密鍵の生成](#generate-public-and-private-keys-for-your-jira-connection)
* [ [!DNL Jira] でクライアントアプリをコンシューマーとして設定する](#configure-the-client-app-as-a-consumer-in-jira)
* [ [!DNL Jira]  [!DNL Workfront Fusion] のサーバーまたは Jira データセンターへの接続の作成](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion)

#### [!DNL Jira] 接続の公開鍵と秘密鍵の生成

[!DNL Workfront Fusion Jira] 接続の秘密鍵を取得するには、公開鍵と秘密鍵を生成する必要があります。

1. ターミナルで、次の `openssl` コマンドを実行します。

   * `openssl genrsa -out jira_privatekey.pem 1024`

     このコマンドは、1024 ビットの秘密鍵を生成します。

   * `openssl req -newkey rsa:1024 -x509 -key jira_privatekey.pem -out jira_publickey.cer -days 365`

     このコマンドは X509 証明書を作成します。

   * `openssl pkcs8 -topk8 -nocrypt -in jira_privatekey.pem -out jira_privatekey.pcks8`

     このコマンドは、秘密鍵（PKCS8 形式）を `jira_privatekey.pcks8`
ファイルに抽出します。

   * `openssl x509 -pubkey -noout -in jira_publickey.cer  > jira_publickey.pem`

     このコマンドは、証明書から `jira_publickey.pem` ファイルに公開鍵を抽出します。

     >[!NOTE]
     >
     >Windows を使用している場合は、公開キーを `jira_publickey.pem` ファイルに手動で保存する必要がある場合があります。
     >
     >1. ターミナルで、次のコマンドを実行します。
     >   
     >   `openssl x509 -pubkey -noout -in jira_publickey.cer`
     >   
     >1. ターミナル出力をコピーする（`-------BEGIN PUBLIC KEY--------` と `-------END PUBLIC KEY--------` を含む）
     >   
     >1. ターミナル出力を `jira_publickey.pem` という名前のファイルに貼り付けます。


1. [ [!DNL Jira]](#configure-the-client-app-as-a-consumer-in-jira) でクライアントアプリをコンシューマーとして設定するに進んでください

#### [!DNL Jira] でクライアントアプリをコンシューマーとして設定する

1. [!DNL Jira] インスタンスにログインします。
1. 左のナビゲーションパネルで、**[!UICONTROL [!DNL Jira]設定]** ![](assets/jira-settings-icon.png)／**[!UICONTROL アプリケーション]**／**[!UICONTROL アプリケーションリンク]**&#x200B;をクリックします。
1. 「**[!UICONTROL リンクするアプリケーションの URL を入力]**」フィールドに、次のように入力します。

   ```
   https://app.workfrontfusion.com/oauth/cb/workfront-jiraserver-oauth1
   ```

1. 「**[!UICONTROL 新しいリンクを作成]**」をクリックします。「入力した URL から応答が受信しませんでした」というエラーメッセージを無視します。
1. **[!UICONTROL アプリケーションをリンク]**&#x200B;ウィンドウで、**[!UICONTROL Consumer key]** および **[!UICONTROL 共有シークレット]**&#x200B;フィールドに値を入力します。

   これらのフィールドの値を選択できます。

1. **[!UICONTROL Consumer key]** および&#x200B;**[!UICONTROL 共有シークレット]**&#x200B;フィールドの値を安全な場所にコピーします。

   これらの値は、設定プロセスの後半で必要になります。

1. URL フィールドに次のように入力します。

   | フィールド | 説明 |
   |---|---|
   | [!UICONTROL リクエストトークン URL] | `<Jira base url>/plugins/servlet/oauth/request-token` |
   | [!UICONTROL 認証 URL] | `<Jira base url>/plugins/servlet/oauth/authorize` |
   | [!UICONTROL アクセストークン URL] | `<Jira base url>/plugins/servlet/oauth/access-token` |

1. **[!UICONTROL 受信リンクを作成]**&#x200B;チェックボックスを選択します。
1. 「**[!UICONTROL 続行]**」をクリックします。
1. **[!UICONTROL アプリケーションをリンク]**&#x200B;ウィンドウで、次のフィールドに入力します。

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Consumer Key]</p> </td> 
      <td> 安全な場所にコピーした Consumer key を貼り付けます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Consumer name]</td> 
      <td>任意の名前を入力します。この名前は、参照用です。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Public key]</td> 
      <td><code>[!DNL jira_publickey.pem]</code> ファイルから公開鍵を貼り付けます。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL 続行]**」をクリックします。
1.  [!DNL Workfront Fusion]](#create-a-connection-to-jira-server-or-jira-data-center-in-workfront-fusion) で  [!DNL Jira Server]  または  [!DNL Jira Data Center]  への[接続を作成

#### [!DNL Workfront Fusion] で [!DNL Jira Server] または [!DNL Jira Data Center] への接続を作成

>[!NOTE]
>
>[!DNL Jira Server] アプリで [!DNL Jira Server] または [!DNL Jira Data Center] に接続します。
1. [!DNL Workfront Fusion] で任意の [!DNL Jira Server] モジュールで、「[!UICONTROL 接続]」フィールドの横にある「**[!UICONTROL 追加]**」をクリックします。
1. [!UICONTROL 接続の作成]パネルで、次のフィールドに入力します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td> <p>接続の名前を入力</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Consumer Key]</td> 
      <td><a href="#configure-the-client-app-as-a-consumer-in-jira" class="MCXref xref">[!DNL Jira]</a> でのクライアントアプリのコンシューマーとしての設定で、安全な場所にコピーした Consumer key に貼り付けます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Private Key]</td> 
      <td><a href="#generate-public-and-private-keys-for-your-jira-connection" class="MCXref xref">[!DNL Jira] 接続のパブリックキーとプライベートキーの生成</a>で作成した <code>[!DNL jira_privatekey.pcks8]</code> ファイルのとプライベートキーに貼り付けます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Service URL]</td> 
      <td>[!DNL Jira] インスタンス URLを入力します。 </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**[!UICONTROL 続行]**」をクリックして接続を作成し、モジュールに戻ります。

## [!DNL Jira Software] モジュールとそのフィールド

[!DNL Jira Software] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL Jira Software] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) におけるモジュール間の情報のマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [トリガー](#triggers)
* [アクション](#actions)
* [検索](#searches)

### トリガー

#### [!UICONTROL レコードの監視]

このトリガーモジュールは、レコードが追加、更新または削除された時点でシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>レコードの監視に使用する Web フックを選択します。 </p> <p>新規の web フックを追加するには、次の手順に従います。</p> 
    <ol> 
     <li value="1"><strong>[!UICONTROL Add]</strong> をクリックします。</li> 
     <li value="2">Web フックの名前を入力します。</li> 
     <li value="3"> <p>Web フックに使用する接続を選択します。 </p> <p>[!DNL Jira Software] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の<a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL Jira Software] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </li> 
     <li value="4"> <p>ソフトウェアで監視するレコードの種類を選択します。</p> 
      <ul> 
       <li>[!UICONTROL Comment] </li> 
       <li>[!UICONTROL Issue]</li> 
       <li>[!UICONTROL Project] </li> 
       <li>[!UICONTROL Sprint]</li> 
      </ul> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL スプリントへのイシューの追加]](#add-issue-to-sprint)
* [[!UICONTROL カスタム API 呼び出し]](#custom-api-call)
* [[!UICONTROL レコードの作成]](#create-a-record)
* [[!UICONTROL レコードの削除]](#delete-a-record)
* [[!UICONTROL 添付ファイルのダウンロード]](#download-an-attachment)
* [[!UICONTROL レコードの読み取り]](#read-a-record)
* [[!UICONTROL レコードの更新]](#update-a-record)

#### [!UICONTROL スプリントへのイシューの追加]

このアクションモジュールは、スプリントに 1 つ以上のイシューを追加します。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Jira Software] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL Jira Software] と [!DNL Workfront Fusion]</a> の接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sprint ID]</td> 
   <td>イシューを追加するスプリントのスプリント ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Issue ID or Keys]</td> 
   <td>スプリントに追加する各イシューのイシュー ID またはキーを追加します。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを作成]

このアクションモジュールは、Jira に新しいレコードを作成します。

このモジュールは、レコードに関連付けられた標準フィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Jira Software] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL Jira Software] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>モジュールで作成するレコードのタイプを選択します。レコードタイプを選択すると、そのレコードタイプに固有の他のフィールドがモジュールに表示されます。</p> 
    <ul> 
     <li>[!UICONTROL Attachment]</li> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL カスタム API 呼び出し]

このアクションモジュールは、[!DNL Jira Software] API に対して認証済みのカスタム呼び出しを実行します。これにより、他の [!DNL Jira Software] モジュールでは不可能なデータフロー自動処理を作成できます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Jira Software] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事内の <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL Jira Software]を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>相対パスを入力します<code>&lt;Instance URL>/rest/api/2/ </code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]</a>での HTTP リクエストメソッドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>リクエストのヘッダーを標準 JSON オブジェクトの形式で追加します。</p> <p>例： <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] によって、認証ヘッダーが追加されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>API 呼び出しのクエリを標準 JSON オブジェクトの形式で追加します。</p> <p>例： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文の内容を追加します。</p> <p>メモ：  <p><code>if</code> などの条件ステートメントを JSON で使用する場合は、条件ステートメントの外側に引用符を挿入します。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを削除]

このアクションモジュールは、特定のレコードを削除します。

レコードの ID を指定します。

このモジュールは、レコードの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Jira Software] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL Jira Software] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>モジュールで削除するレコードのタイプを選択します。 </p> 
    <ul> 
     <li>[!UICONTROL Attachment]</li> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID or Key]</td> 
   <td>削除するレコードの ID またはキーを入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 添付ファイルをダウンロード]

このアクションモジュールは、特定の添付ファイルをダウンロードします。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Jira Software] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事内の <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL Jira Software] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>ダウンロードする添付ファイルの ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードの読み取り]

このアクションモジュールは、[!DNL Jira Software] の単一レコードからデータを読み取ります。

レコードの ID を指定します。

このモジュールは、レコードに関連付けられた標準フィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Jira Software] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL Jira Software] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>モジュールが読み取る [!DNL Jira] レコードのタイプを選択します。</p> 
    <ul> 
     <li>[!UICONTROL Attachment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL User]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>受け取る出力を選択します。出力オプションは、「[!UICONTROL Record Type]」フィールドで選択したレコードのタイプに基づいて使用できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td> <p>モジュールが読み取るレコードの一意の [!DNL Jira Software] ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを更新]

このアクションモジュールは、イシューやプロジェクトなどの既存のレコードを更新します。

レコードの ID を指定します。

このモジュールは、レコードの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Jira Software] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL Jira Software] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>モジュールで更新するレコードのタイプを選択します。レコードタイプを選択すると、そのレコードタイプに固有の他のフィールドがモジュールに表示されます。</p> 
    <ul> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint] </li> 
     <li>[!UICONTROL Transition issue]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID or Key]</td> 
   <td>アップデートするレコードの ID またはキーを入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

### 検索

* [[!UICONTROL レコードをリスト表示]](#list-records)
* [[!UICONTROL レコードを検索]](#search-for-records)

#### [!UICONTROL レコードをリスト表示]

この検索モジュールは、検索クエリに一致する特定のタイプのすべての項目を取得します

この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Jira Software] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL Jira Software] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>モジュールのリストに表示するレコードのタイプを選択します。レコードタイプを選択すると、そのレコードタイプに固有の他のフィールドがモジュールに表示されます。</p> 
    <ul> 
     <li>[!UICONTROL Comment]</li> 
     <li>[!UICONTROL Issue]</li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Sprint issue]</li> 
     <li>[!UICONTROL Worklog]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Max Results]</p> </td> 
   <td> <p>シナリオの実行サイクルごとにモジュールが取得するレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">Offset</td> 
    <td> Enter or map the ID of the first item you want to retrieve details for. This is a way to paginate the records. If you enter the 5000th item as the offset, the module would return items 5000-9999.</td> 
   </tr>
  --> 
 </tbody> 
</table>

#### [!UICONTROL レコードを検索]

この検索モジュールは、指定された検索クエリに一致するレコードを [!DNL Jira Software] のオブジェクト内で検索します。

この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Jira Software] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の <a href="#connect-jira-software-to-workfront-fusion" class="MCXref xref" data-mc-variable-override="">[!DNL Jira Software] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td> <p>モジュールで検索するレコードのタイプを選択します。レコードタイプを選択すると、そのレコードタイプに固有の他のフィールドがモジュールに表示されます。</p> 
    <ul> 
     <li>[!UICONTROL Issues]</li> 
     <li> <p>[!UICONTROL Issues by JQL (Jira Query Lanuguage)] </p> <p>JQL について詳しくは、Atlassian のヘルプサイトで <a href="https://www.atlassian.com/blog/jira-software/jql-the-most-flexible-way-to-search-jira-14#:~:text=JQLstandsforJiraQuery,projectmanagers%2Candbusinessusers.">JQL</a> を参照してください。 </p> </li> 
     <li>[!UICONTROL Project]</li> 
     <li>[!UICONTROL Project by issue]</li> 
     <li>[!UICONTROL User]</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>
