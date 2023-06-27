---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Anaplan モジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオの場合、Anaplan を使用するワークフローを自動化でき、複数のサードパーティのアプリケーションやサービスに接続できます。
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
exl-id: 03bcd0a4-c8ec-4f44-b1e1-b57e79595309
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1844'
ht-degree: 1%

---

# [!DNL Anaplan] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Anaplan]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

シナリオの作成手順については、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

モジュールについて詳しくは、 [のモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 前提条件

使用する前に [!DNL Anaplan] コネクタを使用する場合は、次の前提条件が満たされていることを確認する必要があります。

* アクティブな [!UICONTROL アナプラン] アカウント
* ワークスペース、モデル、およびその他を設定する必要があります [!DNL Anaplan] オブジェクト [!UICONTROL アナプラン] 次よりも前にアカウント [!DNL Workfront Fusion] 操作できます。

## 接続 [!DNL Anaplan] から [!DNL Workfront Fusion] {#connect-anaplan-to-workfront-fusion}

の接続を作成するには、以下を実行します。 [!DNL Anaplan] モジュール：

1. クリック **[!UICONTROL 追加]** の横 [!UICONTROL 接続] ボックス
1. 接続タイプを選択します。

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan] [!UICONTROL 基本 ]</td> 
      <td> <p>An [!DNL Anaplan] [!UICONTROL Basic] 接続で接続を作成するには、電子メールアドレスとパスワードのみが必要です。 </p> <p>接続の名前を入力し、メールアドレスと、 [!DNL Anaplan] アカウント</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Anaplan] [!UICONTROL CA 証明書 ]</td> 
      <td> <p>An [!DNL Anaplan] [!UICONTROL CA 証明書 ] 接続には、[!UICONTROL 証明書キー ]、[!UICONTROL エンコードされたデータ ] および [!UICONTROL エンコードされた署名済みデータ ] が必要です。 これらは、 [!DNL Anaplan] アカウント 手順については、 [!DNL Anaplan] ドキュメント。</p> <p>接続の名前を入力し、 [!DNL Anaplan] アカウント</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **[!UICONTROL 続行]** 接続を保存し、モジュールに戻ります。

## [!DNL Anaplan] モジュールとそのフィールド

