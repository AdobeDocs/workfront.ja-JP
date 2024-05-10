---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Adobe Fireflyモジュール
description: ' [!DNL Adobe Workfront Fusion]  のシナリオでは、 [!DNL Adobe Firefly] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。'
author: Becky
feature: Workfront Fusion, Digital Content and Documents
source-git-commit: c932f869de9ff842a7bbb809bc60ec1d53350b51
workflow-type: tm+mt
source-wordcount: '1215'
ht-degree: 37%

---

# [!DNL Adobe Firefly] モジュール

[!DNL Adobe Workfront Fusion] のシナリオでは、[!DNL Adobe Firefly] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。

シナリオの作成手順が必要な場合は、[](../../workfront-fusion/scenarios/create-a-scenario.md) でのシナリオの作成を参照してください。

モジュールについては、[モジュール： [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)を参照してください。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> <p>新規：[!UICONTROL Standard]</p><p>または</p><p>現在：[!UICONTROL 作業 ] 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在：いいえ [!DNL Workfront Fusion] ライセンス要件</p>
   <p>または</p>
   <p>レガシー：任意 </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>新規：</p> <ul><li>[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Workfront] プラン：組織による購入が必要です [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] プラン： [!DNL Workfront Fusion] が含まれます。</li></ul>
   <p>または</p>
   <p>現在：組織による購入が必要です。 [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

[!DNL Adobe Firefly] コネクタを使用する前に、次の前提条件が満たされていることを確認する必要があります。

* アクティブな [!DNL Adobe Firefly] アカウントが必要です。

## [!DNL Adobe Firefly] への接続の作成

[!DNL Adobe Firefly] モジュールの接続を作成するには、次の手順に従います。

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
        <td role="rowheader">[!UICONTROL Environment]</td>
        <td>実稼動環境と非実稼動環境のどちらに接続するかを選択します。</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Type]</td>
        <td>サービスアカウントと個人アカウントのどちらに接続するかを選択します。</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client ID]</td>
        <td>[!UICONTROL Adobe] [!UICONTROL クライアント ID] を入力します。 これは、の [!UICONTROL 資格情報 ] の詳細セクションにあります [!DNL Adobe Developer Console]</td>
        </tr>
        <tr>
        <td role="rowheader">[!UICONTROL Client Secret]</td>
        <td>[!DNL Adobe] [!UICONTROL Client Secret] を入力します。これは、の [!UICONTROL 資格情報 ] の詳細セクションにあります [!DNL Adobe Developer Console]</td>
        </tr>
      </tbody>
    </table>

1. 「**[!UICONTROL 続行]**」をクリックして接続を保存し、モジュールに戻ります。

## [!DNL Adobe Firefly] モジュールとそのフィールド

[!DNL Adobe Firefly] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL Adobe Firefly] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でモジュールから別のモジュールに情報をマッピングを参照してください。

![](assets/map-toggle-350x74.png)

### カスタム API 呼び出しを実行

このアクションモジュールは、FireflyAPI へのカスタム呼び出しを行います。

使用可能な特定の API については、を参照してください。 [ADOBE FIREFLYAPI](https://developer.adobe.com/firefly-services/docs/firefly-api/) Adobe Developerのドキュメントで説明しています。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Firefly] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >[!DNL Adobe Firefly]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p><code>https://firefly-api-enterprise-stage.adobe.io/</code> への相対パスを入力します。</p>
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
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文の内容を追加します。</p> <p>メモ：  <p><code>if</code> などの条件文を JSON で使用する場合は、条件文を引用符で囲みます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

### 画像を展開

このアクションモジュールは、画像を展開します（オプションで、指定したプロンプトのコンテンツも展開します）。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>[!DNL Adobe Campaign] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >[!DNL Adobe Firefly]</a> への接続を作成を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL プロンプト ]</td> 
   <td>画像を展開するコンテンツのプロンプトを入力またはマップします。 プロンプトが指定されない場合、画像は元の画像に一致するコンテンツで展開されます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 拡張画像形式 ]</td> 
   <td>展開したイメージの保存先となるファイル形式を選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>  <p>前のモジュールからソースファイルを選択するか、ソースファイルの画像ファイル名と画像ファイル（データ）をマッピングします。</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL サイズ ]</td> 
   <td>展開する画像のサイズを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL シード ]</td> 
   <td>整数を入力またはマッピングします。 この同じシードを別の画像を展開モジュールで使用して、異なるスタイルの類似した画像を生成することができます。 </td> 
  </tr> 
 </tbody> 
