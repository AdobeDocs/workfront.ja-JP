---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Split.io モジュール
description: ' [!DNL Adobe Workfront Fusion]  のシナリオでは、 [!DNL Split.io] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。'
author: Becky
feature: Workfront Fusion
exl-id: 4576a2e4-b495-430e-a9de-4e1ec7379ab8
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '1821'
ht-degree: 100%

---

# [!DNL Split.io] モジュール

[!DNL Adobe Workfront Fusion] のシナリオでは、[!DNL Split.io] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。

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

[!DNL Split.io] モジュールを使用するには、[!DNL Split.io] アカウントが必要です。

## [!DNL Split.io] を [!DNL Workfront Fusion] に接続 {#connect-split-io-to-workfront-fusion}

[!DNL Split.io] アカウントへの接続を、[!DNL Split.io] モジュール内から直接作成できます。

1. 任意の [!DNL Split.io] モジュールで、「[!UICONTROL 接続]」フィールドの横にある「**[!UICONTROL 追加]**」をクリックします。
1. 接続に名前を入力します。
1. [!DNL Split.io] API キーを入力します。

   [!DNL Split.io] API キーについて詳しくは、[!DNL Split.io] ドキュメントの[API キー](https://help.split.io/hc/en-us/articles/360019916211-API-keys)を参照してください。

1. 「**[!UICONTROL 続行]**」をクリックして接続を作成し、モジュールに戻ります。

## [!DNL Split.io] モジュールとそのフィールド

[!DNL split.io] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL split.io] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[モジュール間の情報のマッピング： [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)を参照してください。

![](assets/map-toggle-350x74.png)

* [アクション](#actions)
* [検索](#searches)

### アクション

* [[!UICONTROL カスタム API 呼び出し]](#custom-api-call)
* [[!UICONTROL 分割を取得]](#get-split)
* [[!UICONTROL 環境で分割定義を取得]](#get-split-definition-in-environment)
* [[!UICONTROL 分割を作成]](#create-split)
* [[!UICONTROL 分割を削除]](#delete-split)
* [[!UICONTROL 環境で分割定義を作成]](#create-split-definition-in-environment)
* [[!UICONTROL 環境から分割定義を削除]](#remove-split-definition-from-environment)
* [[!UICONTROL 環境でスプリット定義を部分更新]](#partial-update-split-definition-in-environment)
* [[!UICONTROL タグを関連付け]](#associate-tags)

#### [!UICONTROL カスタム API 呼び出し]

このアクションモジュールでは、[!DNL split.io] API への認証済みのカスタム呼び出しを行うことができます。これにより、他の [!DNL split.io] モジュールでは不可能なデータフローの自動化を作成できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Split.io] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事内の <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">[!DNL Split.io] を [!UICONTROL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td><code>https://api.split.io/internal/api/v2/</code> への相対パスを入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> での HTTP リクエストメソッドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>リクエストのヘッダーを標準 JSON オブジェクトの形式で追加します。</p> <p>例： <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion は認証ヘッダーを追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>API 呼び出しのクエリを標準 JSON オブジェクトの形式で追加します。</p> <p>例： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文の内容を追加します。</p> <p>メモ：  <p>JSON で <code>if</code> のような条件ステートメントを使用する場合は、条件ステートメントの外側に引用符を付けます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>各シナリオの実行サイクル中に、モジュールが操作するレコードの最大数を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL スプリットを取得]

このアクションモジュールがスプリットを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Split.io] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事内の <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">[!DNL Split.io] を [!UICONTROL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>取得するスプリットを含むワークスペースを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>取得するスプリットの名前を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 環境でスプリット定義を取得]

このアクションモジュールは、指定された環境から特定のスプリット定義を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Split.io] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事内の <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">[!DNL Split.io] を [!UICONTROL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>取得するスプリット定義を含むワークスペースを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Environment Name or ID]</td> 
   <td>取得するスプリット定義を含む環境を選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>スプリット定義を取得するスプリットの名前を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL スプリットを作成]

このアクションモジュールは、トラフィックタイプを指定して、組織内に新しいスプリットを作成します。

>[!NOTE]
>
>API はどの環境でもスプリットを設定しません。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Split.io] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事内の <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">[!DNL Split.io] を [!UICONTROL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>スプリットを作成するワークスペースを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Traffic Type ID or Name]</td> 
   <td>分割の作成に使用するトラフィックタイプを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>作成する分割の名前を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Description]</td> 
   <td>作成する分割の [!UICONTROL split] の説明を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 分割を削除]

このアクションモジュールは、組織から分割を削除します。これにより、すべての環境から分割定義の設定が自動的に解除されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Split.io] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">[!UICONTROL Workfront Fusion] への [!DNL Split.io] の接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>分割を削除するワークスペースを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>削除する分割の名前を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 環境で分割定義を作成]

このアクションモジュールは、特定の環境の分割定義を設定します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Split.io] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">[!UICONTROL Workfront Fusion] への [!DNL Split.io] の接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>分割定義を作成するワークスペースを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Environment Name or ID]</td> 
   <td>分割定義を作成する環境を選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>定義を作成する分割の名前を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comments]</td> 
   <td>分割定義に追加するコメントを入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rules]</td> 
   <td> <p>定義に追加するターゲティングルールごとに、「<b>[!UICONTROL Add item]</b>」をクリックし、ルールを入力またはマッピングします。</p> <p>ターゲットルールについて詳しくは、[!DNL Split.io] ドキュメントの<a href="https://docs.split.io/reference#create-split-definition-in-environment">環境で分割定義を作成</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Default rule]</td> 
   <td> <p>他のルールの仕様を満たさないトラフィックに対して分割で使用するルールを入力またはマッピングします。</p> <p>ターゲットルールについて詳しくは、[!DNL Split.io] ドキュメントの<a href="https://docs.split.io/reference#create-split-definition-in-environment">環境で分割定義を作成</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Default treatment]</td> 
   <td> <p>分割が強制終了した場合、または顧客がトラフィック配分に含まれていない場合に分割で使用する処理を入力またはマッピングします。</p> <p>処理について詳しくは、[!DNL Split.io] ドキュメントの<a href="https://docs.split.io/reference#create-split-definition-in-environment">環境で分割定義を作成</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Treatments]</td> 
   <td> <p>定義に追加する処理ごとに、「<b>[!UICONTROL Add item]</b>」をクリックし、処理を入力またはマッピングします。</p> <p>処理について詳しくは、[!DNL Split.io] ドキュメントの<a href="https://docs.split.io/reference#create-split-definition-in-environment">環境で分割定義を作成</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 環境から分割定義を削除]

