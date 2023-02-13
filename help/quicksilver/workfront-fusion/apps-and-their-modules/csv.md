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
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---

# CSV

この [!DNL Adobe Workfront Fusion] [!UICONTROL CSV] モジュールを使用すると、CSV ファイルを作成し、受け取ったテキスト値やファイルから CSV テキストを解析できます。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>  <p>[!UICONTROL [!DNL Workfront Fusion] 自動化 (WA)</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL CSV を作成]

この [!UICONTROL CSV を作成] 集約機能を使用すると、受け取ったテキスト値から csv テキストを作成できます。

集約について詳しくは、 [の集約モジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL ソースモジュール ]</td>
        <td>必要なフィールドの集計に使用するモジュールを選択します。</td>
    </tr>
    <tr>
        <td>[!UICONTROL 集計フィールド ]</td>
        <td>集計するフィールドを、使用可能なフィールドのリストから選択します。</td>
    </tr>
    <tr>
        <td>[!UICONTROL 最初の行にヘッダーを含める ]</td>
        <td>結果にヘッダーを含める場合は、このオプションを選択します。</td>
    </tr>
    <tr>
        <td>[!UICONTROL Group by]</td>
        <td>結果をグループ化するフィルターを入力します。 例えば、日付を入力します。</td>
    </tr>
    <tr>
        <td>[!UICONTROL 空の集計後に処理を停止 ]</td>
        <td>結果がない場合にシナリオを停止するには、このオプションを選択します。</td>
    </tr>
</table>

## [!UICONTROL CSV を作成（詳細）]

この [!UICONTROL CSV を作成（詳細）] 集約機能を使用すると、受け取ったテキスト値から CSV テキストを作成できます。 結果の CSV ファイルで CSV 列を定義するデータ構造を使用しています。 定義が完了すると、列は CSV モジュール設定のフィールドとして表示され、シナリオの後のモジュールにマッピングできます。

集約について詳しくは、 [の集約モジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースモジュール ]</td> 
   <td>必要なフィールドを集計するために使用するアプリモジュールを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL データ構造 ]</td> 
   <td> <p>必要な方法でフィールドを集計するデータ構造を選択します。 データ構造を定義した後、項目を対応するフィールドにマッピングできます。</p> <p>詳しくは、 <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">のデータ構造 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 最初の行にヘッダーを含める ] </td> 
   <td>結果にヘッダーを含める場合は、このオプションを選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group by] </td> 
   <td>結果をグループ化するフィルターを入力します。 例えば、日付を入力します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 空の集計後に処理を停止 ] </td> 
   <td>結果がない場合にシナリオを停止するには、このオプションを選択します。 </td> 
  </tr> 
 </tbody> 
</table>


