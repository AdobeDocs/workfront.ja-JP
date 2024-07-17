---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: XML
description: XML アプリを使用すると、XML／Parse XML モジュールを介して XML 形式のテキストを解析し、バンドルに変換して、他のモジュールでデータの使用が可能になります。XML／Create XML モジュールを使用して、バンドルを XML 形式のテキストに変換することもできます。
author: Becky
feature: Workfront Fusion
exl-id: 3459e930-8156-4171-8920-34f4e07bc530
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1457'
ht-degree: 100%

---

# XML

[!UICONTROL XML] アプリを使用すると、[!UICONTROL XML]／[!UICONTROL Parse XML] モジュールを介して XML 形式のテキストを解析し、それをバンドルに変換して、他のモジュールでデータの使用が可能になります。[!UICONTROL XML]／[!UICONTROL Create XML] モジュールを使用して、バンドルを XML 形式のテキストに変換することもできます。

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

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## [!UICONTROL XML を解析]

[!UICONTROL XML]／[!UICONTROL Parse XML] モジュールは、XML 形式のテキストを解析し、XML から抽出されたすべての情報を含む単一のバンドルを出力します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Data structure]</p> </td> 
   <td> <p>データ構造は、XML の構造を記述し、以下のモジュールのマッピングパネルでモジュールの出力を使用できるようにします。</p> <p>解析する XML のサンプルがある場合は、それを使用してデータ構造を生成できます。</p> 
    <ol> 
     <li value="1">「<strong>[!UICONTROL Add]</strong> 」ボタンをクリックします。</li> 
     <li value="2">「<strong>[!UICONTROL Generator]</strong>」ボタンをクリックします。</li> 
     <li value="3">XML サンプルを「<strong>[!UICONTROL Sample data]</strong>」フィールドに入力します。</li> 
     <li value="4">「<strong>[!UICONTROL Save]</strong>」をクリックします。</li> 
     <li value="5">データ構造が正常に生成されたことを確認します。</li> 
     <li value="6"> <p>「<strong>[!UICONTROL Save]</strong>」ボタンをクリックして、データ構造を保存します。</p> <p>手順 2～5 をスキップして、空のデータ構造を指定できます。データ構造が空の場合、モジュールが少なくとも 1 回実行されるまで、モジュールの出力はマッピングパネルで使用できません。</p> </li> 
    </ol> <p>詳しくは、<a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> のデータ構造を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Preserve numbers as text]</td> 
   <td>数値をテキスト（文字列）値として保持するには、このオプションを有効にします。それ以外の場合、数値は数値にキャストされます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL XML]</p> </td> 
   <td> <p>解析する XML 形式のテキストを入力またはマップします。</p> <p>数式を使用する場合、結果の値のタイプが [!UICONTROL Text] データ型である（または自動的に強制的に適用される）ことを確認します。 </p> <p> <img src="assets/if-you-use-a-formula-350x164.png" style="width: 350;height: 164;"> </p> <p>結果の値の型が [!UICONTROL Buffer] （バイナリデータ）の場合、 <code>toString()</code> 関数を使用して、テキストデータ型に変換します。詳しくは、<a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> での型強制および <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">[!UICONTROL Adobe Workfront Fusion] の項目データ型</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**例：** URL から XML ファイルをダウンロードしてその内容を解析するには：
