---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Microsoft Office 365 メール
description: ' [!DNL Adobe Workfront Fusion]  のシナリオ内では、Microsoft Office 365 メールを使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりすることができます。'
author: Becky
feature: Workfront Fusion
exl-id: 29b69e8c-a889-441e-a052-287f1db2052d
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '1886'
ht-degree: 100%

---

# [!DNL Microsoft Office 365 Email]

[!DNL Adobe Workfront Fusion] シナリオ内では、[!UICONTROL Microsoft Office 365 メール]を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりすることができます。

[!DNL Adobe Workfront Fusion] で [!UICONTROL Office 365 メール] を使用するには、[!UICONTROL Office 365 アカウント] が必要です。アカウントは www.office.com で作成できます。

[!UICONTROL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、[ [!DNL Adobe Workfront Fusion]  への接続の作成 - 基本手順](../../workfront-fusion/connections/connect-to-fusion-general.md)を参照してください。

同意すると、リダイレクトされて [!UICONTROL Workfront Fusion] 管理ページに戻り、シナリオの作成を続けることができます。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td>
  <td> <p>[!UICONTROL Pro] 以降</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!DNL Adobe Workfront] の [!UICONTROL Select] または [!UICONTROL Prime] のプランを利用する場合、この記事で説明する機能を使用するには [!DNL Adobe Workfront] と [!DNL Adobe Workfront Fusion] を組織で購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明する機能を使用するには、組織で [!DNL Adobe Workfront] と [!DNL Adobe Workfront Fusion] を購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion]ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

[!DNL Microsoft Office 365 Email] モジュールを使用するには、[!DNL Microsoft Office 365 Email] アカウントが必要です。

## [!DNL Microsoft Office 365 Email] モジュールとそのフィールド

[!DNL Microsoft Office 365 Email] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL Microsoft Office 365 Email] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) のモジュール間での情報のマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [メッセージ](#message)
* [ドラフトメッセージ](#draft-message)
* [添付ファイル](#attachment)
* [その他](#other)

### メッセージ

* [[!UICONTROL メッセージの監視]](#watch-messages)
* [[!UICONTROL メッセージの検索]](#search-messages)
* [[!UICONTROL メッセージの取得]](#get-a-message)
* [[!UICONTROL メッセージの作成と送信]](#create-and-send-a-message)
* [[!UICONTROL メッセージの移動]](#move-a-message)
* [[!UICONTROL メッセージの削除]](#delete-a-message)

#### [!UICONTROL メッセージの監視]

新しい電子メールメッセージが送信または受信されるとトリガーされます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Watch Messages]</p> </td> 
   <td> <p>監視するメッセージを選択します。</p> 
    <ul> 
     <li>[!UICONTROL Only Unread]</li> 
     <li>[!UICONTROL Only read]</li> 
     <li>[!UICONTROL All]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mail Folder]</td> 
   <td> <p>監視するメッセージが含まれているフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>検索クエリを入力します。検索クエリの作成方法について詳しくは、[!DNL Microsoft]サポート記事の<a href="https://support.microsoft.com/ja-jp/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=ja-jp&amp;rs=ja-jp&amp;ad=jp">[!DNL Outlook.com]</a> でメールと人物を検索を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>1 回のシナリオ実行サイクルで [!DNL Workfront Fusion] が返すメッセージの最大数 を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メッセージの検索]

特定の基準に基づいてメッセージを検索します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mail Folder]</td> 
   <td> <p>検索するメッセージを含んだフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search]</td> 
   <td>検索クエリを入力します。検索クエリの記述方法については、[!DNL Microsoft] サポート記事の「<a href="https://support.microsoft.com/ja-jp/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=ja-jp&amp;rs=ja-jp&amp;ad=jp">[!DNL Outlook.com]</a> でメールや連絡先を検索する」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
   <td> <p>結果の並べ替え方法を選択します。</p> 
    <ul> 
     <li>[!UICONTROL Subject (Ascending or descending)]</li> 
     <li>[!UICONTROL Created Date Time (Ascending or descending)]</li> 
     <li>[!UICONTROL Last Modified Date Time (Ascending or descending)]</li> 
     <li>[!UICONTROL Received Date Time (Ascending or descending)]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>1 回のシナリオ実行サイクルで [!DNL Workfront Fusion] から返されるメッセージの最大数を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メッセージの取得]

特定のメッセージのメタデータを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> メタデータを取得するメッセージの ID を選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Get MIME contents]</td> 
   <td>メッセージの MIME コンテンツに関するデータを取得するには、このオプションを有効にします。[!UICONTROL MIME] コンテンツには、画像、オーディオ、ビデオまたはその他のファイルタイプが含まれる可能性があります。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メッセージの作成と送信]

メールメッセージを作成して送信します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>メッセージの件名行を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Body Content Type]</td> 
   <td>メッセージの本文の内容を HTML にするかテキストにするかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content]</td> 
   <td> <p>メールのメッセージ本文テキストを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>メールの重要度を次の中から選択します。</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL To Recipients]</p> </td> 
   <td> <p>メッセージの送信先のメールアドレスを追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>連絡先の名前を入力します。</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>連絡先のメールアドレスを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>メッセージのコピーを受け取る受信者を追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>連絡先の名前を入力します。</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>連絡先のメールアドレスを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Bcc Recipients]</p> </td> 
   <td> <p>他の受信者には名前やメールアドレスが表示されないようにしてメッセージのコピーを受け取る受信者を追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>連絡先の名前を入力します。</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>連絡先のメールアドレスを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>添付ファイルをメールに追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>ファイル名を入力します。例： <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>フィールドにファイルデータを入力するか、ファイルのソースをマッピングします。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Internet Message Headers]</td> 
   <td> <p>メールのメッセージヘッダーを追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>ヘッダーの名前を入力します。</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>ヘッダーの値を入力します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メッセージの移動]

