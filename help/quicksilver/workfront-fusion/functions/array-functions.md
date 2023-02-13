---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Adobe Workfront Fusion の配列関数
description: Adobe Workfront Fusion マッピングパネルでは、次の配列関数を使用できます。
author: Becky
feature: Workfront Fusion
exl-id: bf065d00-5d84-47e1-8169-bf9e01e2429d
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '603'
ht-degree: 0%

---

# Adobe Workfront Fusion の配列関数

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

## [!UICONTROL add (array;value1;value2;...)]

パラメータで指定された値を配列に追加し、その配列を返します。

## [!UICONTROL contains (array;値 )]

配列に値が含まれているかどうかを検証します。

## [!UICONTROL distinct ( 配列； [key])]

配列内の重複を削除します。 「[!UICONTROL key]」引数を使用して複雑なオブジェクト内のプロパティにアクセスします。 ネストされたプロパティにアクセスするには、ドット表記を使用します。 配列の最初の項目はインデックス 1 です。

>[!INFO]
>
>**例：** `distinct(Contacts[];name)`
>
>「name」プロパティを比較することで、連絡先の配列内の重複を削除します

## [!UICONTROL flatten（配列）]

指定した深さまで、すべてのサブ配列要素が再帰的に連結された新しい配列を作成します。


## [!UICONTROL join (array;区切り文字 )]

各項目の間に指定した区切り文字を使用して、配列のすべての項目を文字列に連結します。

## [!UICONTROL keys (object)]

指定されたオブジェクトまたは配列のプロパティの配列を返します。

## [!UICONTROL length （配列）]

配列内の項目数を返します。

## [!UICONTROL map ( 複合配列；キー[フィルタリングのためのキー];[フィルタリングに使用可能な値])]

複合配列の値を含むプリミティブ配列を返します。 この関数は、値のフィルタリングを許可します。 キーには生の変数名を使用します。

>[!INFO]
>
>**例:**
>
>* `map(Emails[];email)`
  >
>  E メールを含むプリミティブ配列を返します
>
>* `map(Emails[];email;label;work;home)`
  >
>  仕事またはホームと等しいラベルを持つ E メールを含むプリミティブな配列を返します

詳しくは、 [のモジュール間で情報をマッピングする [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)


## [!UICONTROL merge (array1;array2;...)]

1 つ以上の配列を 1 つの配列に結合します。

## [!UICONTROL remove (array;value1;value2;...)]

配列のパラメーターで指定された値を削除します。 この関数は、テキストまたは数値のプリミティブ配列に対してのみ有効です。

## [!UICONTROL reverse （配列）]

配列の最初の要素が最後の要素になり、2 番目の要素が最後から次の要素になります。

## [!UICONTROL slice (array;開始； [終了])]

選択した項目のみを含む新しい配列を返します。

## [!UICONTROL sort (array; [注文]; [key])]

配列の値を並べ替えます。 有効な `order` パラメーターは次のとおりです。

* `asc`

   （デフォルト） — 昇順：1、2、3、... （タイプ Number）。 A、B、C、a、b、c、... （「テキスト」タイプ）。

* `desc`

   降順：..., 3, 2, 1 （数値タイプ）。..., c, b, a, c, B, A （テキストタイプ）。

* `asc ci`

   大文字と小文字を区別しない昇順A, a, B, b, C, c, c, ... （テキストタイプ）。

* `desc ci`

   大文字と小文字を区別しない降順：..., C, c, B, b, A, a （テキストタイプの場合）

以下を使用： `key` 複雑なオブジェクト内のプロパティにアクセスするためのパラメーター。

キーには生の変数名を使用します。

ネストされたプロパティにアクセスするには、ドット表記を使用します。

配列の最初の項目はインデックス 1 です。

>[!INFO]
>
>**例:**
>
>* `sort(Contacts[];name)`
   >
   >    連絡先の配列を「name」プロパティでデフォルトの昇順に並べ替えます
>
>* `sort(Contacts[];desc;name)`
   >
   >   連絡先の配列を「name」プロパティで降順に並べ替えます
>
>* `sort(Contacts[];asc ci;name)`
   >
   >    大文字と小文字を区別しない昇順で、連絡先の配列を「name」プロパティで並べ替えます
>
>* `sort(Emails[];sender.name)`
   >
   >    「sender.name」プロパティで電子メールの配列を並べ替えます


## [!UICONTROL arrayDifference [array1, array2, mode]]

2 つの配列の違いを返します。

次のいずれかの値を `mode` パラメーター。

* `classic`:のすべての要素を含む新しい配列を返します。 `array1` に存在しない `array2`.

* `symmetric`:両方の配列に共通でない要素の配列を返します。

   つまり、この関数は、 `array1` に存在しない `array2`、および `array2` に存在しない `array1`.

   >[!INFO]
   >
   >**例:**
   >
   >次の配列が考えられます。
   >
   >
   ```
   >myArray = [1,2,3,4,5]
   >```
   >
   >
   ```
   >yourArray = [3,4,5,6,7]
   >```
   >
   >* `arrayDifference [myArray, yourArray, classic]`
      >
      >    戻り値 `[1,2]`
   >
   >* `arrayDifference [yourArray, myArray, classic]`
      >
      >    戻り値 `[6,7]`
   >
   >* `arrayDifference [myArray, yourArray, symmetric]`
      >
      >    戻り値 `[1,2,6,7]`