>
>1. 新しいシナリオを開始します。
>1. [!UICONTROL HTTP]／[!UICONTROL ファイルを取得]モジュールを挿入します。
>1. モジュールの設定を開き、次のように設定します。
>
>   **URL**：XML ファイルの URL（例：`https://siftrss.com/f/rqLy05ayMBJ`）
>
>   ![](assets/url-of-xml-file-350x184.png)
>
>1. 「**[!UICONTROL OK]**」をクリックして、モジュールの設定を保存してモジュールを閉じます。
1. [!UICONTROL XML]／[!UICONTROL XML を解析]モジュールを追加して、[!UICONTROL HTTP]／[!UICONTROL ファイルを取得]モジュールの後に接続し、次のように設定します。
>
<table style="table-layout:auto"> 
&gt;    <col> 
&gt;    <col> 
&gt;    <tbody> 
&gt;     <tr> 
&gt;      <td role="rowheader">[!UICONTROL Data structure]</td> 
&gt;      <td> 
&gt;       <ol> 
&gt;        <li value="1">「<strong>[!UICONTROL Add]</strong>」ボタンをクリックします。</li> 
&gt;        <li value="2">「<strong>[!UICONTROL Generator]</strong>」ボタンをクリックします。</li> 
&gt;        <li value="3">Web ブラウザーで、新しいタブまたはウィンドウを開きます。</li> 
&gt;        <li value="4">3 番目の手順で使用した URL をアドレスバーに入れ、XML ファイルを取得します。</li> 
&gt;        <li value="5">すべての XML テキストを選択し、クリップボードにコピーします。</li> 
&gt;        <li value="6">タブまたはウィンドウを閉じて、シナリオに戻ります。</li> 
&gt;        <li value="7">コピーした XML テキストを「サンプルデータ」フィールドに貼り付けます。</li> 
&gt;        <li value="8">「<strong>[!UICONTROL Save]</strong>」をクリックします。</li> 
&gt;        <li value="9">データ構造が正常に生成されたことを確認します。</li> 
&gt;        <li value="10">「<strong>[!UICONTROL Save]</strong>」をクリックして、データ構造を保存します。</li> 
&gt;       </ol> <p>手順 2～9 をスキップして、空のデータ構造を指定できます。データ構造が空の場合、モジュールが少なくとも 1 回実行されるまで、モジュールの出力はマッピングパネルで使用できません。</p> </td> 
&gt;     </tr> 
&gt;     <tr> 
&gt;      <td role="rowheader">[!UICONTROL XML]</td> 
&gt;      <td> <p>[!UICONTROL HTTP]／[!UICONTROL Get a file] モジュールの出力からの <code>Data </code> 項目をフィールドにマップします。<code>toString()</code> 関数を使用して、値を [!UICONTROL Buffer]（バイナリデータ）型から [!UICONTROL Text] 型に変換します。</p> <p>数式のコードをコピーして、フィールドに貼り付けることができます。 <code>&#123;&#123;toString(1.data)&#125;&#125;</code></p> <p>バッファーデータ型とテキストデータ型の詳細については、<a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Adobe Workfront Fusion の項目データ型</a>を参照してください。</p> <p> <img src="assets/paste-formula-code-350x99.png" style="width: 350;height: 99;"> </p> </td> 
&gt;     </tr> 
&gt;    </tbody> 
&gt;   </table>

## [!UICONTROL XML 属性の解析]

デフォルトでは、[!UICONTROL XML]／[!UICONTROL XML を解析]モジュールは、属性をこれらの属性を持つノードの子として特別なコレクション `_attributes` に配置します。ノードがテキストノードで、そのノードに属性が含まれている場合、属性の `_attributes` とノードのテキストコンテンツの `_value` の 2 つの特別なプロパティが追加されます。

>[!INFO]
>
**例：**&#x200B;この XML：

```
<root attr="1">
<node attr="ABC">Hello, World</node>
</root>
```

は次のバンドルに変換されます。

![](assets/xml-converted-to-bundle.png)

## XML を作成

[!UICONTROL XML]／[!UICONTROL XML を作成]モジュールは、バンドルを XML 形式のテキストに変換します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Data structure]</p> </td> 
   <td> <p>データ構造は、結果の XML の構造を記述します。作成する XML のサンプルがある場合は、それを使用してデータ構造を生成できます。</p> 
    <ol> 
     <li value="1">「<strong>[!UICONTROL Add]</strong> 」ボタンをクリックします。</li> 
     <li value="2">「<strong>[!UICONTROL Generator]</strong>」ボタンをクリックします。</li> 
     <li value="3">XML サンプルをコピーして、「サンプルデータ」フィールドに貼り付けます。</li> 
     <li value="4">「<strong>[!UICONTROL Save]</strong>」ボタンをクリックします。</li> 
     <li value="5">データ構造が正常に生成されたことを確認します。</li> 
     <li value="6">「<strong>[!UICONTROL Save]</strong>」をクリックして、データ構造を保存します。</li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Root element name]</td> 
   <td>XML のルート要素の名前を入力します。デフォルト値は <code>root</code> です。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Doctype SYSTEM ID]</td> 
   <td><code> !DOCTYPE SYSTEM</code> 宣言で使用するファイル名を入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Doctype PUBLIC ID]</td> 
   <td><code> !DOCTYPE PUBLIC</code> 宣言で使用するファイル名を入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Strip Xml Declaration]</td> 
   <td>XML 宣言 <code>&lt;?xml ... ?&gt;</code> と <code>&lt;!DOCTYPE ... &gt;</code> を削除し、XML ルート要素とその内容だけを残すには、このオプションを有効にします。</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
