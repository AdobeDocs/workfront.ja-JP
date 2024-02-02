---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion の文字列関数
description: Adobe Workfront Fusion マッピングパネルでは、次の文字列関数を使用できます。
author: Becky
feature: Workfront Fusion
exl-id: c6676a87-2498-4de8-b877-7edc30aeabae
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '774'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] の文字列関数

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンスは必要ありません。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランの場合、この記事で説明する機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明する機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## [!UICONTROL ASCII（テキスト; [ダイアクリティカルマークを削除]）]

テキスト文字列から非 ASCII 文字をすべて削除します。

>[!INFO]
>
>**例：**
>
>* `ascii(` `Wěošrčkřfžrýoáníté` `)`
>
>   戻り値：[!DNL Workfront]
>
>* `ascii(` `ěščřž` `;` `true` `)`
>
>   戻り値：[!UICONTROL escrz]

## [!UICONTROL base64（text）]

テキストを base64 に変換します。

>[!INFO]
>
>**例：**
>
>`base64( workfront )`
>
>戻り値：d29ya2Zyb250==

## [!UICONTROL 大文字（テキスト）]

テキスト文字列の最初の文字を大文字に変換します。

>[!INFO]
>
>**例：**
>
>`capitalize( workfront )`
>
>戻り値：[!DNL Workfront]

## 次を含む（テキスト;検索文字列）

テキストに検索文字列が含まれているかどうかを検証します。

>[!INFO]
>
>**例：**
>
>* `contains( Hello World ; Hello )`
>
>   戻り値：[!UICONTROL true]
>
>* `contains( Hello World ; Bye )`
>
>   戻り値：[!UICONTROL false]

## [!UICONTROL decodeURL（テキスト）]

URL 内の特殊文字をテキストにデコードします。

>[!INFO]
>
>**例：**
>`decodeURL( Automate%20your%20workflow )`
>
>戻り値：[!UICONTROL ワークフローを自動化]

## [!UICONTROL encodeURL（テキスト）]

一部のテキストの特殊文字を有効な URL アドレスにエンコードします。

## [!UICONTROL escapeHTML（テキスト）]

テキスト内のすべての HTML タグをエスケープします。

>[!INFO]
>
>**例：**
>
>`escapeHTML( <b>Hello</b> )`
>
> 戻り値：`&lt;b&gt;Hello&lt;/b&gt;`

## [!UICONTROL escapeMarkdown（text）]

テキスト内のすべての Markdown タグをエスケープします。

>[!INFO]
>
>**例：**
>
>`escapeMarkdown( # Header )`
>
>戻り値：`&#35; Header`

## [!DNL indexOf (string; value; [start])]

文字列内で指定された値が最初に現れる位置を返します。検索対象の値がない場合、このメソッドは「-1」を返します。開始値は、文字列内で検索を開始する位置を示します。

>[!INFO]
>
>**例：**
>
>* `indexOf( Workfront ; o )`
>
>   戻り値：1
>
>* `indexOf( Workfront ; x )`
>
>   戻り値：-1
>
>* `indexOf( Workfront ; o ; 3 )`
>
>   戻り値：6

## [!UICONTROL 長さ（テキストまたはバッファー）]

テキスト文字列の長さ（文字数）またはバイナリバッファー（バイト単位のバッファーサイズ）を返します。

>[!INFO]
>
>**例：**
>
>`length( hello )`
>
>戻り値：5

## [!UICONTROL 小文字（テキスト）]

文字列内のすべてのアルファベット文字を小文字に変換します。

>[!INFO]
>
>**例：**
>
>`lower( Hello )`
>
>戻り値：hello

## [!UICONTROL md5（テキスト）]

文字列の md5 ハッシュを計算します。

>[!INFO]
>
>**例：**
>
>`md5( Workfront )`
>
>戻り値：`1448bbbeaa7a9b8091d426999f1f666b`

## [!UICONTROL 置換（テキスト、検索文字列、置換文字列）]

検索文字列を新しい文字列に置き換えます。

>[!INFO]
>
>**例：**
>
>`replace( Hello World ; Hello ; Hi )`
>
>戻り値：[!UICONTROL Hi World]

（`/.../` で囲まれた）正規表現は、フラグの組み合わせ（`g`、`i`、`m` など）と共に検索文字列として使用できます。

>[!INFO]
>
>**例：**
>
>![](assets/replace---1-350x31.png)
>
>これらの数値 X X X X はすべて X に置き換えられます

置換文字列には、次の特殊な置換パターンを含めることができます。

* `$&` は、一致する部分文字列を挿入します。
* `$n` は、n が 100 未満の正の整数で、括弧内の n 番目のサブマッチ文字列を挿入します。これは 1 つのインデックスです。

