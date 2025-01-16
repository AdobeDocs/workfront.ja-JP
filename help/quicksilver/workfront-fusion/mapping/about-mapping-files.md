---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: ' [!DNL Adobe Workfront Fusion] でのファイルのマッピングについて'
description: Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。 この記事は廃止されましたが、この機能を説明する新しい記事へのリンクが含まれています。
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 84%

---

# [!DNL Adobe Workfront Fusion] でのファイルのマッピングについて

>[!IMPORTANT]
>
>Adobe Workfront Fusion のドキュメントが新しい場所に移動されました。
>
>この記事の情報は、次の記事に記載されています。
>
>* [ モジュール間でのファイルのマッピング ](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/map-data/map-files.html)
>
>ブックマークを更新してください。
>
>この記事は現在更新されておらず、近い将来に削除されます。

一部のモジュールには、ファイルを処理する機能があります。これらのモジュールは、さらなる処理のために送信される出力ファイルを返すことも、処理のためにファイルを渡すことを要求することもできます。これらのモジュールが連携してファイルを処理できるようにするには、相互にマッピングする必要があります。

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
  </tr>  </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] のライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  のライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## ファイルのマッピング

ファイルを操作する機能を持つモジュールには、次の 2 つの情報が必要です。

* ファイル名
* ファイルコンテンツ（データ）

ファイルをマッピングする際に、データを取得するシナリオ内のモジュールを選択します。ファイル名とファイルコンテンツは、そのまま自動的にマッピングされます。

>[!NOTE]
>
>URL からファイルを処理する必要がある場合、`HTTP > Get a File` モジュールを使用して URL からファイルをダウンロードし、そのファイルを `HTTP > Get a File` モジュールからシナリオ内の目的のモジュールのフィールドにマッピングすることをお勧めします。

>[!INFO]
>
>**例：**&#x200B;この例では、ドキュメントを [!DNL Adobe Workfront] から [!DNL Google Drive] にダウンロードする方法を示します。[!DNL Workfront] トリガー[!UICONTROL レコードを監視]は、名前や ID など、各ドキュメントに関する詳細情報を返します。
>
>次のモジュール、[!UICONTROL ドキュメントをダウンロード]では、実際のデータをダウンロードして、Google Drive にアップロードできるようにします。
>
>この情報を [!DNL Google Drive] にマッピングしてアップロードできるようにするには、情報のマッピング元のソースファイルを指定する必要があります。ソースファイルの下で [!DNL Workfront]／[!UICONTROL ドキュメントをダウンロード]オプションを選択すると、[!DNL Workfront Fusion] は、[!DNL Workfront] のドキュメントが指定された Google フォルダーにアップロードされるように、ファイル名とファイルコンテンツをマッピングします。
>
>![](assets/wf-download-document-350x605.png)
>
>ただし、ファイル名を変更し、データをそのままにしておく場合は、[!UICONTROL マップ]オプションを使用して、ファイル名とファイルコンテンツを個別にマッピングできます。拡張子を含む完全なファイル名を入力します。テキスト形式とバイナリ形式（写真、ビデオ、PDF など）がサポートされています。
>
>![](assets/use-the-map-option-350x358.png)
