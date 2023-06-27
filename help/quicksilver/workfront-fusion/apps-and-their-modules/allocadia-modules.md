---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Allocadia モジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオの場合、Allocadia を使用するワークフローを自動化し、複数のサードパーティのアプリケーションやサービスに接続できます。
author: Becky
feature: Workfront Fusion
exl-id: f1edefd1-9fe0-48fc-bea2-c3f9facf7363
source-git-commit: a3756f9345cbc9417a6fd110306dfa50aecc81a2
workflow-type: tm+mt
source-wordcount: '1401'
ht-degree: 0%

---

# [!DNL Allocadia] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Allocadia]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

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

使用する [!DNL Allocadia] モジュールの場合、 [!DNL Allocadia] アカウント

## 接続 [!DNL Allocadia] から [!DNL Workfront Fusion]

次に、 [!DNL Allocadia] 内部から直接アカウント [!DNL Allocadia] モジュール。

1. 任意の [!DNL Allocadia] モジュール、クリック **[!UICONTROL 追加]** の横 [!UICONTROL 接続] フィールドに入力します。
1. 北米のサーバーを使用するか、ヨーロッパのサーバーを使用するかを選択します。
1. ユーザー名とパスワードを入力します。
1. クリック **[!UICONTROL 続行]** 接続を作成し、モジュールに戻ります。

## [!DNL Allocadia] モジュールとそのフィールド

設定時に [!DNL Allocadia] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Allocadia] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [トリガー](#triggers)
* [アクション](#actions)
* [検索](#searches)

### トリガー

#### [!UICONTROL レコードを監視]

このトリガー・モジュールは、特定のタイプのオブジェクトが追加、更新、またはその両方された場合にシナリオを実行します。 このモジュールは、レコードまたはレコードに関連付けられているすべての標準フィールドと、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> <table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>Allocadia アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">[!UICONTROL Allocadia] をWorkfront Fusion に接続</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">フィルター</td> 
   <td> <p>シナリオで「新しいレコードのみ」、「[!UICONTROL 更新済みレコードのみ」、「新規および更新済みレコード」のどれを監視するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">エンティティタイプ</td> 
   <td>モジュールで監視する Allocadia レコードタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">出力</td> 
   <td> <p>モジュールの出力に含めるフィールドを選択します。 使用できるフィールドは、選択したエンティティタイプによって異なります。</p> </td> 
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
* [レコードを作成](#create-record)
* [レコードを削除](#delete-record)
* [レコードを更新](#update-record)

#### [!UICONTROL カスタム API 呼び出し]

このアクションモジュールを使用すると、 [!DNL Allocadia] API これにより、他のユーザーが達成できないデータフローの自動化を作成できます [!DNL Allocadia] モジュール。

アクションは、指定したエンティティタイプ（Allocadia オブジェクトタイプ）に基づいて実行されます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Allocadia] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">接続 [!DNL Allocadia] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>相対パスを入力 <code>https://api-na.allocadia.com/{version}</code> または <code>https://api-eu.allocadia.com/{version}</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メソッド ]</td> 
   <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] によって、認証ヘッダーが追加されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しのクエリを追加します。</p> <p>例： <code>{"name":"something-urgent"}</code></p> </td> 
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

#### [!UICONTROL レコードの読み取り]

このアクションモジュールは、 [!DNL Allocadia].

レコードの ID を指定します。

このモジュールは、レコードに関連付けられた標準フィールドと、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Allocadia] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">接続 [!DNL Allocadia] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL エンティティタイプ ]</td> 
   <td>タイプを選択 [!DNL Allocadia] レコードを作成します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td> <p>モジュールの出力に含めるフィールドを選択します。 使用できるフィールドは、選択した [!UICONTROL エンティティタイプ ] によって異なります。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>一意の [!DNL Allocadia] モジュールが読み取るレコードの ID。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを作成]

このアクションモジュールは、レコードを作成します。

このモジュールは、レコードと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Allocadia] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">接続 [!DNL Allocadia] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL エンティティタイプ ]</td> 
   <td>行項目または列の選択に基づいて新しいレコードを作成するかどうかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 予算 ]</td> 
   <td> <p>レコードを作成する予算を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Column choices]</td> 
   <td>新しいレコードの作成に使用する列を選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Label]</td> 
   <td>新しいレコードのラベルを入力またはマッピング</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを削除]

このアクションモジュールは、特定のレコードを削除します。

レコードの ID を指定します。

このモジュールは、レコードと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Allocadia] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">接続 [!DNL Allocadia] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL エンティティタイプ ]</td> 
   <td> <p>削除するエンティティのタイプを選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 行項目 ]</strong> </p> <p>行項目 ID を入力</p> </li> 
     <li> <p><strong>[!UICONTROL 列の選択 ]</strong> </p> <p>レコードを削除する予算を選択し、列 ID と選択 ID を入力します。</p> </li> 
     <li> <p><strong>[!UICONTROL Forecast Tags]</strong> </p> <p>レコードを削除する予算を選択し、タグ ID を入力します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL レコードを更新]

このアクションモジュールは、行項目、ユーザー、列選択などのレコードを更新します。

レコードの ID を指定します。

このモジュールは、レコードと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>[!UICONTROL Allocadia] アカウントの接続手順 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">接続 [!DNL Allocadia] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL エンティティタイプ ]</td> 
   <td>タイプを選択 [!DNL Allocadia] を記録します。 選択したエンティティタイプに基づいて、その他のフィールドが表示されます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 予算 ]</td> 
   <td> <p>レコードを更新する予算を選択します。 </p> </td> 
  </tr> 
 </tbody> 
</table>

### 検索

#### [!UICONTROL レコードを検索]

この検索モジュールは、 [!DNL Allocadia] 指定した検索クエリに一致する

この情報は、シナリオの後続のモジュールにマッピングできます。

必要なレコードのタイプを指定します。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   td role="rowheader"&gt; <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Allocadia] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-allocadia-to-workfront-fusion" class="MCXref xref">接続 [!DNL Allocadia] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL エンティティタイプ ]</td> 
   <td>タイプを選択 [!DNL Allocadia] を記録します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 予算 ]</td> 
   <td> <p>検索する予算を選択します。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 結果セット ]</td> 
   <td>モジュールで「All Matching Records」を返すか、「First Matching Records」のみを返すかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードの最大数 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 検索条件 ]</td> 
   <td>検索するフィールドを選択し、操作を選択し、検索する値を入力またはマッピングします。 次の項目を追加できます。 [!DNL AND] または [!DNL OR] ルールを使用して検索をさらに絞り込むことができます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td> <p>モジュールの出力に含めるフィールドを選択します。 使用できるフィールドは、選択したエンティティタイプによって異なります。</p> </td> 
  </tr> 
 </tbody> 
</table>
