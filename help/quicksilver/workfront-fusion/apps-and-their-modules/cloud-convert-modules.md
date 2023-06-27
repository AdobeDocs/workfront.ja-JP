---
title: CloudConvert モジュール
description: CloudConvert モジュール
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: e21ef8a0-bec0-43fc-a495-c00b4023a273
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '3041'
ht-degree: 0%

---

# [!DNL CloudConvert] モジュール

Adobe Workfront Fusion シナリオでは、CloudConvert を使用するワークフローを自動化し、それを複数のサードパーティのアプリケーションおよびサービスに接続することができます。 この [!DNL CloudConvert] モジュールを使用すると、ジョブ、タスク、および [!DNL CloudConvert] アカウント

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

## 接続 [!DNL CloudConvert] から [!DNL Workfront Fusion] {#connect-cloudconvert-to-workfront-fusion}

次の手順で [!DNL CloudConvert] アカウント [!DNL Workfront Fusion]の場合は、 [!DNL CloudConvert] アカウント

1. にログインします。 [!DNL CloudConvert] のアカウントを開き、 [!UICONTROL ダッシュボード].
1. を開きます。 **[!UICONTROL 認証] > [!UICONTROL API キー]** 」セクションに入力します。
1. クリック **[!UICONTROL 新しい API キーを作成]**.
1. API キーの名前を入力し、使用するスコープを有効にして、[ ] をクリックします **[!UICONTROL 作成]**.
1. 提供されたトークンをコピーし、安全な場所に保存します。
1. In [!DNL Workfront Fusion]、シナリオの作成を開始し、 [!DNL CloudConvert] モジュール **[!UICONTROL 接続の作成]** ダイアログ。

   手順については、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. 手順 5 で保存したトークンを入力し、「 」をクリックします。 **[!UICONTROL 続行]** 接続を確立するために。

## [!DNL CloudConvert] モジュールとそのフィールド {#cloudconvert-modules-and-their-fields}

設定時に [!DNL CloudConvert] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL CloudConvert] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [一般的なタスク](#common-tasks)
* [ジョブ](#jobs)
* [タスク](#tasks)
* [その他](#other)

### 一般的なタスク

* [Web サイトのキャプチャ](#capture-a-website)
* [[!UICONTROL ファイルの変換]](#convert-a-file)
* [アーカイブの作成](#create-an-archive)
* [ファイルを結合](#merge-files)
* [ファイルの最適化](#optimize-a-file)

#### [!UICONTROL Web サイトのキャプチャ]

このアクションモジュールは、指定された Web サイトをキャプチャし、PDF、JPG、PNG 形式で保存します。

Web サイトの URL と、情報の保存場所などのその他の情報を指定します。

このモジュールは、ファイルの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL CloudConvert] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">接続 [!DNL CloudConvert] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>取得する Web サイトの URL を入力します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力形式 ] </td> 
   <td>キャプチャした Web サイトを PNG、JPG、PDF形式で保存するかどうかを選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル名 ] </td> 
   <td>ターゲット出力ファイルのファイル名（拡張子も含む）を入力します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers] </td> 
   <td> <p>（オプション）リクエストヘッダーを定義します。 </p> <p>これは、例えば、指定した URL で認証が必要な場合に便利です。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL コンバージョンおよびエンジン固有のオプション ] </p> </td> 
   <td>コンバージョンとエンジン固有のオプションを指定します。 使用可能なオプションを表示するには、 <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> ドキュメント <code>input_format</code> および <code>output_format</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイルのダウンロード ] </td> 
   <td> <p>モジュールの出力にファイルデータも含める場合は、このオプションを有効にします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルの変換]

ファイルを選択した出力形式に変換します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL CloudConvert] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">接続 [!DNL CloudConvert] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 入力ファイル ]</td> 
   <td>を使用してファイルをアップロードするかどうかを選択します。 [!DNL Workfront Fusion] または、ファイルのアップロード元の URL を指定します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイルのアップロード ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL からのファイルの読み込み ]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL URL]</strong> </p> <p>変換するファイルの URL を入力します。</p> </li> 
     <li> <p><strong>[!UICONTROL Headers]</strong></p> <p>リクエストヘッダーを定義します（オプション）。 これは、例えば、指定した URL で認証が必要な場合に便利です。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 形式 ]</td> 
   <td>変換するファイルの入力形式を指定するかどうかを選択します。 指定しなかった場合、入力ファイルの拡張子が入力形式として使用されます。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Input Format]</td> 
   <td>ファイルの現在の形式を選択します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 出力形式 ]</td> 
   <td>ファイルの変換先のファイル形式を選択します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL ファイル名 ]</td> 
   <td>ターゲット出力ファイルのファイル名（拡張子を含む）を選択します。</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL コンバージョンおよびエンジン固有のオプション ] </p> </td> 
   <td>コンバージョンとエンジン固有のオプションを指定します。 使用可能なオプションを表示するには、 <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> ドキュメント <code>input_format</code> および <code>output_format</code>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL ファイルのダウンロード ] </td> 
   <td> <p>モジュールの出力にファイルデータも含める場合は、このオプションを有効にします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アーカイブの作成]

