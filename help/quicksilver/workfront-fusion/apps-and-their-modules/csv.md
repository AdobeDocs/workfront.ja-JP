---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: CSV
description: Adobe Workfront Fusion CSV モジュールを使用すると、CSV ファイルを作成し、受け取ったテキスト値またはファイルから CSV テキストを解析できます。
author: Becky
feature: Workfront Fusion
exl-id: 4e37482a-e84e-4ab2-a48f-7e7bfbecee56
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '1000'
ht-degree: 100%

---

# CSV

[!DNL Adobe Workfront Fusion] [!UICONTROL CSV] モジュールを使用すると、CSV ファイルを作成し、受け取ったテキスト値やファイルから CSV テキストを解析できます。

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
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]、[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront]プランをご利用の場合、この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明する機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## [!UICONTROL CSV を作成]

[!UICONTROL CSV を作成]アグリゲータを使用すると、受け取ったテキスト値から CSV テキストを作成できます。

アグリゲータについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md) のアグリゲータモジュールを参照してください。

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>必要なフィールドの集計に使用するモジュールを選択します。</td>
    </tr>
    <tr>
        <td>[!UICONTROL Aggregated Fields]</td>
        <td>集計するフィールドを、使用可能なフィールドのリストから選択します。</td>
    </tr>
    <tr>
        <td>[!UICONTROL Include headers in the first row]</td>
        <td>結果にヘッダーを含める場合は、このオプションを選択します。</td>
    </tr>
    <tr>
        <td>[!UICONTROL Group by]</td>
        <td>結果をグループ化するフィルターを入力します。例えば、日付を入力します。</td>
    </tr>
    <tr>
        <td>[!UICONTROL Stop processing after an empty aggregation]</td>
        <td>結果がない場合にシナリオを停止するには、このオプションを選択します。</td>
    </tr>
</table>

## [!UICONTROL CSV を作成（詳細）]

[!UICONTROL CSV を作成（詳細）]アグリゲータを使用すると、受け取ったテキスト値から CSV テキストを作成できます。結果の CSV ファイルで CSV 列を定義するデータ構造を使用しています。定義が完了すると、列は CSV モジュール設定のフィールドとして表示され、シナリオの後のモジュールにマッピングできます。

アグリゲータについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md) のアグリゲータモジュールを参照してください。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td>必要なフィールドを集計するために使用するアプリモジュールを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data Structure]</td> 
   <td> <p>必要な方法でフィールドを集計するデータ構造を選択します。データ構造を定義した後、項目を対応するフィールドにマッピングできます。</p> <p>詳しくは、<a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> のデータ構造を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include headers in the first row] </td> 
   <td>結果にヘッダーを含める場合は、このオプションを選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group by] </td> 
   <td>結果をグループ化するフィルターを入力します。例えば、日付を入力します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stop processing after an empty aggregation] </td> 
   <td>結果がない場合にシナリオを停止するには、このオプションを選択します。 </td> 
  </tr> 
 </tbody> 
</table>


