---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Gmail モジュール
description: ' [!DNL Adobe Workfront Fusion]  シナリオでは、Gmail を使用するワークフローを自動化でき、また、Gmail を複数のサードパーティのアプリケーションやサービスに接続できます。'
author: Becky
feature: Workfront Fusion
exl-id: 1987156c-e003-4f99-8913-cb47f77efbfc
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: ht
source-wordcount: '1833'
ht-degree: 100%

---

# [!DNL Gmail] モジュール

[!DNL Adobe Workfront Fusion] のシナリオでは、[!DNL Gmail] を使用するワークフローを自動化したり、複数のサードパーティアプリケーションやサービスに接続したりできます。

シナリオの作成手順が必要な場合は、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) でのシナリオの作成を参照してください。モジュールについて詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md) のモジュールを参照してください。

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion]ライセンス要件なし。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

[!DNL Gmail] モジュールを使用するには、[!DNL Gmail] アカウントが必要です。

## [!DNL Gmail] を [!DNL Workfront Fusion] に接続 {#connect-gmail-to-workfront-fusion}

* [[!DNL G Suite] を使用して  [!DNL Gmail]  を  [!DNL Workfront Fusion]  に接続](#connect-gmail-to-workfront-fusion-usingg-suite)
* [ [!DNL gmail.com]  または  [!DNL googlemail].comを使用して  [!DNL Gmail]  を  [!DNL Workfront Fusion]  に接続](#connect-gmail-to-workfront-fusion-using-gmailcom-or-googlemailcom)

### [!DNL  G Suite] を使用して [!DNL Gmail] を [!DNL Workfront Fusion] に接続 {#connect-gmail-to-workfront-fusion-using-g-suite}

[!DNL G Suite] アカウントの [!UICONTROL Workfront Fusion] への接続について詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md) でのシナリオの作成記事内の[モジュールのアプリまたは web サービスの  [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) への接続を参照してください。

### [!DNL gmail.com] または [!DNL googlemail].com を使用して [!DNL Gmail] を [!DNL Workfront Fusion] に接続 {#connect-gmail-to-workfront-fusion-using-gmail-com-or-googlemail-com}

[!DNL @gmail.com] または [!DNL @googlemail.com] ユーザーは、[!UICONTROL クライアント ID] および[!UICONTROL クライアントの秘密鍵]を取得するために、[ [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) 上で OAuth クライアントを作成する必要があります。

OAuth クライアントを作成し、[!UICONTROL クライアント ID] および[!UICONTROL クライアントの秘密鍵]を取得する方法に関する段階的な手順については、[カスタム OAuth クライアントを使用して Adobe Workfront Fusion を Google Services に接続](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md)を参照してください。

## [!DNL Gmail] モジュールとそのフィールド

[!DNL Gmail] モジュールを設定する際に、[!DNL Workfront Fusion] では、以下にリストされたフィールドが表示されます。これらと共に、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の「[!DNL Gmail]」フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) であるモジュールから別のモジュールへ情報をマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [トリガー](#triggers)
* [アクション](#actions)
* [イテレータ](#iterators)

### トリガー

#### [!UICONTROL メールを監視]

このトリガーモジュールは、処理対象の新しいメールを受信した場合にシナリオを実行します。

このモジュールは、レコードに関連付けられたすべての標準フィールドと、接続を介してアクセスされるカスタムフィールドおよび値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Gmail] アカウントの [!DNL Workfront Fusion] への接続手順については、この記事内の<a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">[!DNL Gmail] の [!UICONTROL Workfront Fusion] への接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>監視するメールフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Filter type] </td> 
   <td> <p>メールの監視に使用するフィルタータイプを選択</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Simple filter]</strong> </p> <p>[!UICONTROL Criteria]、[!UICONTROL Sender Email Address]、[!UICONTROL Subject]、[!UICONTROL Search Phrase] の各フィールドに入力</p> </li> 
     <li> <p> <strong>[!UICONTROL Gmail filter]</strong> </p> <p>「[!UICONTROL Query]」フィールドに、メールのフィルタリングに使用するクエリを入力します。</p> <p>[!DNL Gmail] フィルターについて詳しくは、<a href="https://support.google.com/mail/answer/7190">[!DNL Gmail] ドキュメントの検索演算子</a>を参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Criteria]</td> 
   <td>[!UICONTROL all email]、[!UICONTROL only read emails]、[!UICONTROL only unread] の各メールを監視するかどうかを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Sender email address]</td> 
   <td> <p> メールアドレスを入力して、そのアドレスから送信されたメールのみを監視します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject]</td> 
   <td>テキスト文字列を入力して、件名にそのテキスト文字列が含まれるメールのみを監視します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Search phrase]</td> 
   <td>テキスト文字列を入力して、メールの任意の場所でそのテキスト文字列を持つメールのみを監視します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Mark email message(s) as read when fetched]</td> 
   <td> <p> 取得したメールを既読としてマークするには、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Maximum number of results]</td> 
   <td> <p> [!DNL Workfront Fusion] が 1 回のサイクルで処理する結果の最大数を設定します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL メールを送信]](#send-an-email)
* [[!UICONTROL 下書きを作成]](#create-a-draft)
* [[!UICONTROL メールを既読としてマーク]](#mark-an-email-as-read)
* [[!UICONTROL メールを未読としてマーク]](#mark-an-email-as-unread)
* [[!UICONTROL メールの移動]](#move-an-email)
* [[!UICONTROL メールのコピー]](#copy-an-email)
* [[!UICONTROL メールの削除]](#delete-an-email)
* [[!UICONTROL メールラベルの変更]](#modify-email-labels)

#### [!UICONTROL メールの送信]

このアクションモジュールは、新しいメールを送信します。

メールの受信者を指定します。

モジュールは、メールの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Gmail] アカウントの [!DNL Workfront Fusion] への接続手順については、この記事内の<a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">[!DNL Gmail] の [!DNL Workfront Fusion]</a> への接続を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL From]</td> 
   <td> <p>送信者のメールアドレスを入力またはマッピングします。</p> <p>メモ：入力したメールアドレスが正しくない場合は、お使いのアカウントが、自分のアドレスとは異なるアドレスからメールを送信する権限を持っていない可能性があるので、メッセージの送信時にエラーが発生する場合があります。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL To] </td> 
   <td> <p>「<strong>[!UICONTROL Add]</strong>」をクリックし、各受信者のメールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject] </td> 
   <td> <p>メールの件名を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Content] </td> 
   <td> <p>メールコンテンツ（メッセージ本文）を入力またはマッピングします。HTML タグを使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attachments] </td> 
   <td> <p>「<strong>[!UICONTROL Add]</strong>」をクリックして添付ファイルを追加します。前のモジュールからファイルをマッピングできます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copy recipients]</td> 
   <td> <p> 「<strong>[!UICONTROL Add]</strong>」をクリックし、各コピー受信者のメールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Blind copy recipients]</td> 
   <td> <p> 「<strong>[!UICONTROL Add]</strong>」をクリックし、各ブラインドコピー受信者のメールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下書きの作成]

