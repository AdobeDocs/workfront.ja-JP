---
filename: figma-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: 図モジュール
description: を使用 [!DNL Adobe Workfront Fusion] 図モジュールでは、コメント、ファイル、ファイルバージョン、またはプロジェクトの一覧を取得できます。 また、コメントを投稿したり、Figma API を呼び出したりすることもできます。
author: Becky
exl-id: d88db592-32d4-4765-952f-9ffb58cf1720
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '2309'
ht-degree: 1%

---

# [!DNL Figma] モジュール

を使用 [!DNL Adobe Workfront Fusion] [!DNL Figma] モジュールを使用して、コメント、ファイル、ファイルバージョン、またはプロジェクトのリストを取得できます。 また、コメントを投稿したり、 [!DNL Figma] API

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

使用する [!DNL Figma] モジュールの場合、 [!DNL Figma] アカウント

## [!DNL Figma] モジュールとそのフィールド

設定時に [!DNL Figma] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Figma] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [コメント](#comments)

* [プロジェクトとファイル](#projects-and-files)

* [コンポーネントとスタイル](#components-and-styles)

* [その他](#other)


### コメント

* [コメントの削除](#delete-a-comment)

* [コメントをリスト](#list-comments)

* [コメントを投稿](#post-a-comment)


#### [!UICONTROL コメントの削除]

このアクションモジュールは、ファイルから 1 つのコメントを削除します。

<table style="table-layout:auto"> 
  <col/>
  <col />
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td> <p>接続方法 [!DNL Figma] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順。</a></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ファイル ID]</td>
      <td>コメントを追加するファイルのファイル ID を入力またはマッピングします。 </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL コメント ]</td>
      <td>削除するコメントのテキストを入力します。</td>
    </tr>
  </tbody>
</table>

#### [!UICONTROL コメントをリスト]

この検索モジュールは、 [!DNL Figma].

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td> <p>接続方法 [!DNL Figma] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ファイル ID]</td>
      <td>
        <p>コメントを取得するファイルのファイル ID を入力またはマッピングします。 </p>
        <ul>
          <li>
            <p>ID が不明な場合は、 <b>[!UICONTROL ファイルを検索 ]</b> ファイルが関連付けられているプロジェクトの ID を入力またはマッピングし、ファイルを選択します。</p>
          </li>
          <li>
            <p>プロジェクトの ID が不明な場合は、 <b>[!UICONTROL プロジェクトを検索 ]</b> ファイルが関連付けられているプロジェクトを所有するチームの ID を入力またはマップし、プロジェクトを選択してから、ファイルを選択します。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 制限 ]</td>
      <td>各シナリオの実行サイクル中にモジュールが返すコメントの最大数を入力またはマッピングします。</td>
    </tr>
  </tbody>
</table>


#### [!UICONTROL コメントを投稿]

このアクションモジュールは、Figma ファイルにコメントを投稿します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td> <p>接続方法 [!DNL Figma] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順。</a></p>
    </tr>
    <tr>
      <td  role="rowheader">[!UICONTROL ファイル ID]</td>
      <td>
        <p>コメントを投稿するファイルのファイル ID を入力またはマッピングします。 </p>
        <ul>
          <li>
            <p>ファイルの ID が不明な場合は、 <b>[!UICONTROL ファイルを検索 ]</b> ファイルが関連付けられているプロジェクトの ID を入力またはマッピングし、ファイルを選択します。</p>
          </li>
          <li>
            <p>ファイルの ID を探していて、プロジェクトの ID が不明な場合は、 <b>[!UICONTROL プロジェクトを検索 ]</b> ファイルが関連付けられているプロジェクトを所有するチームの ID を入力またはマッピングします。 プロジェクトを選択し、ファイルを選択します。</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL コメント ]</td>
      <td>コメントのテキストを入力します。</td>
    </tr>
  </tbody>
</table>


### プロジェクトとファイル

* [ファイルまたは画像の取得](#get-a-file-or-image)

* [ファイルのバージョン履歴のリスト](#list-file-version-history)

* [プロジェクトファイルのリスト](#list-project-files)

* [プロジェクトのリスト](#list-projects)


#### [!UICONTROL ファイルまたは画像の取得]

このアクションモジュールは、Figma ライブラリから 1 つのファイルまたは画像を取得します

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td> <p>接続方法 [!DNL Figma] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL オブジェクトタイプ ]</td>
      <td>
        <p>取得するオブジェクトのタイプを選択します。</p>
        <ul>
          <li>
            <p><b>[!UICONTROL ファイル ]</b>
            </p>
            <p>このモジュールは、[!UICONTROL キー ] によって参照されるドキュメントを JSON オブジェクトとして返します。 ファイルキーは、任意の Figma ファイル URL から解析できます。</p>
            <p>フィールドについては、 <a href="#Get2" class="MCXref xref" >[!UICONTROL ファイルまたは画像を取得します。ファイル ]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL ファイルノード ]</b>
            </p>
            <p>ID によって参照されるノードを JSON オブジェクトとして返します。 ノードは [!DNL Figma] [!UICONTROL キー ] によって参照されたファイル。</p>
            <p>フィールドについては、 <a href="#Get3" class="MCXref xref" >[!UICONTROL ファイルまたは画像を取得します。ファイルノード ]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL 画像 ]</b>
            </p>
            <p>このモジュールは、ファイルから画像をレンダリングします。</p>
            <p>フィールドについては、 <a href="#Get4" class="MCXref xref" >[!UICONTROL ファイルまたは画像を取得します。画像 ]</a>.</p>
          </li>
          <li>
            <p><b>[!UICONTROL 画像の塗り ]</b>
            </p>
            <p>このモジュールは、ドキュメント内の画像の塗りに存在するすべての画像のダウンロードリンクを返します。 画像の塗りは次のようになります。 [!DNL Figma] は、ユーザが指定したすべてのイメージを表します。 画像を [!DNL Figma], [!DNL Figma] は、画像を表す単一の塗りつぶしを持つ長方形を作成します。ユーザは、長方形（および塗りつぶしのプロパティ）を変換できます。</p>
            <p>フィールドについては、 <a href="#Get5" class="MCXref xref" >[!UICONTROL ファイルまたは画像を取得します。画像の塗り ]</a>.</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


##### [!UICONTROL ファイルまたは画像を取得します。ファイル]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL ファイルキー ]</td>
      <td>JSON を返すファイルを選択します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL バージョン ID]</td>
      <td>モジュールが返すファイルのバージョンを入力またはマッピングします。 現在のモジュールでは、このフィールドを空白のままにします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ノード ID]</td>
      <td>
        <p>ドキュメントのサブセットのみを返すには、モジュールが返すノードを入力します。 このモジュールは、リストに表示されたノード、その子、およびルートノードとリストされたノードの間のすべてのノードを返します。</p>
        <p>返すノードごとに、 <b>[!UICONTROL 追加 ]</b> ノードのテキストを入力します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL の深さ ]</td>
      <td>
        <p>結果を返すドキュメントツリー内の深さを表す整数を入力またはマップします。 </p>
        <div class="example"><span class="autonumber"><span><b>例: </b></span></span>
          <ul>
            <li>
              <p>ページのみを返すには、 <code>1</code>.</p>
            </li>
            <li>
              <p>ページとトップレベルオブジェクトを返すには、 <code>2</code>.</p>
            </li>
          </ul>
        </div>
        <p>すべてのノードを返す場合は、このフィールドを空白のままにします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ジオメトリ ]</td>
      <td>ベクトルデータを返すには、 <code>paths</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL プラグインデータ ]</td>
      <td>プラグイン ID のコンマ区切りリストおよび文字列「[!UICONTROL shared]」。 これらのプラグインによって書き込まれたドキュメント内に存在するすべてのデータは、 <code>pluginData</code> および <code>sharedPluginData</code> プロパティ。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ブランチデータ ]</td>
      <td>要求されたファイルのブランチメタデータを返すには、このオプションを有効にします。 ファイルがブランチの場合、返される応答にメインファイルのキーが含まれます。 ファイルにブランチがある場合、そのメタデータが返される応答に含まれます。 デフォルト: <code>false</code>.</td>
    </tr>
  </tbody>
