---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: ServiceNow モジュール
description: ' [!DNL Adobe Workfront Fusion]  のシナリオでは、 [!DNL ServiceNow] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。'
author: Becky
feature: Workfront Fusion
exl-id: b362cd8b-06b3-4f4c-b405-a2afc24abddb
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '1613'
ht-degree: 100%

---

# [!DNL ServiceNow] モジュール

[!DNL Adobe Workfront Fusion] のシナリオでは、[!DNL ServiceNow] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。

シナリオの作成手順が必要な場合は、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) でのシナリオの作成を参照してください。

モジュールについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md) のモジュールを参照してください。

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
   <p>従来のライセンス要件： [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、[!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も組織で購入する必要があります。[!DNL Workfront Fusion] は [!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明されている機能を使用するには、[!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについては、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

[!DNL ServiceNow] モジュールを使用するには、[!DNL ServiceNow] アカウントが必要です。

## [!DNL ServiceNow] を [!DNL Workfront Fusion] に接続

[!DNL ServiceNow] モジュールへの接続を作成するには、以下を実行します。

1. 最初の [!DNL ServiceNow] モジュールの設定を開始するときは、「[!UICONTROL 接続]」ボックスの横にある「**[!UICONTROL 追加]**」をクリックします。
1. 以下の情報を入力します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td>新しい [!DNL ServiceNow] 接続の名前を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Username]</p> </td> 
      <td>[!DNL ServiceNow] ユーザー名を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Password]</p> </td> 
      <td>ServiceNow パスワードを入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Instance]</p> </td> 
      <td> <p><code>https://</code>を付けずに[!DNL ServiceNow]アカウントのアドレスを入力します（通常は<code>&lt;company>.service-now.com</code>）。</p> </td> 
     </tr> 
    </tbody> 
   </table>

## [!UICONTROL ServiceNow] モジュールとそのフィールド

[!DNL ServiceNow] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL ServiceNow] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でモジュールから別のモジュールに情報をマッピングを参照してください。

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>カスタムレコードが「[!UICONTROL レコードタイプ]」フィールドで選択された場合、カスタムフィールドの読み込みに時間がかかる場合があります。
>
>カスタムレコードがない場合、ドロップダウンは空になります。

