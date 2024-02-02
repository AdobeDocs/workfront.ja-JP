---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Allocadia モジュール
description: ' [!DNL Adobe Workfront Fusion]  シナリオでは、Allocadia を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりすることができます。'
author: Becky
feature: Workfront Fusion
exl-id: f1edefd1-9fe0-48fc-bea2-c3f9facf7363
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: ht
source-wordcount: '1401'
ht-degree: 100%

---

# [!DNL Allocadia] モジュール

[!DNL Adobe Workfront Fusion] のシナリオでは、[!DNL Allocadia] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion]ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

[!DNL Allocadia] モジュールを使用するには、[!DNL Allocadia] アカウントが必要です。

## [!DNL Allocadia] を [!DNL Workfront Fusion] に接続

[!DNL Allocadia] アカウントへの接続を、[!DNL Allocadia] モジュール内から直接作成できます。

1. 任意の [!DNL Allocadia] モジュールで、「[!UICONTROL 接続]」フィールドの横にある「**[!UICONTROL 追加]**」をクリックします。
1. 北米のサーバーを使用するか、ヨーロッパのサーバーを使用するかを選択します。
1. ユーザー名とパスワードを入力します。
1. 「**[!UICONTROL 続行]**」をクリックし、接続を作成して、モジュールに戻ります。

## [!DNL Allocadia] モジュールとそのフィールド

[!DNL Allocadia] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL Allocadia] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でモジュールから別のモジュールに情報をマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [トリガー](#triggers)
* [アクション](#actions)
* [検索](#searches)

### トリガー

#### [!UICONTROL レコードを監視]

このトリガーモジュールは、特定のタイプのオブジェクトが追加、更新、またはその両方が行われた場合にシナリオを実行します。このモジュールは、レコードに関連付けられたすべての標準フィールドと、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> <table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Allocadia アカウントを [!DNL Workfront Fusion] に接続する手順について詳しくは、<a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!UICONTROL Connect Allocadia] をWorkfront Fusion に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">フィルター</td> 
   <td> <p>シナリオで新規レコードのみを監視するか、[!UICONTROL Updated Records Only] を監視するか、新規およびアップデートされたレコードを監視するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">エンティティタイプ</td> 
   <td>モジュールで監視する Allocadia レコードタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">出力</td> 
   <td> <p>モジュールの出力に含めるフィールドを選択します。使用できるフィールドは、選択したエンティティタイプによって異なります。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">制限</td> 
   <td> <p>各シナリオの実行サイクル中にモジュールが監視するレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [カスタム API 呼び出し](#custom-api-call)
* [レコードの読み取り](#read-record)
* [記録を作成](#create-record)
* [記録を削除](#delete-record)
* [記録を更新](#update-record)

#### [!UICONTROL カスタム API 呼び出し]

このアクションモジュールでは、[!DNL Allocadia] API への認証済みのカスタム呼び出しを実行できます。こうすることで、他の [!DNL Allocadia] モジュールでは不可能なデータフロー自動処理を作成できます。

アクションは、指定したエンティティタイプ（Allocadia オブジェクトタイプ）に基づいて実行されます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Allocadia] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事にある<a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!DNL Allocadia] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td><code>https://api-na.allocadia.com/{version}</code> または <code>https://api-eu.allocadia.com/{version}</code> への相対パスを入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]</a> での HTTP リクエストメソッドを参照してください。</p> </td> 
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

#### [!UICONTROL レコードを読み取り]

このアクションモジュールは、[!DNL Allocadia] の単一レコードからデータを読み取ります。

レコードの ID を指定します。

このモジュールは、レコードに関連付けられた標準フィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Allocadia] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事にある<a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!DNL Allocadia] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>モジュールが読み取る [!DNL Allocadia] レコードのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>モジュールの出力に含めるフィールドを選択します。使用できるフィールドは、選択した [!UICONTROL Entity Type] によって異なります。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>モジュールが読み取るレコードの一意の [!DNL Allocadia] ID を入力またはマッピングします。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを作成]

このアクションモジュールは、レコードを作成します。

このモジュールは、レコードの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Allocadia] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事にある<a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!DNL Allocadia] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>レコードを新規作成する場合、行項目に基づいて作成か、列の選択に基づいて作成かを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Budgets]</td> 
   <td> <p>レコードを作成する予算を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Column choices]</td> 
   <td>新しいレコードの作成に使用する列を選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Label]</td> 
   <td>新しいレコードのラベルの入力またはマッピング</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードの削除]

このアクションモジュールは、特定のレコードを削除します。

レコードの ID を指定します。

このモジュールは、レコードの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Allocadia] アカウントを [!DNL Workfront Fusion] に接続する方法については、この記事の<a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!DNL Allocadia] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td> <p>削除するエンティティのタイプを選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Line item]</strong> </p> <p>行項目 ID を入力</p> </li> 
     <li> <p><strong>[!UICONTROL Column Choice]</strong> </p> <p>レコードを削除する予算を選択し、列 ID と選択 ID を入力します。</p> </li> 
     <li> <p><strong>[!UICONTROL Forecast Tags]</strong> </p> <p>レコードを削除する予算を選択し、タグ ID を入力します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードの更新]

このアクションモジュールは、行項目、ユーザー、列選択などのレコードを更新します。

レコードの ID を指定します。

このモジュールは、レコードの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!UICONTROL Allocadia] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の<a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!DNL Allocadia] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>モジュールが更新する [!DNL Allocadia] レコードのタイプを選択します。選択したエンティティタイプに基づいて、その他のフィールドが表示されます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Budgets]</td> 
   <td> <p>レコードを更新する予算を選択します。 </p> </td> 
  </tr> 
 </tbody> 
</table>

### 検索

#### [!UICONTROL レコードの検索]

この検索モジュールは、指定された検索クエリに一致するレコードを [!DNL Allocadia] のオブジェクト内で検索します。

この情報は、シナリオ内の後続のモジュールにマッピングできます。

必要なレコードのタイプを指定します。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>[!DNL Allocadia] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事にある<a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!DNL Allocadia] を [!DNL Workfront Fusion]</a> に接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Entity Type]</td> 
   <td>モジュールで検索する [!DNL Allocadia] レコードのタイプを選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Budgets]</td> 
   <td> <p>検索する予算を選択します。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Result set]</td> 
   <td>モジュールで条件に一致するすべてのレコードを返すか、条件に一致する最初のレコードのみを返すかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximal count of records]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search criteria]</td> 
   <td>検索するフィールドを選択し、操作を選択し、検索する値を入力またはマッピングします。[!DNL AND] または [!DNL OR] ルールを追加して検索をさらに絞り込むことができます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td> <p>モジュールの出力に含めるフィールドを選択します。使用できるフィールドは、選択したエンティティタイプによって異なります。</p> </td> 
  </tr> 
 </tbody> 
</table>
