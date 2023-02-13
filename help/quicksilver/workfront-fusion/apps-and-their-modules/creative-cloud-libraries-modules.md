---
filename: creative-cloud-libraries-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Creative Cloud Libraries モジュール
description: を使用 [!DNL Adobe Workfront Fusion Adobe Creative Cloud] ライブラリモジュールを使用すると、要素やライブラリが作成または更新されたときにシナリオを開始できます。 また、要素をアップロード、取得、アーカイブまたはリストすることも、 [!DNL Adobe Creative Cloud Libraries] API
author: Becky
exl-id: 8affa34b-803d-48a5-a986-9fbe0cb8c8f5
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1193'
ht-degree: 0%

---

# Adobe Creative Cloud Libraries Modules

を使用 [!DNL Adobe Workfront Fusion] [!DNL Adobe Creative Cloud Libraries] モジュールを使用すると、要素またはライブラリが作成または更新されたときにシナリオを開始できます。 また、要素をアップロード、取得、アーカイブまたはリストすることも、 [!DNL Adobe Creative Cloud Libraries] API

シナリオの作成手順については、 [シナリオの作成](../../workfront-fusion/scenarios/create-a-scenario.md).

モジュールについて詳しくは、 [のモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] 計画*</td>
      <td>
        <p>[!UICONTROL Pro] 以降</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
      <td>
        <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td>
      <td >
        <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ]</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">製品</td>
      <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td>
    </tr>
  </tbody>
</table>


ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 前提条件

使用する [!DNL Adobe Creative Cloud Libraries] モジュールの場合、 [!UICONTROL Adobe Creative Cloud] アカウント

## [!UICONTROL Adobe Creative Cloud Libraries] モジュールとそのフィールド

設定時に [!UICONTROL Adobe Creative Cloud Libraries] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Adobe Creative Cloud Libraries] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)


* [要素](#elements)

* [ライブラリ](#libraries)

* [その他](#other)


### 要素

* [[!UICONTROL 要素のアーカイブ]](#archive-an-element)

* [[!UICONTROL 要素の取得]](#get-an-element)

* [[!UICONTROL リスト要素]](#list-elements)

* [[!UICONTROL 要素のアップロード]](#upload-an-element)

* [!UICONTROL [ ライブラリの新しい要素を監視する ]](#watch-new-element-in-library)

* [[!UICONTROL 更新された要素を監視する]](#watch-updated-elements)


#### [!UICONTROL 要素のアーカイブ]

このアクションモジュールは、要素をライブラリからアーカイブします。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td>接続方法 [!DNL Adobe Creative Cloud] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ライブラリ ID]</td>
      <td >アーカイブする要素を含むライブラリを選択します。</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL 要素 ID]</td>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyA-Column2-LightGray">アーカイブする要素を選択します。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 要素の取得]

このアクションモジュールは、ライブラリから単一の要素を返します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td>接続方法 [!DNL Adobe Creative Cloud] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ライブラリ ID]</td>
      <td >取得する要素を含むライブラリを選択します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 要素 ID]</td>
      <td>取得する要素の ID を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL セレクター ]</td>
      <td>
        <p>モジュールが返す情報のタイプを選択します。 </p>
        <ul>
          <li>
            <p><b>[!UICONTROL デフォルト ]</b>
            </p>
            <p>ベースデータ</p>
          </li>
          <li>
            <p><b>[!UICONTROL 詳細 ]</b>
            </p>
            <p>すべての使用可能なデータ</p>
          </li>
          <li>
            <p><b>[!UICONTROL 表示域 ]</b>
            </p>
            <p>ライブラリ要素に関連付けられたアセットの統合されたリスト</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL リスト要素]

このアクションモジュールは、ライブラリ内の要素のリストを取得します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td>接続方法 [!DNL Adobe Creative Cloud] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ライブラリ ID]</td>
      <td >要素のリストを表示するライブラリを選択します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Order by]</td>
      <td>名前順に結果を並べ替えるか、要素が最後に変更された日付順に選択します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL の種類 ]</td>
      <td >MIME タイプを入力して、指定した MIME タイプで識別される要素に結果を制限します。 例: <code>string</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL セレクター ]</td>
      <td>
        <p>モジュールが返す情報のタイプを選択します。 </p>
        <ul>
          <li>
            <p><b>[!UICONTROL デフォルト ]</b>
            </p>
            <p>ベースデータ</p>
          </li>
          <li>
            <p><b>[!UICONTROL 詳細 ]</b>
            </p>
            <p>すべての使用可能なデータ</p>
          </li>
          <li>
            <p><b>[!UICONTROL 表示域 ]</b>
            </p>
            <p>ライブラリ要素に関連付けられたアセットの統合されたリスト</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 制限 ]</td>
      <td>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 要素のアップロード]

