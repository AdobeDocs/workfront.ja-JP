---
title: Adobe PDF Services
description: Adobe PDF Services
author: Becky
draft: Probably
feature: Workfront Fusion, Digital Content and Documents
exl-id: e0a5736b-dbdb-43c6-83ff-e88a5625a5bf
source-git-commit: b43ea012d7c649c94011f72f010ae24895e6ef4b
workflow-type: tm+mt
source-wordcount: '3590'
ht-degree: 0%

---

# [!DNL Adobe PDF Services]

を使用 [!DNL Adobe Workfront Fusion] [!DNL Adobe PDF Services]を使用すると、PDFファイルからデータを抽出したり、指定したデータから新しいPDFファイルを生成したりできます。 さらに、様々なファイルタイプをPDFに変換したり、PDFを他のファイルタイプに変換したりできます。 PDFサービスでは、PDFファイルのメタデータの組み合わせ、圧縮、読み取りを行うことや、ファイルのパスワード保護を制御することもできます。

シナリオの作成手順については、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

モジュールについて詳しくは、 [のモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

PDFサービスに使用する API について詳しくは、 [Adobeドキュメント生成 API](https://www.adobe.io/apis/documentcloud/dcsdk/doc-generation.html).

## を使用する際のセキュリティに関する考慮事項 [!DNL Adobe PDF Services]

<!--

* [You do not need an [!DNL Adobe] account](#you-do-not-need-an-adobe-account) 
* [[!DNL Workfront Fusion] does not store your files](#workfront-fusion-does-not-store-your-files)

### You do not need an [!DNL Adobe] account 

Because [!DNL Workfront Fusion] is part of the [!DNL Adobe] product suite, you don't need a separate [!DNL Adobe] account to use these tools. Each tool accesses [!DNL Adobe] PDF functionality without using a connection.

Although [!DNL Workfront Fusion] does not require an [!DNL Adobe] account to use the PDF Services, the modules do require a connection. There are no credentials involved in this connection, and you provide only a name for the connection itself.

### [!DNL Workfront Fusion] does not store your files 

-->

The [!DNL Adobe PDF Services] ファイルの読み取り、変換、変更はできますが、どちらもできません [!DNL Adobe] nor [!DNL Workfront Fusion] ファイルまたはデータを保存します。 つまり、

* ファイルのセキュリティを含め、ファイルの制御を維持する
* 必要ない [!UICONTROL Adobe] ストレージまたはクラウドストレージアカウントを使用して、PDFサービスを使用します。

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

## 前提条件

OAuth サーバー間 API を作成するには、Adobe開発者コンソールにAdobe PDF Services API を追加する必要があります。 API を追加する場合は、「 OAuth Server-to-Server 」オプションを選択します。

手順については、 [OAuth を使用してプロジェクトに API を追加](https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/) Adobe開発者向けドキュメント。

## への接続の作成 [!DNL Adobe PDF Services]

の接続を作成するには、以下を実行します。 [!DNL Adobe PDF Services] モジュール：

1. 任意の [!DNL Adobe PDF Services] モジュール、クリック **[!UICONTROL 追加]** 「接続」ボックスの横に表示されます。

1. 次のフィールドに入力します。

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL 接続タイプ ]</td>
          <td>
            <p>サーバー間接続と JWT 接続のどちらを作成するかを選択します。</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL 接続名 ]</td>
          <td>
            <p>この接続の名前を入力します。</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL クライアント ID]</td>
          <td>を入力します。 [!DNL Adobe] [!UICONTROL クライアント ID]。 これは、 [!DNL Adobe Developer Console].<p>資格情報の検索方法については、 <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >資格情報</a> (Adobe開発者向けドキュメント )。</p></td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL クライアント秘密鍵 ]</td>
          <td>を入力します。 [!DNL Adobe] [!UICONTROL クライアント秘密鍵 ]。 これは、 [!DNL Adobe Developer Console].<p>資格情報の検索方法については、 <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >資格情報</a> (Adobe開発者向けドキュメント )。</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL テクニカルアカウント ID] （JWT のみ）</td>
          <td>を入力します。 [!DNL Adobe] [!UICONTROL テクニカルアカウント ID]。 これは、 [!DNL Adobe Developer Console].<p>資格情報の検索方法については、 <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >資格情報</a> (Adobe開発者向けドキュメント )。</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL 組織 ID] （JWT のみ）</td>
          <td>を入力します。 [!DNL Adobe] [!UICONTROL 組織 ID]。 これは、 [!DNL Adobe Developer Console].<p>資格情報の検索方法については、 <a href="https://developer.adobe.com/developer-console/docs/guides/services/services-add-api-oauth/#credentials" class="MCXref xref" >資格情報</a> (Adobe開発者向けドキュメント )。</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL メタスコープ ] （JWT のみ）</td>
          <td>
            接続に必要なメタスコープを入力します。
          </td>
        </tr>
       </tbody>
    </table>