ZIP、RAR、7Z、TAR、TAR.GZ または TAR.BZ2 アーカイブに 1 つ以上のファイルを追加できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL CloudConvert] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">接続 [!DNL CloudConvert] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 入力ファイル ]</p> </td> 
   <td> <p>アーカイブに追加するファイルを指定します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイルのアップロード ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL からのファイルの読み込み ]</p> </td> 
   <td> <p><strong>[!UICONTROL URL]</strong> </p> <p>アーカイブするファイルの URL を入力します。</p> <p><strong>[!UICONTROL Headers]</strong> </p> <p>リクエストヘッダーを定義します（オプション）。 これは、例えば、指定した URL で認証が必要な場合に便利です。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力形式 ]</td> 
   <td> <p> アーカイブ済みファイルのターゲット形式を選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル名 ]</td> 
   <td> <p> ターゲット出力ファイルのファイル名（拡張子を含む）を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL コンバージョンおよびエンジン固有のオプション ] </td> 
   <td> <p>コンバージョンとエンジン固有のオプションを指定します。 使用可能なオプションを表示するには、 <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> ドキュメント <code>input_format</code> および <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイルのダウンロード ]</td> 
   <td> <p>モジュールの出力にファイルデータも含める場合は、このオプションを有効にします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルを結合]

2 つ以上のファイルを 1 つのPDFに結合する。 入力ファイルがPDFでない場合、入力ファイルは自動的にPDFに変換されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL CloudConvert] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">接続 [!DNL CloudConvert] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 入力ファイル ]</p> </td> 
   <td> <p>マージするファイルを指定します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイルのアップロード ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL からのファイルの読み込み ]</p> </td> 
   <td> <p><strong>[!UICONTROL URL]</strong> </p> <p>アーカイブするファイルの URL を入力します。</p> <p><strong>[!UICONTROL Headers]</strong> </p> <p>リクエストヘッダーを定義します（オプション）。 これは、例えば、指定した URL で認証が必要な場合に便利です。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力形式 ]</td> 
   <td> <p> マージされたファイルのターゲットフォーマットを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル名 ]</td> 
   <td> <p> ターゲット出力ファイルのファイル名（拡張子を含む）を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL コンバージョンおよびエンジン固有のオプション ] </td> 
   <td> <p>コンバージョンとエンジン固有のオプションを指定します。 使用可能なオプションを表示するには、 <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> ドキュメント <code>input_format</code> および <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイルのダウンロード ]</td> 
   <td> <p>モジュールの出力にファイルデータも含める場合は、このオプションを有効にします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルの最適化]

このアクションモジュールは、ファイルをPDF、PNG、またはJPG形式で最適化および圧縮します。

ファイルと、最適化および保存のためのパラメーターを指定します。

