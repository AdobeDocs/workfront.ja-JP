---
filename: airtable-modules
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Airtable モジュール
description: Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。 この記事は廃止されましたが、この機能を説明する新しい記事へのリンクが含まれています。
author: Becky
feature: Workfront Fusion
exl-id: 1d78e0db-9a77-437d-a72f-88fb256981c0
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '1934'
ht-degree: 95%

---

# Airtable モジュール

>[!IMPORTANT]
>
>Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。
>
>この記事の情報は、次の記事に記載されています。
>
>* [ 空冷モジュール ](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/airtable-modules.html)
>
>ブックマークを更新してください。
>
>この記事は現在更新されておらず、近い将来に削除されます。


[!DNL Adobe Workfront Fusion] 対応の [!DNL Airtable] コネクタを使用すると、[!DNL Airtable] アカウント内のイベントに基づいてシナリオを開始したり、レコードを作成、アップロード、更新したり、レコードを検索したり、Airtable API に対するカスタム API 呼び出しを実行したりできます。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>この記事で説明されている機能を使用するには、組織で [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

この記事の機能を使用するには、Airtable アカウントが必要です。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For more information, see the tutorial .</p>
-->

## Airtable API 情報

Airtable コネクタでは、以下を使用します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">ベース URL</td> 
   <td>https://api.airtable.com/v0</td> 
  </tr>
  <tr> 
   <td role="rowheader">API タグ</td> 
   <td>v3.3.28</td> 
  </tr>
 </tbody> 
 </table>

## Airtable を Workfront Fusion に接続 {#connect-airtable-to-workfront-fusion}

<!--

1. Log in to your Airtable account.
1. Open your account overview and generate the API key.
-->
1. Workfront Fusion と、必要なモジュールの&#x200B;**接続を作成**&#x200B;ダイアログを開きます。
1. 接続に名前を入力します。
1. （オプション）「詳細設定を表示」をクリックし、Airtable のクライアント ID とクライアントシークレットを入力します。
1. 「**続行**」ボタンをクリックして接続を作成し、モジュールに戻ります。

## Airtable モジュールとそのフィールド

### レコード

* [レコードを作成](#create-a-record)
* [レコードを削除](#delete-a-record)
* [レコードを取得](#get-a-record)
* [レコードを検索](#search-records)
* [レコードを更新](#update-a-record)
* [レコードをアップサート](#upsert-a-record)
* [レコードを監視](#watch-records)
* [応答を監視](#watch-responses)
* [API 呼び出しを実行](#make-an-api-call)

#### レコードを作成 {#create-a-record}

このアクションモジュールは、新しいレコードを作成します。

レコードに含めるデータと、その保存場所を指定します。

このモジュールは、レコードに関連付けられた標準フィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>接続 </td> 
   <td> <p>Airtable アカウントを Workfront Fusion に接続する手順について詳しくは、この記事の <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Airtable を Workfront Fusion に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>基本 </td> 
   <td> <p>新しいレコードが属するベースを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>テーブル </td> 
   <td> <p>新しいレコードが属するテーブルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>レコード</p> </td> 
   <td> <p>新しいレコードの値を入力します。使用可能なフィールドは、選択したテーブルに基づきます。</p> <!--<p>For more information on field types, search for "Supported field types" in the Airtable documentation.</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>Multiple lines of text, which may contain "mention tokens", for example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong> : Add the attachment. Airtable will download the file from the provided <code>url</code> and keep its own copy of it. If the File name field is left empty, Airtable generates the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05 (ISO 8601 formatted date)</li> 
     <li>Phone number:</li> 
     <li><strong>Emails</strong>: A valid email address.</li> 
     <li><strong>URL</strong>: A valid URL (for example, airtable.com or https://airtable.com/universe).</li> 
     <li><strong>Number</strong>: Enter a number.</li> 
     <li><strong>Currency</strong>: Currency value.</li> 
     <li><strong>Percent</strong>: A percentage value. Must be higher than or equal to 0.</li> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation. </li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs will be reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>スマートリンク</td> 
   <td> <p>別のテーブルにリンクするフィールドにレコード ID の代わりに名前を入力するには、このオプションを有効にします。一致がない場合、リンクされたテーブルにレコードが自動的に作成されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### レコードの削除 {#delete-a-record}

このアクションモジュールは、特定のレコードを削除します。

レコードの ID と場所を指定します。

このモジュールは、レコードの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>接続 </td> 
   <td> <p>Airtable アカウントを Workfront Fusion に接続する手順について詳しくは、この記事の <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Airtable を Workfront Fusion に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>基本 </td> 
   <td> <p>削除するレコードを含むベースを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>テーブル </td> 
   <td> <p>削除するレコードを含むテーブルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>レコード ID</td> 
   <td> <p>モジュールで削除するレコードの一意の Airtable ID を入力またはマッピングします。例えば、レコードを検索モジュールを使用して ID を取得できます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### レコードを取得 {#get-a-record}

このアクションモジュールは、レコードの詳細を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>接続 </td> 
   <td> <p>Airtable アカウントを Workfront Fusion に接続する手順について詳しくは、この記事の <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Airtable を Workfront Fusion に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>基本 </td> 
   <td> <p>取得するレコードが含まれているテーブルを含むベースを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>テーブル</td> 
   <td> <p> 詳細を取得するレコードを含むテーブルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>レコード ID</td> 
   <td> <p> 詳細を取得するレコードの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### レコードの検索 {#search-records}

この検索モジュールは、指定した検索クエリに一致するレコードを Airtable のオブジェクト内で検索します。

この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>接続 </td> 
   <td> <p>Airtable アカウントを Workfront Fusion に接続する手順について詳しくは、この記事の <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Airtable を Workfront Fusion に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>基本 </td> 
   <td> <p>レコードを検索するベースを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>テーブル </td> 
   <td> <p>レコードを検索するテーブルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>式</p> </td> 
   <td> <p>レコードのフィルタリングに使用する数式です。式は各レコードに対して評価され、結果が <code>0</code>、<code>false</code>、<code>""</code>、<code>NaN</code>、<code>[]</code> または <code>#Error!</code> でない場合は、レコードが応答に含まれます。</p> <p><code>view</code> と組み合わせた場合は、そのビュー内で数式を満たすレコードのみが返されます。</p> <p>例えば、名前が空でないレコードのみを含めるには、次のように渡します。<code> NOT({Name} = '')</code></p> <p>詳しくは、Airtable サポートドキュメントで数式フィールドの参照に関する情報を検索してください。</p> </td> 
  </tr> 
  <tr> 
   <td>並べ替え </td> 
   <td> <p>並べ替えの方向と、結果の並べ替えに使用するフィールドを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>表示 </td> 
   <td> <p>レコードを検索するビューを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>制限</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### レコードの更新 {#update-a-record}

このアクションモジュールは、特定のレコードを更新します。

レコードの ID と、レコードに含める新しいデータを指定します。

このモジュールは、レコードに関連付けられた標準フィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>接続 </td> 
   <td> <p>Airtable アカウントを Workfront Fusion に接続する手順について詳しくは、この記事の <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Airtable を Workfront Fusion に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>基本 </td> 
   <td> <p>更新するレコードを含むベースを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>テーブル </td> 
   <td> <p>更新するレコードを含むテーブルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>レコード ID </td> 
   <td> <p>モジュールで更新するレコードの一意の Airtable ID を入力またはマッピングします。例えば、レコードを検索モジュールを使用して ID を取得できます。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>レコード</p> </td> 
   <td> <p>新しいレコードの値を入力します。使用可能なフィールドは、選択したテーブルによって異なります。</p> <!--<p>In order to delete the content of the field, use the erase function. </p>  <p>Field types (via airtable.com/api):</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>The string can contain multiple lines of text with "mention tokens." For example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong>: Add the attachment. Airtable will download the file from the provided url and keep its own copy of it. If the File name field is left empty, Airtable will generate the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05. (ISO 8601 formatted date)</li> 
     <li><strong>Phone number</strong>: A telephone number, for example, (415) 555-9876.</li> 
     <li><strong>Email</strong>valid email address.</li> 
     <li><strong>URL</strong>: lid URL such as airtable.com or https://airtable.coiverse.</li> 
     <li><strong>Number</strongnter a number.</li> 
     <li><strong>Currency</stro Currency value.</li> 
     <li><strong>Percent</stronA percentage value; must be equal to or more than 0i> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation.</li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs is reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>スマートリンク</td> 
   <td> <p>別のテーブルにリンクするフィールドに、レコード ID の代わりに名前を入力します。一致がない場合、リンクされたテーブルにレコードが自動的に作成されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### レコードをアップサート

このアクションモジュールは、特定のレコードを更新または挿入します。

レコードの ID と、レコードに含める新しいデータを指定します。

このモジュールは、レコードに関連付けられた標準フィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>接続 </td> 
   <td> <p>Airtable アカウントを Workfront Fusion に接続する手順について詳しくは、この記事の <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Airtable を Workfront Fusion に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>基本 </td> 
   <td> <p>更新するレコードを含むベースを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>テーブル </td> 
   <td> <p>更新するレコードを含むテーブルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>レコード ID </td> 
   <td> <p>レコードを更新する場合は、モジュールで更新するレコードの一意の Airtable ID を入力またはマッピングします。例えば、レコードを検索モジュールを使用して ID を取得できます。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>レコード</p> </td> 
   <td> <p>新しいレコードの値を入力します。使用可能なフィールドは、選択したテーブルによって異なります。</p> <!-- <p>In order to delete the content of the field, use the erase function. </p>  <p>Field types (via airtable.com/api):</p> 
    <ul> 
     <li> <p><strong>Text</strong>: string</p> <p>A single line of text.</p> </li> 
     <li> <p><strong>Long text</strong>: string</p> <p>The string can contain multiple lines of text with "mention tokens." For example:</p><pre>&lt;airtable:mention id="menE1i9oBaGX3DseR"&gt;@Alex&lt;/airtable:mention&gt;</pre> </li> 
     <li><strong>Attachment</strong>: Add the attachment. Airtable will download the file from the provided url and keep its own copy of it. If the File name field is left empty, Airtable will generate the name automatically.</li> 
     <li><strong>Checkbox</strong>: Select one of the options.</li> 
     <li><strong>Multiple select</strong>: Select multiple options in the checklist.</li> 
     <li><strong>Single select</strong>: Select one option from the drop-down menu.</li> 
     <li><strong>Collaborator</strong>: Enter the email that uniquely identifies a user in Airtable who this base is shared with.</li> 
     <li><strong>Date</strong>: UTC date, for example, 2019-09-05. (ISO 8601 formatted date)</li> 
     <li><strong>Phone number</strong>: A telephone number, for example, (415) 555-9876.</li> 
     <li><strong>Email</strong>valid email address.</li> 
     <li><strong>URL</strong>: lid URL such as airtable.com or https://airtable.coiverse.</li> 
     <li><strong>Number</strongnter a number.</li> 
     <li><strong>Currency</stro Currency value.</li> 
     <li><strong>Percent</stronA percentage value; must be equal to or more than 0i> 
     <li><strong>Duration</strong>: Enter the duration time. If you need help, see the information about the duration field type in the Airtable support documentation.</li> 
     <li><strong>Rating</strong>: Enter the number. For example, "3 stars" is 3. A rating cannot be 0.</li> 
     <li><strong>Link</strong>: Enter the linked records IDs from the table. The order of record IDs is reversed compared to what you see in the app.</li> 
     <li><strong>Rollup</strong>: Computed value: COUNT(values)</li> 
     <li><strong>Lookup</strong>: Array of long text fields</li> 
     <li><strong>Autonumber</strong>: Automatically incremented unique counter for each record.</li> 
     <li> <p><strong>Barcode</strong>: The barcode object may contain the following two properties, both of which are optional.</p> <p>Barcode data (text)</p> <p>Barcode symbology, for example, "upce" or "code39" (type)</p> </li> 
    </ul> --></td> 
  </tr> 
  <tr> 
   <td>スマートリンク</td> 
   <td> <p>別のテーブルにリンクするフィールドに、レコード ID の代わりに名前を入力します。一致がない場合、リンクされたテーブルにレコードが自動的に作成されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### レコードを監視 {#watch-records}

このトリガーモジュールは、指定したテーブルでレコードが作成またはアップデートされたときにシナリオを開始します。

>[!NOTE]
>
>このモジュールを使用するには、テーブルで「作成時刻」フィールドまたは「最終変更時刻」フィールドを作成する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>接続 </td> 
   <td> <p>Airtable アカウントを Workfront Fusion に接続する手順について詳しくは、この記事の <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Airtable を Workfront Fusion に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>基本 </td> 
   <td> <p>新しいレコードを監視するベースを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>テーブル </td> 
   <td> <p>新しいレコードを監視するテーブルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>トリガー設定</p> </td> 
   <td> <p>トリガーフィールド</p> <p>レコードの並べ替えに使用する <code>Created Time</code> または <code>Last Modified Time</code> フィールド。スキーマに <code>Created Time</code> または <code>Last Modified Time</code> フィールドが含まれていない場合は、作成する必要があります。 </p> <p>ラベルフィールド</p> <p>レコードのラベルとして使用されるフィールド（開始場所を選択ダイアログ内など）。</p> </td> 
  </tr> 
  <tr> 
   <td>制限</td> 
   <td> <p>各シナリオの実行サイクル中にモジュールが監視するレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>ビュー</td> 
   <td> <p>使用するビューを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>式</p> </td> 
   <td> <p>レコードのフィルタリングに使用する数式です。式は各レコードに対して評価され、結果が <code>0</code>、<code>false</code>、<code>""</code>、<code>NaN</code>、<code>[]</code> または <code>#Error!</code> でない場合は、レコードが応答に含まれます。</p> <p><code>view</code> と組み合わせた場合は、そのビュー内で数式を満たすレコードのみが返されます。</p> <p>例えば、名前が空でないレコードのみを含めるには、次のように渡します。<code> NOT({Name} = '')</code></p> <p>詳しくは、Airtable サポートドキュメントの数式フィールドの参照に関する情報を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### 応答を監視

このトリガーモジュールは、フォームが送信されたときにシナリオを開始します。

>[!NOTE]
>
>この機能は有料の Airtable Pro プランでのみ利用できます。

web フック URL は、Workfront Fusion で生成してから、Airtable のフォーム設定に追加する必要があります。

1. 新しい応答を監視モジュールを Workfront Fusion シナリオに追加します。
1. web フック URL を生成してコピーします。

   手順については、[Adobe Workfront Fusion のインスタントトリガー（web フック）](../../workfront-fusion/webhooks/instant-triggers-webhooks.md)を参照してください。

1. Airtable アカウントにログインします。
1. ベースと、フォームに使用するテーブルを開き、フォームビューを作成します。
1. 必要に応じてフォームを設定し、フォームを下にスクロールして、「フォーム送信後に URL にリダイレクト」オプションを有効にします。
1. 表示されるダイアログボックスに、手順 2 で生成した web フック URL を入力し、web フック URL の直後に ？record_id={record_id} を追加してレコード ID をモジュールの出力に含め、「保存」をクリックします。結果の URL は、例えば、次のようになります。
1. Workfront Fusion のシナリオに戻り、応答を監視モジュールのみを実行して、Airtable からフィールドを読み込み、それらのフィールドを他のモジュールにマッピングできるようにします。
1. 「フォーム送信後に URL にリダイレクト」オプションが有効になっていて、web フック URL が追加（上記の手順 6）されているAirtable でフォームを送信します。

   応答を監視モジュールがトリガーされ、目的のデータが読み込まれます。

1. Airtable／レコードを取得モジュールを、Airtable／応答を監視モジュールの直後に追加し、record_id を「レコード ID」フィールドにマッピングします。

これで、フォームが送信されるたびに、Workfront Fusion シナリオの応答を監視モジュールがトリガーされ、レコードを取得モジュールが、送信されたフォームの詳細を返します。

#### API 呼び出しを実行

#### カスタム API 呼び出し

このアクションモジュールでは、[!DNL Airtable] API への認証済みのカスタム呼び出しを実行できます。これにより、他の [!DNL Airtable] モジュールでは不可能なデータフロー自動処理を実現できます。

アクションは、指定したエンティティタイプ（Allocadia オブジェクトタイプ）に基づいて実行されます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>接続</p> </td> 
   <td> <p>Airtable アカウントを Workfront Fusion に接続する手順について詳しくは、この記事の <a href="#connect-airtable-to-workfront-fusion" class="MCXref xref">Airtable を Workfront Fusion に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td><code>https://api.airtable.com/}</code> への相対パスを入力します。例：<code>v0/{base}/{table}</code> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">メソッド</td> 
   <td> <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]</a> での HTTP リクエストメソッドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ヘッダー</td> 
   <td> <p>リクエストのヘッダーを標準 JSON オブジェクトの形式で追加します。</p> <p>例： <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] によって、認証ヘッダーが追加されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">クエリ文字列</td> 
   <td> <p>キーと値の形式で API 呼び出しのクエリを追加する</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">本文</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文の内容を追加します。</p> <p>メモ：  <p><code>if</code> などの条件文を JSON で使用する場合は、条件文を引用符で囲みます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