1. クリック **[!UICONTROL 続行]** 接続を保存し、モジュールに戻ります。


## [!DNL Adobe PDF Services] モジュールとそのフィールド

設定時に [!DNL PDF Services], [!DNL Workfront Fusion] に、以下のフィールドを示します。 これらに加えて、アプリやサービスでのアクセスレベルなどの要因に応じて、追加のフィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [であるモジュールから別のモジュールに情報をマッピングします。 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL ドキュメントを生成]](#generate-document)
* [[!UICONTROL テキストを抽出/表]](#extract-text--table)
* [[!UICONTROL PDFファイルを結合]](#combine-pdf-files)
* [[!UICONTROL PDFファイルを圧縮]](#compress-pdf-files)
* [[!UICONTROL ドキュメントをPDFファイルに変換]](#convert-document-to-pdf-file)
* [[!UICONTROL HTMLをPDFファイルに変換]](#convert-html-to-pdf-file)
* [[!UICONTROL 画像をPDFファイルに変換]](#convert-image-to-pdf-file)
* [[!UICONTROL PDFを文書に変換]](#convert-pdf-to-document)
* [[!UICONTROL PDFを画像に変換]](#convert-pdf-to-image)
* [[!UICONTROL PDFファイルの線形化]](#linearize-a-pdf-file)
* [[!UICONTROL PDFファイルの OCR]](#ocr-for-pdf-file)
* [[!UICONTROL ページ操作]](#page-manipulation)
* [[!UICONTROL PDFアクセシビリティの自動タグ付け]](#pdf-accessibility-auto-tag)
* [[!UICONTROL PDFファイルのプロパティ]](#pdf-file-properties)
* [[!UICONTROL ProtectPDFファイル]](#protect-pdf-file)
* [[!UICONTROL PDF・ファイルの保護を解除]](#remove-protection-of-a-pdf-file)
* [PDFファイルの分割](#split-a-pdf-file)

### [!UICONTROL ドキュメントを生成]

The [!UICONTROL ドキュメントを生成] モジュールを使用すると、選択したデータを含むPDFを作成するための強力な方法が提供されます。 これを書式設定するには、 [!DNL Microsoft Word] テンプレートを使用するか、JSON 形式でデータを指定します。

詳しくは、 [!UICONTROL [!DNL Adobe PDF Services] ドキュメントを生成] 機能については、 [ドキュメント生成の概要](https://www.adobe.io/apis/documentcloud/dcsdk/docs.html) （内） [!DNL Adobe Document Services] ドキュメント。

* [以下を使用します。 [!UICONTROL ドキュメントを生成] モジュール [!DNL Microsoft Word] テンプレート](#use-the-generate-document-module-with-a-microsoft-word-template)
* [以下を使用します。 [!UICONTROL ドキュメントを生成] JSON を使用したモジュール](#use-the-generate-document-module-with-json)

#### 以下を使用します。 [!UICONTROL ドキュメントを生成] モジュール [!DNL Microsoft Word] テンプレート

<!--
>[!NOTE]
>
>For a discussion of Microsoft Word templates, see [Microsoft Word Template modules](../../workfront-fusion/apps-and-their-modules/microsoft-word-templates-modules.md). 
>
>You do not need to use Microsoft Word template modules to use a Microsoft Word template with the PDF Services Generate document module.
-->

次の手順で [!UICONTROL ドキュメントを生成] モジュール [!UICONTROL Microsoft Word] テンプレートの作成が必要な場合は、まずテンプレートを作成する必要があります。 手順については、 [!DNL Microsoft Office] ドキュメント。

次の項目に入力： [!UICONTROL ドキュメントを生成] モジュールのフィールドを次に示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>このモジュールに使用する接続を選択します。</p> への接続を作成する手順については、 [!DNL Adobe PDF Services]を参照してください。 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >への接続の作成 [!DNL Adobe PDF Services]</a> 」を参照してください。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> <p>このソースファイルは、 [!DNL Microsoft Word ]モジュールが新しいテンプレートの生成に使用するPDF。</p> <p>でプロジェクトを作成することをお勧めします。 [!DNL Workfront] （の） [!DNL Microsoft Word] で使用するテンプレート [!DNL Workfront Fusion]. その後、 [!DNL Workfront] / [!UICONTROL ドキュメントをダウンロード ] モジュールを使用して、適切なテンプレートをシナリオに取り込みます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力形式 ]</td> 
   <td> <p>生成するドキュメントの形式を選択します。</p> 
    <ul> 
     <li> <p>PDF</p> </li> 
     <li> <p>DOCX</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 結合用のデータ ]</td> 
   <td> <p>テキストに置き換えるテンプレートの値タグごとに、次のように入力します。</p> 
    <ul> 
     <li> <p>[!UICONTROL キー ]</p> <p>キーを入力します。 テンプレートでは、キーは値タグに表示されるテキストです。 例えば、値タグにテキストを配置する場合は、 <code>&#123;&#123;name&#125;&#125;</code>，と入力します。 <code>name </code>キーフィールドに入力します。</p> </li> 
     <li> <p>値のタイプ</p> <p>値フィールド内のデータを、値、オブジェクト、またはオブジェクトの配列のどれにするかを選択します。</p> </li> 
     <li> <p>[!UICONTROL 値 ]</p> <p>生成後のドキュメントで、値タグの代わりに表示するテキストを入力またはマッピングします。</p> </li> 
    </ul> <p> <img src="assets/generate-with-template-350x241.png" style="width: 350;height: 241;"> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### 以下を使用します。 [!UICONTROL ドキュメントを生成] JSON を使用したモジュール

次の手順で [!UICONTROL ドキュメントを生成] JSON を使用したモジュールで、次のようにフィールドに入力します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>このモジュールに使用する接続を選択します。</p> への接続を作成する手順については、 [!DNL Adobe PDF Services]を参照してください。 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >への接続の作成 [!DNL Adobe PDF Services]</a> 」を参照してください。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力形式 ]</td> 
   <td> <p>生成するドキュメントの形式を選択します。</p> 
    <ul> 
     <li> <p>PDF</p> </li> 
     <li> <p>DOCX</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 結合用のデータ ]</td> 
   <td> <p>このモジュールで JSON を使用するには、このフィールドでマッピングを有効にする必要があります。</p> <p>ドキュメントを生成する JSON を入力またはマッピングします。 </p> <p>このフィールドに JSON を直接入力するか、JSON モジュールから JSON 出力をマッピングすることができます。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL テキストを抽出/表]

このアクションモジュールを使用すると、データをPDFファイルから抽出できます。 このモジュールは、段落やテーブルの単一のセル内のテキストなど、個々のテキスト要素を出力します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>このモジュールに使用する接続を選択します。</p> への接続を作成する手順については、 [!DNL Adobe PDF Services]を参照してください。 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >への接続の作成 [!DNL Adobe PDF Services]</a> 」を参照してください。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON として抽出する要素 ]</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL テキスト ]</p> </li> 
     <li> <p>[!UICONTROL テーブル ]</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 境界ボックスを抽出しますか？]</td> 
   <td>テキストの境界ボックスに関するデータを抽出するには、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力のスタイル設定情報を含めますか？]</td> 
   <td>出力 JSON にスタイル情報を追加するには、このオプションを有効にします。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDFファイルを結合]

このアクションモジュールは、複数のPDFファイルを取得し、それらを 1 つのPDFファイルに組み合わせます。 例えば、このモジュールは、 [!UICONTROL Workfront] プロジェクトの完了時に、単一のPDFにプロジェクトを追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>このモジュールに使用する接続を選択します。</p> への接続を作成する手順については、 [!DNL Adobe PDF Services]を参照してください。 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >への接続の作成 [!DNL Adobe PDF Services]</a> 」を参照してください。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ドキュメント ]</td> 
   <td> <p>集約モジュールを使用して、文書を収集してPDFに組み合わせることも、手動で文書を追加することもできます。 </p> <p>[!UICONTROL Array Aggregator] モジュールを使用して、以前のモジュールの出力を集計することをお勧めします。 集約を使用すると、ファイルの名前、場所、数を知る必要がなくなります。 したがって、集約を使用すると、結合するドキュメントを手動で入力するよりも、柔軟性と拡張性が高くなります。</p> <p>[!UICONTROLPDFーとファイルを結合 ] モジュールを集約と共に使用するには、「[!UICONTROL ドキュメント ]」フィールドでマッピングを有効にする必要があります。 </p> <p>この例では、[!UICONTROL 関連レコードの読み取り ] モジュールはプロジェクトに関連付けられたドキュメントを識別し、[!UICONTROL ドキュメントのダウンロード ] モジュールは各ドキュメントをダウンロードします。 すべてのPDFーは配列に集計され、[!UICONTROLPDFーを結合 ] ファイルモジュールに渡されます。</p> <p> <img src="assets/combine-example-350x104.png" style="width: 350;height: 104;"> </p> <p>手動でドキュメントを入力することもできます。</p> <p>結合PDFに含めるドキュメントごとに、次の手順を実行します。</p> 
    <ol> 
     <li value="1"> <p>「[!UICONTROL ドキュメントを追加 ]」をクリックします。</p> </li> 
     <li value="2"> <p>「[!UICONTROL ソースファイル ]」フィールドで、含めるドキュメントを出力するモジュールを選択するか、ソースファイルの名前とデータをマッピングします。 </p> </li> 
     <li value="3"> <p>（オプション）ソースファイルの特定のページのみを含める場合は、追加するページ範囲ごとに、 <strong>[!UICONTROL 項目を追加 ]</strong> 「[!UICONTROL ページ ]」フィールドに、含めるページ範囲の最初と最後のページを入力し、 <strong>[!UICONTROL 追加 ]</strong>. 1 つのドキュメントから複数のページ範囲を含めることができます。</p> </li> 
     <li value="4"> <p>クリック <strong>[!UICONTROL 追加 ]</strong>. </p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDFファイルを圧縮]

このアクションモジュールは、PDFファイルを取得し、圧縮します。 これは、帯域幅やメモリの節約に役立ちます。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>このモジュールに使用する接続を選択します。</p> への接続を作成する手順については、 [!DNL Adobe PDF Services]を参照してください。 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >への接続の作成 [!DNL Adobe PDF Services]</a> 」を参照してください。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> <p>ソースファイルはPDF形式です。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 圧縮レベル ]</td> 
   <td>使用する圧縮レベルを選択します。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL ドキュメントをPDFファイルに変換]

このツールは、ドキュメントをPDFファイルに変換します。 ソースファイルは、次のいずれかのドキュメント形式である必要があります。

* DOC
* XLS
* PPT
* TXT
* RTF

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>このモジュールに使用する接続を選択します。</p> への接続を作成する手順については、 [!DNL Adobe PDF Services]を参照してください。 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >への接続の作成 [!DNL Adobe PDF Services]</a> 」を参照してください。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> <p>ソースファイルは、次のいずれかの形式で指定する必要があります。</p> 
    <ul> 
     <li> <p>DOC</p> </li> 
     <li> <p>XLS</p> </li> 
     <li> <p>PPT</p> </li> 
     <li> <p>TXT</p> </li> 
     <li> <p>RTF</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 言語 ]</td> 
   <td> <p>ソースドキュメントのデフォルト言語を選択します。 これにより、ソースファイルにフォントが含まれていない場合、モジュールは適切なフォントを選択できます。</p> <p>次の言語から選択します。</p> 
    <ul> 
     <li> <p>en-US（デフォルト）：英語（米国）</p> </li> 
     <li> <p>ca-ES：カタロニア語（スペイン）</p> </li> 
     <li> <p>cs-CZ：チェコ語（チェコ共和国）</p> </li> 
     <li> <p>da-DK：デンマーク語（デンマーク）</p> </li> 
     <li> <p>de-DE：ドイツ語（ドイツ）</p> </li> 
     <li> <p>en-AE：英語（アラブ首長国連邦）</p> </li> 
     <li> <p>en-GB：英語（英国）</p> </li> 
     <li> <p>en-IL：英語（イスラエル）</p> </li> 
     <li> <p>en-US：英語（米国）</p> </li> 
     <li> <p>es-ES：スペイン語（スペイン）</p> </li> 
     <li> <p>es-MX：スペイン語（メキシコ）</p> </li> 
     <li> <p>eu-ES：バスク語（スペイン）</p> </li> 
     <li> <p>fi-FI：フィンランド語（フィンランド）</p> </li> 
     <li> <p>fr-CA：フランス語（カナダ）</p> </li> 
     <li> <p>fr-FR：フランス語（フランス）</p> </li> 
     <li> <p>fr-MA：フランス語（モロッコ）</p> </li> 
     <li> <p>hr-HR：クロアチア語（クロアチア）</p> </li> 
     <li> <p>hu-HU：ハンガリー語（ハンガリー）</p> </li> 
     <li> <p>it-IT：イタリア語（イタリア）</p> </li> 
     <li> <p>ja-JP：日本語（日本）</p> </li> 
     <li> <p>kr-KR：韓国語（韓国）</p> </li> 
     <li> <p>nb-NO：ノルウェー語（ブークモール）（ノルウェー）</p> </li> 
     <li> <p>nl-NL：オランダ語（オランダ）</p> </li> 
     <li> <p>pl-PL：ポーランド語（ポーランド）</p> </li> 
     <li> <p>pt-BR：ポルトガル語（ブラジル）</p> </li> 
     <li> <p>pt-PT：ポルトガル語（ポルトガル）</p> </li> 
     <li> <p>ro-RO：ルーマニア語（ルーマニア）</p> </li> 
     <li> <p>ru-RU：ロシア語（ロシア）</p> </li> 
     <li> <p>sk-SK：スロバキア語（スロバキア）</p> </li> 
     <li> <p>sl-SI：スロベニア語（スロベニア）</p> </li> 
     <li> <p>sv-SE：スウェーデン語（スウェーデン）</p> </li> 
     <li> <p>tr-TR：トルコ語（トルコ）</p> </li> 
     <li> <p>uk-UA：ウクライナ語（ウクライナ）</p> </li> 
     <li> <p>zh-CN：中国語（中国本土）</p> </li> 
     <li> <p>zh-TW：中国語（台湾）</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL HTMLをPDFファイルに変換]

このツールは、HTMLファイルを変換ファイルにPDFします。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>このモジュールに使用する接続を選択します。</p> への接続を作成する手順については、 [!DNL Adobe PDF Services]を参照してください。 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >への接続の作成 [!DNL Adobe PDF Services]</a> 」を参照してください。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> <p>重要：ソースファイルはHTML形式または ZIP 形式である必要があります。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON]</td> 
   <td> <p>HTMLが JavaScript 変数を参照する場合、ここにこれらの変数を含めることができます。 </p> <p>各変数で、 <strong>[!UICONTROL 項目を追加 ]</strong> 変数のキーと値を含めます。</p> <p>メモ:   
     <ul> 
      <li> <p>ZIP ファイルからPDFを作成する場合、ソース販促物には次のようなスクリプト要素を含める必要があります。 <code> &lt;script src='./json.js' type='text/javascript'&gt;&lt;/script&gt;</code> </p> </li> 
      <li> <p>URL からPDFを作成する場合、ページがレンダリングされる前に、この JSON オブジェクトのコンテンツがブラウザー VM に挿入されます。 </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ヘッダーおよびフッターを含める ]</td> 
   <td> <p>このオプションを有効にすると、ヘッダードキュメントのヘッダーとPDFが作成されます。</p> 
    <ul> 
     <li> <p>ヘッダーには、日付とドキュメントタイトルが含まれます。</p> </li> 
     <li> <p>フッターには、ファイル名とページ番号が含まれます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ページの幅 ]</td> 
   <td>用紙の幅をインチ単位で入力します。 モジュールは、この情報を使用して、作成したモジュールファイル内のページのPDFを設定します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ページの高さ ]</td> 
   <td>用紙の高さをインチ単位で入力します。 モジュールは、この情報を使用して、作成したモジュールファイル内のページのPDFを設定します。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL 画像をPDFファイルに変換]

