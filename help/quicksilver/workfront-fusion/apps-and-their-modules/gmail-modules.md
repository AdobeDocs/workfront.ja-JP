---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Gmail モジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオの場合、Gmail を使用するワークフローを自動化でき、また、Gmail を複数のサードパーティのアプリケーションやサービスに接続できます。
author: Becky
feature: Workfront Fusion
exl-id: 1987156c-e003-4f99-8913-cb47f77efbfc
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1833'
ht-degree: 0%

---

# [!DNL Gmail] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Gmail]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

シナリオの作成手順については、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). モジュールについて詳しくは、 [のモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

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

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 前提条件

使用する [!DNL Gmail] モジュールの場合、 [!DNL Gmail] アカウント

## 接続 [!DNL Gmail] から [!DNL Workfront Fusion] {#connect-gmail-to-workfront-fusion}

* [接続 [!DNL Gmail] から [!DNL Workfront Fusion] [!DNL G Suite] の使用](#connect-gmail-to-workfront-fusion-usingg-suite)
* [接続 [!DNL Gmail] から [!DNL Workfront Fusion] using [!DNL gmail.com] または [!DNL googlemail].com](#connect-gmail-to-workfront-fusion-using-gmailcom-or-googlemailcom)

### 接続 [!DNL Gmail] から [!DNL Workfront Fusion] using[!DNL  G Suite] {#connect-gmail-to-workfront-fusion-using-g-suite}

接続方法 [!DNL G Suite] アカウント [!UICONTROL Workfront Fusion]を参照してください。 [モジュールのアプリまたは Web サービスの接続先 [!DNL Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md#connect) 記事内 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

### 接続 [!DNL Gmail] から [!DNL Workfront Fusion] using [!DNL gmail.com] または [!DNL googlemail].com {#connect-gmail-to-workfront-fusion-using-gmail-com-or-googlemail-com}

次の場合、 [!DNL @gmail.com] または [!DNL @googlemail.com] ユーザーは、 [の [!DNL Google Cloud Platform]](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) 得るために [!UICONTROL クライアント ID] および [!UICONTROL クライアント秘密鍵].

OAuth クライアントを作成し、 [!UICONTROL クライアント ID] および [!UICONTROL クライアント秘密鍵]を参照してください。 [カスタム OAuth クライアントを使用してAdobe Workfront Fusion をGoogle Services に接続する](../../workfront-fusion/connections/connect-fusion-to-google-using-oauth.md).

## [!DNL Gmail] モジュールとそのフィールド

設定時に [!DNL Gmail] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Gmail] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [トリガー](#triggers)
* [アクション](#actions)
* [イテレータ](#iterators)

### トリガー

#### [!UICONTROL メールを見る]

このトリガーモジュールは、処理対象の新しい E メールを受信した場合にシナリオを実行します。

このモジュールは、レコードまたはレコードに関連付けられているすべての標準フィールドと、接続がアクセスするカスタムフィールドおよび値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Gmail] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">接続 [!DNL Gmail] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>監視する電子メールフォルダを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フィルタータイプ ] </td> 
   <td> <p>メールの監視に使用するフィルターの種類を選択します</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 簡易フィルター ]</strong> </p> <p>[!UICONTROL 条件 ]、[!UICONTROL Sender Email Address]、[!UICONTROL Subject]、[!UICONTROL Search Phrase] の各フィールドに入力します。</p> </li> 
     <li> <p> <strong>[!UICONTROL Gmail フィルター ]</strong> </p> <p>「[!UICONTROL クエリ ]」フィールドに、電子メールのフィルタリングに使用するクエリを入力します。</p> <p>詳しくは、 [!DNL Gmail] フィルター、詳しくは、 <a href="https://support.google.com/mail/answer/7190">検索演算子</a> 内 [!DNL Gmail] ドキュメント。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 条件 ]</td> 
   <td>[!UICONTROL すべての電子メール ]、[!UICONTROL は電子メールの読み取りのみ ]、[!UICONTROL のみ未読 ] の電子メールを視聴するかどうかを選択します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 送信者の電子メールアドレス ]</td> 
   <td> <p> 電子メールアドレスを入力して、そのアドレスから送信された電子メールのみを監視します。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 件名 ]</td> 
   <td>テキスト文字列を入力して、件名にそのテキスト文字列が含まれる電子メールのみを監視します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 検索フレーズ ]</td> 
   <td>テキスト文字列を入力して、そのテキスト文字列を持つ電子メールを電子メールの任意の場所に監視します。</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 電子メールメッセージを取得時に既読としてマーク ]</td> 
   <td> <p> 取得したメールを既読としてマークするには、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 結果の最大数 ]</td> 
   <td> <p> 結果の最大数を設定 [!DNL Workfront Fusion] は、1 サイクルの間にと連携します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL 電子メールを送信]](#send-an-email)
* [[!UICONTROL 下書きの作成]](#create-a-draft)
* [[!UICONTROL メールを既読としてマーク]](#mark-an-email-as-read)
* [[!UICONTROL メールを未読としてマーク]](#mark-an-email-as-unread)
* [[!UICONTROL E メールの移動]](#move-an-email)
* [[!UICONTROL E メールのコピー]](#copy-an-email)
* [[!UICONTROL E メールの削除]](#delete-an-email)
* [[!UICONTROL 電子メールラベルを変更]](#modify-email-labels)

#### [!UICONTROL 電子メールを送信]

このアクションモジュールは、新しい電子メールを送信します。

電子メールの受信者を指定します。

モジュールは、電子メールの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Gmail] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">接続 [!DNL Gmail] から [!DNL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 元 ]</td> 
   <td> <p>送信者の E メールアドレスを入力またはマッピングします。</p> <p>注意：入力した電子メールアドレスが正しくない場合、お使いのアカウントには、自分のアドレスとは異なるアドレスから電子メールを送信する権限がない可能性があるので、メッセージの送信時にエラーが発生する場合があります。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL から ] </td> 
   <td> <p>クリック <strong>[!UICONTROL 追加 ]</strong>」をクリックし、各受信者の電子メールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 件名 ] </td> 
   <td> <p>電子メールの件名を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL コンテンツ ] </td> 
   <td> <p>E メールコンテンツ（メッセージ本文）を入力またはマッピングします。 HTMLタグを使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 添付ファイル ] </td> 
   <td> <p>クリック <strong>[!UICONTROL 追加 ]</strong> 添付ファイルを追加します。 前のモジュールからファイルをマッピングできます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 受信者をコピー ]</td> 
   <td> <p> クリック <strong>[!UICONTROL 追加 ]</strong>」をクリックし、コピーの各受信者の電子メールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ブラインドコピーの受信者 ]</td> 
   <td> <p> クリック <strong>[!UICONTROL 追加 ]</strong>」をクリックし、各ブラインドコピーの受信者の電子メールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下書きの作成]

