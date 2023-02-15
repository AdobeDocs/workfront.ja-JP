---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: XML
description: XML アプリを使用すると、XML &gt；を介して XML 形式のテキストを解析できます。XML モジュールを解析し、バンドルに変換して、他のモジュールでデータを使用できるようにします。 XML &gt；を使用して、バンドルを XML 形式のテキストに変換することもできます。XML モジュールを作成
author: Becky
feature: Workfront Fusion
exl-id: 3459e930-8156-4171-8920-34f4e07bc530
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '1405'
ht-degree: 1%

---

# XML

この [!UICONTROL XML] XML 形式のテキストを [!UICONTROL XML] > [!UICONTROL XML を解析] モジュールを作成し、他のモジュールでデータを使用できるようにバンドルに変換します。 また、 [!UICONTROL XML] > [!UICONTROL XML を作成] モジュール

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>  </td>  
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL XML を解析]

この [!UICONTROL XML] > [!UICONTROL XML を解析] モジュールは、XML 形式のテキストを解析し、XML から抽出されたすべての情報を含む単一のバンドルを出力します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL データ構造 ]</p> </td> 
   <td> <p>データ構造は、XML の構造を記述し、以下のモジュールのマッピングパネルでモジュールの出力を使用できるようにします。</p> <p>解析する XML のサンプルがある場合は、それを使用してデータ構造を生成できます。</p> 
    <ol> 
     <li value="1">次をクリック： <strong>[!UICONTROL 追加 ]</strong> 」ボタンをクリックします。</li> 
     <li value="2">次をクリック： <strong>[!UICONTROL Generator]</strong> 」ボタンをクリックします。</li> 
     <li value="3">XML サンプルを <strong>[!UICONTROL サンプルデータ ]</strong> フィールドに入力します。</li> 
     <li value="4">クリック <strong>[!UICONTROL 保存 ]</strong>.</li> 
     <li value="5">データ構造が正常に生成されたことを確認します。</li> 
     <li value="6"> <p>次をクリック： <strong>[!UICONTROL 保存 ]</strong> ボタンをクリックして、データ構造を保存します。</p> <p>手順 2 ～ 5 をスキップして、空のデータ構造を指定できます。 データ構造が空の場合、モジュールが少なくとも 1 回実行されるまで、モジュールの出力はマッピングパネルで使用できません。</p> </li> 
    </ol> <p>詳しくは、 <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">のデータ構造 [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 数値をテキストとして保持 ]</td> 
   <td>数値をテキスト（文字列）値として保持するには、このオプションを有効にします。 それ以外の場合、数値は数値にキャストされます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL XML]</p> </td> 
   <td> <p>解析する XML 形式のテキストを入力またはマップします。</p> <p>数式を使用する場合、結果の値のタイプが [!UICONTROL Text] データ型である（または自動的に強制的に適用される）ことを確認します。 </p> <p> <img src="assets/if-you-use-a-formula-350x164.png" style="width: 350;height: 164;"> </p> <p>結果の値の型が [!UICONTROL Buffer] （バイナリデータ）の場合、 <code>toString()</code> 関数を使用して、Text データ型に変換します。 詳しくは、 <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">強制入力 [!DNL Adobe Workfront Fusion]</a> および <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">[!UICONTROL Adobe Workfront Fusion] の項目データタイプ</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**例：** URL から XML ファイルをダウンロードしてその内容を解析するには：
>
>1. 新しいシナリオを作成します。
>1. 挿入 [!UICONTROL HTTP] > [!UICONTROL ファイルの取得] モジュール
>1. モジュールの設定を開き、次のように設定します。