このモジュールは、ファイルの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL CloudConvert] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">接続 [!DNL CloudConvert] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 入力ファイル ]</td> 
   <td>Workfront Fusion を使用してファイルをアップロードするか、ファイルのアップロード元の URL を指定するかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ファイルのアップロード ]</p> </td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL からのファイルの読み込み ] </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL URL]</strong>:変換するファイルの URL を入力します。</li> 
     <li><strong>[!UICONTROL Headers]</strong>:（オプション）リクエストヘッダーを定義します。 これは、例えば、指定した URL で認証が必要な場合に便利です。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Optimization for] </td> 
   <td> <p>特定のターゲットニーズに合わせた最適化プロファイルを選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Web]</strong>:Web の最適化（デフォルト）</p> 
      <ul> 
       <li>Web の冗長データと不要なデータを削除</li> 
       <li>イメージをダウンサンプル、クリップ、インテリジェントに圧縮</li> 
       <li>フォントの結合とサブセット化</li> 
       <li>色の変換RGB</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL 印刷 ]</strong>:印刷の最適化</p> 
      <ul> 
       <li> <p>印刷のために冗長で不要なデータを削除</p> </li> 
       <li> <p>イメージをダウンサンプル、クリップ、インテリジェントに圧縮</p> </li> 
       <li> <p>フォントの結合とサブセット化</p> </li> 
       <li> <p>カラーを CMYK に変換</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL アーカイブ ]</strong>:アーカイブ用の最適化</p> 
      <ul> 
       <li> <p>アーカイブ用に冗長かつ不要なデータを削除</p> </li> 
       <li> <p>画像をインテリジェントに圧縮</p> </li> 
       <li> <p>フォントの結合とサブセット化</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL スキャンされた画像 ]</strong>:スキャンされた画像の最適化</p> 
      <ul> 
       <li> <p>主にラスターPDFで構成される画像に最適化されたプロファイル</p> </li> 
       <li> <p>画質を大幅に低下させることなく画像を圧縮する</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL 最大サイズ縮小 ]</strong>:最大サイズ削減のための最適化</p> 
      <ul> 
       <li> <p>可能な限り最大の圧縮を使用</p> </li> 
       <li> <p>表示品質が低下する可能性がある</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 入力形式 ] </td> 
   <td>最適化する入力ファイルの形式を選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイル名 ]</td> 
   <td> <p>ターゲット出力ファイルのファイル名（拡張子も含む）を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL コンバージョンおよびエンジン固有のオプション ]</td> 
   <td> <p>コンバージョンとエンジン固有のオプションを指定します。 使用可能なオプションを表示するには、 <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] API</a> ドキュメント <code>input_format</code> および <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイルのダウンロード ]</td> 
   <td> <p>モジュールの出力にファイルデータも含める場合は、このオプションを有効にします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### ジョブ

* [[!UICONTROL ジョブの作成（詳細）]](#create-a-job-advanced)
* [[!UICONTROL 新規ジョブイベント]](#new-job-event)
* [[!UICONTROL ジョブのリスト]](#list-jobs)
* [[!UICONTROL ジョブを取得]](#get-a-job)
* [[!UICONTROL ジョブの削除]](#delete-a-job)

#### [!UICONTROL ジョブの作成（詳細）]

このモジュールはジョブを作成します。 1 つのジョブは、 [!UICONTROL 名前] フィールドを使用し、 [!UICONTROL 入力] フィールドに入力します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL CloudConvert] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">接続 [!DNL CloudConvert] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 入力ファイル ]</td> 
   <td> <p>を使用してファイルをアップロードするかどうかを選択します。 [!DNL Workfront Fusion]、またはファイルのアップロード元の URL を指定します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ファイルのアップロード ]</td> 
   <td> <p>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL からのファイルの読み込み ]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL URL]</strong>:処理するファイルの URL を入力します。</li> 
     <li><strong>[!UICONTROL Headers]</strong>:（オプション）リクエストヘッダーを定義します。 これは、例えば、指定した URL で認証が必要な場合に便利です。</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL タスク ]</p> </td> 
   <td> <p>ジョブ内で実行されるタスクを追加します。</p> <p>操作のフィールドの説明は、対応するセクションで確認してください。</p> 
    <ul> 
     <li><a href="#convert-a-file" class="MCXref xref">[!UICONTROL ファイルの変換 ]</a> </li> 
     <li><a href="#capture-a-website" class="MCXref xref">[!UICONTROL Web サイトのキャプチャ ]e</a> </li> 
     <li><a href="#optimize-a-file" class="MCXref xref">[!UICONTROL ファイルの最適化 ]</a> </li> 
     <li><a href="#create-an-archive" class="MCXref xref">[!UICONTROL アーカイブの作成 ]</a> </li> 
     <li><a href="#merge-files" class="MCXref xref">[!UICONTROL ファイルの結合 ]</a> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL コマンドの実行 ]</strong> </p> <p>コマンドの実行の詳細については、 <a href="https://cloudconvert.com/api/v2/command#command-tasks">[!DNL CloudConvert] API ドキュメント</a>.</p> </li> 
     <li> <p><strong>[!UICONTROL 一時 URL へのファイルの書き出し ]</strong> </p> <p> タスク名と入力タスク名を指定します（例：コンバージョン）。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL タグ ] </td> 
   <td> <p>タグを入力します。 タグは、ジョブを識別する任意の文字列です。 これらは効果がなく、ジョブを ID に関連付けるのに使用できます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ジョブの削除]