設定時に [!DNL Anaplan] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Anaplan] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [トリガー](#triggers)
* [アクション](#actions)
* [検索](#searches)

### トリガー

#### [!DNL Watch records]

このトリガーモジュールは、選択されたタイプのレコードが作成または更新されると、シナリオを開始します。

>[!NOTE]
>
>このモジュールは、新しいレコードのデータを返します。 変更された既存のレコードのデータは返されません。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>への接続を作成する手順 [!DNL Anaplan]を参照してください。 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">接続 [!DNL Anaplan] から [!DNL Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">監視するオブジェクトのタイプ</td> 
   <td>監視する項目のタイプを選択します。 シナリオは、このタイプのレコードが作成または更新された時点で開始されます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">&lt;object&gt; ID</td> 
   <td>監視対象のオブジェクトに関連付けられているモデルやモジュールなど、Anaplan にオブジェクトの ID を入力します</td> 
  </tr> 
  <tr> 
   <td role="rowheader">制限</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが [action] に設定するレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL リスト項目の作成]](#create-a-list-item)
* [[!UICONTROL カスタム API 呼び出しを実行する]](#make-a-custom-api-call)
* [[!UICONTROL レコードを読み取る]](#read-a-record)
* [[!UICONTROL アクションの実行]](#run-an-action)
* [[!UICONTROL レコードの更新]](#update-a-record)
* [[!UICONTROL ファイルのアップロード]](#upload-a-file)

#### [!UICONTROL リスト項目の作成]

このアクションモジュールは、Anaplan 内のリストに新しい項目を追加します。

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL 接続 ]</td>
        <td>への接続を作成する手順 [!DNL Anaplan]を参照してください。 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">接続 [!DNL Anaplan] から [!DNL Workfront Fusion]</a> 」を参照してください。</td>
    </tr>
    <tr>
        <td>[!UICONTROL Workspace ID]</td>
        <td>項目を追加するリストが含まれる Analyplan Workspace の ID を選択またはマッピングします。</td>
    </tr>
    <tr>
        <td>[!UICONTROL モデル ID]</td>
        <td>項目を追加するリストが含まれるモデルの ID を選択またはマッピングします。</td>
    </tr>
    <tr>
        <td>[!UICONTROL リスト ID]</td>
        <td>項目を作成するリストの ID を選択またはマップします。</td>
    </tr>
    <tr>
        <td>[!UICONTROL 名前 ]</td>
        <td>新しい項目の名前を入力します。</td>
    </tr>
    <tr>
        <td>[!UICONTROL コード ]</td>
        <td>新しい項目のコードを入力します。 コードは、同じ名前の行項目を区別できるユーザー生成コードです。</td>
    </tr>
    <tr>
        <td>[!UICONTROL 親 ]</td>
        <td>新しいアイテムを作成する親アイテムの名前を入力します。</td>
    </tr>
    <tr>
        <td>[!UICONTROL プロパティ ]</td>
        <td>項目を追加するリストにカスタムプロパティがある場合は、値を追加するプロパティを選択し、値を追加します。</td>
    </tr>
    <tr>
        <td>[!UICONTROL サブセット ]</td>
        <td>項目を追加するリストにカスタムサブセットがある場合、項目を追加するサブセットを選択してから、「 」を選択します <b>[!UICONTROL はい ]</b> をクリックして、新しい項目をそのサブセットに追加します。</td>
    </tr>
</table>

#### [!UICONTROL カスタム API 呼び出しを実行する]

このモジュールを使用すると、 [!DNL Anaplan] API

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>への接続を作成する手順 [!DNL Anaplan]を参照してください。 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">接続 [!DNL Anaplan] から [!DNL Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>相対パスを入力 <code>https://api.anaplan.com/2/0/</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL メソッド ]</p> </td> 
   <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] は、認証ヘッダーを自動的に追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ] </td> 
   <td> <p>リクエストクエリ文字列を入力します。</p> </td> 
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

このアクションモジュールは、既存のレコードを削除します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>への接続を作成する手順 [!DNL Anaplan]を参照してください。 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">接続 [!DNL Anaplan] から [!DNL Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>削除するオブジェクトを含む Anaplan Workspace の ID を選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL モデル ID]</td> 
   <td>削除するオブジェクトを含むモデルの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">削除</td> 
   <td> <p>削除するオブジェクトのタイプを選択します。</p> 
    <ul> 
     <li> <p><b>アクション</b> </p> <p>削除するアクションを選択またはマッピングします。</p> </li> 
     <li> <p><b>リスト項目</b> </p> <p>項目を削除するリストを選択し、削除する項目の ID またはコードを入力またはマッピングします</p>  </li> 
     <li> <p><b>[!UICONTROL ファイル ]</b> </p> <p>削除するファイルを選択またはマッピングします。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを読み取る]

このアクションモジュールは、単一のレコードを読み取ります。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>への接続を作成する手順 [!DNL Anaplan]を参照してください。 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">接続 [!DNL Anaplan] から [!DNL Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>読み取るレコードのタイプを選択します。</p> 
    <ul> 
     <li> <p><b>モデル</b> </p> <p>読み取るモデルの ID を選択またはマッピングします</p> </li> 
     <li> <p><b>モデルリスト</b> </p> <p>読み取るリストを含むワークスペースおよびモデルの ID を選択またはマッピングして、リストを選択します。 「 [!UICONTROL データタイプ ] 」フィールドで、データとメタデータのどちらを読み取るかを選択します。</p> </li> 
     <li> <p><b>モデルのバージョン</b> </p> <p>読み取るモデルの ID を選択またはマッピングします。</p> </li> 
     <li> <p><b>ユーザー</b> </p> <p>使用中のアカウントの所有者に関するデータを返すか、別のユーザーに関するデータを返すかを選択します。 別のユーザーを選択する場合は、ユーザーの名前を選択します。</p> </li> 
     <li> <p><b>ワークスペース</b> </p> <p>読み取るワークスペースの ID を選択またはマッピングします。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アクションの実行]

このアクションモジュールは、アクションのインポート、エクスポート、削除、または処理を行います。

<table style="table-layout:auto"> 
     <col/>
     <col/>
     <tbody>
      <tr>
        <td role="rowheader">[!UICONTROL 接続 ]</td>
        <td>への接続を作成する手順 [!DNL Anaplan]を参照してください。 <a href="#Connect" class="MCXref xref" >[!UICONTROL Analytics Fusion をWorkfront Fusion に接続 ]</a> 」を参照してください。</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL Workspace ID]</td>
        <td>の ID を選択またはマッピング [!DNL Anaplan] アクションを実行するワークスペース</td>
      </tr>
      <tr >
        <td role="rowheader">[!UICONTROL モデル ID]</td>
        <td>アクションを実行するモデルの ID を選択またはマッピングします。</td>
      </tr>
      <tr>
        <td role="rowheader">[!UICONTROL アクションタイプ ]</td>
        <td>
          <p>実行するアクションを選択します</p>
            <ul>
              <li>
                <p><b>[!UICONTROL 削除 ]</b>
                </p>
                <p>削除するアクションの ID を入力またはマッピングします。</p>
              </li>
              <li>
                <p><b>[!UICONTROL 書き出し ]</b>
                </p>
                <p>使用するエクスポート定義の ID を入力またはマッピングします。 次のファイル形式に書き出すことができます。</p>
                  <ul>
                    <li>
                      <p>XLS</p>
                    </li>
                    <li>
                      <p>XLSX</p>
                    </li>
                    <li>
                      <p>CSV</p>
                    </li>
                  </ul>
                </li>
                <li>
                  <p><b>[!UICONTROL 読み込み ] </b>
                  </p>
                  <p style="font-weight: normal;">使用するインポート定義の ID を入力またはマッピングします。</p>
                </li>
                <li>
                 <p><b>[!UICONTROL Process]</b>
                 </p>
                  <p>使用するプロセスの ID を入力またはマッピングします。 </p>
                </li>
              </ul>
            </td>
          </tr>
        </tbody>
      </table>


#### [!UICONTROL レコードの更新]

このアクションモジュールは、 [!UICONTROL アナプラン].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>への接続を作成する手順 [!DNL Anaplan]を参照してください。 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">接続 [!DNL Anaplan] から [!DNL Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>更新するレコードのタイプを選択します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL リスト項目 ]</b> </p> <p>フィールドについては、 <a href="#create-a-list-item" class="MCXref xref">リスト項目の作成</a> 」を参照してください。</p> </li> 
     <li> <p><b>[!UICONTROL モジュールのセルデータ ]</b> </p> <p>セルのデータを更新すると、そのデータを使用するすべてのダウンストリーム計算も更新されます。</p> <p>次のフィールドに入力します。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL モデル ID]</b> </p> <p>更新するセルを含むモデルを選択またはマッピングします。</p> </li> 
       <li> <p><b>[!UICONTROL モジュール ID]</b> </p> <p>更新するセルを含むモジュールを選択またはマッピングします</p> </li> 
       <li> <p><b>[!UICONTROL 行項目名 ]</b> </p> <p>更新するセルの行項目を選択またはマッピングします</p> </li> 
       <li> <p style="font-weight: bold;">[!UICONTROLDimensionID]</p> <p>行項目上のディメンションを選択またはマッピングします。</p> 
       <p><b>メモ: </b> 
       <ul>
       <li> Dimensionキー（値）は、次のいずれかである必要があります <code>dimensionName</code> （次へ）または <code>dimensionId</code> (ID)。</li>
       <li>項目キー（値）は <code>itemName</code> （テキスト）、 <code>itemCode</code> （テキスト）または <code>itemId</code> (ID)。</li>
       <li>Dimensionと項目キーは、同じタイプ（テキストまたは ID）である必要があります。
       </ul>
        </p> 
        <p>ディメンションについて詳しくは、 [!DNL Anaplan Anapedia].</p> </li> 
       <li> <p><b>[!UICONTROL 値 ]</b> </p> <p>セルの新しい値を入力またはマッピングします。</p> </li> 
      </ul> </li> 
     <li> <p><b>[!UICONTROL モデルの現在の会計年度 ]</b> </p> <p>会計年度を更新するモデルのワークスペース ID とモデル ID を入力し、モデルの新年を入力またはマッピングします。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルのアップロード]

