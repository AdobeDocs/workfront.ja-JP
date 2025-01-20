---
filename: workday-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Workday モジュール
description: Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。 この記事は廃止されましたが、この機能を説明する新しい記事へのリンクが含まれています。
author: Becky
feature: Workfront Fusion
exl-id: 535573e0-b6ad-43a2-b7cb-ed32d1dc8d16
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1080'
ht-degree: 89%

---

# [!DNL Workday] モジュール

>[!IMPORTANT]
>
>Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。
>
>この記事の情報は、次の記事に記載されています。
>
>* [Workday モジュール ](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/workday-modules.html)
>
>ブックマークを更新してください。
>
>この記事は現在更新されておらず、近い将来に削除されます。

[!DNL Adobe Workfront Fusion] のシナリオでは、[!DNL Workday] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。

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
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] の [!DNL Adobe Workfront] プランがある場合、この記事に記載されている機能を使用するには、組織で [!DNL Adobe Workfront Fusion] の購入 [!DNL Adobe Workfront] 必要です。 [!DNL Workfront Fusion] は、[!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront]を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

[!DNL Workday] モジュールを使用するには、

* [!DNL Workday] アカウントが必要です。

* [!DNL Workday] で OAuth アプリケーションを作成する必要があります。手順については、[!DNL Workday] のドキュメントを参照してください。

## Workday API の情報

Workday コネクタでは、以下を使用します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">ベース URL</td> 
   <td>https://&lbrace;&lbrace;connection.servicesUrl&rbrace;&rbrace;/api</td> 
  </tr>
  <tr> 
   <td role="rowheader">API タグ</td> 
   <td>v1.6.4</td> 
  </tr>
 </tbody> 
 </table>

## [!DNL Workday] を [!DNL Workfront Fusion] に接続

1. 任意の [!DNL Workfront Fusion] モジュールで、「[!UICONTROL 接続]」フィールドの横にある「[!UICONTROL 追加]」をクリックします。

2. 次のフィールドに入力します。

   <table style="table-layout:auto"> 
        <col/>
        <col/>
        <tbody>
            <tr>
                <td role="rowheader">
                    <p role="rowheader">[!UICONTROL Connection name]</p>
                </td>
                <td>接続の名前を入力</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Workday host]</td>
                <td><code>https://</code> を付けずに [!DNL Workday] ホストのアドレスを入力します。例：<code>mycompany.workday.com</code></td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Services URL]</td>
                <td><code>https://</code> を付けずに [!DNL Workday] web サービスのアドレスを入力します。例：<code>mycompany-services.workday.com</code></td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Tenant name]</td>
                <td>この [!DNL Workday] アカウントのテナントを入力します。テナントは所属先組織の識別子で、Workday へのログインに使用する URL に含まれています。例：アドレス <code>https://www.myworkday.com/mycompany</code> の場合、テナントは <code>mycompany</code> です。</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Client ID]</td>
                <td>この接続で使用する [!DNL Workday] アプリケーションのクライアント ID を入力します。これは、[!DNL Workday] でアプリケーションを作成する際に取得します。</td>
            </tr>
            <tr>
                <td  role="rowheader">[!UICONTROL Client Secret]</td>
                <td>この接続で使用する [!DNL Workday] アプリケーションのクライアントシークレットを入力します。これは、[!DNL Workday] でアプリケーションを作成する際に取得します。</td>
            </tr>
            <tr>
                <td role="rowheader">[!UICONTROL Session timeout (min)]</td>
                <td >認証トークンの有効期限を分単位で入力します。</td>
            </tr>
        </tbody>
    </table>


3. 「[!UICONTROL 続行]」をクリックして接続を保存し、モジュールに戻ります。

## [!DNL Workday] モジュールとそのフィールド

[!DNL Workday] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL Workday] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でモジュールから別のモジュールに情報をマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [アクション](#action)

* [検索](#search)


### アクション

* [[!UICONTROL レコードを作成]](#create-a-record)

* [[!UICONTROL レコードを削除]](#delete-a-record)

* [[!UICONTROL カスタム API 呼び出しを実行]](#make-a-custom-api-call)

* [[!UICONTROL レコードを更新]](#update-a-record)


#### [!UICONTROL レコードを作成]

このアクションモジュールは、[!DNL Workday] 内で 1 つのレコードを作成します。

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>[!DNL Workday] アカウントを Workfront Fusion に接続する手順については、<a href="#Connect" class="MCXref xre[!DNL ]f" >[!DNL Workday] を [!DNL Workfront Fusion]</a> に接続を参照してください。</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Record Type]</td>
            <td>作成するレコードのタイプを選択します。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>作成するレコードの ID を入力またはマッピングします。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Subresource ID]</td>
            <td >作成するサブリソースの ID を入力またはマッピングします。</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL レコードを削除]

このアクションモジュールは、[!DNL Workday] 内のレコードを 1 つ削除します。

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>[!DNL Workday] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="#Connect" class="MCXref xre[!DNL ]f" >[!DNL Workday] を [!DNL Workfront Fusion]</a> に接続を参照してください。</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Record type]</td>
            <td>削除するレコードのタイプを選択します。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Specific record type]</td>
            <td>削除するレコードの特定のタイプを選択します。これらは、選択したレコードタイプに基づきます。</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Subresource ID]</td>
            <td>削除するサブリソースの ID を入力またはマッピングします。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >削除するレコードの ID を入力またはマッピングします。</td>
        </tr>
    </tbody>