このモジュールは、すべてのタスクとデータを含むジョブを削除します。

>[!NOTE]
>
>ジョブは、終了後 24 時間後に自動的に削除されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL CloudConvert] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">接続 [!DNL CloudConvert] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Job ID]</td> 
   <td> <p>削除するジョブの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ジョブを取得]

このモジュールは、ジョブの詳細を取得します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL CloudConvert] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">接続 [!DNL CloudConvert] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Job ID]</td> 
   <td> <p>詳細を取得するジョブの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ジョブのリスト]

このモジュールは、アカウントで実行されたすべてのジョブを取得します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL CloudConvert] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">接続 [!DNL CloudConvert] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ステータス ] </td> 
   <td> <p>返されたジョブをフィルターするジョブステータスを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ] </td> 
   <td> <p>1 回の実行サイクルで返されるWorkfront Fusion 2.0 のジョブ数を設定します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 新規ジョブイベント]

トリガー：アカウントまたはタスク内のジョブが作成、完了、または失敗したとき。

>[!NOTE]
>
>* が作成したジョブ [!UICONTROL ジョブの作成（詳細）] モジュールは次のもので構成される *somer* タスク。
>* この [!UICONTROL 新規ジョブイベント] トリガーは、 *個人版* タスクが作成されたか、完了したか、失敗しました。
>

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td>ウェブフック名を入力します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL CloudConvert] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">接続 [!DNL CloudConvert] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力形式 ] </td> 
   <td>キャプチャした Web サイトを PNG、JPG、PDF形式で保存するかどうかを選択します。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL イベント ]</td> 
   <td>ジョブまたはタスクの作成時、完了時、失敗時にモジュールをトリガーするかどうかを選択します。</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* 配列集約を使用する場合（変換するファイル形式が異なるファイルが多数ある場合など）、 **[!UICONTROL 入力形式がわかりません]** オプション [!UICONTROL タスクを追加] ダイアログ。 それ以外の場合は、エラーが返されます。
>* ジョブ内のタスクをリンクしています（名前 > 入力、名前 > 入力…）:
>
>  ![](assets/linking-name-across-jobs-350x808.png)>

### タスク

* [[!UICONTROL タスクを取得]](#get-a-task)
* [[!UICONTROL ファイルのダウンロード]](#download-a-file)
* [[!UICONTROL タスクのリスト]](#list-tasks)
* [[!UICONTROL タスクを再試行]](#retry-a-task)
* [[!UICONTROL タスクのキャンセル]](#cancel-a-task)
* [[!UICONTROL タスクの削除]](#delete-a-task)

#### [!UICONTROL タスクのキャンセル]

このモジュールは、ステータスが「待機中」または「処理中」のタスクをキャンセルします。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL CloudConvert] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">接続 [!DNL CloudConvert] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL タスク ID]</td> 
   <td> <p> キャンセルするタスクの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL タスクの削除]

すべてのデータを含むタスクを削除します。

>[!NOTE]
>
>タスクは、終了してから 24 時間後に自動的に削除されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL CloudConvert] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">接続 [!DNL CloudConvert] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL タスク ID]</td> 
   <td> <p> 削除するタスクの ID を入力（マップ）します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ファイルのダウンロード]

このモジュールは、指定されたタスクからファイル名とファイルデータを取得します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL CloudConvert] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">接続 [!DNL CloudConvert] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL タスク ID]</td> 
   <td> <p> ファイルのダウンロード元のタスクの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL タスクを取得]

