---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: データストアモジュール
description: データベースやシンプルなテーブルと同様に、 [!DNL Adobe Workfront Fusion]  データストアではシナリオのデータを保存して、個々のシナリオやシナリオ実行の間でデータを転送することができます。データストアを使用すると、同期中に様々なシステムから新しいデータを保存できます。
author: Becky
feature: Workfront Fusion
exl-id: 1dc9cb88-d1b9-4a67-91fb-be980cc1ccd1
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 98%

---

# [!UICONTROL データストア]モジュール

データベースやシンプルなテーブルと同様に、[!DNL Adobe Workfront Fusion] データストアではシナリオのデータを保存して、個々のシナリオやシナリオ実行の間でデータを転送することができます。データストアを使用すると、同期中に様々なシステムから新しいデータを保存できます。

データストアモジュールを使用すると、[!DNL Adobe Workfront Fusion] データストアでレコードの追加、置換、更新、取得、削除、検索、カウントを行えるようになります。

データストアの作成、編集、トラブルシューティングについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md) のデータストアを参照してください。

Workfront Fusion のデータストアに関するビデオの紹介については、以下を参照してください。

* [データストア](https://video.tv.adobe.com/v/3427029/){target=_blank}

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
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration]、[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
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

## 前提条件

[!UICONTROL データストア]を使用するには、まずデータストアを作成する必要があります。

データストアの作成について詳しくは、[[!UICONTROL Adobe Workfront Fusion のデータストア]](../../workfront-fusion/modules/data-stores.md)を参照してください。

## [!UICONTROL データストア]モジュールとそのフィールド

データストアモジュールを設定する際、[!DNL Workfront Fusion] には以下のフィールドが表示されます。これらのほか、アプリやサービスでのアクセスレベルなどの要因に応じて、追加のデータストアフィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でモジュールから別のモジュールに情報をマッピングを参照してください。

![](assets/map-toggle-350x74.png)

すべての[!UICONTROL データストア]モジュールは、アクションタイプのモジュールです。

* [レコードの追加 / 置換](#addreplace-a-record)
* [レコードの更新](#update-a-record)
* [レコードを取得](#get-a-record)
* [レコードの有無の確認](#check-the-existence-of-a-record)
* [レコードの削除](#delete-a-record)
* [すべてのレコードの削除](#delete-all-records)
* [レコードの検索](#search-records)
* [レコードのカウント](#count-records)

### [!UICONTROL レコードを追加 / 置換]

このアクションモジュールは、レコードを追加または置き換えます。

データストアとレコードのキーを指定します。

このモジュールは、レコードの ID および関連するフィールドと共に、接続を介してアクセスされるカスタムフィールドとその値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

>[!NOTE]
>
>データストアに同じ名前で既に存在するレコードを追加しようとするとエラーが発生し、「[!UICONTROL 既存のレコードを上書き]」オプションが無効になります。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> レコードを作成するデータストアを選択または追加します。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>モジュールで追加または置換するレコードの一意のキーを入力します。このキーは、後でレコードを取得するために使用できます。このフィールドを空白のままにすると、キーが自動的に生成されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Overwrite an existing record] </td> 
   <td> <p>レコードを上書きする場合は、このオプションを有効にします。上書きするレコードは、上記の「キー」フィールドで指定する必要があります。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record] </td> 
   <td> <p>レコードのフィールドに目的の値を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードの更新]

このアクションモジュールは、レコードを更新します。

データストアとレコードのキーを指定します。

このモジュールは、レコードの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> レコードを作成するデータストアを選択または追加します。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>モジュールで更新するレコードの一意のキーを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Insert missing record] </td> 
   <td> <p>このオプションを有効にすると、指定したキーを持つレコードがまだ存在しない場合、新しいレコードが作成されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record]</td> 
   <td> <p> レコードの更新対象フィールドに、目的の値を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードの取得]

このアクションモジュールは、レコードを取得します。

データストアとレコードのキーを指定します。

このモジュールは、レコードの ID および関連するフィールドと共に、接続を介してアクセスされるカスタムフィールドとその値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> レコードを取得するデータストアを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>モジュールで取得するレコードの一意のキーを入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードの存在の確認]

このアクションモジュールは、特定のレコードが存在するかどうかを指定します。

データストアとレコードのキーを指定します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>レコードの存在を確認するデータストアを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>存在するかどうかをモジュールで確認するレコードの一意のキーを入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードの削除]

このアクションモジュールは、レコードを削除します。

データストアとレコードのキーを指定します。

このモジュールは、レコードの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>レコードの存在を確認するデータストアを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>モジュールで削除するレコードの一意のキーを入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL すべてのレコードを削除]

このアクションモジュールは、特定のデータストアからすべてのレコードを削除します。

データストアを指定します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>すべてのレコードを削除するデータストアを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードを検索]

この検索モジュールは、指定した検索クエリに一致する、データストア内のオブジェクト内のレコードを検索します。

この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> 検索するデータストアを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>検索のフィルターを設定します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Sort]</p> </td> 
   <td> <p style="font-weight: normal;">並べ替えの基準となる各フィールドに対して、次のフィールドに入力します。</p> <p style="font-weight: bold;">[!UICONTROL Key]</p> <p>結果の並べ替えに使用する列名を選択します。</p> <p style="font-weight: bold;">[!UICONTROL Order]</p> <p>昇順または降順のどちらで結果を並べ替えるかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p> 1 回の実行サイクル中に、[!DNL Workfront Fusion] が返す検索結果の最大数を設定します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continue the execution of the route even if the module returns no results]</td> 
   <td> <p> 有効にした場合、このモジュールが結果を返さなくても、このモジュールが処理の一部となるルートが処理を続行します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードをカウント]

このアクションモジュールは、データストア内のレコードに番号を付けます。

データストアを指定します。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>カウントするレコードを含むデータストアを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>