**例：**
>
一般的なユースケースは、[!DNL Google] スプレッドシートを XML に変換することです。
>
1. [!DNL Google Sheets]／[!UICONTROL 行を選択]モジュールを使用してデータを取得します。[!DNL Google] スプレッドシートから行を取得するモジュールを設定します。「**[!UICONTROL 返される行の最大数]**」を小さい数に設定しますが、テスト用に 1 より大きい値（例：3）に設定します。[!DNL Google Sheets] モジュールを右クリックし、「**[!UICONTROL このモジュールのみを実行]**」を選択して実行します。モジュールの出力を確認します。
1. [!DNL Google Sheets] モジュールの後に、[!UICONTROL 配列アグリゲーター]モジュールを接続します。モジュール設定で、「**[!UICONTROL ソースノード]**」フィールドから [!DNL Google Sheets] モジュール を選択します。その他のフィールドは、現時点ではそのままにしておきます。
1. [!UICONTROL Array Aggregator] モジュールの後に [!UICONTROL XML]／[!UICONTROL Create XML] モジュールを 接続します。
>
モジュールの設定には、XML 出力の構造を記述したデータ構造が必要です。「**[!UICONTROL 追加]**」ボタンをクリックして、データ構造の設定を開きます。このデータ構造を作成する最も簡単な方法は、XML サンプルから自動的に生成することです。
>
1. 「**[!UICONTROL ジェネレーター]**」ボタンをクリックし、XML サンプルを「[!UICONTROL サンプルデータ]」フィールドに貼り付けます。
>
![](assets/sample-data-field-350x146.png)
>
1. 「**[!UICONTROL 保存]**」をクリックします。これで、データ構造の「仕様」フィールドに、生成された構造が含まれます。
1. データ構造の名前をより具体的なものに変更し、「**[!UICONTROL 保存]**」をクリックします。ルート配列属性に対応するフィールドは、JSON モジュールの設定で、マッピング可能なフィールドとして表示されます。
1. フィールドの横にある「**[!UICONTROL マップ]**」ボタンをクリックし、[!UICONTROL Array aggregator] から出力された `Array[]` 項目をそれにマッピングします。
1. 「**[!UICONTROL OK]**」をクリックして、XML モジュールの設定を閉じます。
1. [!UICONTROL Array Aggregator] モジュールの設定を開きます。**[!UICONTROL ターゲット構造]**&#x200B;をカスタムから、親 XML 要素に対応する XML モジュールのフィールドに変更します。[!DNL Google Sheets] モジュールの項目を適切なフィールドにマッピングします。
1. 「**[!UICONTROL OK]**」をクリックして、Array Aggregator モジュールの設定を閉じます。
1. シナリオを実行します。
>
XML モジュールは、正しい XML ファイルを出力します。
>
1. [!DNL Google Sheets] モジュールの設定を開き、すべてのデータを処理するためのスプレッドシートの行数よりも大きくなるように「[!UICONTROL 返される行の最大数]」の数値を増やします。
>
結果の XML は [!DNL Dropbox] に保存したり、メールで添付ファイルとして送信したり、FTP 経由でサーバーにアップロードしたりできます。

## XML 属性の追加

複雑なノード（他のノードを含むノード）に属性を追加する場合は、カスタムデータ構造内の複雑なメモに対して、`_attributes` という名前のコレクションを追加する必要があります。このコレクションはノード属性にマッピングされます。属性をテキストノードに追加する場合（例：`<node attr="1">abc</node>`）、カスタムデータ構造内のこのノードに、属性のコレクション `_attributes` とノード値のテキストプロパティ `_value` を追加する必要があります。

```
{
   "name": "node",
   "type": "collection",
   "spec": [
      {
         "name": "_attributes",
         "type": "collection"
         "spec": [
            {
               "name": "attr1",
               "type": "text"
            }
         ]
      },
      {
         "name": "_value",
         "type": "text"
      }
   ]
}
```

## トラブルシューティング：[!UICONTROL XML を解析]モジュールからデータをマッピングできません

データ構造が正しく定義されていることを確認します。または、空のデータ構造を使用し、モジュールを少なくとも 1 回実行して XML 入力を処理することもできます。
