---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: ' [!DNL Adobe] Workfront Fusion で配列をマッピング'
description: 配列は、Adobe Workfront Fusion のモジュールフィールドにマッピングできます。
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: f87bc22f4ce70f266a199fcb54c5a74f9e3ba914
workflow-type: tm+mt
source-wordcount: '865'
ht-degree: 46%

---

# [!DNL Adobe Workfront Fusion] で配列をマッピング

配列は、以下を含む特別なタイプの項目です。

* 1 つ以上のテキスト値（単純配列）
* 同じタイプの 1 つ以上のコレクション（複合配列）

>[!INFO]
>
>**例：**[!UICONTROL メールの監視]モジュールは、すべてのメールの添付ファイルの配列を返します。すべての添付ファイルは、名前、コンテンツ、サイズなどを含むコレクションを表します。

詳しくは、 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md) での [ 項目データタイプを参照してください。

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

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。



## 配列全体のマッピング

1. 配列をマッピングするモジュールで、配列をマッピングするフィールドをクリックします。 配列のマッピング先のフィールドです。

1. 表示されるボックスで、項目をマッピングします。

   パネルを使用すると、他のタイプの項目と同じ方法でフィールドをマッピングできます。各項目に個別に入力しないで、別の配列をターゲットフィールドにマッピングする場合は、「[!UICONTROL マップ]」ボタンを使用します。この場合、両方の配列（ソース配列とターゲット配列）の構造が同じであることを確認します。

   1 つの配列には、任意の数の項目を追加できます。

イテレータを使用して、配列を個々のバンドルに分割できます。詳しくは、 [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/modules/iterator-module.md)内の[[!UICONTROL イテレータ]モジュールを参照してください。

## 新しい配列への項目のマッピング

Workfront Fusion の一部のフィールドでは、要素を配列にマッピングできます。 例えば、チェックリスト項目の配列を、Workfront ボード / チェックリスト項目を追加モジュールに作成できます。 モジュールを実行すると、すべてのチェックリスト項目がカードに追加されます。

「項目を追加」と表示されるモジュールフィールドは、すべて配列を作成します。

![ 項目を追加 ](assets/add-item.png)

配列に要素を追加するには、次の手順に従います。

1. 「**項目を追加**」をクリックします
1. 開いたパネルに、項目の詳細を入力します。
1. 「**追加**」をクリックします。
1. （オプション）  配列に追加する各要素に対して、手順 1 ～ 3 を繰り返します。

## 配列要素のマッピング


### 数値別に配列要素をマッピングします

配列要素は、配列名の後に角括弧で囲まれた数字として表示されます。 このインデックス番号を使用して、配列の個々の要素をフィールドにマッピングできます。

![](assets/map-array-1st-element.png)

>[!NOTE]
>
>Workfront Fusion の配列インデックス作成は 1 から開始します。

配列要素をマッピングするには：

1. 要素をマッピングするフィールドをクリックします。

   マッピングパネルが開きます。

1. マッピングする要素を含む配列を見つけます。
1. アレイの横にあるドロップダウン矢印をクリックします。
1. マッピングする要素をクリックします。

   要素がマッピングされます。インデックスは 1 です。 これにより、配列の最初の要素がマッピングされます。

1. 配列の別の要素をマッピングするには、[1 をクリックし ] マッピングする配列要素のインデックス番号を入力します。

   ![](assets/access-another-element.png)

### 指定されたキーで配列の要素をマッピングする

一部の配列には、メタデータや属性などのキー値項目を持つコレクションが含まれています。 これらの値の 1 つを使用するには、指定されたキー値で要素を検索し、対応する値を値項目から取得できます。 `map()` 関数と `get()` 関数を組み合わせた数式を使用することをお勧めします。



>[!BEGINSHADEBOX]

次の例は、[!DNL Jira] アプリの出力を示しています。

![](assets/output-of-jira-app-350x100.png)

この例では、ID が 10108 の特定の添付ファイルについて、添付ファイルの配列からファイル名を取得します。

この例では、次の出力が生成されます。

![](assets/output-from-jira-350x261.png)

この式は次のように説明できます。

* `map`

   1. `map()` の最初のパラメーター関数は配列の項目全体です。
   1. 2 つ目のパラメーターは、値の項目の未加工の名前です。未加工の名前を取得するには、[!UICONTROL マッピング]パネルの項目にポインタを合わせます。

      ![](assets/obtain-raw-name-350x124.png)

      >[!NOTE]
      >
      >すべてのパラメーターでは大文字と小文字が区別されます。この例では、アイテムのラベルが生の名前と異なるのは大文字のみですが、生の名前を使用する必要があります。

   1. 3 番目のパラメーターは、キー項目の生の名前です。

      ![](assets/3rd-parameter-350x166.png)

   1. 4 番目のパラメーターは指定されたキー値です。

  `map()` 関数は配列を返すので（指定されたキー値を持つ他の要素が存在する可能性があるため）、その最初の要素を取得するために `get()` 関数を適用する必要があります。

* `get`

   1. `get()` 関数の最初のパラメーターは、`map()` 関数の結果です。

   1. 2 番目のパラメーターは要素のインデックスです。 この例では、インデックスは `1` です。

この例では、次の出力が生成されます。

![](assets/output-from-jira-350x261.png)

>[!ENDSHADEBOX]

`map()` 関数の詳細については、[ 配列関数 ](/help/quicksilver/workfront-fusion/functions/array-functions.md) を参照してください。

`get()` 関数の詳細については、[ 一般関数 ](/help/quicksilver/workfront-fusion/functions/general-functions.md) を参照してください。

## 配列要素を一連のバンドルに変換します

配列は[!UICONTROL イテレータ]モジュールを使用して、一連のバンドルに変換することができます。詳しくは、[[!UICONTROL Iterator] モジュール ](/help/quicksilver/workfront-fusion/modules/iterator-module.md) を参照してください。

![](assets/series-of-bundles.png)

