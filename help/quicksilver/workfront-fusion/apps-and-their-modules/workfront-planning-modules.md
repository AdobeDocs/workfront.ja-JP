---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Adobe Workfront Planning モジュール
description: を使用 [!DNL Adobe Workfront Planning] モジュールを使用する場合は、 [!DNL Adobe Workfront Fusion] シナリオに基づいて [!DNL Adobe] Workfront Planning のアカウント、契約およびその他のレコードの作成、読み取り、更新、設定した条件を使用したレコードの検索、ドキュメントのアップロードを行います。
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 892fdaf3-935e-4e66-a01c-9e9b6e0daf3e
source-git-commit: 593612fea52d917904605cf3d97403347c9c9ac0
workflow-type: tm+mt
source-wordcount: '1018'
ht-degree: 47%

---

# [!DNL Adobe Workfront Planning] モジュール

を使用 [!DNL Adobe Workfront Planning] モジュールを使用すると、Workfront Planning でトリガーが発生した場合にシナリオを作成できます。 また、レコードの作成、読み取り、更新、削除をおこなったり、 [!DNL Adobe Workfront Planning] アカウント。

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
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront]を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## [!DNL Adobe Workfront Planning] への接続の作成

[!DNL Workfront Planning] アカウントへの接続を、[!DNL Workfront Fusion] モジュール内から直接作成できます。

1. 任意の [!DNL Workfront Planning] モジュールで、「[!UICONTROL 接続]」ボックスの横にある「**[!UICONTROL 追加]**」をクリックします。
1. この接続の名前を入力します。
1. 実稼動環境に接続するか、実稼動以外の環境に接続するかを選択します。
1. サービスアカウントと個人アカウントのどちらに接続するかを選択します。
1. 「**[!UICONTROL SAML ログイン]**」をクリックして接続を作成し、モジュールに戻ります。

## [!DNL Adobe Workfront Planning] モジュールとそのフィールド

### イベントを見る

このトリガー・モジュールは、Workfront Planning でレコード、レコード・タイプ、またはワークスペースが作成、更新、または削除されたときにシナリオを開始します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>使用する Webhook を選択するか、「追加」をクリックして新しい Webhook を作成します。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Workfront Planning] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >[!DNL Adobe Workfront Planning]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Object type]</td>
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

このアクションモジュールは、Workfront Planning 内の 1 つのレコードタイプを ID で削除します。

>[!WARNING]
>
>Workfront Planning でレコードタイプを削除すると、レコードタイプテーブル内のすべてのレコードも削除されます。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Workfront Planning] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >[!DNL Adobe Workfront Planning]</a> への接続を作成を参照してください。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL レコードタイプ ID]</p>
      </td>
      <td>削除するフィールドの ID を入力またはマッピングします。</td> 
      </tr>
  </tbody>
</table>

### カスタム API 呼び出しを実行

このモジュールは、[!DNL Adobe Workfront Planning] API に対してカスタム API 呼び出しを実行します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Workfront Planning] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >[!DNL Adobe Workfront Planning]</a> への接続を作成を参照してください。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/に対する相対パスを入力してください</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL API version]</p>
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
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>クエリ文字列に追加するキーと値のペアごとに、 <b>項目を追加</b> キーと値を入力します。</p>
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

<!--

### Delete a field

This action module deletes a single field in Workfront Planning by its ID.

>[!WARNING]
>
>Deleting a field in Workfront Planning deletes it and any data in it from every object of that record type in Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
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


This action module retrieves a single field in Workfront Planning by its ID.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
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

### レコードを作成

この操作により、Workfront Planning に 1 つのレコードが作成されます。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Workfront Planning] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >[!DNL Adobe Workfront Planning]</a> への接続を作成を参照してください。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL レコードタイプ ID]</p>
      </td>
      <td>作成するレコードのタイプを入力またはマッピングします。 使用可能なレコードのタイプは、Workfront Planning アカウントに基づいています。</td> 
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

このアクションモジュールは、Workfront Planning で指定したレコードを削除します。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Workfront Planning] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >[!DNL Adobe Workfront Planning]</a> への接続を作成を参照してください。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record ID]</p>
      </td>
      <td>削除するレコードの ID を入力またはマッピングします。</td> 
      </tr>
  </tbody>
</table>

<!--

### Get all records

This action module retrieves all records from an [!DNL Adobe Workfront Planning] account.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
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

### レコードを取得

このアクションモジュールは、 [!DNL Adobe Workfront Planning]:ID で指定されます。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Workfront Planning] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >[!DNL Adobe Workfront Planning]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record ID]</td>
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
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Workfront Planning] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >[!DNL Adobe Workfront Planning]</a> への接続を作成を参照してください。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>取得するレコードを含むワークスペースを選択またはマッピングします。</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record type]</td>
      <td>取得するレコードのタイプを選択します。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned records]</p>
      </td>
      <td>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</td> 
  </tbody>
</table>

### レコードタイプの取得

このアクションモジュールは、 [!DNL Adobe Workfront Planning] アカウント。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Workfront Planning] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >[!DNL Adobe Workfront Planning]</a> への接続を作成を参照してください。</td>
    </tr>
  </tbody>
</table>

### レコードを更新

この操作により、Workfront Planning の 1 つのレコードが更新されます。

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>[!DNL Adobe Workfront Planning] への接続を作成する手順については、この記事の<a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >[!DNL Adobe Workfront Planning]</a> への接続を作成を参照してください。</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record ID]</p>
      </td>
      <td>更新するレコードのタイプを入力またはマッピングします。 使用可能なレコードのタイプは、Workfront Planning アカウントに基づいています。</td> 
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
