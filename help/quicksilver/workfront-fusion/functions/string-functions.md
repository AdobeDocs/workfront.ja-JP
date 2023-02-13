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
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 3%

---

# の文字列関数 [!DNL Adobe Workfront Fusion]

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p><p>[!UICONTROL [!DNL Workfront Fusion] 自動化 (WA)</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL ascii (text; [読み分けを取り除く])]

テキスト文字列から非 ascii 文字をすべて削除します。

>[!INFO]
>
>**例:**
>
>* `ascii(` `Wěošrčkřfžrýoáníté` `)`
   >
   >   戻り値： [!DNL Workfront]
>
>* `ascii(` `ěščřž` `;` `true` `)`
   >
   >   戻り値： [!UICONTROL escrz]


## [!UICONTROL base64 （テキスト）]

テキストを base64 に変換します。

>[!INFO]
>
>**例:**
>
>`base64( workfront )`
>
>戻り値：d29ya2Zyb250==

## [!UICONTROL 大文字（テキスト）]

文字列の最初の文字を大文字に変換します。

>[!INFO]
>
>**例:**
>
>`capitalize( workfront )`
>
>戻り値： [!DNL Workfront]

## contains (text;検索文字列 )

テキストに検索文字列が含まれているかどうかを検証します。

>[!INFO]
>
>**例:**
>
>* `contains( Hello World ; Hello )`
   >
   >   戻り値： [!UICONTROL true]
>
>* `contains( Hello World ; Bye )`
   >
   >   戻り値： [!UICONTROL false]


## [!UICONTROL decodeURL （テキスト）]

URL 内の特殊文字をテキストにデコードします。

>[!INFO]
>
>**例:**
>`decodeURL( Automate%20your%20workflow )`
>
>戻り値： [!UICONTROL ワークフローの自動化]

## [!UICONTROL encodeURL （テキスト）]

一部のテキストの特殊文字を有効な URL アドレスにエンコードします。

## [!UICONTROL escapeHTML （テキスト）]

テキスト内のすべてのHTMLタグをエスケープします。

>[!INFO]
>
>**例:**
>
>`escapeHTML( <b>Hello</b> )`
>
> 戻り値： `&lt;b&gt;Hello&lt;/b&gt;`

## [!UICONTROL escapeMarkdown(text)]

テキスト内のすべての Markdown タグをエスケープします。

>[!INFO]
>
>**例:**
>
>`escapeMarkdown( # Header )`
>
>戻り値： `&#35; Header`

## [!DNL indexOf (string; value; [start])]

文字列内で指定された値が最初に現れる位置を返します。 検索対象の値がない場合、このメソッドは「 —1」を返します。 開始値は、文字列内で検索を開始する位置を示します。

>[!INFO]
>
>**例:**
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


## [!UICONTROL length （テキストまたはバッファ）]

テキスト文字列の長さ（文字数）またはバイナリバッファ（バイト単位のバッファサイズ）を返します。

>[!INFO]
>
>**例:**
>
>`length( hello )`
>
>戻り値：5

## [!UICONTROL lower (text)]

文字列内のすべてのアルファベット文字を小文字に変換します。

>[!INFO]
>
>**例:**
>
>`lower( Hello )`
>
>戻り値：こんにちは

## [!UICONTROL md5 （テキスト）]

文字列の md5 ハッシュを計算します。

>[!INFO]
>
>**例:**
>
>`md5( Workfront )`
>
>戻り値： `1448bbbeaa7a9b8091d426999f1f666b`

## [!UICONTROL replace (text;search string;;置換文字列 )]

検索文字列を新しい文字列に置き換えます。

>[!INFO]
>
>**例:**
>
>`replace( Hello World ; Hello ; Hi )`
>
>戻り値： [!UICONTROL こんにちは]

正規表現 ( `/.../`) はフラグの組み合わせ ( `g`, `i`, `m`) を追加しました。

>[!INFO]
>
>**例:**
>
>![](assets/replace---1-350x31.png)
>
>これらの数値 X X X X はすべて X に置き換えられます

置換文字列には、次の特殊な置換パターンを含めることができます。

* `$&` 一致した部分文字列を挿入します。
* `$n` n は 100 未満の正の整数で、括弧内の n 番目のサブマッチ文字列を挿入します。 これは 1 つのインデックスです。

>[!INFO]
>
>**例:**
>
>![](assets/variable-value-350x63.png)
>
>戻り値：電話番号 `+420777111222`
>>![](assets/variable-value---2-350x55.png)
>戻り値：電話番号： `+420777111222`