このツールは、画像を画像ファイルにPDFします。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>このモジュールに使用する接続を選択します。</p> への接続を作成する手順については、 [!DNL Adobe PDF Services]を参照してください。 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >への接続の作成 [!DNL Adobe PDF Services]</a> 」を参照してください。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とイメージファイルをマップします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDFを文書に変換]

このツールは、PDFファイルをドキュメントに変換します。 出力ファイルには、次のいずれかの形式を選択できます。

* DOC
* DOCX
* PPTX
* XLSX
* RTF

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>このモジュールに使用する接続を選択します。</p> への接続を作成する手順については、 [!DNL Adobe PDF Services]を参照してください。 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >への接続の作成 [!DNL Adobe PDF Services]</a> 」を参照してください。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> <p>ソースファイルはPDF形式です。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力ファイル形式 ]</td> 
   <td> <p>ファイルを出力する形式を次の中から選択します。</p> 
    <ul> 
     <li> <p>DOC</p> </li> 
     <li> <p>DOCX</p> </li> 
     <li> <p>PPTX</p> </li> 
     <li> <p>XLSX</p> </li> 
     <li> <p>RTF</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDFを画像に変換]

このツールは、PDFを PNG またはJPEG形式の画像に変換し、ZIP として出力します。 PDFは 1 ページにつき 1 つの画像に変換され、各画像の末尾がページ番号になります。 その後、画像ファイルが ZIP ファイルに結合されます。