このアクションモジュールは、新しい電子メールの下書きを作成し、指定したフォルダーに追加します。

ドラフトを作成するフォルダーを指定します。

モジュールは、電子メールドラフトの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Gmail] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">接続 [!DNL Gmail] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>を選択します。 [!DNL Gmail] 下書きを作成するフォルダーです。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL から ] </td> 
   <td> <p>クリック <strong>[!UICONTROL 追加 ]</strong>」をクリックし、各受信者の電子メールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 件名 ] </td> 
   <td> <p>電子メールの件名を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL コンテンツ ] </td> 
   <td> <p>E メールコンテンツ（メッセージ本文）を入力またはマッピングします。 HTMLタグを使用できます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 添付ファイル ] </td> 
   <td> <p>クリック <strong>[!UICONTROL 追加 ]</strong> 添付ファイルを追加します。 前のモジュールからファイルをマッピングできます。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 受信者をコピー ]</td> 
   <td> <p> クリック <strong>[!UICONTROL 追加 ]</strong>」をクリックし、コピーの各受信者の電子メールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL ブラインドコピーの受信者 ]</td> 
   <td> <p> クリック <strong>[!UICONTROL 追加 ]</strong>」をクリックし、各ブラインドコピーの受信者の電子メールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メールを既読としてマーク]