このモジュールは、タスクの詳細を取得します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL CloudConvert] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">接続 [!DNL CloudConvert] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL タスク ID]</td> 
   <td> <p>詳細を取得するタスクの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL タスクのリスト]

このモジュールは、フィルター設定に基づいて、アカウント内のすべてのタスクを取得します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL CloudConvert] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">接続 [!DNL CloudConvert] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ステータス ] </td> 
   <td> <p>返されたタスクをフィルターするタスクのステータスを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Job ID] </td> 
   <td> <p>指定したジョブ内のタスクのみを返すように、ジョブ ID を入力またはマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 操作 ] </td> 
   <td> <p>指定した操作のタスクのみを返す操作のタイプを入力します。 </p> <p>注意：[!UICONTROL 可能な操作リスト ] モジュールを使用して、操作を取得します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ] </td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すレコードの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL タスクを再試行]

このモジュールは、別のタスクの設定（ペイロード）に基づいて、新しいタスクを作成します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL CloudConvert] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">接続 [!DNL CloudConvert] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL タスク ID]</td> 
   <td> <p> 新しいタスクを作成するタスクの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### その他

* [[!UICONTROL 情報を取得]](#get-my-info)
* [[!UICONTROL API 呼び出しを実行する]](#make-an-api-call)

#### [!UICONTROL 情報を取得]

現在のユーザーに関する認証済みアカウントの詳細を取得します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>接続方法 [!DNL CloudConvert] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">接続 [!DNL CloudConvert] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL API 呼び出しを実行する]

カスタム API 呼び出しを実行できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ]</td> 
   <td> <p>[Fusion App] アカウントをWorkfront Fusion に接続する手順については、 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Adobe Workfront Fusion への接続の作成 — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>相対パスを入力 <code>https://api.cloudconvert.com/</code>. 例： <code>/v2/tasks</code></p> <p>使用可能なエンドポイントの一覧については、 <a href="https://cloudconvert.com/api/v2">[!DNL CloudConvert] API v2 ドキュメント</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メソッド ]</td> 
   td&gt; <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion 2.0 により、認証ヘッダーが追加されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しのクエリを追加します。</p> <p>例： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で API 呼び出しの本文の内容を追加します。 <code>if</code> JSON で、条件文の外側に引用符を置きます。<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

**例：** タスクのリスト

次の API 呼び出しは、CloudFront アカウントからすべてのタスクを返します。

URL: `/v2/tasks`

メソッド: `GET`

![](assets/cloudconvert-api-example-input.png)

検索結果は、モジュールの「出力」の「 [!UICONTROL バンドル] > [!UICONTROL 本文] > [!UICONTROL データ].

この例では、次の 6 つのタスクが返されました。

![](assets/cloudconvert-api-example-output.png)

## トラブルシューティング {#troubleshooting}

考えられるエラーとその解決策については、次の表を参照してください。

<table style="table-layout:auto">
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>エラー</p> </th> 
   <th>次のステップ</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[!UICONTROL 出力ファイルのサイズが、シナリオで許可されている制限を超えています。]</span> </p> </td> 
   <td> <p>ファイルサイズの制限を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[!UICONTROL 最大コンバージョン時間を超えました。]</span> </p> </td> 
   <td> <p>無料 [!DNL CloudConvert] プランでは、1 日 25 分のコンバージョンが提供されます。 ご利用が無料プランの制限を超えた場合は、（プリペイド）パッケージまたはサブスクリプションに切り替えることができます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[!UICONTROL フレームサイズを読み取れませんでした：1508 にシークできませんでした。 � /output/JLIADSA00137P0.mp3:無効な引数です。]</span> </p> </td> 
   <td> <p>このエラーは、例えば、ファイルを MP3 から WAV に変換する場合に発生します。 正しいファイルだけでなく、ファイルへの参照も見つかるので、正しい領域を選択していることを確認してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL RuntimeError:] </p> <p><span style="font-weight: normal;">[!UICONTROL 繰り返しの最大数を超えました。]</span> </p> </td> 
   <td> <p>対応する [!DNL CloudConvert] のジョブ [!DNL CloudConvert] ダッシュボードのジョブのリストと、ジョブの期間を確認します。</p> <p> <img src="assets/cloudconvert-duration-350x177.png" style="width: 350;height: 177;"> </p> <p>この [!DNL CloudConvert] &gt; [!UICONTROL Convert a File] モジュールのタイムアウトが 3 分に設定されている。 ジョブの期間が 3 分を超える場合 ( 場合によっては、 [!DNL CloudConvert] サービス ) の場合、モジュールは上記のエラーをスローします。</p> <p>この場合、次のいずれかのオプションを検討します。</p> 
    <ul> 
     <li>を有効にします。 <strong>[!UICONTROL 不完全な実行の保存を許可 ]</strong> オプションを使用して、後で手動で解決するために不完全な実行を保存することができます。 必要に応じて、エラー処理ルートを [!DNL CloudConvert] モジュールに [!UICONTROL Break] ディレクティブを設定し、不完全な実行を自動的に解決する。</li> 
     <li>を無効にします。 <strong>[!UICONTROL ファイルをダウンロード ] オプション</strong> 内 [!DNL CloudConvert] &gt; [!UICONTROL ファイルを変換 ] モジュール この場合、モジュールは変換結果を待ちません。 変換結果を取得するには、新しいシナリオを作成し、 [!DNL CloudConvert] &gt; [!UICONTROL 新規ジョブイベント ]トリガー</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## のワークフローの例 [!DNL CloudConvert] コネクタ

