---
content-type: tips-tricks-troubleshooting
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: ' [!DNL Adobe Workfront Fusion] でのテキストパーサーのトラブルシューティング'
description: Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。 この記事は廃止されましたが、この機能を説明する新しい記事へのリンクが含まれています。
author: Becky
feature: Workfront Fusion
exl-id: 8a3821cf-d0c6-4917-86e7-90a4872a5795
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '474'
ht-degree: 85%

---

# [!DNL Adobe Workfront Fusion] でのテキストパーサーのトラブルシューティング

>[!IMPORTANT]
>
>Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。
>
>この記事の情報は、次の記事に記載されています。
>
>* [テキストパーサー](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/text-parser.html)
>
>ブックマークを更新してください。
>
>この記事は現在更新されておらず、近い将来に削除されます。

出力するテキストパーサーを取得できない場合は、この情報を使用します。

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

[!DNL Adobe Workfront Fusion] のライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  のライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## トラブルシューティング

例えば、ケースシナリオの場合、ファイルドキュメント「filename.docx」のファイルタイプを解析するには、ファイル名の拡張子は常に DOCX、CSV、PDF など様々です。

この場合に使用できる式は [!DNL \..+] です。

regex101.com の正規表現でこれを使用すると、完全一致が得られます。

![](assets/regex-expression-350x130.png)

上の画像では、ファイル拡張子が正しく一致していました。これを取り込んでテキストパーサーに実装しようとすると、次のようになります。

![](assets/text-parser-350x602.png)

一致するものはありません。

![](assets/text-parser-you-dont-get-a-match-350x365.png)

この理由は、「i」が一致あたりの一致数のみを示すので、この場合は 2 回一致があるので、「i」の後に数値「1」と「2」が続きます。このユースケースの場合、2 番目に一致した値のみをフィルターで照合または渡す必要がある場合は、数値で表される値を指定できます。

![](assets/text-parser-matches-350x355.png)

解析する部分に括弧を追加する必要のある一致値を取得するには（例えば、「filename.docx」から「docx」のみを抽出する）、このケースシナリオで使用する正規表現式に従って、括弧を \ に適用する必要があります。(.+)

これにより、DOCX が取り込まれ、グループに配置され、「.」が残ります。それ以外

![](assets/text-parser-get-matches-350x592.png)

次の図に示す出力では、キャプチャするグループは任意の文字（行末文字を除く）に一致します。

![](assets/text-parser-output-350x389.png)

正規表現も組み込んだもう 1 つの回避策は、replace 関数を使用することです

`{{replace("abcdefghijklmno pqr stuvw xyz.docx"; "/.\./"; ".")}}`

次に、`abcdefghijklmno pqr stuvw xyz.docx` を実際のファイル名変数に置き換えます。
