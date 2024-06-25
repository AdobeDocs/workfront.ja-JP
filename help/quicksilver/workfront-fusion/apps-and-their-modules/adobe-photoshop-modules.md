---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Adobe Photoshop モジュール
description: Adobe Photoshop モジュールを使用すると、Adobe Photoshop アカウント内のイベントに基づくAdobe Workfront Fusion シナリオの開始、契約書やその他のレコードの作成、読み取りまたは更新、設定した条件を使用したレコードの検索、ドキュメントのアップロードを行うことができます。
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: f20192ea-e363-4fba-8bd2-b1d50443918d
source-git-commit: 6bcf404432129a812b5e4d840b59e72f036ec723
workflow-type: tm+mt
source-wordcount: '1547'
ht-degree: 36%

---

# [!DNL Adobe Photoshop] モジュール

[!DNL Adobe Workfront Fusion] のシナリオでは、[!DNL Adobe Photoshop] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。


シナリオの作成手順が必要な場合は、[](../../workfront-fusion/scenarios/create-a-scenario.md) でのシナリオの作成を参照してください。

モジュールについては、[モジュール： [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)を参照してください。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] プラン*</td>
      <td>
        <p>[!UICONTROL Pro] 以降</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
      <td>
        <p>[!UICONTROL Plan]、[!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td>
      <td >
        <p>[!UICONTROL Workfront Fusion for Work Automation and Integration]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">製品</td>
      <td>この記事で説明されている機能を使用するには、組織で [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。</td>
    </tr>
    </tr>
  </tbody>
</table>


&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

&#42;&#42;について [!DNL Adobe Workfront Fusion] ライセンス，「参照」 [!DNL [Adobe Workfront Fusion] licenses](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 前提条件

[!DNL Adobe Photoshop] コネクタを使用する前に、次の前提条件が満たされていることを確認する必要があります。

* アクティブな [!DNL Adobe Photoshop] アカウントが必要です。

## [!DNL Adobe Photoshop] への接続の作成

[!DNL Adobe Photoshop] モジュールの接続を作成するには、次の手順に従います。

1. 「接続」ボックスの横に表示される「**[!UICONTROL 追加]**」をクリックします。

1. 次のフィールドに入力します。

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
        <td role="rowheader">[!UICONTROL Connection name]</td>
        <td>
          <p>この接続の名前を入力します。</p>
        </td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>[!UICONTROL Adobe] [!UICONTROL クライアント ID] を入力します。 これは、の [!UICONTROL 資格情報 ] の詳細セクションにあります [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>[!DNL Adobe] [!UICONTROL Client Secret] を入力します。これは、の [!UICONTROL 資格情報 ] の詳細セクションにあります [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Technical account ID]</td>
        <td>[!DNL Adobe] [!UICONTROL Technical account ID] を入力します。これは、の [!UICONTROL 資格情報 ] の詳細セクションにあります [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Organization ID]</td>
        <td>[!DNL Adobe] [!UICONTROL Organization ID] を入力します。これは、の [!UICONTROL 資格情報 ] の詳細セクションにあります [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Private key]</td>
        <td>
          <p>[!DNL Adobe Developer Console] で資格情報が作成された際に生成された秘密鍵を入力します。 </p>
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
              <p>クリック <b>保存</b> ファイルを抽出して [!UICONTROL ]e 接続設定に戻ります。</p>
            </li>
          </ol>
        </td>
        </tr>
      </tbody>
    </table>

1. 「**[!UICONTROL 続行]**」をクリックして接続を保存し、モジュールに戻ります。

## [!DNL Adobe Photoshop] モジュールとそのフィールド

[!DNL Adobe Photoshop] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL Adobe Photoshop] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でモジュールから別のモジュールに情報をマッピングを参照してください。

![](assets/map-toggle-350x74.png)


### アクション

* [新しいPSDの作成](#create-a-new-psd)
* [テキストレイヤーを編集](#edit-text-layers)
* [深度ブラーを実行](#execute-depth-blur)
* [Photoshop アクションの実行](#execute-photoshop-actions)
* [製品の切り抜きを実行](#execute-product-crop)
* [レイヤー情報を取得](#get-layer-info)
* [カスタム API 呼び出しの実行](#make-a-custom-api-call)

#### 新しいPSDの作成

このアクションモジュールは、オプションのレイヤーを持つ新しいPSDを作成し、レンディションを生成したり、PSDとして保存したりします。

このモジュールに関連するフィールドについては、を参照してください。 [新しいPSDの作成](https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/documentCreate) Adobe Photoshopのドキュメントで説明しています。

#### テキストレイヤーを編集

Photoshop ファイルのテキストレイヤーを編集します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Photoshop] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >[!DNL Adobe Photoshop]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 入力ファイルの保存場所 ]</td>
      <td>
        <p>編集するファイルが格納されているファイルサービスを選択します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 入力ファイル URL]</p>
      </td>
   <td> 編集するファイルの URL またはパスを入力またはマップします。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 不足フォントの管理 ]</td>
      <td>
        <p>ドキュメントに 1 つ以上の不足しているフォントがある場合に実行するアクションを選択します。 フォントが指定されていない場合、モジュールはデフォルトのフォントを使用します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 既定のフォント ]  </td>
      <td>
        <p>ドキュメントのグローバルデフォルトとして使用するフォントの完全な Postscript 名を入力します。 このフォントは、フォントが見つからないテキストレイヤーに使用され、そのレイヤーに特別に提供された他のフォントはありません。 このフォントが見つからない場合は、見つからないフォントの管理で指定したオプションが有効になります。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL レイヤー ]</td>
   <td> <p>レイヤ オプションの詳細については、を参照してください。 <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/text">テキストレイヤーを編集</a> Adobe Photoshopのドキュメントで説明しています。</p>  </td>     </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 出力ファイルの保存場所 ]</td>
      <td>
        <p>編集したファイルを保存するファイルサービスを選択します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 出力ファイル URL]</p>
      </td>
   <td> 編集したファイルを保存する場所の URL またはパスを入力またはマップします。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 出力ファイルの種類 ]</p>
      </td>
   <td> 編集するファイルのファイル タイプを選択します。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>既に存在する出力ファイルを新しく編集したファイルで上書きするかどうかを選択します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 圧縮 ]</p>
      </td>
   <td> 出力ファイルの圧縮レベルを選択します。 </td> 
    </tr>
  </tbody>