>[!INFO]
>
>**例：** MOV から MP4 形式へのビデオの変換
>
>1. 訪問 [https://cloudconvert.com/video-converter](https://>cloudconvert.com/video-converter)
>1. クリック **[!UICONTROL ファイルを選択]** サンプル MOV ファイルを選択します。
>1. の横にあるドロップダウンをクリックします。 **[!UICONTROL 変換先]** を選択します。 **[!UICONTROL MP4]**.
>
>1. 次をクリック： **[!UICONTROL レンチ]** アイコン
>1. 必要に応じて、MP4 圧縮設定を設定します。
>1. クリック **[!UICONTROL 変換]**.
>1. 変換処理が完了したら、「 **[!UICONTROL ダウンロード]**.
>1. 変換後のビデオを確認します。
>1. 手順 5 の最適な変換設定が見つかるまで、手順 1 ～ 8 を繰り返します。
>1. 訪問 [https://cloudconvert.com/api/v2/convert#convert-tasks](https://cloudconvert.com/api/v2/convert#convert-tasks)
>1. 選択 **[!UICONTROL mov]** の **[!UICONTROL input_format]** フィールドに入力します。
>
>1. 選択 **[!UICONTROL mp4]** の **[!UICONTROL output_format]** フィールドに入力します。
>
>1. video_codec、crf など、使用可能なすべてのパラメーターのリスト。 が表示されます。
>1. Workfront Fusion 2.0 で、 **[!UICONTROL CloudConvert]** > **[!UICONTROL ファイルの変換]** モジュールを設定します。
>
>1. モジュールの設定を開きます。
>1. 以下に示すように、モジュールを設定します。
>
>   ![](assets/cloudconvert-mp4-example.png)
>
>1. すべての設定を「コンバージョン」および「エンジン固有のオプション」フィールドに必ず含めてください。手順 5 の各設定で、手順 13 の対応するパラメーターとその対応する値を探します。