>[!INFO]
>
>**例：**
>
>![](assets/variable-value-350x63.png)
>
>戻り値：電話番号 `+420777111222`
>>
>![](assets/variable-value---2-350x55.png)
>
>戻り値：電話番号：`+420777111222`

>[!CAUTION]
>
>置き換える文字列引数内で、`/ is (?<number>\d+)/` のような名前付きキャプチャグループを使用しないでください。その場合、エラーが発生します。

正規表現について詳しくは、[テキストパーサー](../../workfront-fusion/apps-and-their-modules/text-parser.md)を参照してください。

## [!UICONTROL sha1（テキスト、[エンコード]、[キー]）]

文字列の sha1 ハッシュを計算します。キー引数が指定されている場合は、sha1 HMAC ハッシュが代わりに返されます。サポートされるエンコーディング：「hex」（デフォルト）、「base64」または「latin1」。

>[!INFO]
>
>**例：**
>
>`sha1( workfront )`
>
>戻り値：b2b30b8ae1f9e5b40fbb0696eaabdbfd8d0c087f

## [!UICONTROL sha256（テキスト、[エンコード]、[キー]）]

文字列の sha256 ハッシュを計算します。キー引数が指定されている場合は、sha256 HMAC ハッシュが代わりに返されます。サポートされるエンコーディング：「hex」（デフォルト）、「base64」または「latin1」。>

>[!INFO]
>
>**例：**
>
>`sha256( workfront )`
>
>戻り値：ed3d7397eec7b94453035b67ba4468c883ee3bedeb57137f7371f2e0cf5e2bbc

## [!UICONTROL sha512（テキスト、[出力エンコーディング]、[キー]、[キーエンコード]）]

文字列の sha512 ハッシュを計算します。キー引数が指定されている場合は、sha512 HMAC ハッシュが代わりに返されます。

サポートされるエンコード：

* 「[!UICONTROL hex]」（デフォルト）
* &quot;[!UICONTROL base64]&quot;
* &quot;[!UICONTROL latin1]&quot;

サポートされるキーエンコーディングは次のとおりです。

* 「[!UICONTROL テキスト]」（デフォルト）
* 「[!UICONTROL hex]」
* 「[!UICONTROL base64]」または「[!UICONTROL バイナリ]」

「[!UICONTROL バイナリ]」キーエンコーディングを使用する場合、キーは文字列ではなく、バッファーである必要があります。

>[!INFO]
>
>**例：**
>
>`sha512(workfront)`
>
>戻り値：789ae41b9456357e4f27c6a09956a767abbb8d80b206003ffdd1e94dbc687cd119b85e1e19db58bb44b234493af35fd431639c0345aadf2cf7ec26e9f4a7fb19

## [!UICONTROL split (text; separator)]

文字列を部分文字列の配列に分割します。

>[!INFO]
>
>**例：**
>
>`split( John, George, Paul ; , )`

## [!UICONTROL startcase (text)]

すべての単語の最初の文字を大文字にし、その他すべての文字を小文字にします。

>[!INFO]
>
>**例：**
>`startcase( hello WORLD )`
>
>戻り値：[!UICONTROL Hello World]

## [!UICONTROL stripHTML (text)]

テキストからすべての HTML タグを削除します。

>[!INFO]
>
>**例：**
>
>`stripHTML( <b>Hello</b> )`
>
>戻り値：Hello

## [!UICONTROL substring (text; start;end)]

テキスト文字列（text）の「start」位置と「end」位置の間の部分を返します。

>[!INFO]
>
>**例：**
>
>* `substring( Hello ; 0 ; 3)`
>
>   戻り値：Hel
>
>* `substring( Hello ; 1 ; 3 )`
>
>   戻り値：el

## [!UICONTROL toBinary (value)]

任意の値をバイナリデータに変換します。

2 番目の引数としてエンコードを指定し、16 進数または Base64 からバイナリデータにバイナリ変換を適用することもできます。

>[!INFO]
>
>**例：**
>
>* `toBinary( Workfront )`
>
>   戻り値：57 6f 72 6b 66 72 6f 6e 74
>
>* `toBinary( V29ya2Zyb250 ; base64 )`
>
>   戻り値：57 6f 72 6b 66 72 6f 6e 74

## [!UICONTROL toString (value)]

任意の値を文字列に変換します。

## [!UICONTROL trim (text)]

テキストの先頭または末尾の空白文字を削除します。

## [!UICONTROL upper (text)]

テキスト文字列内のすべてのアルファベット文字を大文字に変換します。

>[!INFO]
>
>**例：**
>
>`upper( Hello )`
>
>戻り値：[!UICONTROL HELLO]
