---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Adobe Workfront Fusion での型の強制
description: このドキュメントでは、 [!DNL Adobe Workfront Fusion] は、予期されるデータ形式と予期しないデータ形式で値を受け取る場合に動作します。
author: Becky
feature: Workfront Fusion
exl-id: 847a17c9-bd67-4132-81a8-2a5fe8d516cb
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '638'
ht-degree: 1%

---

# 強制入力 [!DNL Adobe Workfront Fusion]

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
   <td>
   <p>現在のライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>
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

### 型強制

このドキュメントでは、 [!DNL Adobe Workfront Fusion] は、予期されるデータ形式と予期しないデータ形式で値を受け取る場合に動作します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>予測</th> 
   <th>受信済み</th> 
   <th> <p>説明</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>配列 </td> 
   <td>配列 </td> 
   <td> <p>値は変更されずに渡されます。</p> </td> 
  </tr> 
  <tr> 
   <td>配列 </td> 
   <td>その他 </td> 
   <td> <p>受け取った値が配列型でない場合、 [!DNL Workfront Fusion] が配列を作成し、最初の（および唯一の）要素が受け取った値になります。</p> </td> 
  </tr> 
  <tr> 
   <td>ブール型 </td> 
   <td>ブール型 </td> 
   <td> <p>値は変更されずに渡されます。</p> </td> 
  </tr> 
  <tr> 
   <td>ブール型 </td> 
   <td>数値 </td> 
   <td> <p>値が 0 の場合でも、値は論理はいに変換されます。</p> </td> 
  </tr> 
  <tr> 
   <td>ブール型 </td> 
   <td>テキスト </td> 
   <td> <p>値が false の場合、または値が空の場合は、論理値 No に変換されます。 そうでない場合は、論理はいに変換されます。</p> </td> 
  </tr> 
  <tr> 
   <td>ブール型 </td> 
   <td>その他 </td> 
   <td> <p>受け取った値が存在する（null でない）場合、値は論理 Yes に変換されます。</p> </td> 
  </tr> 
  <tr> 
   <td>バッファ </td> 
   <td>バッファ </td> 
   <td> <p>コードページが期待どおりの場合にのみ、値は変更されずに渡されます。 コードページが異なる場合、 [!DNL Workfront Fusion] が受け取った値を要求されたコードページに変換します。 この変換がサポートされていない場合、 [!DNL Workfront Fusion] 検証エラーを返します。</p> </td> 
  </tr> 
  <tr> 
   <td>バッファ </td> 
   <td>ブール型 </td> 
   <td> <p>値はテキストに変換され (true/false)、前述の手順に従ってバイナリデータに変換されます。</p> </td> 
  </tr> 
  <tr> 
   <td>バッファ </td> 
   <td>日付 </td> 
   <td> <p>値は ISO 8601 テキストに変換され、その後、テキストへの変換の手順に従ってバイナリデータに変換されます。</p> </td> 
  </tr> 
  <tr> 
   <td>バッファ </td> 
   <td>数値 </td> 
   <td> <p>値はテキストに変換され、上記の手順に従ってバイナリデータに変換されます。</p> </td> 
  </tr> 
  <tr> 
   <td>バッファ </td> 
   <td>テキスト </td> 
   <td> <p>値はバイナリデータに変換され、期待どおりにエンコードされます。 期待されるエンコーディングが指定されていない場合は、utf8 エンコーディングが使用されます。</p> </td> 
  </tr> 
  <tr> 
   <td>バッファ </td> 
   <td>その他 </td> 
   <td> <p>[!DNL Workfront Fusion] 検証エラーを返します。</p> </td> 
  </tr> 
  <tr> 
   <td>コレクション </td> 
   <td>コレクション </td> 
   <td> <p>値は変更されずに渡されます。</p> </td> 
  </tr> 
  <tr> 
   <td>コレクション </td> 
   <td>その他 </td> 
   <td> <p>[!DNL Workfront Fusion] 検証エラーを返します。</p> </td> 
  </tr> 
  <tr> 
   <td>日付 </td> 
   <td>日付 </td> 
   <td> <p>値は変更されずに渡されます。</p> </td> 
  </tr> 
  <tr> 
   <td>日付 </td> 
   <td>テキスト </td> 
   <td> <p>[!DNL Workfront Fusion] がテキストを日付に変換します。 変換が失敗した場合は、検証エラーが返されます。 日付には、日、月、年を含める必要があります。 日付には、時間とタイムゾーンを含めることができます。 デフォルトのタイムゾーンは設定に基づいています。 例:</p> <p><code>2016-06-20T17:26:44.356Z</code> </p> <p><code>2016-06-20 19:26:44 GMT+02:00</code> </p> <p><code>2016-06-20 19:26+0200</code> </p> <p><code>2016-06-20 17:26:44</code> </p> <p><code>2016-06-20</code> </p> <p><code>2016/06/20 17:26:44</code> </p> <p><code>2016/06/20 19:26:44+02:00</code> </p> <p><code>2016/06/20 17:26</code> </p> <p><code>2016/06/20 5:26 PM</code> </p> <p><code>2016/06/20</code> </p> <p><code>06/20/2016 17:26:44</code> </p> <p><code>06/20/2016 19:26:44+02:00</code> </p> <p><code>06/20/2016 17:26</code> </p> <p><code>06/20/2016 5:26 PM</code> </p> <p><code>06/20/2016</code> </p> <p><code>20.6.2016 17:26:44</code> </p> <p><code>20.6.2016 19:26:44+02:00</code> </p> <p><code>20.6.2016 17:26</code> </p> <p><code>20.6.2016</code> </p> </td> 
  </tr> 
  <tr> 
   <td>日付 </td> 
   <td>その他 </td> 
   <td> <p>[!DNL Workfront Fusion] 検証エラーを返します。</p> </td> 
  </tr> 
  <tr> 
   <td>数値 </td> 
   <td>数値 </td> 
   <td> <p>値は変更されずに渡されます。</p> </td> 
  </tr> 
  <tr> 
   <td>数値 </td> 
   <td>テキスト </td> 
   <td> <p>[!DNL Workfront Fusion] はテキストを数値に変換します。 変換が失敗した場合は、検証エラーが返されます。</p> </td> 
  </tr> 
  <tr> 
   <td>数値 </td> 
   <td>その他 </td> 
   <td> <p>[!DNL Workfront Fusion] 検証エラーを返します。</p> </td> 
  </tr> 
  <tr> 
   <td>テキスト </td> 
   <td>テキスト </td> 
   <td> <p>値は変更されずに渡されます。</p> </td> 
  </tr> 
  <tr> 
   <td>テキスト </td> 
   <td>配列 </td> 
   <td> <p>指定された配列がテキストへの変換をサポートしている場合、値が変換されます。 そうでない場合、 [!DNL Workfront Fusion] 検証エラーを返します。</p> </td> 
  </tr> 
  <tr> 
   <td>テキスト </td> 
   <td>ブール型 </td> 
   <td> <p>値はテキストに変換されます (true/false)。</p> </td> 
  </tr> 
  <tr> 
   <td>テキスト </td> 
   <td>バッファ </td> 
   <td> <p>バイナリデータに対してテキストエンコーディングが指定されている場合、値はテキストに変換されます。 そうでない場合、 [!DNL Workfront Fusion] 検証エラーを返します。</p> </td> 
  </tr> 
  <tr> 
   <td>テキスト </td> 
   <td>日付 </td> 
   <td> <p>値が ISO 8601 テキストに変換されます。</p> </td> 
  </tr> 
  <tr> 
   <td>テキスト </td> 
   <td>数値 </td> 
   <td> <p>値がテキストに変換されます。</p> </td> 
  </tr> 
  <tr> 
   <td>テキスト </td> 
   <td>その他 </td> 
   <td> <p>[!DNL Workfront Fusion] 検証エラーを返します。</p> </td> 
  </tr> 
  <tr> 
   <td>時間 </td> 
   <td>時間 </td> 
   <td> <p>値は変更されずに渡されます。</p> </td> 
  </tr> 
  <tr> 
   <td>時間 </td> 
   <td>テキスト </td> 
   <td> <p>[!DNL Workfront Fusion] 時間を時間に変換しようとします:minutes:秒形式 変換が失敗した場合は、検証エラーが返されます。</p> </td> 
  </tr> 
  <tr> 
   <td>時間 </td> 
   <td>その他 </td> 
   <td> <p>[!DNL Workfront Fusion] 検証エラーを返します。</p> </td> 
  </tr> 
 </tbody> 
</table>
