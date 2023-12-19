---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: AdobeMaestro モジュール
description: を使用 [!DNL Adobe Maestro] モジュールを使用する場合は、 [!DNL Adobe Workfront Fusion] シナリオに基づいて [!DNL Adobe] Maestro アカウント、契約およびその他のレコードの作成、読み取り、更新、設定した条件を使用したレコードの検索、ドキュメントのアップロードを行います。
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
source-git-commit: fe0c867b218879c1d0d969112eb62878782a40ad
workflow-type: tm+mt
source-wordcount: '1007'
ht-degree: 0%

---

# [!DNL Adobe Maestro] モジュール

を使用 [!DNL Adobe Maestro] モジュールを使用すると、Maestro でトリガーが発生した場合にシナリオを作成できます。 また、レコードの作成、読み取り、更新、削除をおこなったり、 [!DNL Adobe Maestro] アカウント。

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
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
   <p>従来のライセンス要件： [!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件： [!UICONTROL Select] または [!UICONTROL Prime] がある場合 [!DNL Adobe Workfront] プラン（組織で購入する必要がある） [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。 [!DNL Workfront Fusion] は、[!UICONTROL Ultimate] に含まれています [!DNL Workfront] プラン</p>
   <p>または</p>
   <p>従来の製品要件：組織は購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## への接続の作成 [!DNL Adobe Maestro]

次に対する接続を作成できます： [!DNL Maestro] 内部から直接アカウントを取得する [!DNL Workfront Fusion] モジュール。

1. 任意の [!DNL Maestro] アプリモジュール、クリック **[!UICONTROL 追加]** の横 [!UICONTROL 接続] ボックス。
1. この接続の名前を入力します。
1. 実稼動環境に接続するか、実稼動以外の環境に接続するかを選択します。
1. サービスアカウントと個人アカウントのどちらに接続するかを選択します。
1. クリック **[!UICONTROL SAML ログイン]** 接続を作成し、モジュールに戻ります。

## [!DNL Adobe Maestro] モジュールとそのフィールド

### イベントを見る

このトリガーモジュールは、レコード、レコードタイプ、またはワークスペースが Maestro で作成、更新、または削除されたときにシナリオを開始します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>使用する Webhook を選択するか、「追加」をクリックして新しい Webhook を作成します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td>への接続を作成する手順については、 [!DNL Adobe Maestro]を参照してください。 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >への接続の作成 [!DNL Adobe Maestro]</a> 」を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL オブジェクトタイプ ]</td>
      <td>レコード、レコードの種類、またはワークスペースを監視するかどうかを選択します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 監視するオブジェクト ]</td>
      <td>新規を監視するかどうかを選択します。 レコードの更新、新規作成、更新、削除。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL この接続による更新を除外 ]</p>
      </td>
      <td>このオプションを有効にすると、このモジュールで使用される接続によって変更が行われた場合にシナリオがトリガーされなくなります。 これにより、このシナリオがトリガーアクションを実行した場合に、シナリオの別のインスタンスがトリガーされるのを防ぎます。</td> 
      </tr>
  </tbody>
</table>

### レコードタイプの削除

このアクションモジュールは、ID で Maestro 内の 1 つのレコードタイプを削除します。

>[!WARNING]
>
>Maestro でレコードタイプを削除すると、レコードタイプテーブル内のすべてのレコードも削除されます。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td>への接続を作成する手順については、 [!DNL Adobe Maestro]を参照してください。 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >への接続の作成 [!DNL Adobe Maestro]</a> 」を参照してください。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL レコードタイプ ID]</p>
      </td>
      <td>削除するフィールドの ID を入力またはマッピングします。</td> 
      </tr>
  </tbody>
</table>

### カスタム API 呼び出しをおこなう

