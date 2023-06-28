---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: JSON モジュール
description: Adobe Workfront Fusion JSON アプリは、Adobe Workfront Fusion がデータコンテンツをさらに操作したり新しい JSON コンテンツを作成したりできるように、JSON 形式のデータを処理するモジュールを提供します。
author: Becky
feature: Workfront Fusion
exl-id: 60540608-9d2e-4e10-9fb2-5388dda64784
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1205'
ht-degree: 1%

---

# [!UICONTROL JSON モジュール]

この [!DNL Adobe Workfront Fusion] [!UICONTROL JSON] アプリは、次のように、JSON 形式でデータを処理するためのモジュールを提供します。 [!DNL Adobe Workfront Fusion] では、データコンテンツをさらに操作したり、新しい JSON コンテンツを作成したりできます。

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
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] [!UICONTROL] の [!UICONTROL] [!DNL Workfront Fusion] 自動化 (WA)</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] がある場合 [!DNL Adobe Workfront] プラン（組織で購入する必要がある） [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。 [!DNL Workfront Fusion] は、[!UICONTROL Ultimate] に含まれています [!DNL Workfront] プラン</p>
   <p>または</p>
   <p>従来の製品要件：組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## JSON を解析

* [データ構造](#data-structure)
* [コレクションとアレイ](#collection-vs-array)

### データ構造

データ構造は、JSON データの編成方法を記述し、個々の JSON 項目をシナリオ内の他のモジュールにマッピングできるようにします。 データ構造を指定しない場合、モジュールを手動で実行し、 [!DNL Workfront Fusion] 指定された JSON から構造を構築します。

1. を [!UICONTROL JSON を解析] モジュールをシナリオに追加します。
1. 内 **[!UICONTROL JSON 文字列]** 「 」フィールドで、データ構造を作成する JSON を入力します。
1. 他のモジュールを [!UICONTROL JSON を解析] モジュールを追加しました。 理由： [!DNL Workfront Fusion] はまだ JSON データの構造を把握していないので、 [!UICONTROL JSON を解析] モジュールをシナリオ内の他のモジュールに追加します。
1. シナリオを手動で実行します。 これにより、 [!UICONTROL JSON を解析] モジュールを使用して、指定した JSON から JSON 構造を識別します。
1. 次のモジュールを接続できます。 「 Parse JSON 」モジュールの項目をマッピングに使用できるようになりました。

詳しくは、 [のデータ構造 [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-structures.md).

### コレクションとアレイ

JSON 文字列フィールドにコレクションが含まれている場合 `{ ... }`の場合、出力はコレクションの項目を含む単一のバンドルです。

>[!INFO]
>
>**例:**
>
>```
>{
>       "name" : "Peter",
>
>    
   "ID" : 1
>}
>```
>
>![](assets/json-collection.png)

JSON 文字列フィールドに配列が含まれる場合 `[ ... ]`の場合、出力は一連のバンドルになります。 各バンドルには、配列の 1 つの要素が含まれます。

>[!INFO]
>
>**例:**
>
>```
>[
>   {
>       "name" : "Peter",
>       "ID" : 1
>   },
>
>  
 {
>       "name" : "Mike",
>       "ID" : 2
>   }
>]
>```
>
>![](assets/json-array.png)

## [!UICONTROL JSON] モジュールとそのフィールド

設定時に [!DNL JSON] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、アプリやサービスでのアクセスレベルなどの要因に応じて、追加の JSON フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [JSON に集計](#aggregate-to-json)
* [JSON を XML に変換](#convert-json-to-xml)
* [JSON を解析](#parse-json)
* [JSON を作成](#create-json)
* [JSON を変換](#transform-json)

### [!UICONTROL JSON に集計]

この集約モジュールは、以前のモジュールからの出力を JSON に集計します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースモジュール ] </td> 
   <td> <p>JSON に集計するデータを出力するモジュールを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL データ構造 ]</td> 
   <td> <p>JSON の作成に使用するデータ構造を選択します。 データ構造は、このモジュールで使用できる他のフィールドを決定します。 詳しくは、 <a href="#data-structure" class="MCXref xref">データ構造</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL インデント ]</td> 
   <td> <p> タブ、2 つのスペース、4 つのスペースのどれを使用して JSON のインデントを設定するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group by]</td> 
   <td>集計出力をグループ化する式を定義します。 この式には、1 つ以上のマッピングされた項目を含めることができます。 集計されたデータは、この式の値を使用してグループに分割されます。 各グループは、キー（評価された式）と値（集計テキスト）を持つ個別のバンドルとして出力されます。 キーを後続のモジュールのフィルターとして使用できます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 空の集計後に処理を停止 ]</td> 
   <td>結果がない場合にシナリオを停止するには、このオプションを有効にします。</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL JSON を XML に変換]

このアクションモジュールは、JSON 文字列を XML に変換します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON 文字列 ] </td> 
   <td> <p>XML に変換する JSON を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL JSON を解析]

このアクションモジュールは、JSON 文字列を解析してデータ構造にし、JSON 文字列内のデータにアクセスできるようにします。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL データ構造 ]</td> 
   <td> <p>JSON の作成に使用するデータ構造を選択します。 詳しくは、 <a href="#data-structure" class="MCXref xref">データ構造</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON 文字列 ] </td> 
   <td> <p>解析する JSON を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL JSON を作成]