このアクションモジュールは、電子メールを既読としてマークします。

電子メールの ID とそのフォルダーを指定します。

モジュールは、電子メールの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Gmail] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">接続 [!DNL Gmail] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>を選択します。 [!DNL Gmail] 電子メールを格納するフォルダー。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 電子メール ID (UID)]</td> 
   <td> <p> 電子メール ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メールを未読としてマーク]

このアクションモジュールは、メールまたはメールの下書きを未読としてマークします。

電子メールの ID とそのフォルダーを指定します。

モジュールは、電子メールの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Gmail] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">接続 [!DNL Gmail] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>を選択します。 [!DNL Gmail] 電子メールを格納するフォルダー。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 電子メール ID (UID)] </td> 
   <td> <p>未読としてマークする電子メールの電子メール ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL E メールの移動]

このアクションモジュールは、電子メールまたは電子メール下書きを指定したフォルダーに移動します。

電子メールのフォルダー、宛先フォルダーおよび ID を指定します。

モジュールは、電子メールの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Gmail] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">接続 [!DNL Gmail] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>を選択します。 [!DNL Gmail] 移動する電子メールを含むソースフォルダー。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 保存先フォルダー ]</td> 
   <td> <p> を選択します。 [!DNL Gmail] 電子メールの移動先のターゲットフォルダーです。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 電子メール ID (UID)]</td> 
   <td> <p> 移動する電子メールの電子メール ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL E メールのコピー]

このアクションモジュールは、電子メールまたは電子メールの下書きを指定したフォルダーにコピーします。

電子メールのフォルダー、宛先フォルダーおよび ID を指定します。

モジュールは、電子メールの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Gmail] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">接続 [!DNL Gmail] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL フォルダー ] </td> 
   <td> <p>を選択します。 [!DNL Gmail] コピーする電子メールを含むソースフォルダー。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 保存先フォルダー ]</td> 
   <td> <p>を選択します。 [!DNL Gmail] 電子メールのコピー先となるターゲットフォルダーです。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 電子メール ID (UID)]</td> 
   <td> <p>コピーする電子メールの電子メール ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL E メールの削除]

このアクションモジュールは、指定したフォルダーから電子メールまたは電子メール下書きを削除します。

モジュールは、電子メールの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Gmail] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">接続 [!DNL Gmail] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL [!DNL Gmail] メッセージ ID]</p> </td> 
   <td> <p>削除する電子メールの電子メール ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Permanently] </td> 
   <td> <p>モジュールがごみ箱フォルダーに移動するのではなく、電子メールを恒久的に削除できるようにするには、このオプションを有効にします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 電子メールラベルを変更]

このアクションモジュールは、指定した電子メールメッセージのラベルを変更します。

モジュールは、電子メールの ID と関連するフィールドのほか、接続がアクセスするカスタムフィールドと値を返します。 この情報は、シナリオの後続のモジュールにマッピングできます。

このモジュールを設定する際には、次のフィールドが表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Gmail] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-gmail-to-workfront-fusion" class="MCXref xref">接続 [!DNL Gmail] から [!UICONTROL Workfront Fusion]</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL [!DNL Gmail] メッセージ ID]</td> 
   <td> <p> 削除する電子メールの電子メール ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL ラベルを追加 ]</p> </td> 
   <td> <p>選択した電子メールメッセージに追加するラベルを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL 削除するラベル ]</td> 
   <td> <p> 選択した電子メールメッセージから削除するラベルを選択またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>[!UICONTROL 追加するラベル] および [!UICONTROL 削除するラベル] フィールドは、ユーザーが作成したラベルのみを読み込みます。

### イテレータ

#### [!UICONTROL 添付ファイルを繰り返し]

E メールの添付ファイルを繰り返し処理できます。 各添付ファイルは、モジュールの出力内の個別のバンドルです。 詳しくは、 [Adobe Workfront Fusion の Iterator モジュール](../../workfront-fusion/modules/iterator-module.md).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL ソースモジュール ] </td> 
   <td> <p>添付ファイルを繰り返すモジュールを選択します。 </p> </td> 
  </tr> 
 </tbody> 
</table>
