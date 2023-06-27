---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: ServiceNow モジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL ServiceNow]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。
author: Becky
feature: Workfront Fusion
exl-id: b362cd8b-06b3-4f4c-b405-a2afc24abddb
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1613'
ht-degree: 1%

---

# [!DNL ServiceNow] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL ServiceNow]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

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

使用する [!DNL ServiceNow] モジュールの場合、 [!DNL ServiceNow] アカウント

## 接続 [!DNL ServiceNow] から [!DNL Workfront Fusion]

の接続を作成するには、以下を実行します。 [!DNL ServiceNow] モジュール：

1. クリック **[!UICONTROL 追加]** の横 [!UICONTROL 接続] 最初の [!DNL ServiceNow] モジュール。
1. 以下を入力します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 接続名 ]</p> </td> 
      <td>新しい [!DNL ServiceNow] 接続</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL ユーザー名 ]</p> </td> 
      <td>を入力します。 [!DNL ServiceNow] ユーザー名。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL パスワード ]</p> </td> 
      <td>ServiceNow パスワードを入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL インスタンス ]</p> </td> 
      <td> <p>アドレスを入力 [!DNL ServiceNow] ～を除くアカウント <code>https://</code> ( 通常 <code>&lt;company>.service-now.com</code>) をクリックします。</p> </td> 
     </tr> 
    </tbody> 
   </table>

## [!UICONTROL ServiceNow] モジュールとそのフィールド

設定時に [!DNL ServiceNow] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL ServiceNow] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>カスタムレコードが[!UICONTROL レコードタイプ]「 」フィールドに値を入力すると、カスタムフィールドの読み込みに時間がかかる場合があります。
>
>カスタムレコードがない場合、ドロップダウンは空になります。

* [[!UICONTROL レコードを監視]](#watch-records)
* [[!UICONTROL カスタム API 呼び出し]](#custom-api-call)
* [[!UICONTROL レコードを読み取る]](#read-a-record)
* [[!UICONTROL ユーザーを非アクティブ化する]](#deactivate-a-user)
* [[!UICONTROL 添付ファイルのダウンロード]](#download-an-attachment)
* [[!UICONTROL 添付ファイルのアップロード]](#upload-an-attachment)
* [[!UICONTROL レコードの作成]](#create-a-record)
* [[!UICONTROL レコードの更新]](#update-a-record)
* [[!UICONTROL レコードの削除]](#delete-a-record)
* [[!UICONTROL レコードの検索]](#search-for-records)

### [!UICONTROL レコードを監視]

このトリガーモジュールは、レコードが作成または更新されたときにシナリオをアクティブ化します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>ServiceNow アカウントを次に接続する手順については、 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">接続 [!DNL ServiceNow] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table type]</td> 
   <td>監視するテーブルがカスタムテーブルか標準テーブルかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td>監視するレコードの種類を選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 表示 ]</td> 
   <td>表示する値のタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td>モジュールから出力するフィールドを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フィルター ]</td> 
   <td>新しいレコードと更新されたレコードのどちらを監視するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL カスタム API 呼び出し]

このアクションモジュールを使用すると、 [!DNL ServiceNow] API これにより、他のユーザーが達成できないデータフローの自動化を作成できます [!DNL ServiceNow] モジュール。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>ServiceNow アカウントを次に接続する手順については、 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">接続 [!DNL ServiceNow] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 相対 URL]</td> 
   <td> <p>モジュールとやり取りする Web サーバーのアドレスを入力します。</p> <p>相対 URL を入力できます。つまり、プロトコルを含める必要はありません ( 例えば、 <code>http://</code>) を最初にクリックします。 これは、Web サーバー上でインタラクションが発生していることを示しています。</p> <p>例： <code>[!DNL /api/conversations].create</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メソッド ]</td> 
   td&gt; <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> </td> 
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

### [!UICONTROL レコードを読み取る]

このアクションモジュールは、 [!DNL ServiceNow] を記録します。

このモジュールは、レコードに関連付けられた標準フィールドと、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>ServiceNow アカウントを次に接続する手順については、 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">接続 [!DNL ServiceNow] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードシステム ID]</td> 
   <td>一意の [!DNL ServiceNow] モジュールが読み取るレコードの ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table type]</td> 
   <td>読み取るレコードがカスタムテーブルか標準テーブルかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td>タイプを選択 [!DNL ServiceNow] レコードを作成します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 表示 ]</td> 
   <td>表示する値のタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td>モジュールから出力するフィールドを選択します。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL ユーザーを非アクティブ化する]

このアクションモジュールは、 [!DNL ServiceNow] システム ID を使用します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>ServiceNow アカウントを次に接続する手順については、 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">接続 [!DNL ServiceNow] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ユーザーシステム ID]</td> 
   <td> 一意の [!DNL ServiceNow] モジュールを非アクティブ化するユーザーの ID。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 添付ファイルのダウンロード]

このアクションモジュールは、添付ファイルを [!DNL ServiceNow] レコード。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>ServiceNow アカウントを次に接続する手順については、 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">接続 [!DNL ServiceNow] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 添付ファイルシステム ID]</td> 
   <td> 一意の [!DNL ServiceNow] モジュールをダウンロードする添付ファイルの ID。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 添付ファイルのアップロード]

このアクションモジュールは、添付ファイルを [!DNL ServiceNow] レコード。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>ServiceNow アカウントを次に接続する手順については、 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">接続 [!DNL ServiceNow] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL テーブル名 ]</td> 
   <td>添付ファイルをアップロードするテーブルの名前を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL システム ID]</td> 
   <td>一意の [!DNL ServiceNow] 添付ファイルをアップロードするシステムの ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル名 ]</td> 
   <td>添付ファイルの名前を入力またはマッピング</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイルコンテンツ ]</td> 
   <td>アップロード先のファイルを入力またはマッピングします [!DNL ServiceNow].</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードの作成]