例えば、8 ページの「TestFile」という名前のファイルでは、「TestFile_1」から「TestFile_8」までの 8 つの画像が生成されます。 このモジュールの出力は、8 つの画像を含む ZIP ファイルです。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>このモジュールに使用する接続を選択します。</p> への接続を作成する手順については、 [!DNL Adobe PDF Services]を参照してください。 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >への接続の作成 [!DNL Adobe PDF Services]</a> 」を参照してください。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> <p>ソースファイルはPDF形式です。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力ファイル形式 ]</td> 
   <td> <p>ファイルを出力する形式を次の中から選択します。</p> 
    <ul> 
     <li>PNG</li> 
     <li>JPEG</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDFファイルの線形化]

このツールは、PDFドキュメントを線形化して、Web に最適化されたPDFドキュメントを作成します。 線形化PDFドキュメントは、ドキュメント全体をダウンロードする必要なく、ページごとに表示できます。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>このモジュールに使用する接続を選択します。</p> への接続を作成する手順については、 [!DNL Adobe PDF Services]を参照してください。 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >への接続の作成 [!DNL Adobe PDF Services]</a> 」を参照してください。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDFファイルの OCR]

このツールは、ファイルに対して光学式文字認識 (OCR) を実行し、PDFを生成します。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>このモジュールに使用する接続を選択します。</p> への接続を作成する手順については、 [!DNL Adobe PDF Services]を参照してください。 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >への接続の作成 [!DNL Adobe PDF Services]</a> 」を参照してください。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL OCR タイプ ]</td> 
   <td> 
    <ul> 
     <li> <p>[!UICONTROL 元の画像を変更 ] タイプの場合は、テキストを検索および選択できますが、クリーンアッププロセス中に元の画像が変更されてから（例えば、デスケッドして）、その上に非表示のテキストレイヤーが配置されます。 このタイプを使用すると、不要なアーティファクトが削除され、場合によっては読みやすいドキュメントになることがあります。 </p> </li> 
     <li> <p>[!UICONTROL 元の画像が変更されていない場合 ] タイプでは、検索可能なテキストレイヤーが元の画像の上にオーバーレイされますが、この場合、元の画像は変更されません。 このタイプを選択すると、元の画像に対する最大の忠実度が生成されます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 言語 ]</td> 
   <td>このドキュメントの言語を選択します。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL ページ操作]

