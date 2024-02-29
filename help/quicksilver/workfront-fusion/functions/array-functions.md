---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion の配列関数
description: 次の配列関数は、Adobe Workfront Fusion マッピングパネルで使用できます。
author: Becky
feature: Workfront Fusion
exl-id: bf065d00-5d84-47e1-8169-bf9e01e2429d
source-git-commit: 5860e75d0a6521abbe082668749f78058fe7a114
workflow-type: tm+mt
source-wordcount: '679'
ht-degree: 96%

---

# Adobe Workfront Fusion の配列関数

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件は不要。</p>
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

## [!UICONTROL add (array; value1; value2; ...)]

パラメーターで指定された値を配列に追加し、その配列を返します。

## [!UICONTROL contains (array; value)]

配列に値が含まれているかどうかを確認します。

## [!UICONTROL distinct (array; [key])]

配列内の重複を削除します。複雑なオブジェクト内のプロパティにアクセスするには、「[!UICONTROL キー]」引数を使用します。ネストされたプロパティにアクセスするには、ドット表記を使用します。配列内の最初の項目はインデックス 1 です。

>[!INFO]
>
>**例：**`distinct(Contacts[];name)`
>
>「名前」プロパティを比較して、連絡先の配列内の重複を削除します。

## [!UICONTROL flatten (array)]

すべてのサブ配列要素が再帰的に連結された新しい配列を、指定された深さまで作成します。


## [!UICONTROL join (array; separator)]

各項目間に指定された区切り記号を使用して、配列のすべての項目を文字列に連結します。

## [!UICONTROL keys (object)]

指定されたオブジェクトまたは配列のプロパティの配列を返します。

## [!UICONTROL length (array)]

配列内の項目の数を返します。

## [!UICONTROL map (complex array; key;[フィルタリング用キー];[フィルタリングに使用可能な値])]

複素配列の値を含むプリミティブ配列を返します。この関数を使用すると、値をフィルターできます。キーには変数名を使用します。

>[!INFO]
>
>**例：**
>
>* `map(Emails[];email)`
>
>  メールを含むプリミティブ配列を返します
>
>* `map(Emails[];email;label;work;home)`
>
>  職場または自宅に等しいラベルを持つメールのプリミティブ配列を返します。

詳しくは、[[!UICONTROL Adobe Workfront Fusion のモジュール間で情報をマッピング]](../../workfront-fusion/mapping/map-information-between-modules.md)を参照してください。


## [!UICONTROL merge (array1; array2; ...)]

1 つまたは複数の配列を 1 つの配列に結合します。

## [!UICONTROL remove (array; value1; value2; ...)]

配列のパラメーターに指定された値を削除します。この関数は、テキストまたは数値のプリミティブ配列に対してのみ有効です。

## [!UICONTROL reverse (array)]

配列の最初の要素が最後の要素になり、2 番目の要素が最後から 2 番目の要素になります。

## [!UICONTROL slice (array; start; [end])]

選択された項目のみを含む新しい配列を返します。

## [!UICONTROL sort (array; [order]; [key])]

配列の値を並べ替えます。`order` パラメーターの有効な値は次のとおりです。

* `asc`

  （デフォルト）ー 昇順：番号タイプの場合は 1、2、3、...。A、B、C、a、b、c、...テキスト型の場合

* `desc`

  降順：番号型の場合は　...、3、2、1。テキスト型の場合は ...、c、b、a、C、B、A。

* `asc ci`

  大文字と小文字を区別しない昇順：テキスト型の場合は A、a、B、b、C、c、...。

* `desc ci`

  大文字と小文字を区別しない降順：テキスト型の場合は ...、C、c、B、b、A、a。

`key` パラメーターを使用して、複雑なオブジェクト内のプロパティにアクセスします。

キーには変数名を使用します。

ネストされたプロパティにアクセスするには、ドット表記を使用します。

配列内の最初の項目はインデックス 1 です。

>[!INFO]
>
>**例：**
>
>* `sort(Contacts[];name)`
>
>    連絡先の配列を「名前」プロパティによってデフォルトの昇順で並べ替えます。
>
>* `sort(Contacts[];desc;name)`
>
>   連絡先の配列を「名前」プロパティで降順に並べ替えます
>
>* `sort(Contacts[];asc ci;name)`
>
>    連絡先の配列を「名前」プロパティによって大文字と小文字を区別しない昇順で並べ替えます。
>
>* `sort(Emails[];sender.name)`
>
>    メールの配列を「sender.name」プロパティで並べ替えます。

## [!UICONTROL arrayDifference [array1, array2, mode]]

2 つの配列の差を返します。

`mode` パラメーターに次のいずれかの値を入力します。

* `classic`：`array2` に存在しない `array1` のすべての要素を含む新しい配列を返します。

* `symmetric`：両方の配列に共通ではない要素の配列を返します。

  つまり、この関数は、`array2` に存在しない`array1` のすべての要素と、`array1` に存在しない `array2` のすべての要素を含む配列を返します。

  >[!INFO]
  >
  >**例：**
  >
  >次の配列があるとします。
  >
  >```
  >myArray = [1,2,3,4,5]
  >```
  >
  >```
  >yourArray = [3,4,5,6,7]
  >```
  >
  >* `arrayDifference [myArray, yourArray, classic]`
  >
  >    `[1,2]` を返します
  >
  >* `arrayDifference [yourArray, myArray, classic]`
  >
  >    `[6,7]` を返します
  >
  >* `arrayDifference [myArray, yourArray, symmetric]`
  >
  >    `[1,2,6,7]` を返します

## toArray

この関数は、コレクションをキーと値のペアの配列に変換します。

>[!INFO]
>
>**例：**
>
>コレクションが指定された
>
>`{ key1: "value1", key2: "value2:}`
>
>関数
>
>`toArray({ key1: "value1", key2: "value2:})`
>
>キーと値のペアの配列を返します
>
>`[{ key1: "value1"}, { key2: "value2"}]`