このアクションモジュールは、 [!DNL ServiceNow] レコード。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>ServiceNow アカウントを次に接続する手順については、 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">接続 [!DNL ServiceNow] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table type]</td> 
   <td>カスタムテーブルと標準テーブルのどちらでレコードを作成するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td>タイプを選択 [!DNL ServiceNow] を記録します。 その後、このレコードタイプで使用可能なフィールドに入力できます。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードの更新]

このアクションモジュールは、 [!DNL ServiceNow] レコード。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>ServiceNow アカウントを次に接続する手順については、 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">接続 [!DNL ServiceNow] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードシステム ID]</td> 
   <td>一意の [!DNL ServiceNow] モジュールを更新するレコードの ID。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table type]</td> 
   <td>更新するレコードがカスタムテーブルか標準テーブルのどちらにあるかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td>タイプを選択 [!DNL ServiceNow] を記録します。 その後、このレコードタイプで使用可能なフィールドに入力できます。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードの削除]

このアクションモジュールは、インシデントまたはユーザーを削除します。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>ServiceNow アカウントを次に接続する手順については、 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">接続 [!DNL ServiceNow] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td>インシデントを削除するか、ユーザーを削除するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL システム ID]</td> 
   <td>一意の [!DNL ServiceNow] モジュールで削除するレコードの ID。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードの検索]

このモジュールは、選択した条件を使用してレコードを検索します。

このモジュールは、レコードに関連付けられた標準フィールドと、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>ServiceNow アカウントを次に接続する手順については、 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-servicenow-to-workfront-fusion" class="MCXref xref">接続 [!DNL ServiceNow] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table type]</td> 
   <td>検索するテーブルがカスタムテーブルか標準テーブルかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td>検索するレコードのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 結果セット ]</td> 
   <td>条件に一致するすべてのレコードを返すか、最初のレコードのみを返すかを選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードの最大数 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 検索タイプ ]</td> 
   <td> <p>モジュールで実行する検索のタイプを選択します</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 詳細クエリ ]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL 検索クエリ ]</p> <p>カスタム検索クエリを入力します。 詳しくは、 [!DNL ServiceNow] カスタム検索クエリについては、 <a href="https://docs.servicenow.com/bundle/orlando-platform-user-interface/page/use/common-ui-elements/reference/r_OpAvailableFiltersQueries.html">ServiceNow クエリドキュメント</a>.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL シンプル ]</strong> </p> 
      <ul> 
       <li> <p>[!UICONTROL 検索条件 ]</p> <p>モジュールで検索する条件を入力します。 検索フィルターの設定について詳しくは、 <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Adobe Workfront Fusion でシナリオにフィルターを追加する</a>.</p> </li> 
       <li> <p>[!UICONTROL 並べ替え基準 ]</p> <p>モジュールで結果を並べ替えるフィールド、および昇順と降順のどちらで並べ替えるかを指定します。</p> </li> 
      </ul> </li> 
    </ul> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 表示 ]</td> 
   <td>表示する値のタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td>モジュールから出力するフィールドを選択します。</td> 
  </tr> 
 </tbody> 
</table>