このアクションモジュールは、新しいメールの下書きを作成し、指定したフォルダーに追加します。

下書きを作成するフォルダーを指定します。

このモジュールは、メールの下書きの ID と関連するフィールドのほか、この接続がアクセスするカスタムフィールドと値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Gmail] アカウントを [!DNL Workfront Fusion] に接続する手順については、この記事の <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">[!DNL Gmail] を [!UICONTROL Workfront Fusion] に接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>下書きを作成する [!DNL Gmail] フォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL To] </td> 
   <td> <p>「<strong>[!UICONTROL Add]</strong>」をクリックし、各受信者のメールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Subject] </td> 
   <td> <p>メールの件名を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Content] </td> 
   <td> <p>メールコンテンツ（メッセージ本文）を入力またはマッピングします。HTML タグを使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Attachments] </td> 
   <td> <p>「<strong>[!UICONTROL Add]</strong>」をクリックして添付ファイルを追加します。前のモジュールからファイルをマッピングできます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Copy recipients]</td> 
   <td> <p> 「<strong>[!UICONTROL Add]</strong>」をクリックし、各コピー受信者のメールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Blind copy recipients]</td> 
   <td> <p> 「<strong>[!UICONTROL Add]</strong>」をクリックし、各ブラインドコピー受信者のメールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メールを既読としてマーク]