* [[!UICONTROL レコードを監視]](#watch-records)
* [[!UICONTROL カスタム API 呼び出し]](#custom-api-call)
* [[!UICONTROL レコードの読み取り]](#read-a-record)
* [[!UICONTROL ユーザーを非アクティブ化]](#deactivate-a-user)
* [[!UICONTROL 添付ファイルをダウンロード]](#download-an-attachment)
* [[!UICONTROL 添付ファイルをアップロード]](#upload-an-attachment)
* [[!UICONTROL レコードを作成]](#create-a-record)
* [[!UICONTROL レコードをアップデート]](#update-a-record)
* [[!UICONTROL レコードを削除]](#delete-a-record)
* [[!UICONTROL レコードを検索]](#search-for-records)

### [!UICONTROL レコードを監視]

このトリガーモジュールは、レコードが作成またはアップデートされたときにシナリオをアクティブ化します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>ServiceNow アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事にある<a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">[!DNL ServiceNow] を [!UICONTROL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table type]</td> 
   <td>監視するテーブルがカスタムテーブルであるか標準テーブルであるかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td>監視するレコードのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>表示する値のタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>モジュールから出力するフィールドを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>新しいレコードまたは更新されたレコードのどちらを監視するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL カスタム API 呼び出し]

このアクションモジュールは、[!DNL ServiceNow] API に対して認証済みのカスタム呼び出しを実行します。これにより、他の [!DNL ServiceNow] モジュールでは達成できないデータフローの自動化を作成できます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>ServiceNow アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">[!DNL ServiceNow] を [!UICONTROL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Relative URL]</td> 
   <td> <p>モジュールとやり取りする web サーバー上のアドレスを入力します。</p> <p>相対 URL を入力できます。つまり、<code>http://</code> などのプロトコルを最初に含める必要はありません。これは、web サーバー上でやり取りが発生していることを示しています。</p> <p>例： <code>[!DNL /api/conversations].create</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]</a> での HTTP リクエストメソッドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>リクエストのヘッダーを標準 JSON オブジェクトの形式で追加します。</p> <p>例： <code>{"Content-type":"application/json"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>API 呼び出しのクエリを標準 JSON オブジェクトの形式で追加します。</p> <p>例： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文の内容を追加します。</p> <p>メモ：  <p><code>if</code> などを条件ステートメントを JSON で使用する場合は、条件ステートメントの外側に引用符を置きます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードの読み取り]

このアクションモジュールは、システム IDを使用して [!DNL ServiceNow] レコードを読み取ります。

このモジュールは、レコードに関連付けられた標準フィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>ServiceNow アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">[!DNL ServiceNow] を [!UICONTROL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record System ID]</td> 
   <td>モジュールが読み取るレコードの一意の [!DNL ServiceNow] ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table type]</td> 
   <td>読み取るレコードがカスタムテーブルか標準テーブルかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>モジュールが読み取る [!DNL ServiceNow] レコードのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>表示する値のタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>モジュールから出力するフィールドを選択します。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL ユーザーを非アクティブ化する]

このアクションモジュールは、システム ID を使用することで [!DNL ServiceNow] でユーザーを非アクティブ化します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>ServiceNow アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">[!DNL ServiceNow] を [!UICONTROL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL User System ID]</td> 
   <td> モジュールを非アクティブ化するユーザーの一意の [!DNL ServiceNow] ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 添付ファイルのダウンロード]

このアクションモジュールは、[!DNL ServiceNow] レコードの添付ファイルをダウンロードします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>ServiceNow アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">[!DNL ServiceNow] を [!UICONTROL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Attachment System ID]</td> 
   <td> モジュールでダウンロードする添付ファイルの一意の [!DNL ServiceNow] ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 添付ファイルをアップロード]

このアクションモジュールは、添付ファイルを [!DNL ServiceNow] レコードにアップロードします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>ServiceNow アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">[!DNL ServiceNow] を [!UICONTROL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table name]</td> 
   <td>添付ファイルをアップロードするテーブルの名前を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL System ID]</td> 
   <td>添付ファイルをアップロードするシステムの一意の [!DNL ServiceNow] ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>添付ファイルの名前を入力またはマッピングします</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File content]</td> 
   <td>[!DNL ServiceNow] にアップロードするファイルを入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードを作成]

このアクションモジュールは、新しい [!DNL ServiceNow] レコードを作成します。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>ServiceNow アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事にある <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">[!DNL ServiceNow] を [!UICONTROL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table type]</td> 
   <td>カスタムテーブルと標準テーブルのどちらでレコードを作成するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>モジュールで作成する [!DNL ServiceNow] レコードのタイプを選択します。その後で、このレコードタイプで使用可能なフィールドに入力できます。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードをアップデート]

このアクションモジュールは、新しい [!DNL ServiceNow] レコードを作成します。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>ServiceNow アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">[!DNL ServiceNow][!UICONTROL Workfront Fusion] への接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record System ID]</td> 
   <td>モジュールでアップデートするレコードの一意の [!DNL ServiceNow] ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table type]</td> 
   <td>アップデートするレコードがカスタムテーブルにあるか、標準テーブルにあるかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>モジュールでアップデートする [!DNL ServiceNow] レコードのタイプを選択します。その後で、このレコードタイプで使用可能なフィールドに入力できます。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードの削除]

このアクションモジュールは、インシデントやユーザーを削除します。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>ServiceNow アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">[!DNL ServiceNow][!UICONTROL Workfront Fusion] への接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record Type]</td> 
   <td>インシデントを削除するか、ユーザーを削除するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL System ID]</td> 
   <td>モジュールで削除するレコードの一意の [!DNL ServiceNow] ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードの検索]

このモジュールは、選択した条件を使用してレコードを検索します。

このモジュールは、レコードに関連付けられた標準フィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>ServiceNow アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">[!DNL ServiceNow][!UICONTROL Workfront Fusion] への接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table type]</td> 
   <td>検索するテーブルがカスタムテーブルか標準テーブルかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td>検索するレコードのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Result set]</td> 
   <td>モジュールが条件に一致するすべてのレコードを返すか、条件に一致する最初のレコードのみを返すかを選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximal count of records]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search type]</td> 
   <td> <p>モジュールで実行する検索のタイプを選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Advanced query]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL Search Query]</p> <p>カスタム検索クエリを入力します。[!DNL ServiceNow]カスタム検索クエリについて詳しくは、<a href="https://docs.servicenow.com/bundle/orlando-platform-user-interface/page/use/common-ui-elements/reference/r_OpAvailableFiltersQueries.html">ServiceNow のクエリドキュメント</a>を参照してください。</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Simple]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL Search Criteria]</p> <p>モジュールで検索する条件を入力します。検索フィルターの設定に関して詳しくは、<a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Adobe Workfront Fusion でシナリオにフィルターを追加</a>を参照してください。</p> </li> 
       <li> <p>[!UICONTROL Sort by]</p> <p>モジュールで結果を並べ替える基準となるフィールドと、結果を昇順または降順のどちらで並べ替えるかを指定します。</p> </li> 
      </ul> </li> 
    </ul> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Display]</td> 
   <td>表示する値のタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>モジュールから出力するフィールドを選択します。</td> 
  </tr> 
 </tbody> 
</table>