>
>   **URL**:XML ファイルの URL ( 例： `https://siftrss.com/f/rqLy05ayMBJ`)
>
>   ![](assets/url-of-xml-file-350x184.png)
>
>1. クリック **[!UICONTROL OK]**&#x200B;をクリ&#x200B;ックし、モジュールの設定を保存して閉じます。
>1. 追加 [!UICONTROL XML] > [!UICONTROL XML を解析] モジュール、次の後に接続 [!UICONTROL HTTP] > [!UICONTROL ファイルの取得] をモジュール化し、次のように設定します。
><table style="table-layout:auto"> 
>    <col> 
>    <col> 
>    <tbody> 
>     <tr> 
>      <td role="rowheader">[!UICONTROL データ構造 ]</td> 
>      <td> 
>       <ol> 
>        <li value="1">次をクリック： <strong>[!UICONTROL 追加 ]</strong> 」ボタンをクリックします。</li> 
>        <li value="2">次をクリック： <strong>[!UICONTROL Generator]</strong> 」ボタンをクリックします。</li> 
>        <li value="3">Web ブラウザーで、新しいタブまたはウィンドウを開きます。</li> 
>        <li value="4">3 番目の手順で使用した URL をアドレスバーに入れ、XML ファイルを取得します。</li> 
>        <li value="5">すべての XML テキストを選択し、クリップボードにコピーします。</li> 
>        <li value="6">タブまたはウィンドウを閉じて、シナリオに戻ります。</li> 
>        <li value="7">コピーした XML テキストを「サンプルデータ」フィールドに貼り付けます。</li> 
>        <li value="8">クリック <strong>[!UICONTROL 保存 ]</strong>.</li> 
>        <li value="9">データ構造が正常に生成されたことを確認します。</li> 
>        <li value="10">クリック <strong>[!UICONTROL 保存 ]</strong> をクリックして、データ構造を保存します。</li> 
>       </ol> <p>手順 2 ～ 9 をスキップして、空のデータ構造を指定できます。 データ構造が空の場合、モジュールが少なくとも 1 回実行されるまで、モジュールの出力はマッピングパネルで使用できません。</p> </td> 
>     </tr> 
>     <tr> 
>      <td role="rowheader">[!UICONTROL XML]</td> 
>      <td> <p>を <code>Data </code>[!UICONTROL HTTP] / [!UICONTROL ファイルを取得 ] モジュールの出力からフィールドにアイテムを入力します。 以下を使用： <code>toString()</code> 関数を使用して、値を [!UICONTROL Buffer] （バイナリデータ）型から [!UICONTROL Text] 型に変換します。</p> <p>数式のコードをコピーして、フィールドに貼り付けることができます。 <code>&#123;&#123;toString(1.data)&#125;&#125;</code></p> <p>Buffer データ型と Text データ型の詳細については、 <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Adobe Workfront Fusion の項目データ型</a>.</p> <p> <img src="assets/paste-formula-code-350x99.png" style="width: 350;height: 99;"> </p> </td> 
>     </tr> 
>    </tbody> 
>   </table>


## [!UICONTROL XML 属性の解析]

デフォルトでは、 [!UICONTROL XML] > [!UICONTROL XML を解析] モジュールは、属性を特別なコレクションに格納します。 `_attributes` を、これらの属性を持つノードの子として追加します。 ノードがテキストノードで、そのノードに属性が含まれている場合、次の 2 つの特別なプロパティが追加されます。 `_attributes` 属性と `_value` ノードのテキストコンテンツ用。

>[!INFO]
**例：** この XML は次のようになります。

```
<root attr="1">
<node attr="ABC">Hello, World</node>
</root>
```

は次のバンドルに変換されます。

![](assets/xml-converted-to-bundle.png)

## XML を作成

この [!UICONTROL XML] > [!UICONTROL XML を作成] モジュールは、バンドルを XML 形式のテキストに変換します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL データ構造 ]</p> </td> 
   <td> <p>データ構造は、結果の XML の構造を記述します。 作成する XML のサンプルがある場合は、それを使用してデータ構造を生成できます。</p> 
    <ol> 
     <li value="1">次をクリック： <strong>[!UICONTROL 追加 ]</strong> 」ボタンをクリックします。</li> 
     <li value="2">次をクリック： <strong>[!UICONTROL Generator]</strong> 」ボタンをクリックします。</li> 
     <li value="3">XML サンプルをコピーして、「サンプルデータ」フィールドに貼り付けます。</li> 
     <li value="4">次をクリック： <strong>[!UICONTROL 保存 ]</strong> 」ボタンをクリックします。</li> 
     <li value="5">データ構造が正常に生成されたことを確認します。</li> 
     <li value="6">クリック <strong>[!UICONTROL 保存 ]</strong> をクリックして、データ構造を保存します。</li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ルート要素名 ]</td> 
   <td>XML のルート要素の名前を入力します。 デフォルト値は <code>root</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Doctype SYSTEM ID]</td> 
   <td>使用するファイル名を<code> !DOCTYPE SYSTEM</code> 宣言</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Doctype PUBLIC ID]</td> 
   <td>使用するファイル名を<code> !DOCTYPE PUBLIC</code> 宣言</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Xml 宣言を削除 ]</td> 
   <td>XML 宣言を削除するには、このオプションを有効にします <code>&lt;?xml ... ?&gt;</code> および <code>&lt;!DOCTYPE ... &gt;</code>XML のルート要素とその内容のみを残します。</td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