このモジュールは、 [!DNL Adobe Maestro] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td>への接続を作成する手順については、 [!DNL Adobe Maestro]を参照してください。 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >への接続の作成 [!DNL Adobe Maestro]</a> 」を参照してください。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL パス ]</p>
      </td>
      <td>
        <p>https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/に対する相対パスを入力してください</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL API バージョン ]</p>
      </td>
      <td>
        <p>使用する API バージョンを選択します。 バージョンを選択しない場合、デフォルトで最新バージョンが使用されます。</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL API パスの上書き ]</p>
      </td>
      <td>
        <p>https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/に対する相対パスを入力してください</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL メソッド ]</p>
      </td>
   <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">での HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p>
        <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] は、認証ヘッダーを自動的に追加します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL クエリ文字列 ]  </td>
      <td>
        <p>クエリ文字列に追加するキーと値のペアごとに、 <b>項目を追加</b> キーと値を入力します。</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL 本文 ]</td>
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文のコンテンツを追加します。</p> <p>注意：  <p>条件ステートメント ( <code>if</code> JSON で、条件文の外側に引用符を置きます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

<!--

### Delete a field

This action module deletes a single field in Maestro by its ID.

>[!WARNING]
>
>Deleting a field in Maestro deletes it and any data in it from every object of that record type in Maestro.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Field ID]</p>
      </td>
      <td>Enter or map the ID of the record type you want to delete.</td> 
      </tr>
  </tbody>
</table>

### Get a field 


This action module retrieves a single field in Maestro by its ID.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Field ID]</p>
      </td>
      <td>Enter or map the ID of the field you want to delete.</td> 
      </tr>
  </tbody>
</table>

-->

### レコードの作成

この操作により、Maestro に 1 つのレコードが作成されます。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td>への接続を作成する手順については、 [!DNL Adobe Maestro]を参照してください。 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >への接続の作成 [!DNL Adobe Maestro]</a> 」を参照してください。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL レコードタイプ ID]</p>
      </td>
      <td>作成するレコードのタイプを入力またはマッピングします。 使用可能なレコードタイプは、Maestro アカウントに基づきます。</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>その他のフィールド</p>
      </td>
      <td>これらのフィールドは、選択したレコードタイプに基づいています。</td> 
      </tr>
     <tr>
  </tbody>
</table>

### レコードの削除

このアクションモジュールは、Maestro 内の指定されたレコードを削除します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td>への接続を作成する手順については、 [!DNL Adobe Maestro]を参照してください。 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >への接続の作成 [!DNL Adobe Maestro]</a> 」を参照してください。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL レコード ID]</p>
      </td>
      <td>削除するレコードの ID を入力またはマッピングします。</td> 
      </tr>
  </tbody>
</table>

<!--

### Get all records

This action module retrieves all records from an [!DNL Adobe Maestro] account.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Maestro], see <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >Create a connection to [!DNL Adobe Maestro]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned records]</p>
      </td>
      <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td> 
      </tr>
  </tbody>
</table>

-->

### レコードの取得

このアクションモジュールは、 [!DNL Adobe Maestro]:ID で指定されます。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td>への接続を作成する手順については、 [!DNL Adobe Maestro]を参照してください。 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >への接続の作成 [!DNL Adobe Maestro]</a> 」を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL レコード ID]</td>
      <td>取得するレコードの ID を入力またはマッピングします。</td>
    </tr>
  </tbody>
</table>

### レコードタイプ別にレコードを取得

このアクションモジュールは、指定されたタイプのすべてのレコードを取得します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td>への接続を作成する手順については、 [!DNL Adobe Maestro]を参照してください。 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >への接続の作成 [!DNL Adobe Maestro]</a> 」を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>取得するレコードを含むワークスペースを選択またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL レコードタイプ ]</td>
      <td>取得するレコードのタイプを選択します。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL 返されるレコードの最大数 ]</p>
      </td>
      <td>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</td> 
  </tbody>
</table>

### レコードタイプの取得

このアクションモジュールは、 [!DNL Adobe Maestro] アカウント。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td>への接続を作成する手順については、 [!DNL Adobe Maestro]を参照してください。 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >への接続の作成 [!DNL Adobe Maestro]</a> 」を参照してください。</td>
    </tr>
  </tbody>
</table>

### レコードを更新

この操作により、Maestro 内の 1 つのレコードが更新されます。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL 接続 ]</td>
      <td>への接続を作成する手順については、 [!DNL Adobe Maestro]を参照してください。 <a href="#create-a-connection-to-adobe-maestro" class="MCXref xref" >への接続の作成 [!DNL Adobe Maestro]</a> 」を参照してください。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL レコード ID]</p>
      </td>
      <td>更新するレコードのタイプを入力またはマッピングします。 使用可能なレコードタイプは、Maestro アカウントに基づきます。</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>その他のフィールド</p>
      </td>
      <td>これらのフィールドは、選択したレコードタイプに基づいています。</td> 
      </tr>
     <tr>
  </tbody>
</table>

### レコードを検索

このアクションモジュールは、指定した条件に基づいてレコードのリストを取得します。

>[!NOTE]
>
>このモジュールは作成中です。