</table>


### [!UICONTROL カスタム API 呼び出しを実行]

このアクションモジュールでは、[!DNL Workday] API への認証済みのカスタム呼び出しを実行できます。これにより、他の [!DNL Workday] モジュールでは不可能なデータフロー自動処理を作成できます。

このモジュールを設定する際には、次のフィールドが表示されます。

このモジュールは、ステータスコードと共に API 呼び出しのヘッダーと本文を返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!DNL Connection]</p> </td> 
            <td>[!DNL Workday] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="#Connect" class="MCXref xre[!DNL ]f" >[!DNL Workday] を [!DNL Workfront Fusion]</a> に接続を参照してください。</td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td><code style="color: #ff1493;">https://&lt;tenantHostname>/api/&lt;serviceName>/&lt;version>/&lt;tenant></code> への相対パスを入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a>での HTTP リクエストメソッドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>リクエストのヘッダーを標準 JSON オブジェクトの形式で追加します。</p> <p>例： <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] によって認証ヘッダーが追加されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>API 呼び出しのクエリを標準 JSON オブジェクトの形式で追加します。</p> <p>例： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文の内容を追加します。</p> <p>メモ：  <p>JSON で <code>if</code> のような条件文を使用する場合は、条件文を引用符で囲みます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードの更新]

このアクションモジュールは [!DNL Workday] で 1 つのレコードを更新します。

<table style="table-layout:auto"> 
    <col/>
    <col/>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>[!DNL Workday] アカウントを Workfront Fusion に接続する方法について詳しくは、<a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] to Workfront Fusion]</a>を参照してください。</td>
        </tr>
        <tr>
            <td  role="rowheader">レコードタイプ</td>
            <td>更新するレコードのタイプ [!UICONTROL ] を選択します。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td>更新するレコードの ID を入力またはマッピングします。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Subresource ID]</td>
            <td >更新するサブリソースの ID を入力またはマッピングします。</td>
        </tr>
    </tbody>
</table>

### 検索

* [[!UICONTROL レコードの読み取り]](#read-a-record)

* [[!UICONTROL レコードのリスト]](#list-records)


#### [!UICONTROL レコードの読み取り]

このアクションモジュールは 1 つのレコードを読み取ります。

<table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
        <tr>
            <td role="rowheader">[!UICONTROL Connection]</td>
            <td>[!DNL Workday] アカウントを Workfront Fusion に接続する方法について詳しくは、<a href="#Connect" class="MCXref xref" >[!UICONTROL Connect [!DNL Workday] to Workfront Fusion]</a>を参照してください。</td>
        </tr>
        <tr>
            <td  role="rowheader">[!UICONTROL Record type]</td>
            <td>削除するレコードのタイプを選択します。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL Specific record type]</td>
            <td>読み取る特別なタイプのレコードを選択します。これらは、選択したレコードタイプに基づきます。</td>
        </tr>
        <tr>
            <td role="rowheader">[!UICONTROL ID] </td>
            <td >削除するレコードの ID を入力またはマッピングします。</td>
        </tr>
    </tbody>
</table>

#### [!UICONTROL レコードのリスト]

この検索モジュールは、指定されたタイプのレコードのリストを取得します。

<table style="table-layout:auto"> 
      <col/>
      <col/>
      <tbody>
          <tr>
              <td role="rowheader">[!UICONTROL Connection]</td>
              <td>[!DNL Workday] アカウントを [!DNL Workfront Fusion] に接続する方法について詳しくは、<a href="#Connect" class="MCXref xref" >[!DNL Workday] を [!DNL Workfront Fusion]</a> に接続を参照してください。</td>
          </tr>
          <tr>
              <td  role="rowheader">[!UICONTROL Record Type]</td>
              <td>取得するレコードのタイプを選択します。</td>
          </tr>
          <tr>
              <td role="rowheader">[!UICONTROL Limit]</td>
              <td >
                  <p>シナリオの実行サイクルごとにモジュールが取得するレコードの最大数を入力またはマッピングします。</p>
              </td>
          </tr>
      </tbody>
  </table>
