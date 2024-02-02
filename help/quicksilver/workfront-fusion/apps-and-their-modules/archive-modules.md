---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: モジュールのアーカイブ
description: ' [!DNL Adobe Workfront Fusion]  シナリオの場合、zip 形式のファイルなどのアーカイブを複数のサードパーティのアプリケーションやサービスに接続できます。例えば、次のシナリオを設定できます。'
author: Becky
feature: Workfront Fusion
exl-id: e29b6d39-3666-4d6d-a178-1983ae9f3aa9
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: ht
source-wordcount: '552'
ht-degree: 100%

---

# [!UICONTROL アーカイブ]モジュール

[!DNL Adobe Workfront Fusion] シナリオの場合、zip 形式のファイルなどのアーカイブをシナリオで使用して、自動化または統合で使用できます。

シナリオの作成手順が必要な場合は、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) でのシナリオの作成を参照してください。モジュールについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md) のモジュールを参照してください。

## [!UICONTROL アーカイブ]モジュールとそのフィールド

[!UICONTROL アーカイブ]モジュールの設定時に、[!DNL Workfront Fusion] には以下のフィールドが表示されます。これらとともに、アプリやサービスのアクセスレベルなどの要因に応じて、追加の「[!UICONTROL アーカイブ]」フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) での、1 つのモジュールから別のモジュールへの情報のマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [[!UICONTROL アーカイブを抽出]](#extract-an-archive)
* [[!UICONTROL アーカイブを作成]](#create-an-archive)
* [[!UICONTROL インフレート]](#inflate)
* [[!UICONTROL デフレート]](#deflate)

## [!UICONTROL アーカイブを抽出]

このアクションモジュールは、指定したファイルをアーカイブから抽出します。

このモジュールは、ファイルの ID や関連するフィールドのほか、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p> インポートするファイルを選択してください。このファイルは、以前のモジュール（[!DNL Workfront]／[!UICONTROL Download a document] モジュールなど）からマッピングできます。</p>  </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**例：**&#x200B;定義された [!DNL Dropbox] フォルダー（アーカイブなど）から ZIP ファイルを取得し、[!UICONTROL アーカイブ]モジュールを使用して抽出し、[!UICONTROL メール]または [!DNL Gmail] モジュールを使用して、抽出したファイルを目的のメールアドレスに添付ファイルとして送信します。
>
>![](assets/example-dropbox-350x134.png)

## [!UICONTROL アーカイブを作成]

このアグリゲータモジュールは、目的のファイルを [!UICONTROL ZIP] または [!UICONTROL TAR] アーカイブに追加します。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source module]</td> 
   <td> <p> ファイルの取得元のモジュールを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type] </td> 
   <td> <p>ファイルを [!UICONTROL ZIP] アーカイブまたは [!UICONTROL TAR] アーカイブのどちらに追加するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comment]</td> 
   <td>アーカイブに追加するコメントを入力します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Group by]</td> 
   <td> <p>集約出力をグループ化する式を定義します。この式には、1 つ以上のマッピングされた項目を含めることができます。集約されたデータは、この式の値を使用してグループに分割されます。各グループは、キー（評価された式）と値（集約されたテキスト）を持つ個別のバンドルとして出力されます。キーを後続のモジュールのフィルターとして使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stop processing after an empty aggregation]</td> 
   <td>結果がない場合にシナリオを停止するには、このオプションを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Archive name]</td> 
   <td> <p> 作成したアーカイブの名前を入力します。拡張機能は追加しないでください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p>以前のモジュールで使用したソースファイルを選択するか、ソースファイルの名前とデータをマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**例：**[!DNL Gmail]／[!UICONTROL メールを監視]モジュールを使用して受信メールを見ます。メールを受け取ると、添付ファイルは個々のバンドルに反復され、[!DNL ZIP] ファイルにアーカイブされて、定義された Dropbox フォルダーに保存されます。
>
>![](assets/example-gmail-350x102.png)

## [!UICONTROL インフレート]

この変換モジュールは、インフレーションアルゴリズムを用いてバイナリデータを解凍します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data] </td> 
   <td> <p>インフレート関数を使用して、インフレートするデータを入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL デフレート]

この変換モジュールは、デフレーションアルゴリズムを使用してバイナリデータを圧縮します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data] </td> 
   <td> <p>deflate 関数を使用して、圧縮するデータを入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>