</table>

##### [!UICONTROL ファイルまたは画像を取得します。ファイルノード]

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL ファイルキー ]</td>
      <td>JSON を返すファイルを選択します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ノード ID]</td>
      <td>
        <p>モジュールが返し、変換するノードを入力します</p>
        <p>返すノードごとに、 <b>[!UICONTROL 追加 ]</b> ノードのテキストを入力します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL バージョン ID]</td>
      <td>モジュールが返すファイルのバージョンを入力またはマッピングします。 現在のモジュールでは、このフィールドを空白のままにします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL の深さ ]</td>
      <td>
        <p>結果を返すドキュメントツリー内の深さを表す整数を入力またはマップします。 </p>
        <div class="example"><span class="autonumber"><span><b>例: </b></span></span>
          <ul>
            <li>
              <p>ページのみを返すには、 <code>1</code>.</p>
            </li>
            <li>
              <p>ページとトップレベルオブジェクトを返すには、 <code>2</code>.</p>
            </li>
          </ul>
        </div>
        <p>すべてのノードを返す場合は、このフィールドを空白のままにします。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ジオメトリ ]</td>
      <td>ベクトルデータを返すには、 <code>paths</code>.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL プラグインデータ ]</td>
      <td>プラグイン ID のコンマ区切りリストおよび文字列「shared」。 これらのプラグインによって書き込まれたドキュメント内に存在するすべてのデータは、 pluginData プロパティと sharedPluginData プロパティの結果に含まれます。</td>
    </tr>
  </tbody>
