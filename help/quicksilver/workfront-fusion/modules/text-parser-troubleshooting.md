---
content-type: tips-tricks-troubleshooting
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: でのテキストパーサーのトラブルシューティング [!DNL Adobe Workfront Fusion]
description: 出力するテキストパーサーを取得できない場合は、この情報を使用します。
author: Becky
feature: Workfront Fusion
exl-id: 8a3821cf-d0c6-4917-86e7-90a4872a5795
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '365'
ht-degree: 0%

---

# でのテキストパーサーのトラブルシューティング [!DNL Adobe Workfront Fusion]

出力するテキストパーサーを取得できない場合は、この情報を使用します。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## トラブルシューティング

例えば、ファイルドキュメント「filename.docx」のファイルタイプを解析し、ファイル名の拡張子は常に DOCX から CSV へのPDFによって異なるようにします。

この場合に使用できる式は次のとおりです。 [!DNL \..+]

regex101.com の正規表現でこれを使用すると、完全に一致します。

![](assets/regex-expression-350x130.png)

上の画像では、ファイル拡張子が正しく一致していました。 これを取り込んでテキストパーサーに実装しようとする場合：

![](assets/text-parser-350x602.png)

一致するものはありません：

![](assets/text-parser-you-dont-get-a-match-350x365.png)

この理由は、「i」が一致あたりの一致数のみを示すので、この場合は 2 回一致し、「i」の後に数値「1」と「2」が続きます。 この場合、2 番目に一致した値のみをフィルターで照合または渡す必要がある場合は、数値で表される値を指定できます。

![](assets/text-parser-matches-350x355.png)

解析する部分に角括弧を追加する必要のある一致値を取得する（例えば、「filename.docx」から「docx」のみを抽出する）には、この場合の使用する正規表現式に従って、角括弧を\に適用する必要があります。(.+)

これにより、DOCX が取り込まれ、グループに配置され、「。」 それ以外に

![](assets/text-parser-get-matches-350x592.png)

次の図に示す出力では、キャプチャグループは任意の文字（行終端子を除く）に一致します。

![](assets/text-parser-output-350x389.png)

正規表現も組み込むもう 1 つの回避策は、 replace 関数を使用することです

`{{replace("abcdefghijklmno pqr stuvw xyz.docx"; "/.\./"; ".")}}`

次に、 `abcdefghijklmno pqr stuvw xyz.docx` を実際のファイル名変数に設定します。