</table>

#### 深度ブラーを実行

このアクション モジュールは、選択したファイルに対して深度ブラーを実行します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Photoshop] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >[!DNL Adobe Photoshop]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 入力ファイルの保存場所 ]</td>
      <td>
        <p>編集するファイルが格納されているファイルサービスを選択します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 入力ファイル URL]</p>
      </td>
   <td> 編集するファイルの URL またはパスを入力またはマップします。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 出力ファイルの保存場所 ]</td>
      <td>
        <p>編集したファイルを保存するファイルサービスを選択します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 出力ファイル URL]</p>
      </td>
   <td> 編集したファイルを保存する場所の URL またはパスを入力またはマップします。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 出力ファイルの種類 ]</p>
      </td>
   <td> 編集するファイルのファイル タイプを選択します。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Other fields]</td>
      <td>
        <p>その他のデプス ブラーオプションについては、を参照してください。 <a href="https://developer.adobe.com/photoshop/photoshop-api-docs/api/#tag/Photoshop/operation/depthBlur">深度ブラーを実行 </a>（Adobe Photoshop API ドキュメント）。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>既に存在する出力ファイルを新しく編集したファイルで上書きするかどうかを選択します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 圧縮 ]</p>
      </td>
   <td> 出力ファイルの圧縮レベルを選択します。 </td> 
    </tr>
  </tbody>
</table>

#### Photoshop アクションの実行