</table>


##### ファイルまたは画像を取得します。画像

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL ファイルキー ]</td>
      <td>JSON を返すファイルを選択します。</td>
    </tr>
    <tr>
      <td role="rowheader" [!UICONTROL>ノード ID]</td>
      <td>
        <p>モジュールをレンダリングするノードを入力します。</p>
        <p>レンダリングするノードごとに、 <b>[!UICONTROL 追加 ]</b> ノードのテキストを入力します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL スケール ]</td>
      <td>画像を拡大・縮小するには、拡大・縮小率を入力またはマッピングします。 この数は 0.01 ～ 4 の範囲で指定する必要があります。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 形式 ]</td>
      <td>
        <p>画像出力の形式を選択します。</p>
        <ul>
          <li>
            <p>JPG</p>
          </li>
          <li>
            <p>PNG</p>
          </li>
          <li>
            <p>SVG</p>
          </li>
          <li>
            <p>PDF</p>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROLSVG- Include ID]</td>
      <td>すべてのオプション要素の ID 属性を含めるには、このSVGを有効にします。 デフォルト：[!UICONTROL false]。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROLSVG — 線を簡素化 ]</td>
      <td>このオプションを有効にすると、内側/外側のストロークがシンプルになり、可能な場合は、代わりにストローク属性が使用されます。 &lt;mask&gt;. デフォルト：[!UICONTROL true]</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 絶対範囲を使用 ]</td>
      <td>切り抜くか、ノードの周囲のスペースが空であるかに関係なく、ノードの全寸法を使用するには、このオプションを有効にします。 切り抜かずにテキストノードを書き出すには、このオプションを使用します。 デフォルト：[!UICONTROL false]。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL バージョン ID]</td>
      <td>モジュールが返すファイルのバージョンを入力またはマッピングします。 現在のモジュールでは、このフィールドを空白のままにします。</td>
    </tr>
  </tbody>
</table>

##### ファイルまたは画像を取得します。画像の塗り

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL ファイルキー ]</td>
      <td>JSON を返すファイルを選択します。</td>
    </tr>
  </tbody>
</table>

### [!UICONTROL ファイルのバージョン履歴のリスト]

この検索モジュールは、 [!UICONTROL フィグマ].
<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td> <p>接続方法 [!DNL Figma] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順。</a></p>
    <tr>
      <td role="rowheader">[!UICONTROL ファイル ID]</td>
      <td>
        <p>バージョン履歴を取得するファイルのファイル ID を入力またはマッピングします。 </p>
        <ul>
          <li>
            <p>ファイルの ID が不明な場合は、 <b>[!UICONTROL ファイルを検索 ]</b> ファイルが関連付けられているプロジェクトの ID を入力またはマッピングし、ファイルを選択します。</p>
          </li>
          <li>
            <p>ファイルの ID を探していて、プロジェクトの ID が不明な場合は、 <b>[!UICONTROL プロジェクトを検索 ]</b> ファイルが関連付けられているプロジェクトを所有するチームの ID を入力またはマッピングします。 プロジェクトを選択し、ファイルを選択します。</p>
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

#### [!UICONTROL プロジェクトファイルのリスト]

この検索モジュールは、指定されたプロジェクト内のすべてのファイルの一覧を返します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td> <p>接続方法 [!DNL Figma] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ファイル ID]</td>
      <td>
        <p>ファイルを取得するプロジェクトのプロジェクト ID を入力またはマッピングします。 </p>
        <ul>
          <li>
            <p>プロジェクトの ID が不明な場合は、 <b>[!UICONTROL プロジェクトを検索 ]</b> プロジェクトが関連付けられているチームの ID を入力またはマッピングし、プロジェクトを選択します。</p>
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