</table>

## 画像を埋める

このアクションモジュールは、画像のマスクされた領域を、必要に応じて、指定したプロンプトのコンテンツで埋めます。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>[!DNL Adobe Campaign] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >[!DNL Adobe Firefly]</a> への接続を作成を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL プロンプト ]</td> 
   <td>イメージを埋めるコンテンツの入力を求めるプロンプトを入力またはマップします。 プロンプトが指定されない場合、画像には元の画像と一致するコンテンツが入力されます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 塗り潰し画像形式 ]</td> 
   <td>塗りつぶし画像を保存するファイル形式を選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Image]</td> 
   <td>  <p> クリック <b>画像を追加</b>. 前のモジュールからソースファイルを選択するか、ソースファイルの画像ファイル名と画像データをマッピングします。</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL マスク ]</td> 
   <td>  <p> クリック <b>マスクを追加</b>. 前のモジュールからソースファイルを選択するか、ソースファイルのマスクファイル名とマスクデータをマッピングします。 マスクファイルは、生成されたコンテンツで入力されるカスタムマスクを表します。</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL サイズ ]</td> 
   <td>塗りつぶし画像のサイズを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL シード ]</td> 
   <td>整数を入力またはマッピングします。 この同じシードを別の画像を展開モジュールで使用して、異なるスタイルの類似した画像を生成することができます。 </td> 
  </tr> 
 </tbody> 
</table>

## 画像を生成

このアクションモジュールは、指定されたプロンプトに基づいてと画像を生成します。 オプションで参照画像を指定することもできます。この場合、生成された画像は参照画像のスタイルと一致します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>[!DNL Adobe Campaign] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-firefly" class="MCXref xref" >[!DNL Adobe Firefly]</a> への接続を作成を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL プロンプト ]</td> 
   <td>作成するイメージのプロンプトを入力またはマップします。 プロンプトの詳細を使用すると、画像に表示されるものを詳細に制御できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL で生成されたイメージ形式 ]</td> 
   <td>展開したイメージの保存先となるファイル形式を選択します。 デフォルトを選択した場合、参照画像が指定されていないと、ファイル形式はJPEGになります。 参照画像を指定した場合、生成される画像のファイル形式は参照画像と同じになります。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>  <p>前のモジュールからソースファイルを選択するか、ソースファイルの参照画像ファイル名と参照画像ファイル（データ）をマッピングします。 参照画像のスタイルに一致する画像が生成されます。</p> </td> 
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL プリセット ]</td> 
   <td>プリセットスタイルを使用する場合は、「項目を追加」をクリックし、使用するスタイルを入力またはマップします。<p>プリセットスタイルのリストについては、を参照してください。 <a href="https://developer.adobe.com/firefly-services/docs/firefly-api/guides/concepts/styles/" >画像モデルスタイル</a> （Adobe開発者向けドキュメント）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 負のプロンプト ]</td> 
   <td>生成されたコンテンツで避ける単語を入力またはマッピングします。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL コンテンツ クラス ]</td> 
   <td>生成された画像を写真に近づけるのか、それとも作成されたアートに近づけるのかを選択します。 <ul><li><b>写真</b><p>「絞り」、「シャッタースピード」（秒単位）、「視野」（ミリメートル単位）の値を入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL シード ]</td> 
   <td>整数を入力またはマッピングします。 この同じシードを別の画像を展開モジュールで使用して、異なるスタイルの類似した画像を生成することができます。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL サイズ ]</td> 
   <td>生成される画像のサイズを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL の強さ ]</td> 
   <td>生成される画像がプリセットのスタイルまたは参照画像と一致する強度を表す整数を入力またはマッピングします。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 視覚強度 ]</td> 
   <td>写真の既存の視覚特性の全体的な強度を表す整数を入力またはマッピングします。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Locale]</td> 
   <td>ロケールが指定された場合、モジュールは指定されたロケールにより関連性の高いコンテンツを生成します。 <p>ロケールは、ISO 639-1 言語コードおよび ISO 3166-1 地域で提供する必要があります。</p><p> 例： <code>en-US</code></p></td> 
  </tr> 
 </tbody> 
</table>