このアクションモジュールは、特定の環境の分割定義の設定を解除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Split.io] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">[!UICONTROL Workfront Fusion] への [!DNL Split.io] の接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>分割定義を削除するワークスペースを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Environment Name or ID]</td> 
   <td>スプリット定義を削除する環境を選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>定義を削除するスプリットの名前を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comments]</td> 
   <td>分割定義に追加するコメントを入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 環境でスプリット定義を部分更新]

このアクションモジュールは、特定の環境のスプリット定義を更新します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Split.io] アカウントの [!DNL Workfront Fusion] への接続方法については、この記事内の<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">[!DNL Split.io] の [!UICONTROL Workfront Fusion] への接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>スプリット定義を更新するワークスペースを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Environment Name or ID]</td> 
   <td>スプリット定義を更新する環境を選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>定義を更新するスプリットの名前を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Update content]</td> 
   <td> <p>更新するスプリットの各属性に関して、「<b>[!UICONTROL Add item]</b>」をクリックし、必要な変更を入力またはマッピングします。</p> <p>詳しくは、[!DNL Split.io] ドキュメント内の<a href="https://docs.split.io/reference#partial-update-split-definition-in-environment">環境でスプリット定義を部分更新</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comments]</td> 
   <td>分割定義に追加するコメントを入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL タグを関連付け]

このアクションモジュールは、指定したオブジェクトにタグを追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Split.io] アカウントの [!DNL Workfront Fusion] への接続方法については、この記事内の<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">[!DNL Split.io] の [!UICONTROL Workfront Fusion] への接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>タグを追加するワークスペースを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Name]</td> 
   <td>タグを追加するオブジェクト名を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Type]</td> 
   <td> <p>タグを追加するオブジェクトのタイプを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td> <p>追加するタグごとに、「<b>[!UICONTROL Add item]</b>」をクリックし、タグを入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 検索

* [[!UICONTROL ワークスペースを取得]](#get-workspaces)
* [[!UICONTROL 環境を取得]](#get-environments)
* [[!UICONTROL スプリットを取得]](#get-splits)
* [[!UICONTROL 環境でスプリット定義をリスト]](#list-split-definitions-in-an-environment)
* [[!UICONTROL トラフィックタイプを取得]](#get-traffic-types)

#### [!UICONTROL ワークスペースを取得]

この検索モジュールは、組織のワークスペースを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Split.io] アカウントの [!DNL Workfront Fusion] への接続方法については、この記事内の<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">[!DNL Split.io] の [!UICONTROL Workfront Fusion] への接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>各シナリオの実行サイクル中に、モジュールで取得するワークスペースの最大数を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 環境を取得]

この検索モジュールは、環境のリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Split.io] アカウントの [!DNL Workfront Fusion] への接続方法については、この記事内の<a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">[!DNL Split.io] の [!UICONTROL Workfront Fusion] への接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>リストに表示する環境を含むワークスペースを選択またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 分割を取得]

この検索モジュールは、分割のリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Split.io] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">[!DNL Split.io] を [!UICONTROL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>リストに表示するスプリットを含むワークスペースを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>それぞれのシナリオ実行サイクル中にモジュールが取得するスプリットの最大数を、入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 環境内でスプリット定義をリスト]

この検索モジュールは、特定の環境のスプリット定義のリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Split.io] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">[!DNL Split.io] を [!UICONTROL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>リストに表示するスプリット定義を含むワークスペースを選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Environment Name or ID]</td> 
   <td>リストに表示するスプリット定義を含む環境を選択またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>それぞれのシナリオ実行サイクル中にモジュールが取得するスプリット定義の最大数を、入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL トラフィックタイプを取得]

この検索モジュールは、トラフィックタイプのリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>[!DNL Split.io] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">[!DNL Split.io] を [!UICONTROL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>リストに表示するトラフィックタイプを含むワークスペースを選択またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>
