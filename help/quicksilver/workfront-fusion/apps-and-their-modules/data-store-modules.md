---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: データストアモジュール
description: An [!DNL Adobe Workfront Fusion] データストアは、データベースやシンプルなテーブルと同様に、シナリオからのデータを格納し、個々のシナリオまたはシナリオの実行間でデータを転送できます。 データストアを使用すると、同期中に様々なシステムから新しいデータを保存できます。
author: Becky
feature: Workfront Fusion
exl-id: 1dc9cb88-d1b9-4a67-91fb-be980cc1ccd1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1151'
ht-degree: 0%

---

# [!UICONTROL データストア] モジュール

An [!DNL Adobe Workfront Fusion] データストアは、データベースやシンプルなテーブルと同様に、シナリオからのデータを格納し、個々のシナリオまたはシナリオの実行間でデータを転送できます。 データストアを使用すると、同期中に様々なシステムから新しいデータを保存できます。

データストアモジュールを使用して、 [!DNL Adobe Workfront Fusion] データストア。

データストアの作成、編集、トラブルシューティングについて詳しくは、 [のデータストア [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

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

## 前提条件

使用する [!UICONTROL データストア] モジュールの場合、最初にデータストアを作成する必要があります。

データストアの作成について詳しくは、 [のデータストア [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

## [!UICONTROL データストア] モジュールとそのフィールド

データストアモジュールを設定する際、 [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、アプリやサービスでのアクセスレベルなどの要因に応じて、追加のデータストアフィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

すべて [!UICONTROL データストア] モジュールはアクションタイプのモジュールです。

* [レコードの追加/置換](#addreplace-a-record)
* [レコードの更新](#update-a-record)
* [レコードの取得](#get-a-record)
* [レコードの存在の確認](#check-the-existence-of-a-record)
* [レコードの削除](#delete-a-record)
* [すべてのレコードを削除](#delete-all-records)
* [レコードを検索](#search-records)
* [レコードをカウント](#count-records)

### [!UICONTROL レコードの追加/置換]

このアクションモジュールは、レコードを追加または置き換えます。

データストアとレコードのキーを指定します。

このモジュールは、レコードと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

>[!NOTE]
>
>モジュールは、同じ名前と [!UICONTROL 既存のレコードを上書き] オプションは無効です。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL データストア ]</td> 
   <td> <p> レコードを作成するデータストアを選択または追加します。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL キー ] </td> 
   <td> <p>モジュールで追加または置換するレコードの一意のキーを入力します。 このキーは、後でレコードを取得するために使用できます。 このフィールドを空白のままにすると、キーが自動的に生成されます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 既存のレコードを上書き ] </td> 
   <td> <p>レコードを上書きするには、このオプションを有効にします。 上書きするレコードは、上の「キー」フィールドで指定する必要があります。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL レコード ] </td> 
   <td> <p>レコードのフィールドに必要な値を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードの更新]

このアクションモジュールは、レコードを更新します。

データストアとレコードのキーを指定します。

このモジュールは、レコードと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL データストア ]</td> 
   <td> <p> レコードを作成するデータストアを選択または追加します。 </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL キー ] </td> 
   <td> <p>モジュールで更新するレコードの一意のキーを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 見つからないレコードを挿入 ] </td> 
   <td> <p>指定したキーを持つレコードが存在しない場合に新しいレコードを作成するには、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL レコード ]</td> 
   <td> <p> 更新するレコードのフィールドに、必要な値を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードの取得]

このアクションモジュールは、レコードを取得します。

データストアとレコードのキーを指定します。

このモジュールは、レコードと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL データストア ]</td> 
   <td> <p> レコードの取得元のデータストアを選択します</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL キー ] </td> 
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
   <td>[!UICONTROL データストア ] </td> 
   <td> <p>レコードの存在を確認するデータストアを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL キー ] </td> 
   <td> <p>モジュールが存在するかどうかを確認するレコードの一意のキーを入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードの削除]

このアクションモジュールは、レコードを削除します。

データストアとレコードのキーを指定します。

このモジュールは、レコードと関連するフィールドの ID と、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL データストア ] </td> 
   <td> <p>レコードの存在を確認するデータストアを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL キー ] </td> 
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
   <td>[!UICONTROL データストア ] </td> 
   <td> <p>すべてのレコードを削除するデータストアを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL レコードを検索]

この検索モジュールは、指定した検索クエリに一致する、データストア内のオブジェクト内のレコードを検索します。

この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL データストア ]</td> 
   <td> <p> 検索するデータストアを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL フィルター ]</p> </td> 
   <td> <p>検索のフィルターを設定します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL 並べ替え ]</p> </td> 
   <td> <p style="font-weight: normal;">並べ替えの基準となる各フィールドに対して、次のフィールドに入力します。</p> <p style="font-weight: bold;">[!UICONTROL キー ]</p> <p>結果の並べ替えに使用する列名を選択します。</p> <p style="font-weight: bold;">[!UICONTROL 順序 ]</p> <p>結果を昇順または降順に並べ替えるかどうかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 制限 ]</td> 
   <td> <p> 検索結果の最大数を設定 [!DNL Workfront Fusion] は、1 回の実行サイクルでを返します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL モジュールが結果を返さない場合でも、ルートの実行を続行します ]</td> 
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
   <td>[!UICONTROL データストア ] </td> 
   <td> <p>カウントするレコードを含むデータストアを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>
