---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: の項目データタイプ [!DNL Adobe Workfront Fusion]
description: お使いの [!DNL Adobe Workfront Fusion] シナリオには、バンドルに以下に示す項目のタイプを含めることができます。
author: Becky
feature: Workfront Fusion
exl-id: 36c25a86-0d05-4871-a6a6-4fd54cfcc4b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---

# の項目データタイプ [!DNL Adobe Workfront Fusion]

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

## 項目データタイプ

バンドルには、以下に示す項目のタイプを含めることができます。

項目のタイプに関する情報 [!DNL Workfront Fusion] 相互にコンバージョンを許可する場合は、 [強制入力 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>テキスト</p> </td> 
   <td> <p>最も一般的な項目タイプです。 一部のテキスト項目の場合、 [!DNL Adobe Workfront Fusion] 許容される最大長または最小長を満たしているか、またはアイテムが形式検証（E メール、URL、ファイル名）を実行しているかを確認します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>数値</p> </td> 
   <td> <p>数値項目の場合、 [!DNL Workfront Fusion] は、指定した範囲（許容される最小値または最大値）の入力を検証します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ブール値（はい/いいえ）</p> </td> 
   <td> <p>このタイプは、次の 2 つの値のみを持つ品目に使用されます。true または false。 </p> <p>モジュールを設定する際、ブール型は次の 2 つの形式で表示できます。</p> 
    <ul> 
     <li> <p>必須のフィールドが必須で、入力が必要な場合は、必須のチェックボックスが表示されます。</p> <p> <img src="assets/boolean-checkbox-350x158.jpg" style="width: 350;height: 158;"> </p> </li> 
     <li> <p>空白のままにできるオプションのフィールドは選択ボックスとして表示され、次の 3 つの値から選択できます。 <code>Yes</code>, <code>No</code>、および <code>Not defined</code> （デフォルト）。</p> <p> <img src="assets/boolean-convert-file-350x129.jpg" style="width: 350;height: 129;"> </p> </li> 
    </ul> <p>次をクリックできます。 <strong>[!UICONTROL マップ ]</strong> 別のモジュールの項目に値をマッピングする必要がある場合。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>日付</p> </td> 
   <td> <p>日付は、ISO 8601 の日付フォーマットで入力します。例： <code>2015-09-18T11:58Z</code>. タイムゾーンは、プロファイル設定で変更できます。詳しくは、 <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">でのプロファイル設定の変更 [!DNL Adobe Workfront Fusion]</a>. </p> <p>日付を必要とするフィールドをクリックすると、モジュール設定にポップアップカレンダーが表示されます。 一部の項目では時間は必要ありません。</p> <p>日付項目の値は、プロファイルで選択されたローカルタイムゾーンと Web タイムゾーンを使用して形式設定されます。 項目の上にマウスポインターを置くと、日付項目の値の ISO 8601 バージョンを表示できます。</p> <p>注意：ISO 値が表示されない場合、項目はおそらく日付ではなくテキストです。</p> <p>時刻は <code>hours:minutes:seconds</code> 形式、例：<code>14:03:52</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>バッファ（バイナリデータ）</p> </td> 
   <td> <p>ファイルコンテンツは、通常、バッファータイプのコンテンツ（画像コンテンツ、ビデオファイルなど）として送信されます。 場合によっては、テキストデータがこのタイプに含まれることがあります（例えば、テキストファイル）。 [!DNL Workfront Fusion] では、バイナリコード内のテキストデータをテキストに、テキストをバイナリコード内のテキストデータに自動的に変換できます。 詳しくは、 <a href="../../workfront-fusion/mapping/about-mapping-files.md" class="MCXref xref">[!UICONTROL Adobe Workfront Fusion] でのファイルのマッピングについて</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>コレクション</p> </td> 
   <td> <p>コレクションは、複数のサブ項目で構成される項目です。 電子メールメッセージ内の送信者項目は、コレクションの一例です。送信者名（テキストタイプ）と送信者の e メールアドレス（テキストタイプ）が含まれます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>選択（メニュー）</p> </td> 
   <td> <p>モジュールを設定する際に、 <a href="../../workfront-fusion/modules/configure-a-modules-settings.md" class="MCXref xref">でのモジュールの設定 [!DNL Adobe Workfront Fusion]</a>を使用すると、同じタイプの複数の項目から選択できます。 例えば、 [!DNL Dropbox] モジュール。 </p> <p>モジュールを設定する際に、次の 2 つの形式で選択メニューが表示されます。</p> <p> <p>複数選択できる場合は、チェックボックスが付いた複数の項目が表示されます。</p> <p> <img src="assets/image-kb-type-list-multi-350x232.jpg" style="width: 350;height: 232;"> </p> </p> <p>1 つのオプションのみが可能な場合は、ドロップダウンメニューが表示されます。</p> <p> <img src="assets/select-menu-dropdown-350x130.jpg" style="width: 350;height: 130;"> </p> <p>別のモジュールから項目をマッピングする必要がある場合は、 <strong>マップ</strong> 」ボタンをクリックします。 このボタンをクリックすると、選択メニューではなくテキストフィールドが開きます。 詳しくは、 <a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref">のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>配列</p> </td> 
   <td> <p>配列タイプを使用して、コレクションを含む同じタイプの複数の値を操作できます。 例えば、[!UICONTROL 電子メール ] モジュールは添付ファイルの配列を返し、各添付ファイルには名前、コンテンツ、サイズなどが含まれます。 詳しくは、 <a href="../../workfront-fusion/mapping/map-an-array.md" class="MCXref xref">で配列をマッピングする [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>検証</p> </td> 
   <td> <p>[!DNL Workfront Fusion] は、各タイプの項目に対して検証を実行する場合があります。 項目が検証に合格しない場合、モジュールはデータエラーが原因で処理を停止します。 詳しくは、 <a href="../../workfront-fusion/errors/error-processing.md" class="MCXref xref">でのエラー処理 [!DNL Adobe Workfront Fusion]</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