このモジュールを使用すると、選択したページドキュメント内のページをPDFまたは削除できます。 例えば、縦長表示を横長表示に変更したり、特定のページをPDF文書から削除したりできます。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>このモジュールに使用する接続を選択します。</p> への接続を作成する手順については、 [!DNL Adobe PDF Services]を参照してください。 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >への接続の作成 [!DNL Adobe PDF Services]</a> 」を参照してください。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アクション ]</td> 
   <td> <p>ファイルに対して実行するアクションを選択します。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL 削除 ]</b> </p> <p>ドキュメントからページを削除するには、このオプションを選択します。</p> </li> 
     <li> <p><b>[!UICONTROL 回転 ]</b> </p> <p>ページを回転させ、開始方向を基準にドキュメントページを回転させる角度を時計回りの角度で入力します。</p> <p>ページを縦から横に、またはその逆に回転するには、ページを 90 度または 270 度回転します。</p> <p>ページが上下逆の場合は、180 度回転させます。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ページ ]</td> 
   <td> <p>削除する各ページ範囲で、 <strong>[!UICONTROL 追加 ]</strong> 次に、ページ範囲の最初と最後のページを入力します。 </p> <p>メモ:   
     <ul> 
      <li> <p>負の数を使用して、ドキュメントの最後から戻すことができます。 ドキュメントの最後のページは —1、最後のページの 2 番目は —2 と続きます。</p> </li> 
      <li> <p>単一のページを削除するには、範囲の開始と終了の両方に同じページ番号を設定します。</p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが操作するレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDFアクセシビリティの自動タグ付け]

