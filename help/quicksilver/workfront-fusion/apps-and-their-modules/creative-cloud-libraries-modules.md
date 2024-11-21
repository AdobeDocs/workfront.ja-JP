---
filename: creative-cloud-libraries-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Adobe Creative Cloud ライブラリモジュール
description: ' [!DNL Adobe Workfront Fusion Adobe Creative Cloud]  ライブラリモジュールを使用すると、要素やライブラリが作成または更新されたときにシナリオを開始できます。また、要素をアップロード、取得、アーカイブまたはリストすることも、 [!DNL Adobe Creative Cloud Libraries]  API を呼び出すこともできます。'
author: Becky
feature: Workfront Fusion
exl-id: 8affa34b-803d-48a5-a986-9fbe0cb8c8f5
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '1359'
ht-degree: 81%

---

# Adobe Creative Cloud ライブラリモジュール

[!DNL Adobe Workfront Fusion] [!DNL Adobe Creative Cloud Libraries] モジュールを使用すると、要素やライブラリが作成または更新されたときにシナリオを開始できます。また、要素をアップロード、取得、アーカイブまたはリストすることも、[!DNL Adobe Creative Cloud Libraries] API を呼び出すこともできます。

シナリオの作成手順が必要な場合は、[](../../workfront-fusion/scenarios/create-a-scenario.md) でのシナリオの作成を参照してください。

モジュールについては、[モジュール： [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md)を参照してください。

>[!IMPORTANT]
>
>現在、Creative Cloud Libraries コネクタでは接続を作成できません。 既存の接続は期待どおりに動作します。

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
      <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td>
    </tr>
    <tr>
      <td role="rowheader">製品</td>
      <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランがある場合、この記事で説明する機能を使用するには、組織で [!DNL Adobe Workfront Fusion] の購入 [!DNL Adobe Workfront] 必要です。 [!DNL Workfront Fusion] は、[!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront]を組織で購入する必要があります。</p>
   </td>
    </tr>
  </tbody>
</table>


ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

[!DNL Adobe Creative Cloud Libraries] モジュールを使用するには、[!UICONTROL Adobe Creative Cloud] アカウントが必要です。

## Adobe Creative Cloud ライブラリ API の情報

Adobe Creative Cloud ライブラリコネクタでは、以下を使用します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">ベース URL</td> 
   <td>https://cc-libraries.adobe.io/api/v1</td> 
  </tr>
  <tr> 
   <td role="rowheader">API タグ</td> 
   <td>v1.1.7</td> 
  </tr>
 </tbody> 
 </table>

## [!UICONTROL Adobe Creative Cloud ライブラリ]モジュールおよびそのフィールド

[!UICONTROL Adobe Creative Cloud ライブラリ]モジュール設定時に、[!DNL Workfront Fusion] には以下のフィールドが表示されます。これらと共に、アプリやサービスのアクセスレベルなどの要因に応じて、追加の [!DNL Adobe Creative Cloud Libraries] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) で 1 つのモジュールから別のモジュールに情報をマッピングを参照してください。

![](assets/map-toggle-350x74.png)


* [要素](#elements)

* [ライブラリ](#libraries)

* [その他](#other)


### 要素

* [[!UICONTROL 要素のアーカイブ]](#archive-an-element)

* [[!UICONTROL 要素の取得]](#get-an-element)

* [[!UICONTROL 要素のリスト]](#list-elements)

* [[!UICONTROL 要素のアップロード]](#upload-an-element)

* [!UICONTROL [Watch New Element in Library]](#watch-new-element-in-library)

* [[!UICONTROL 更新された要素の監視]](#watch-updated-elements)


#### [!UICONTROL 要素のアーカイブ]

このアクションモジュールは、要素をライブラリからアーカイブします。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>既存のCreative Cloud Libraries接続を選択します。 現在、Creative Cloud Libraries コネクタでは接続を作成できません。 既存の接続は期待どおりに動作します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >アーカイブする要素を含むライブラリを選択します。</td>
    </tr>
    <tr>
      <td class="TableStyle-TableStyle-List-options-in-steps-BodyB-Column1-LightGray" role="rowheader">[!UICONTROL Element ID]</td>
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
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>既存のCreative Cloud Libraries接続を選択します。 現在、Creative Cloud Libraries コネクタでは接続を作成できません。 既存の接続は期待どおりに動作します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >取得する要素を含むライブラリを選択します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Element ID]</td>
      <td>取得する要素の ID を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Selector]</td>
      <td>
        <p>モジュールが返す情報のタイプを選択します。 </p>
        <ul>
          <li>
            <p><b>[!UICONTROL Default]</b>
            </p>
            <p>ベースデータ</p>
          </li>
          <li>
            <p><b>[!UICONTROL Details]</b>
            </p>
            <p>すべての使用可能なデータ</p>
          </li>
          <li>
            <p><b>[!UICONTROL Representations]</b>
            </p>
            <p>ライブラリ要素に関連付けられたアセットのフラット化されたリスト</p>
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
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>既存のCreative Cloud Libraries接続を選択します。 現在、Creative Cloud Libraries コネクタでは接続を作成できません。 既存の接続は期待どおりに動作します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >要素をリストするライブラリを選択します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Order by]</td>
      <td>結果を名前順に並べ替えるか、要素が最後に変更された日付順に並べ替えるかを選択します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type]</td>
      <td >MIME タイプを入力して、指定した MIME タイプで識別される要素に結果を制限します。例：<code>string</code>。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Selector]</td>
      <td>
        <p>モジュールが返す情報のタイプを選択します。 </p>
        <ul>
          <li>
            <p><b>[!UICONTROL Default]</b>
            </p>
            <p>ベースデータ</p>
          </li>
          <li>
            <p><b>[!UICONTROL Details]</b>
            </p>
            <p>すべての使用可能なデータ</p>
          </li>
          <li>
            <p><b>[!UICONTROL Representations]</b>
            </p>
            <p>ライブラリ要素に関連付けられたアセットのフラット化されたリスト</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL 要素のアップロード]

このアクションモジュールは、小さなファイルアセットを既存のライブラリにアップロードします。最大ファイルサイズは 1 GB です。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>既存のCreative Cloud Libraries接続を選択します。 現在、Creative Cloud Libraries コネクタでは接続を作成できません。 既存の接続は期待どおりに動作します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >要素をリストするライブラリを選択します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Invocation Mode]</td>
      <td>
        <p>このリクエストプロセスを呼び出す処理モードを選択します。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL sync]</b>
            </p>
            <p>API 呼び出しが同期処理されます。処理が完了すると（呼び出しがタイムアウトしない限り）応答が配信されます。</p>
          </li>
          <li>
            <p><b>[!UICONTROL async]</b>
            </p>
            <p>非同期モニター応答は直ちに返され、リクエスト処理は非同期で実行されます。呼び出しは、完了するまでエンドポイントをポーリングする役割を持ちます。</p>
          </li>
          <li>
            <p><b>[!UICONTROL sync,async]</b>（デフォルト）</p>
            <p>リクエストの同期処理が試行されます。処理時間が 5000 ミリ秒を超えると、非同期モニター応答が返されます。リクエストが完了するまで、モニター URL をポーリングする必要があります。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Type File]</td>
      <td >アップロードしたファイルの MIME タイプを入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Source File]</td>
      <td>
        <p>以前のモジュールで使用したソースファイルを選択するか、ソースファイルの名前とデータをマッピングします。</p>
      </td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL ライブラリの新しい要素を監視]