このアクションモジュールは、Anaplan にファイルをアップロードします。 ファイルは、既に Anaplan にアップロードされている必要があります。 このモジュールを使用して、Analyplan 内の追加の場所にアップロードできます。
<table style="table-layout:auto">
<col>
<col>
<tbody>
<tr>
<td role="rowheader">[!UICONTROL 接続 ]</td>
<td>への接続を作成する手順 [!DNL Anaplan]を参照してください。 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">接続 [!DNL Anaplan] から [!DNL Workfront Fusion]</a> 」を参照してください。</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL Workspace ID]</td>
<td>の ID を選択またはマッピング [!DNL Anaplan] ファイルをアップロードするワークスペース。</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL モデル ID]</td>
<td>ファイルをアップロードするモデルの ID を選択またはマッピングします。</td>
</tr>
<tr>
<td role="rowheader">[!UICONTROL ファイル ID]</td>
<td>アップロードするファイルの ID を選択またはマッピングします。</td>
</tr>
</tbody>
</table>
</div>

### 検索

#### [!UICONTROL レコードを取得]

この検索モジュールは、選択したタイプのアクセス可能なすべてのレコードを返します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td>への接続を作成する手順 [!DNL Anaplan]を参照してください。 <a href="#connect-anaplan-to-workfront-fusion" class="MCXref xref">接続 [!DNL Anaplan] から [!DNL Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>取得するレコードのタイプを選択します。</p> 
      <ul> 
       <li> <p><b>[!UICONTROL Workspaces]</b> </p> </li> 
       <li> <p><b>[!UICONTROL モデル ]</b> </p> </li> 
       <li> <p><b>[!UICONTROL 行項目 ]</b> </p> <p>を含むモデルの ID を選択またはマッピングします。 [!DNL line] 取得する項目。</p> </li> 
       <li> <p><b>[!UICONTROL モデルリスト ]</b> </p> <p>取得するモデルリストを含むワークスペース ID とモデル ID を選択またはマッピングします。</p> </li> 
       <li> <p><b>[!UICONTROL モデルカレンダー ]</b> </p> <p>取得するモデルカレンダーが含まれるワークスペースの ID を選択またはマッピングします。</p> </li> 
       <li> <p><b>モデルのバージョン</b> </p> </li> 
       <li> <p>取得するモデルバージョンが含まれるモデルの ID を [!UICONTROL ] 選択またはマッピングします。</p> </li> 
       <li> <p><b>[!UICONTROL ユーザー ]</b> </p> </li> 
       <li> <p><b>[!UICONTROL 表示 ]</b> </p> <p>「モジュール」(Module) または「モデル」(Model) のどちらでビューを選択するかを選択し、取得するビューを含むモジュールまたはモデルの ID を選択またはマッピングします。</p> </li> 
      </ul> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ワークスペースサイズを返す</td> 
   <td>ワークスペースの現在のサイズの見積もりを返すには、このオプションを有効にします。 この予測は、ワークスペースに含まれるすべてのモジュールのサイズに基づいて行われます。</td> 
  </tr> 
 </tbody> 
</table>