このアクションモジュールは、アクセシビリティの使用PDF用にタグ付けされたタグを作成します。 また、問題の一覧を示し、修正を提案するオプションのMicrosoft Excel レポートも作成します。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>このモジュールに使用する接続を選択します。</p> への接続を作成する手順については、 [!DNL Adobe PDF Services]を参照してください。 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >への接続の作成 [!DNL Adobe PDF Services]</a> 」を参照してください。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Shift 見出し ]</td> 
   <td> <p>文書の見出しを移動するには、このオプションを有効にします。</p> 
    <ul> 
     <li> <p><b>[!UICONTROL レポートの生成 ]</b> </p> <p>このオプションを有効にすると、PDFのアクセシビリティの問題とその場所を示すレポートが生成され、これらの問題の修正方法に関する提案が表示されます。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDFファイルのプロパティ]

このツールは、次のようなドキュメントに関する基本情報を抽出します。

* ページ数
* PDFバージョン
* ファイルが暗号化されているかどうか
* ファイルがライナライズされているかどうか
* ファイルに埋め込みファイルが含まれているかどうか

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>このモジュールに使用する接続を選択します。</p> への接続を作成する手順については、 [!DNL Adobe PDF Services]を参照してください。 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >への接続の作成 [!DNL Adobe PDF Services]</a> 」を参照してください。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL ProtectPDFファイル]