メールボックス内の選択されたフォルダーにメールメッセージを移動します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> 別のフォルダーに移動するメッセージの ID を選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mail Folder] </td> 
   <td> <p>メッセージを移動するフォルダーの ID を選択またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メッセージの削除]

既存のメールメッセージを削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する方法について詳しくは、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> 削除するメッセージの ID を選択またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### ドラフトメッセージ

* [ドラフトメッセージの作成](#create-a-draft-message)
* [ドラフトメッセージの送信](#send-a-draft-message)
* [メッセージを更新](#update-a-message)

#### [!UICONTROL ドラフトメッセージの作成]

新しいメールメッセージを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>メッセージの件名行を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body Content Type]</td> 
   <td>メッセージの本文の内容を HTML にするかテキストにするかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content]</td> 
   <td> <p>メールのメッセージ本文テキストを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>メールの重要度を次の中から選択します。</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL To Recipients]</p> </td> 
   <td> <p>メッセージの送信先となる受信者を追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>連絡先の名前を入力します。</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>連絡先のメールアドレスを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>メッセージを受け取る受信者を追加します。</p> 
    <ul> 
     <li> <p><strong>名前</strong> </p> <p>連絡先の名前を入力します。</p> </li> 
     <li> <p><strong>メールアドレス</strong> </p> <p>連絡先のメールアドレスを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>BCC 受信者</p> </td> 
   <td> <p>他の受信者には名前やメールアドレスが表示されないようにしてメッセージのコピーを受け取る受信者を追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>連絡先の名前を入力します。</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>連絡先のメールアドレスを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>添付ファイルをメールに追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>ファイル名を入力します。例： <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>フィールドにファイルデータを入力するか、ファイルのソースをマッピングします。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ドラフトメッセージの送信]

現在ドラフトとなっているメールメッセージを送信します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Draft Message ID]</td> 
   <td> <p> 送信するドラフトのメッセージ ID を選択またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メッセージの更新]

既存のメッセージを更新します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する方法について詳しくは、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a message ID]</td> 
   <td> <p>更新するメッセージを識別する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter Manually]</strong> </p> <p>メッセージ ID を入力またはマッピングします。</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>更新するメッセージを含むフォルダーを選択し、メッセージを選択します</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject]</td> 
   <td> <p>メッセージの件名行を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body content]</td> 
   <td> <p>メールのメッセージ本文テキストを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importance]</td> 
   <td> <p>メールの重要度を次の中から選択します。</p> 
    <ul> 
     <li>[!UICONTROL Low]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL High]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL To Recipients]</p> </td> 
   <td> <p>メッセージの送信先のメールアドレスを追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>連絡先の名前を入力します。</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>連絡先のメールアドレスを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC Recipients]</p> </td> 
   <td> <p>メッセージを受け取る受信者を追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>連絡先の名前を入力します。</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>連絡先のメールアドレスを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Bcc Recipients]</p> </td> 
   <td> <p>他の受信者には名前やメールアドレスが表示されないようにしてメッセージのコピーを受け取る受信者を追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Name]</strong> </p> <p>連絡先の名前を入力します。</p> </li> 
     <li> <p><strong>[!UICONTROL Email Address]</strong> </p> <p>連絡先のメールアドレスを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>添付ファイルをメールに追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>ファイル名を入力します。例： <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>フィールドにファイルデータを入力するか、ファイルのソースをマッピングします。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mark it as Read]</td> 
   <td>このオプションを有効にすると、更新されたメッセージが既読としてマークされます。</td> 
  </tr> 
 </tbody> 
</table>

### 添付ファイル

* [[!UICONTROL 添付ファイルをリスト]](#list-attachments)
* [[!UICONTROL 添付ファイルのダウンロード]](#download-an-attachment)

#### [!UICONTROL 添付ファイルをリスト]

このモジュールは、指定されたメッセージに属する添付ファイルのリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> 添付ファイルを取得するメッセージの ID を選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>各シナリオの実行サイクル中にモジュールが返す添付ファイルの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 添付ファイルのダウンロード]

このモジュールは、指定された添付ファイルをダウンロードします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> ダウンロードする添付ファイルを含むメッセージの ID を選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Attachment ID]</td> 
   <td> <p>ダウンロードする添付ファイルの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### その他

* [[!UICONTROL API 呼び出しの実行]](#make-an-api-call)
* [[!UICONTROL 添付ファイルの追加]](#add-an-attachment)

#### [!UICONTROL API 呼び出しの実行]

このモジュールでは、カスタム API 呼び出しを実行できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Office 365] アカウントを [!DNL Workfront Fusion] に接続する手順については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion] への接続の作成 - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p><code>https://graph.microsoft.com</code> への相対パスを入力します。例：<code> /v1.0/me/messages</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   td&gt; <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">[!DNL Adobe Workfront Fusion]</a> での HTTP リクエストメソッドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。例：<code>{"Content-type":"application/json"}</code>。[!DNL Workfront Fusion] が認証ヘッダーを追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p> API 呼び出しのクエリを標準 JSON オブジェクトの形式で追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文の内容を追加します。</p> <p>メモ：  <p>JSON で <code>if</code> などの条件ステートメントを使用する場合、条件ステートメントの外側に引用符を置きます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 添付ファイルの追加]

このモジュールは、メッセージにサイズの大きい添付ファイルを追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Office 365] アカウントの [!DNL Workfront Fusion] への接続方法については、<a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">接続の作成[!DNL Adobe Workfront Fusion] - 基本手順</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> 添付ファイルを追加するメッセージの ID を選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td> <p>以前のモジュールからファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </td> 
  </tr> 
 </tbody> 
</table>