このアクションモジュールは、メールを既読としてマークします。

メールの ID とそのフォルダーを指定します。

モジュールは、メールの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Gmail] アカウントの [!DNL Workfront Fusion] への接続手順については、この記事内の<a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">[!DNL Gmail] の [!UICONTROL Workfront Fusion] への接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>メールを格納する [!DNL Gmail] フォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email ID (UID)]</td> 
   <td> <p> メール ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メールを未読としてマーク]

このアクションモジュールは、メールまたはメールの下書きを未読としてマークします。

メールの ID とそのフォルダーを指定します。

モジュールは、メールの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Gmail] アカウントの [!DNL Workfront Fusion] への接続手順については、この記事内の<a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">[!DNL Gmail] の [!UICONTROL Workfront Fusion] への接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>メールを格納する [!DNL Gmail] フォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email ID (UID)] </td> 
   <td> <p>未読としてマークするメールのメール ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メールの移動]

このアクションモジュールは、メールまたはメールの下書きを指定したフォルダーに移動します。

メールのフォルダー、宛先フォルダー、および ID を指定します。

モジュールは、メールの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Gmail] アカウントの [!DNL Workfront Fusion] への接続手順については、この記事内の<a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">[!DNL Gmail] の [!UICONTROL Workfront Fusion] への接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>移動するメールを格納する [!DNL Gmail] ソースフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destination folder]</td> 
   <td> <p> メールの移動先となる [!DNL Gmail] ターゲットフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email ID (UID)]</td> 
   <td> <p> 移動するメールのメール ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メールをコピー]

このアクションモジュールは、メールまたはメールのドラフトを指定したフォルダーにコピーします。

メールのフォルダー、宛先フォルダー、および ID を指定します。

モジュールは、メールの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Gmail] アカウントの [!DNL Workfront Fusion] への接続手順については、この記事内の<a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">[!DNL Gmail] の [!UICONTROL Workfront Fusion] への接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Folder] </td> 
   <td> <p>コピーするメールを含む [!DNL Gmail] ソースフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destination folder]</td> 
   <td> <p>ファイルのコピー先となる [!DNL Gmail] ターゲットフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Email ID (UID)]</td> 
   <td> <p>コピーするメールのメール ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メールを削除]

このアクションモジュールは、指定したフォルダーからメールまたはメールのドラフトを削除します。

モジュールは、メールの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Gmail] アカウントの [!DNL Workfront Fusion] への接続手順については、この記事内の<a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">[!DNL Gmail] の [!UICONTROL Workfront Fusion] への接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL [!DNL Gmail] Message ID]</p> </td> 
   <td> <p>削除する電子メールのメール ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permanently] </td> 
   <td> <p>モジュールがごみ箱フォルダーに移動するのではなく、メールを恒久的に削除できるようにするには、このオプションを有効にします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メールラベルを変更]

このアクションモジュールは、指定したメールメッセージのラベルを変更します。

モジュールは、メールの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。この情報は、シナリオ内の後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection] </td> 
   <td> <p>[!DNL Gmail] アカウントの [!DNL Workfront Fusion] への接続手順については、この記事内の<a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">[!DNL Gmail] の [!UICONTROL Workfront Fusion] への接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Gmail] Message ID]</td> 
   <td> <p> 削除する電子メールのメール ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Labels to add]</p> </td> 
   <td> <p>選択したメールメッセージに追加するラベルを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Labels to remove]</td> 
   <td> <p> 選択したメールメッセージから削除するラベルを選択またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>「[!UICONTROL 追加するラベル]」および「[!UICONTROL 削除するラベル]」フィールドは、ユーザーが作成したラベルのみを読み込みます。

### イテレータ

#### [!UICONTROL 添付ファイルを反復]

メールの添付ファイルを反復処理できます。各添付ファイルは、モジュールの出力内の個別のバンドルです。詳しくは、[Adobe Workfront Fusion のイテレータモジュール](../../workfront-fusion/modules/iterator-module.md)を参照してください。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source module] </td> 
   <td> <p>添付ファイルをイテレーションするモジュールを選択します。 </p> </td> 
  </tr> 
 </tbody> 
</table>