<p>Googleの連絡先を、「姓名」と「電子メール」の 2 つの列を持つ CSV ファイルに書き出すとします。 [!UICONTROL Google Contacts] &gt;[!UICONTROL グループから連絡先を取得 ] モジュールの出力バンドルは、次の構造を持ちます。 電子メールアドレスは、 <code>[!UICONTROL Emails[]]</code> item（コレクションの配列）。各コレクションには 2 つの項目が含まれます。 <code>Label</code> および <code>Email</code>.</p>
<p> <img src="assets/transforming-350x546.png" style="width: 350;height: 546;"> </p>
<p>もし、単純な [!DNL Create CSV] モジュールの場合、バンドルの最上位項目に対応するチェックボックスのリストが提供されます。 目盛りを付けようとした場合 <code>Full name</code> および <code>Emails</code> [!UICONTROL CSV を作成 ] モジュールの項目は、次の出力を生成します。これは、おそらく望ましくないものです。</p>
<p>"emails","fullName"</p>
<p>"[object Object]","Shon Winer"</p>
<p>"[object Object]","Lizeth Fulmore"</p>
<p>"[object Object]","Hilario Gullatt"</p>
<p>"[object Object]","Abby Eisenbarth"</p>
<p>項目以降 <code>Full Name</code> は単純型の Text で、正常に書き出されます。 しかし項目は <code>Emails</code>（複雑な型のコレクションの配列）は、[object Object] として書き出されます。これは、コレクションと配列がデフォルトでテキストに変換される方法です。 詳しくは、 <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Adobe Workfront Fusion の項目データ型</a>.</p>
<p>のコンテンツを書き出すには <code>Email </code>最初のコレクションの項目 <code>Emails[]</code> 配列の代わりに、 [!UICONTROL CSV 作成（詳細）] モジュールを使用する必要があります。 このモジュールを使用すると、CSV ファイルの個々の列を定義し、ネストされた列を含む項目をそれらの列にマッピングできます。</p>
<ol>
<li value="1">シナリオに [!UICONTROL CSV を作成（詳細）] モジュールを挿入し、その設定を開きます。</li>
<li value="2">次をクリック： <strong>[!UICONTROL 追加 ]</strong> ボタンをクリックして、[!UICONTROL Data structure] フィールドの横に新しいデータ構造を作成します。</li>
<li value="3"> <p>データ構造の名前を入力し、 <strong>[!UICONTROL 項目を追加 ]</strong> ボタンをクリックして、個々の列を追加します。 2 つの列をエクスポートする場合：「Full Name」と「Email」の場合、生成されるデータ構造は次のようになります。</p> <p> <img src="assets/google-contacts-350x524.png" style="width: 350;height: 524;"> </p> </li>
<li value="4"> <p>データ構造の定義が完了すると、各列に対応するフィールドが [!UICONTROL CSV を作成（詳細）] モジュールの設定に表示され、項目をマッピングできるようになります。 最初の項目を <code>[!UICONTROL Emails[]]</code> 配列とその項目のマッピング <code>Email </code>を「電子メール」フィールドまたは列に追加します。</p> <p> <img src="assets/create-csv-advanced-350x308.png" style="width: 350;height: 308;"> </p> </li>
<li value="5"> <p>シナリオを実行します。 項目以降 <code>Emails[1]: Email</code> 「Email」列にマッピングされたテキストは、単純なタイプで、現在は正しく書き出されます。</p> <p>"氏名","メール"</p> <p>"Shon Winer","Shon@Winer.com"</p> <p>"Lizeth Fulmore","Lizeth@Fulmore.com"</p> <p>"Hilario Gullatt","Hilario@Gullatt.com"</p> <p>"Abby Eisenbarth","Abby@Eisenbarth.com"</p> </li>
</ol>
</div>

## [!UICONTROL CSV を解析]

この [!UICONTROL CSV を解析] 変換サービスを使用すると、受け取ったテキスト値またはファイルから CSV テキストを解析できます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 列数 ]</td> 
   <td>CSV ファイルの列数を指定します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV にヘッダーが含まれています ]</td> 
   <td> <p>CSV テキストの最初の行にヘッダーが含まれている場合は、このオプションを選択します。</p> <p>注意：モジュールでは、これらのヘッダーを使用して出力内の列にラベルを付けません。 代わりに、このフィールドを使用して、ヘッダーが出力データに含まれないようにします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL delimiterType]</td> 
   <td> <p>CSV ファイルの区切り文字を選択します。 区切り文字は、区切られた値またはフィールド間の境界を示すテキスト文字です。</p> 
    <ul> 
     <li>[!UICONTROL コンマ ]</li> 
     <li>[!UICONTROL タブ ]</li> 
     <li> <p>[!UICONTROL Other]</p> <p>「[!UICONTROL その他 ]」を選択した場合は、CSV ファイルで値を区切るために使用する区切り文字を入力します。 1 文字だけを入力する必要があります。<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 引用符なしフィールド内で引用符を保持 ]</td> 
   <td>引用符を保持するには、このオプションを有効にします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV]</td> 
   <td>解析する CSV ファイルを入力またはマッピングします。<p>メモ: <p>データがバイナリ形式（通常はファイルから）で送信される場合は、「toString()」関数を使用してバイナリデータを [!UICONTROL String] に変換する必要があります。</p><p><img src="assets/parse-csv-350x123.png" style="width: 350;height: 123;"></p></p></td> 
  </tr> 
 </tbody> 
</table>
