---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: ドキュメントおよびプルーフを  [!DNL Adobe Workfront plugin]  から  [!DNL Creative Cloud] にアップロード
description: ドキュメントおよびプルーフを  [!DNL Adobe Workfront plugin]  から  [!DNL Creative Cloud] にアップロード
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
hide: true
exl-id: 88870441-8895-477c-9409-f2c33654545a
TQID: https://experienceleague.adobe.com/bZsOnrrwZ7ksCaoM3jfIyeTO00XqG1hDTEmG5VmWOcA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 247
ht-degree: 98%

---

# ドキュメントおよびプルーフを [!DNL Adobe Workfront plugin] から [!DNL Creative Cloud] にアップロード

プロジェクトをドキュメントとしてアップロードすると、すばやくレビューや承認を行ったり、単に [!DNL Adobe Workfront] に保存したりできます。

>[!NOTE]
>
>ドキュメントとプルーフのアップロードは現在、Premiere Pro および After Effects ではサポートされていません。


## ドキュメントの制限事項

この節では、[!DNL Workfront for Adobe Creative Cloud plugins] における既知のドキュメントの制限事項について概説します。

### 新規ドキュメントバージョンは 1 つのファイルのみアップロード可能

[!DNL Workfront] ドキュメントには複数のファイルを含めることができないので、新しいドキュメントバージョンを Workfront にアップロードするには、特定の設定を無効にする必要があります。

>[!NOTE]
>
>複数のファイルを生成する必要がある場合は、代わりにプルーフを作成できます。 新規プルーフは元のドキュメントには関連付けられません。



[!DNL InDesign] でスイッチを単一ファイルに戻すには、次の手順に従います。

1. **書き出しファイル設定を指定**&#x200B;ダイアログボックスを開きます。

   ![ ファイル書き出し設定](assets/file-export-settings.png)

1. 書き出すアセットタイプを見つけ、以下のように設定を調整します。

   <table>
    <tr>
    <td><strong>PDF および PDF 印刷</strong>
    </td>
    <td><strong>個別の PDF ファイルを作成</strong>の選択を解除します。
    </td>
    </tr>
    <tr>
    <td><strong>EPS</strong>
    </td>
    <td>「<strong>範囲</strong>」を選択し、単一のページ番号を入力します。 
    <p>
    <strong>メモ</strong>：ドキュメント全体をアップロードする場合は、プルーフを作成する必要があります。 
    </td>
    </tr>
    <tr>
    <td><strong>EPUB および EPUB 固定</strong>
    </td>
    <td>調整は不要です。
    </td>
    </tr>
    <tr>
    <td><strong>IDML</strong>
    </td>
    <td>調整は不要です。
    </td>
    </tr>
    <tr>
    <td><strong>JPG</strong>
    </td>
    <td>「<strong>範囲</strong>」を選択し、単一のページ番号を入力します。 
    <p>
    <strong>メモ</strong>：ドキュメント全体をアップロードする場合は、プルーフを作成する必要があります。 
    </td>
    </tr>
    <tr>
    <td><strong>PNG</strong>
    </td>
    <td>「<strong>範囲</strong>」を選択し、単一のページ番号を入力します。 
    <p>
    <strong>メモ</strong>：ドキュメント全体をアップロードする場合は、プルーフを作成する必要があります。 
    </td>
    </tr>
    <tr>
    <td><strong>XML</strong>
    </td>
    <td>調整は不要です。 
    </td>
    </tr>
    </table>