>[!CAUTION]
次のような名前付きキャプチャグループを使用しない `/ is (?<number>\d+)/` 置き換える文字列引数内。 その場合、エラーが発生します。

正規表現について詳しくは、 [テキストパーサー](../../workfront-fusion/apps-and-their-modules/text-parser.md).

## [!UICONTROL sha1 (text; [エンコード]; [key])]

文字列の sha1 ハッシュを計算します。 key 引数が指定されている場合は、sha1 HMAC ハッシュが代わりに返されます。 サポートされるエンコード：&quot;hex&quot; （デフォルト）、&quot;base64&quot;または&quot;latin1&quot;

>[!INFO]
**例:**
`sha1( workfront )`
戻り値：b2b30b8ae1f9e5b40fbb0696eaabdbfd8d0c087f

## [!UICONTROL sha256 (text; [エンコード]; [key])]

文字列の sha256 ハッシュを計算します。 key 引数が指定されている場合は、sha256 HMAC ハッシュが代わりに返されます。 サポートされるエンコード：&quot;hex&quot; （デフォルト）、&quot;base64&quot;または&quot;latin1&quot;。>

>[!INFO]
**例:**
`sha256( workfront )`
戻り値：ed3d7397eec7b94453035b67ba4468c883ee3bedeb57137f7371f2e0cf5e2bbc

## [!UICONTROL sha512 (text; [出力エンコーディング]; [key]; [キーエンコード])]

文字列の sha512 ハッシュを計算します。 key 引数が指定されている場合は、sha512 HMAC ハッシュが代わりに返されます。

サポートされるエンコード：

* &quot;[!UICONTROL hex]&quot; （デフォルト）
* &quot;[!UICONTROL base64]&quot;
* &quot;[!UICONTROL latin1]&quot;

サポートされるキーエンコーディング：

* &quot;[!UICONTROL テキスト]&quot; （デフォルト）
* &quot;[!UICONTROL hex]&quot;
* &quot;[!UICONTROL base64]&quot;または&quot;[!UICONTROL バイナリ]&quot;

「[!UICONTROL バイナリ]」キーのエンコード。キーは、文字列ではなく、バッファである必要があります。

>[!INFO]
**例:**
`sha512(workfront)`
戻り値：789ae41b9456357e4f27c6a09956a767abbb8d80b206003ffdd1e94dbc687cd119b85e19db58bb44b234493af35fd431639c0345aadf2cf7ec26e9f4a7fb19

## [!UICONTROL split (text;区切り文字 )]

文字列を部分文字列に分割して、文字列を文字列の配列に分割します。

>[!INFO]
**例:**
`split( John, George, Paul ; , )`

## [!UICONTROL startcase （テキスト）]

すべての単語の最初の文字を大文字にし、その他すべての文字を小文字にします。

>[!INFO]
**例：**
`startcase( hello WORLD )`
戻り値： [!UICONTROL Hello World]

## [!UICONTROL stripHTML（テキスト）]

テキストからすべてのHTMLタグを削除します。

>[!INFO]
**例:**
`stripHTML( <b>Hello</b> )`
戻り値：こんにちは

## [!UICONTROL substring (text;開始；終了 )]

「開始」位置と「終了」位置の間のテキスト文字列の一部を返します。

>[!INFO]
**例:**
* `substring( Hello ; 0 ; 3)`

   戻り値：ヘル
* `substring( Hello ; 1 ; 3 )`

   戻り値：el


## [!UICONTROL toBinary（値）]

任意の値をバイナリデータに変換します。

2 番目の引数としてエンコードを指定し、16 進数または base64 からバイナリデータにバイナリ変換を適用することもできます。

>[!INFO]
**例:**
* `toBinary( Workfront )`

   戻り値：57 6f 72 6b 66 72 6f 6e 74
* `toBinary( V29ya2Zyb250 ; base64 )`

   戻り値：57 6f 72 6b 66 72 6f 6e 74


## [!UICONTROL toString （値）]

任意の値を文字列に変換します。

## [!UICONTROL トリミング（テキスト）]

テキストの先頭または末尾の空白文字を削除します。

## [!UICONTROL upper （テキスト）]

文字列内のすべてのアルファベット文字を大文字に変換します。

>[!INFO]
**例:**
`upper( Hello )`
戻り値： [!UICONTROL こんにちは]
