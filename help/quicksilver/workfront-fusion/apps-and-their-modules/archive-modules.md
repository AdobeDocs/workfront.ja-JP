---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: モジュールをアーカイブ
description: 内 [!DNL Adobe Workfront Fusion] シナリオの場合、zip 形式のファイルなどのアーカイブを複数のサードパーティのアプリケーションやサービスに接続できます。 例えば、次のシナリオを設定できます。
author: Becky
feature: Workfront Fusion
exl-id: e29b6d39-3666-4d6d-a178-1983ae9f3aa9
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# [!UICONTROL アーカイブ] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオの場合は、圧縮ファイルなどのアーカイブをシナリオで使用して、自動化または統合で使用できます。

シナリオの作成手順については、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). モジュールについて詳しくは、 [のモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## [!UICONTROL アーカイブ] モジュールとそのフィールド

設定時に [!UICONTROL アーカイブ] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!UICONTROL アーカイブ] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL アーカイブの抽出]](#extract-an-archive)
* [[!UICONTROL アーカイブの作成]](#create-an-archive)
* [[!UICONTROL 水増し]](#inflate)
* [[!UICONTROL デフレート]](#deflate)

## [!UICONTROL アーカイブの抽出]

このアクションモジュールは、指定したファイルをアーカイブから抽出します。

このモジュールは、ファイルの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL ソースファイル ]</td> 
   <td> <p> 抽出するファイルを選択します。 このファイルは、以前のモジュール ( [!DNL Workfront] &gt;[!UICONTROL ドキュメントをダウンロード ] モジュール )。</p>  </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**例：** 定義したから ZIP ファイルを取得します。 [!DNL Dropbox] フォルダー（アーカイブなど）、を使用して抽出します。 [!UICONTROL アーカイブ] をモジュール化し、抽出したファイルを、 [!UICONTROL 電子メール] または [!DNL Gmail] モジュール。
>
>![](assets/example-dropbox-350x134.png)

## [!UICONTROL アーカイブの作成]

この集約モジュールは、目的のファイルを [!UICONTROL ZIP] または [!UICONTROL TAR] アーカイブ。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL ソースモジュール ]</td> 
   <td> <p> ファイルを取得するモジュールを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL の種類 ] </td> 
   <td> <p>ファイルを [!UICONTROL ZIP] アーカイブまたは [!UICONTROL TAR] アーカイブに追加するかどうかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL コメント ]</td> 
   <td>アーカイブに追加するコメントを入力します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Group by]</td> 
   <td> <p>集計出力をグループ化する式を定義します。 この式には、1 つ以上のマッピングされた項目を含めることができます。 集計されたデータは、この式の値を使用してグループに分割されます。 各グループは、キー（評価された式）と値（集計テキスト）を持つ個別のバンドルとして出力されます。 キーを後続のモジュールのフィルターとして使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 空の集計後に処理を停止 ]</td> 
   <td>結果がない場合にシナリオを停止するには、このオプションを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL アーカイブ名 ]</td> 
   <td> <p> 作成したアーカイブの名前を入力します。 拡張機能は追加しないでください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ソースファイル ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**例：** 次を使用して受信メールを監視する [!DNL Gmail] >[!UICONTROL メールを見る] モジュール。 E メールを受け取ると、添付ファイルは個々のバンドルに繰り返され、次に [!DNL ZIP] ファイルを作成し、定義したDropboxフォルダに保存します。
>
>![](assets/example-gmail-350x102.png)

## [!UICONTROL 水増し]

この変換器モジュールは、膨張アルゴリズムを用いてバイナリデータを解凍する。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL データ ] </td> 
   <td> <p>展開関数を使用して、展開するデータを入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL デフレート]

この変換器モジュールは、デフレーションアルゴリズムを使用してバイナリデータを圧縮します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL データ ] </td> 
   <td> <p>deflate 関数を使用して圧縮するデータを入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>