このツールは、ユーザーまたはPDFのパスワードを使用してパスワードドキュメントを保護します。 また、印刷ドキュメント内の印刷、編集、コピーなど、特定の機能に関する制限もPDFします。 暗号化するコンテンツのタイプと暗号化アルゴリズムを選択します。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>このモジュールに使用する接続を選択します。</p> への接続を作成する手順については、 [!DNL Adobe PDF Services]を参照してください。 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >への接続の作成 [!DNL Adobe PDF Services]</a> 」を参照してください。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> <p>ソースファイルはPDF形式です。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL パスワード保護の種類 ]</td> 
   <td> <p>パスワードを使用して入力パスワードドキュメントを暗号化する場合は、このPDFを有効にします。 このオプションを有効にする場合、次のいずれかまたは両方の値を指定して入力する必要があります。 </p> 
    <ul> 
     <li> <p>[!UICONTROL userPassword]</p> </li> 
     <li> <p>[!UICONTROL ownerPassword] </p> </li> 
    </ul> <p>各パスワードは最大 128 文字までです。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 暗号化アルゴリズム ]</td> 
   <td> <p>暗号化アルゴリズムを選択します。 </p> 
    <ul> 
     <li> <p>[!UICONTROL AES-128 暗号化 ]</p> <p>パスワードは LATIN-I 文字のみをサポートします。 </p> </li> 
     <li> <p>[!UICONTROL AES-256 暗号化 ]</p> <p>パスワードは Unicode 文字セットをサポートしています</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 暗号化するコンテンツ ]</td> 
   <td> <p>暗号化するコンテンツのタイプを選択します。</p> 
    <ul> 
     <li> <p>[!UICONTROL すべてのコンテンツ ]</p> </li> 
     <li> <p>[!UICONTROL メタデータを除くすべてのコンテンツ ]</p> </li> 
     <li> <p>[!UICONTROL 埋め込みデータのみ ] </p> </li> 
    </ul> <p>「[!UICONTROL 埋め込みデータのみ ]」を選択すると、指定されたアクセス権限が無効になります。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 権限 ]</td> 
   <td> <p>印刷、編集、コンテンツのコピーを許可する権限を選択します。</p> <p>権限設定は、[!UICONTROL OwnerPassword] が [!UICONTROL Password Protection Type] フィールドに設定されている場合にのみ使用されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDF・ファイルの保護を解除]