このアクションモジュールは、選択された画像に対してPhotoshopアクションを実行します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Photoshop] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >[!DNL Adobe Photoshop]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 入力ファイルの保存場所 ]</td>
      <td>
        <p>編集するファイルが格納されているファイルサービスを選択します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 入力ファイル URL]</p>
      </td>
   <td> 編集するファイルの URL またはパスを入力またはマップします。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL アクション ファイルの保存場所 ]</td>
      <td>
        <p>アクションファイルが格納されるファイルサービスを選択します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL アクション ファイルの URL]</p>
      </td>
   <td> アクションファイルの URL またはパスを入力またはマッピングします。 </td> 
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL アクション名 ]</p>
      </td>
   <td> 特定のアクションのみを実行する場合は、ActionSet から再生するアクションを指定できます。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL フォント/パターン/ブラシストレージ ]</td>
      <td>
        <p>使用するファイルが格納されているファイルサービスを選択します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL フォント / パターン / ブラシ ファイルの URL]</p>
      </td>
   <td> 使用するファイルの URL またはパスを入力またはマップします。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 出力ファイルの保存場所 ]</td>
      <td>
        <p>編集したファイルを保存するファイルサービスを選択します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 出力ファイル URL]</p>
      </td>
   <td> 編集したファイルを保存する場所の URL またはパスを入力またはマップします。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 出力ファイルの種類 ]</p>
      </td>
   <td> 編集するファイルのファイル タイプを選択します。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>既に存在する出力ファイルを新しく編集したファイルで上書きするかどうかを選択します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 圧縮 ]</p>
      </td>
   <td> 出力ファイルの圧縮レベルを選択します。 </td> 
    </tr>
  </tbody>
</table>

#### 製品の切り抜きを実行

このアクションモジュールは、選択した画像に対して製品の切り抜きを実行します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Photoshop] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >[!DNL Adobe Photoshop]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 入力ファイルの保存場所 ]</td>
      <td>
        <p>切り抜くファイルを格納するファイルサービスを選択します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 入力ファイル URL]</p>
      </td>
   <td> 切り抜くファイルの URL またはパスを入力またはマッピングします。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL ユニット ]</p>
      </td>
   <td> 高さと幅の調整をピクセル単位またはパーセント単位のどちらで記述するかを選択します。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Width]</p>
      </td>
   <td> 追加する幅のパディングの量を入力またはマッピングします。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Height]</p>
      </td>
   <td> 追加する高さのパディングの量を入力またはマッピングします。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 出力ファイルの保存場所 ]</td>
      <td>
        <p>編集したファイルを保存するファイルサービスを選択します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 出力ファイル URL]</p>
      </td>
   <td> 編集したファイルを保存する場所の URL またはパスを入力またはマップします。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 出力ファイルの種類 ]</p>
      </td>
   <td> 編集するファイルのファイル タイプを選択します。 </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Overwrite]</td>
      <td>
        <p>既に存在する出力ファイルを新しく編集したファイルで上書きするかどうかを選択します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 圧縮 ]</p>
      </td>
   <td> 出力ファイルの圧縮レベルを選択します。 </td> 
    </tr>
  </tbody>
</table>

#### レイヤー情報を取得

指定したPSDファイルから画層の情報を取得します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Photoshop] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >[!DNL Adobe Photoshop]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 入力ファイルの保存場所 ]</td>
      <td>
        <p>画層情報を取得するファイルが格納されているファイル サービスを選択します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL 入力ファイル URL]</p>
      </td>
   <td> 画層情報を取得するファイルの URL またはパスを入力またはマップします。 </td> 
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL サムネール ]</p>
      </td>
   <td> </td> 
    </tr>
  </tbody>
</table>

#### カスタム API 呼び出しの実行

このアクションモジュールは、Photoshop API へのカスタム呼び出しを行います。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Photoshop] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-photoshop" class="MCXref xref" >[!DNL Adobe Photoshop]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p><code>https://image.adobe.io/pie/psdService</code> からの相対パスを入力します。例： <code>/photoshopActions</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
   <td> <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]</a>での HTTP リクエストメソッドを参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>リクエストのヘッダーを標準 JSON オブジェクトの形式で追加します。</p>
        <p>例： <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] 認証ヘッダーを自動的に追加します。</p>
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
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文の内容を追加します。</p> <p>メモ：  <p><code>if</code> などの条件文を JSON で使用する場合は、条件文を引用符で囲みます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>