このアクションモジュールは、小さいファイルアセットを既存のライブラリにアップロードします。 最大ファイルサイズは 1 GB です。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td>接続方法 [!DNL Adobe Creative Cloud] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ライブラリ ID]</td>
      <td >要素のリストを表示するライブラリを選択します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 呼び出しモード ]</td>
      <td>
        <p>このリクエストプロセスを呼び出す処理モードを選択します。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL 同期 ]</b>
            </p>
            <p>API 呼び出しが同期的に処理されます。 処理が完了すると（呼び出しがタイムアウトしない限り）応答が配信されます。</p>
          </li>
          <li>
            <p><b>[!UICONTROL async]</b>
            </p>
            <p>非同期モニタ応答は直ちに返され、リクエスト処理は非同期で実行されます。 呼び出しは、完了するまでエンドポイントをポーリングする役割を持ちます。</p>
          </li>
          <li>
            <p><b>[!UICONTROL sync,async]</b> （デフォルト）</p>
            <p>リクエストの同期処理が試行されます。 処理が 5000 ミリ秒を超えると、非同期モニター応答が返されます。 要求が完了するまで、モニター URL をポーリングする必要があります。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL タイプファイル ]</td>
      <td >アップロードするファイルの MIME タイプを入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ソースファイル ]</td>
      <td>
        <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL ライブラリの新しい要素を監視する]

このトリガーモジュールは、要素がライブラリに追加されると、シナリオを開始します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td>接続方法 [!DNL Adobe Creative Cloud] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ライブラリ ID]</td>
      <td >更新された要素を監視するライブラリを選択します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 制限 ]</td>
      <td>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL 更新された要素を監視する]

このトリガーモジュールは、ライブラリ内の要素が更新されると、シナリオを開始します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td>接続方法 [!DNL Adobe Creative Cloud] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ライブラリ ID]</td>
      <td >新しい要素を監視するライブラリを選択します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 制限 ]</td>
      <td>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</td>
    </tr>
  </tbody>
</table>

### ライブラリ

* [[!UICONTROL 新しいライブラリを見る]](#watch-new-libraries)

* [[!UICONTROL 更新されたライブラリを監視する]](#watch-updated-libraries)


#### [!UICONTROL 新しいライブラリを見る]

このトリガーモジュールは、新しいライブラリが作成される際にシナリオを開始します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td>接続方法 [!DNL Adobe Creative Cloud] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 制限 ]</td>
      <td>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 更新されたライブラリを監視する]

このトリガーモジュールは、既存のライブラリが更新されると、シナリオを開始します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td>接続方法 [!DNL Adobe Creative Cloud] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 制限 ]</td>
      <td>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</td>
    </tr>
  </tbody>
</table>

### その他

#### [!UICONTROL API 呼び出しを実行する]

このモジュールは、 [!DNL Adobe Creative Cloud Libraries] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td> <p>Adobe Creative CloudアカウントをWorkfront Fusion に接続する手順については、 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe Workfront Fusion — 基本手順への接続を作成します。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>相対パスを入力 <code>https://cc-libraries.adobe.io/api</code>.</p>
    <p>例： <code>/v1/libraries</code>.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL API バージョン ]</td>
      <td>
        <p>のバージョンを選択 [!DNL Adobe Analytics] 接続先の API。</p>
      </td>
    </tr>    <tr>
      <td role="rowheader">[!UICONTROL メソッド ]</td>
      <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p>
        <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion は、認証ヘッダーを追加します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL クエリ文字列 ]</td>
      <td>
        <p>標準の JSON オブジェクトの形式で、API 呼び出しのクエリを追加します。</p>
        <p>例： <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 本文 ]</td>
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文のコンテンツを追加します。</p> <p>メモ:  <p>条件文 ( <code>if</code> JSON で、条件文の外側に引用符を置きます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
       <tr>
      <td role="rowheader">[!UICONTROL 一時的なドキュメントのアップロード ]</td>
      <td>
      <p>一時的なドキュメントをアップロードする場合は、アップロードするドキュメントのソースファイルを入力します。</p>
      <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p>
    </td>
    </tr>

</tbody>
</table>