このアクションモジュールは、データ構造から JSON を作成します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">データ構造</td> 
   <td> <p>JSON の作成に使用するデータ構造を選択します。 詳しくは、 <a href="#data-structure" class="MCXref xref">データ構造</a> 」を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL JSON を変換]

このアクションモジュールは、オブジェクトを json 文字列に変換します。

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL オブジェクト ]</td> 
   <td> <p>JSON に変換するオブジェクトを入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

## データレコードを JSON に変換中

>[!INFO]
>
>**例：** 次の例は、 [!DNL Google Sheets] を JSON 形式に変更します。
>
>1. を [!DNL Google Sheets] > [!UICONTROL 行を選択] モジュールを使用してデータを取得します。 から行を取得するモジュールを設定します。 [!DNL Google] スプレッドシート。 を設定しま&#x200B;す。**[!UICONTROL 返される行の最大数]** を小さい数に設定しますが、テスト用に 1 より大きい値（例：3）に設定します。 を実行します。 [!DNL Google Sheets] モジュールを右クリックし、「**[!UICONTROL このモジュールのみを実行]**.&quot; モジュールの出力を確認します。
>
1. 接続 [!UICONTROL 配列集約] モジュールの後 [!DNL Google Sheets] モジュール。 モジュールの設定で、 [!DNL Google Sheets] モジュール **[!UICONTROL ソースノード]** フィールドに入力します。 その他のフィールドは、現時点ではそのままにしておきます。
>
1. 接続 [!UICONTROL JSON] > [!UICONTROL JSON を作成] モジュールの後 [!UICONTROL 配列集約] モジュール。 モジュールの設定には、JSON 形式を記述したデータ構造が必要です。 クリック **[!UICONTROL 追加]** をクリックして、データ構造の設定を開きます。 このデータ構造を作成する最も簡単な方法は、JSON サンプルから自動的に生成することです。 クリック **[!UICONTROL ジェネレーター]** をクリックし、JSON サンプルを **[!UICONTROL サンプルデータ]** フィールド：
>
**例:**
>   
>```
>{
>
>"books": [
>
>{
>
>"id": "ID",
>
>"title": "Title",
>
>"author": "Author"
>
>}
>
>]
>
>}
>```
>
1. 「**[!UICONTROL 保存]**」をクリックします。この [!UICONTROL 仕様] フィールドのデータ構造に、生成された構造が含まれるようになりました。
1. データ構造の名前をより具体的なものに変更し、「 **[!UICONTROL 保存]**. ルート配列属性に対応するフィールドは、JSON モジュールの設定で、マッピング可能なフィールドとして表示されます。
>
1. 次をクリック： **[!UICONTROL マップ]** ボタンをクリックし、 `Array[]` 項目を配列集約出力から取得します。
>
1. クリック **[!UICONTROL OK]** 閉じる [!UICONTROL JSON] モジュールの設定。
>
1. の設定を開きます。 [!UICONTROL 配列集約] モジュール。 を **[!UICONTROL ターゲット構造]** から [!UICONTROL カスタム] から [!UICONTROL JSON] ルート配列属性に対応するモジュールのフィールド。 項目を [!DNL Google Sheets] を適切なフィールドに追加します。
>
1. クリック **[!UICONTROL OK]** 閉じる [!UICONTROL 配列集約] モジュールの設定。
>
1. シナリオを実行します。
>
この [!UICONTROL JSON] モジュールは正しい JSON 形式を出力します。
>
1. の設定を開きます。 [!DNL Google Sheets] モジュールを追加し、 [!UICONTROL 返される行の最大数] すべてのデータを処理するには、スプレッドシートの行数より大きい数を指定します。

## トラブルシューティング

### からデータをマッピングできません [!UICONTROL JSON を解析] モジュール

JSON コンテンツが [!UICONTROL JSON を解析] モジュールを作成し、データ構造が正しく定義されていることを確認します。 詳しくは、 [データレコードを JSON に変換中](#transforming-data-records-to-json) 」を参照してください。

### JSON で条件文を使用するとモジュールが失敗する

条件文 ( `if` JSON で、条件文の外側に引用符を置きます。

>[!INFO]
>
**例:**
>
![](assets/quotes-in-json-350x120.png)