> 
>**例:**
> 
>一般的な使用例は、 [!DNL Google] > スプレッドシートを XML に変換します。
>1. を [!DNL Google Sheets] > [!UICONTROL 行を選択] モジュールを使用してデータを取得します。 から行を取得するモジュールを設定します。 [!DNL Google] スプレッドシート。 を設定しま&#x200B;す。**[!UICONTROL 返される行の最大数]** を小さい数に設定しますが、テスト用に 1 より大きい値（例：3）に設定します。 を実行します。 [!DNL Google Sheets] モジュールを右クリックし、「**[!UICONTROL このモジュールのみを実行]**.&quot; モジュールの出力を確認します。
>1. 接続 [!UICONTROL 配列集約] モジュールの後 [!DNL Google Sheets] モジュール。 モジュールの設定で、 [!DNL Google Sheets] モジュール **[!UICONTROL ソースノード]** フィールドに入力します。 その他のフィールドは、現時点ではそのままにしておきます。
>1. 接続 [!UICONTROL XML] > [!UICONTROL XML を作成] モジュールの後 [!UICONTROL 配列集約] モジュール。
>   モジュールの設定には、XML 出力の構造を記述したデータ構造が必要です。 次をクリック： **[!UICONTROL 追加]** ボタンをクリックして、データ構造の設定を開きます。 このデータ構造を作成する最も簡単な方法は、XML サンプルから自動的に生成することです。
>1. 次をクリック： **[!UICONTROL ジェネレーター]** ボタンをクリックし、XML サンプルを [!UICONTROL サンプルデータ] フィールド：
>
>   ![](assets/sample-data-field-350x146.png)
>
>1. 「**[!UICONTROL 保存]**」をクリックします。これで、データ構造の「仕様」フィールドに、生成された構造が含まれます。
>1. データ構造の名前をより具体的なものに変更し、「 **[!UICONTROL 保存]**. ルート配列属性に対応するフィールドは、JSON モジュールの設定で、マッピング可能なフィールドとして表示されます。
>1. 次をクリック： **[!UICONTROL マップ]** ボタンをクリックし、 `Array[]` 項目 [!UICONTROL 配列の集約] 出力先：
>1. クリック **[!UICONTROL OK]** をクリックして、XML モジュールの設定を閉じます。
>1. の設定を開きます。 [!UICONTROL 配列集約] モジュール。 を **[!UICONTROL ターゲット構造]** 親 XML 要素に対応するカスタムから XML モジュールのフィールド。 [!DNL Google Sheets] を適切なフィールドに追加します。
>1. クリック **[!UICONTROL OK]** をクリックして、配列集約モジュールの設定を閉じます。
>1. シナリオを実行します。
>
>   XML モジュールは、正しい XML ファイルを出力します。
>
>1. の設定を開きます。 [!DNL Google Sheets] モジュールを追加し、 [!UICONTROL 返される行の最大数] すべてのデータを処理するには、スプレッドシートの行数より大きい数を指定します。
>
>   結果の XML はに保存できます。 [!DNL Dropbox]、電子メールで送信、FTP 経由でサーバーにアップロードなど。


## XML 属性の追加

複雑なノード（他のノードを含むノード）にアトリビュートを追加する場合は、という名前のコレクションを追加する必要があります。 `_attributes` カスタムデータ構造内の複雑なメモ用。 このコレクションはノード属性にマッピングされます。 属性をテキストノードに追加する場合 ( 例： `<node attr="1">abc</node>`) の場合は、コレクションを追加する必要があります `_attributes` 属性とテキストプロパティの場合 `_value` カスタムデータ構造内のこのノードのノード値。

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

## トラブルシューティング：からデータをマッピングできません [!UICONTROL XML を解析] モジュール

データ構造が正しく定義されていることを確認します。 または、空のデータ構造を使用し、モジュールを少なくとも 1 回実行して XML 入力を処理することもできます。