このツールは、パスワードドキュメントからセキュリティ (PDF保護 ) を削除します。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>このモジュールに使用する接続を選択します。</p> への接続を作成する手順については、 [!DNL Adobe PDF Services]を参照してください。 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >への接続の作成 [!DNL Adobe PDF Services]</a> 」を参照してください。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> <p>ソースファイルはPDF形式です。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL パスワード ]</td> 
   <td>現在ファイルを保護しているパスワードを入力します。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL PDFファイルの分割]

このアクションモジュールは、PDFドキュメントを複数の小さなドキュメントに分割します。 ファイル数、ファイルあたりのページ数、またはページ範囲で分割するかどうかを指定します。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>このモジュールに使用する接続を選択します。</p> への接続を作成する手順については、 [!DNL Adobe PDF Services]を参照してください。 <a href="#create-a-connection-to-adobe-pdf-services" class="MCXref xref" >への接続の作成 [!DNL Adobe PDF Services]</a> 」を参照してください。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> <p>ソースファイルはPDF形式です。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 分割オプション ]</td> 
   <td>ファイルの分割方法を選択します。 
   <ul>
   <li><p><b>ページ範囲</b></p><p>別のドキュメントに分割する各ページ範囲で、 <b>追加</b> をクリックし、開始するページと終了するページを入力します。</p></li>
   <li><p><b>ページ数</b></p><p>新規ドキュメントに含めるページ数を入力します。</p></li>
   <li><p><b>ファイル数</b></p><p>ドキュメントを分割する均等サイズのファイルの数を入力します。</p></li>
   </ul>
   </td> 
  </tr> 
 </tbody> 
</table>