<p>Google の連絡先を、「姓名」と「メール」の 2 つの列を持つ CSV ファイルにエクスポートするとします。[!UICONTROL Google Contacts]／[!UICONTROL Get contacts from a group] モジュールからの出力バンドルは、次の構造を持ちます。メールアドレスは、コレクションの配列である <code>[!UICONTROL Emails[]]</code> 項目内に格納され、各コレクションには <code>Label</code> および <code>Email</code> の 2 つの項目が含まれます。</p>
<p> <img src="assets/transforming-350x546.png" style="width: 350;height: 546;"> </p>
<p>シンプルな [!DNL Create CSV] モジュールを使用する場合、バンドルの最上位項目に対応するチェックボックスのリストが提供されます。<code>Full name</code> 項目および <code>Emails</code> 項目にチェックを付けると、[!UICONTROL Create CSV] モジュールは、次のような望ましくない出力を生成します。</p>
<p>"emails","fullName"</p>
<p>"[object Object]","Shon Winer"</p>
<p>"[object Object]","Lizeth Fulmore"</p>
<p>"[object Object]","Hilario Gullatt"</p>
<p>"[object Object]","Abby Eisenbarth"</p>
<p>項目 <code>Full Name</code> は単純なタイプのテキストであるため、正常にエクスポートされます。しかし項目 <code>Emails</code> は複雑なタイプのコレクションの配列であるため、[object Object] としてエクスポートされます。これは、コレクションと配列がデフォルトでテキストに変換される方法です。詳しくは、<a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Adobe Workfront Fusion の項目のデータ型</a>を参照してください。</p>
<p><code>Emails[]</code> 配列の最初のコレクションの <code>Email </code> 項目のコンテンツをエクスポートするには、[!UICONTROL Create CSV (advanced)] モジュールを使用する必要があります。このモジュールを使用すると、CSV ファイルの個々の列を定義し、ネストされた列を含む項目をそれらの列にマッピングできます。</p>
<ol>
<li value="1">シナリオにモジュール [!UICONTROL Create CSV (advanced)] を挿入し、その設定を開きます。</li>
<li value="2">「[!UICONTROL Data structure]」フィールドの横にある <strong>[!UICONTROL Add]</strong> ボタンをクリックして、新しいデータ構造を作成します。</li>
<li value="3"> <p>データ構造の名前を入力し、<strong>[!UICONTROL Add item]</strong> ボタンをクリックして、個々の列を追加します。「フルネーム」と「メール」の 2 つの列をエクスポートする場合、結果のデータ構造は次のようになります。</p> <p> <img src="assets/google-contacts-350x524.png" style="width: 350;height: 524;"> </p> </li>
<li value="4"> <p>データ構造を正しく定義すると、各列に対応するフィールドが [!UICONTROL Create CSV (advanced)] モジュールの設定に表示され、項目をマッピングできるようになります。<code>[!UICONTROL Emails[]]</code> 配列から最初の項目を取得し、その項目 <code>Email </code> を「メール」フィールド（列）にマッピングします。</p> <p> <img src="assets/create-csv-advanced-350x308.png" style="width: 350;height: 308;"> </p> </li>
<li value="5"> <p>シナリオを実行します。「メール」列にマッピングされた <code>Emails[1]: Email</code> 項目は単純なタイプのテキストであるため、正常にエクスポートされるようになりました。</p> <p>"Full Name","Email"</p> <p>"Shon Winer","Shon@Winer.com"</p> <p>"Lizeth Fulmore","Lizeth@Fulmore.com"</p> <p>"Hilario Gullatt","Hilario@Gullatt.com"</p> <p>"Abby Eisenbarth","Abby@Eisenbarth.com"</p> </li>
</ol>
</div>

## [!UICONTROL CSV の解析]

[!UICONTROL CSV を解析]変換サービスを使用すると、受け取ったテキスト値またはファイルから CSV テキストを解析できます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number of columns]</td> 
   <td>CSV ファイルの列数を指定します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV contains headers]</td> 
   <td> <p>CSV テキストの最初の行がヘッダーの場合は、このオプションを選択します。</p> <p>メモ：このモジュールでは、ヘッダーを使用して出力の列にラベルを付けません。このフィールドは、ヘッダーが出力データに含まれないようにします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL delimiterType]</td> 
   <td> <p>CSV ファイルの区切り文字を選択します。区切り文字は、値の区切りまたはフィールド間の境界を示すテキスト文字です。</p> 
    <ul> 
     <li>[!UICONTROL Comma]</li> 
     <li>[!UICONTROL Tab]</li> 
     <li> <p>[!UICONTROL Other]</p> <p>[!UICONTROL Other] を選択した場合は、値を区切るために CSV ファイルで使用する区切り文字を入力します。正確に 1 文字を入力する必要があります。<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Preserve quotes inside unquoted field]</td> 
   <td>引用符を保持するには、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV]</td> 
   <td>解析する CSV ファイルを入力またはマッピングします。<p>メモ： <p>データが（通常はファイルから）バイナリ形式で取得される場合は、「toString()」関数を使用してバイナリデータを [!UICONTROL String] に変換する必要があります。</p><p><img src="assets/parse-csv-350x123.png" style="width: 350;height: 123;"></p></p></td> 
  </tr> 
 </tbody> 
</table>