このトリガーモジュールは、要素がライブラリに追加されると、シナリオを開始します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>既存のCreative Cloud Libraries接続を選択します。 現在、Creative Cloud Libraries コネクタでは接続を作成できません。 既存の接続は期待どおりに動作します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >アップデートされた要素を監視するライブラリを選択します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL アップデートされた要素を監視]

このトリガーモジュールは、ライブラリ内の要素がアップデートされると、シナリオを開始します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>既存のCreative Cloud Libraries接続を選択します。 現在、Creative Cloud Libraries コネクタでは接続を作成できません。 既存の接続は期待どおりに動作します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Library ID]</td>
      <td >新しい要素を監視するライブラリを選択します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</td>
    </tr>
  </tbody>
</table>

### ライブラリ

* [[!UICONTROL 新しいライブラリを監視]](#watch-new-libraries)

* [[!UICONTROL アップデートされたライブラリを監視]](#watch-updated-libraries)


#### [!UICONTROL 新しいライブラリを監視]

このトリガーモジュールは、新しいライブラリの作成時にシナリオを開始します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>既存のCreative Cloud Libraries接続を選択します。 現在、Creative Cloud Libraries コネクタでは接続を作成できません。 既存の接続は期待どおりに動作します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL アップデートされたライブラリを監視]

このトリガーモジュールは、既存のライブラリの更新時にシナリオを開始します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>既存のCreative Cloud Libraries接続を選択します。 現在、Creative Cloud Libraries コネクタでは接続を作成できません。 既存の接続は期待どおりに動作します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Limit]</td>
      <td>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</td>
    </tr>
  </tbody>
</table>

### その他

#### [!UICONTROL API 呼び出しを実行]

このモジュールは、[!DNL Adobe Creative Cloud Libraries] API に対してカスタム API 呼び出しを実行します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td> <p>Adobe Creative Cloud アカウントを Workfront Fusion に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe Workfront Fusion への接続を作成 - 基本手順を参照してください。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p><code>https://cc-libraries.adobe.io/api</code> への相対パスを入力します。</p>
    <p>例：<code>/v1/libraries</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL API version]</td>
      <td>
        <p>接続する [!DNL Adobe Analytics] APIのバージョンを選択します。</p>
      </td>
    </tr>    <tr>
      <td role="rowheader">[!UICONTROL Method]</td>
      <td> <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a>での HTTP リクエストメソッドを参照してください。</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>リクエストのヘッダーを標準 JSON オブジェクトの形式で追加します。</p>
        <p>例： <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion は認証ヘッダーを追加します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]</td>
      <td>
        <p>API 呼び出しのクエリを標準 JSON オブジェクトの形式で追加します。</p>
        <p>例： <code>{"name":"something-urgent"}</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文の内容を追加します。</p> <p>メモ：  <p><code>if</code> などの条件ステートメントを JSON で使用する場合は、条件ステートメントの外側に引用符を挿入します。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
       <tr>
      <td role="rowheader">[!UICONTROL Upload a transient document]</td>
      <td>
      <p>一時的なドキュメントをアップロードする場合は、アップロードするドキュメントのソースファイルを入力します。</p>
      <p>以前のモジュールで使用したソースファイルを選択するか、ソースファイルの名前とデータをマッピングします。</p>
    </td>
    </tr>

</tbody>
</table>
