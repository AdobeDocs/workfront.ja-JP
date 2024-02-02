---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: ' [!DNL Adobe Workfront Fusion] の項目データタイプ'
description: お使いの  [!DNL Adobe Workfront Fusion]  シナリオには、バンドルに以下に示す項目のタイプを含めることができます。
author: Becky
feature: Workfront Fusion
exl-id: 36c25a86-0d05-4871-a6a6-4fd54cfcc4b1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '708'
ht-degree: 100%

---

# [!DNL Adobe Workfront Fusion] の項目データタイプ

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion]ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を、組織で購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 項目データタイプ

バンドルには、以下に示す項目のタイプを含めることができます。

[!DNL Workfront Fusion] で相互に変換できる項目のタイプについては、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/type-coercion.md) でのタイプの強制を参照してください。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>テキスト</p> </td> 
   <td> <p>最も一般的な項目タイプです。 一部のテキスト項目では、[!DNL Adobe Workfront Fusion] は許容される最大長または最小長を満たしているか、またはアイテムが形式検証（メール、URL、ファイル名）を実行しているかどうかを確認します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>数値</p> </td> 
   <td> <p>一部の数値項目では、[!DNL Workfront Fusion] は指定された範囲（許容される最小値または最大値）の入力を検証する場合があります。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ブール値（はい／いいえ）</p> </td> 
   <td> <p>このタイプは、true または false の 2 つの値のみを持つ項目に使用します。 </p> <p>モジュールを設定する際、ブール値タイプは次の 2 つの形式で表示できます。</p> 
    <ul> 
     <li> <p>フィールドが必須で、入力が必要な場合は、必須のチェックボックスが表示されます。</p> <p> <img src="assets/boolean-checkbox-350x158.jpg" style="width: 350;height: 158;"> </p> </li> 
     <li> <p>空白のままにできるオプションのフィールドは選択ボックスとして表示され、<code>Yes</code>、<code>No</code>、<code>Not defined</code>（デフォルト）の 3 つの値から選択できます。</p> <p> <img src="assets/boolean-convert-file-350x129.jpg" style="width: 350;height: 129;"> </p> </li> 
    </ul> <p>値を別のモジュールの項目にマッピングする必要がある場合は、<strong>[!UICONTROL Map]</strong> をクリックします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>日付</p> </td> 
   <td> <p>日付は、ISO 8601 の日付形式で入力します（例：<code>2015-09-18T11:58Z</code>）。 <a href="../../workfront-fusion/workfront-fusion-basics/change-profile-settings.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのプロファイル設定の変更で説明されているように、タイムゾーンはプロファイル設定で変更できます。 </p> <p>日付を必要とするフィールドをクリックすると、モジュール設定にポップアップカレンダーが表示されます。一部の項目では時間は必須ではありません。</p> <p>日付項目の値は、プロファイルで選択されたローカルタイムゾーンと web タイムゾーンを使用して形式設定されます。 項目の上にポインタを合わせると、日付項目の値の ISO 8601 バージョンを表示できます。</p> <p>メモ：ISO 値が表示されない場合、項目はおそらくテキストで、日付ではありません。</p> <p>時間は <code>hours:minutes:seconds</code> 形式で入力します（例：<code>14:03:52</code>）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>バッファー（バイナリデータ）</p> </td> 
   <td> <p>ファイルコンテンツは、通常、バッファータイプのコンテンツ（画像コンテンツ、ビデオファイルなど）として送信されます。 場合によっては、テキストデータがこのタイプに含まれることがあります（テキストファイルなど）。 [!DNL Workfront Fusion] では、バイナリコード内のテキストデータをテキストに、テキストをバイナリコード内のテキストデータに自動変換できます。 詳しくは、<a href="../../workfront-fusion/mapping/about-mapping-files.md" class="MCXref xref">[!UICONTROL Adobe Workfront Fusion] でのマッピングファイルについて</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>コレクション</p> </td> 
   <td> <p>コレクションとは、複数のサブ項目で構成される項目です。 メールメッセージ内の送信者項目は、コレクションの一例です。このコレクションには、送信者名（テキストタイプ）と送信者のメールアドレス（テキストタイプ）が含まれています。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>選択（メニュー）</p> </td> 
   <td> <p><a href="../../workfront-fusion/modules/configure-a-modules-settings.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのモジュールの設定を行うの説明に従ってモジュール設定を行う場合、同じタイプの複数の項目から選択できます。[!DNL Dropbox] モジュールでの設定のフォルダー選択メニューが一例です。 </p> <p>モジュールを設定する際に、次の 2 つの形式で選択メニューが表示されます。</p> <p> <p>複数選択できる場合は、チェックボックス付きの項目が複数表示されます。</p> <p> <img src="assets/image-kb-type-list-multi-350x232.jpg" style="width: 350;height: 232;"> </p> </p> <p>可能なオプションが 1 つだけの場合は、ドロップダウンメニューが表示されます。</p> <p> <img src="assets/select-menu-dropdown-350x130.jpg" style="width: 350;height: 130;"> </p> <p>別のモジュールから項目をマッピングする必要がある場合は、「<strong>マップ</strong>」ボタンを使用します。 このボタンをクリックすると、選択メニューの代わりにテキストフィールドが開きます。詳しくは、<a href="../../workfront-fusion/mapping/map-information-between-modules.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのモジュール間で情報をマッピングを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>配列</p> </td> 
   <td> <p>配列タイプを使用すると、コレクションを含む同じタイプの複数の値を操作できます。 [!UICONTROL Email] モジュールの例では、添付ファイルの配列を返し、各添付ファイルには名前、コンテンツ、サイズなどが含まれます。 詳しくは、<a href="../../workfront-fusion/mapping/map-an-array.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> で配列をマッピングを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>検証</p> </td> 
   <td> <p>[!DNL Workfront Fusion] では、項目のタイプごとに検証を実行する場合があります。項目が検証に合格しない場合、モジュールはデータエラーが原因で処理を停止します。 詳しくは、<a href="../../workfront-fusion/errors/error-processing.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> でのエラー処理を参照してください。 </p> </td> 
  </tr> 
 </tbody> 
</table>