#### [!UICONTROL プロジェクトのリスト]

この検索モジュールは、指定したチーム内のすべてのプロジェクトのリストを返します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td> <p>接続方法 [!DNL Figma] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL チーム ID]</td>
      <td>ファイルを取得するプロジェクトのプロジェクト ID を入力またはマッピングします。 チーム ID は、Figma のチームのページの URL にあります</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 制限 ]</td>
      <td>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</td>
    </tr>
  </tbody>
</table>


### コンポーネントとスタイル

#### [!UICONTROL スタイルまたはコンポーネントの取得]

このアクションモジュールは、1 つのスタイルまたはコンポーネント、またはスタイルまたはコンポーネントのセットを取得します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td> <p>接続方法 [!DNL Figma] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順。</a></p>
    </tr>
    <tr>
      <td role="rowheader">&lt;[!UICONTROL Object&gt; キー ]</td>
      <td>取得するオブジェクトのキー（一意の識別子）を入力します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL チーム ID]</td>
      <td>レコードまたはレコードが関連付けられているチームの ID を入力またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL ページサイズ ]</td>
      <td>1 ページにつき返す数または結果を入力またはマッピングします。 デフォルト：30.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL After]</td>
      <td>
        <p>結果の取得を開始する前の結果の数を入力またはマッピングします。 これを [!UICONTROL ページサイズ ] フィールドと組み合わせて、結果をページ番号付けできます。</p>
        <p>この値はオブジェクト ID に対応していません。</p>
        <p>このフィールドは、[!UICONTROL Before] フィールドと組み合わせて使用することはできません。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Before]</td>
      <td>
        <p>結果の取得を開始する前の結果の数を入力またはマッピングします。 これを [!UICONTROL ページサイズ ] フィールドと組み合わせて、結果をページ番号付けできます。</p>
        <p>この値はオブジェクト ID に対応していません。</p>
        <p>このフィールドは、[!UICONTROL After] フィールドと組み合わせて使用することはできません。</p>
      </td>
    </tr>
  </tbody>
</table>


### その他

* [API 呼び出しを実行する](#make-an-api-call)

* [イベントを見る](#watch-events)


#### [!UICONTROL API 呼び出しを実行する]

このアクションモジュールを使用すると、認証を通じて考慮する必要なく、Figma API に対してカスタム認証呼び出しをおこなうことができます。 これにより、他の Figma モジュールでは実現できないデータフローの自動化を作成できます。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td> <p>接続方法 [!DNL Figma] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順。</a></p>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL URL]</td>
      <td>
        <p>相対パスを入力 <code>https://api.figma.com/v1/</code>.</p>
        <p>例： <code>[!DNL files/7179110/comments]</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL メソッド ]</td>
      <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p>
        <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] によって、認証ヘッダーが追加されます。</p>
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
  </tbody>
</table>

#### [!UICONTROL イベントを見る]

このトリガーモジュールは、次のイベントの 1 つが、 [!DNL Figma] チームスペース

* ファイルの更新

* ファイルのバージョンの更新

* ファイルの削除

* ライブラリ公開

* ファイルコメント

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>
        <p>モジュールが監視する Webhook を選択します。</p>
        <p>新しい Webhook を追加するには：</p>
        <ol>
          <li value="1">
            <p>クリック <b>[!UICONTROL 追加 ]</b> [!UICONTROL Webhook] フィールドの横にある</p>
          </li>
          <li value="2">
            <p>この Webhook に使用する接続を選択します。 接続方法 [!DNL Figma] [!UICONTROL Workfront Fusion] アカウントについては、 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!UICONTROL Adobe Workfront Fusion] への接続を作成する — 基本手順。</a></p>
          </li>
          <li value="3">
            <p>モジュールで監視するイベントタイプを選択します。</p>
          </li>
          <li value="4">
            <p>Webhook でイベントを監視するチームの ID を入力します。</p>
          </li>
          <li value="5">
            <p>Webhook で監視するイベントの「[!UICONTROL Status]」または「[!UICONTROL Description]」を入力します。</p>
          </li>
          <li value="6">
            <p>クリック <b>[!UICONTROL 保存 ]</b> をクリックして Webhook を保存し、モジュールに戻ります。</p>
          </li>
        </ol>
      </td>
    </tr>
  </tbody>
</table>
