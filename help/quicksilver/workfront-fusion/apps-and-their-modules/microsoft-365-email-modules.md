---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Microsoft Office 365 メール
description: 内 [!DNL Adobe Workfront Fusion] シナリオの場合、Microsoft Office 365 E メールを使用するワークフローを自動化し、それを複数のサードパーティのアプリケーションやサービスに接続することができます。
author: Becky
feature: Workfront Fusion
exl-id: 29b69e8c-a889-441e-a052-287f1db2052d
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '1838'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Email]

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!UICONTROL Microsoft Office 365 メール]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

を使用するには [!UICONTROL Office 365 メール] と [!DNL Adobe Workfront Fusion]の場合、 [!UICONTROL Office 365 アカウント]. 作成はwww.office.comでおこなえます。

接続方法 [!UICONTROL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 [への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順](../../workfront-fusion/connections/connect-to-fusion-general.md)

同意すると、 [!UICONTROL Workfront Fusion] シナリオの作成を続行できる管理ページです。

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## 前提条件

使用する [!DNL Microsoft Office 365 Email] モジュールの場合、 [!DNL Microsoft Office 365 Email] アカウント

## [!DNL Microsoft Office 365 Email] モジュールとそのフィールド

設定時に [!DNL Microsoft Office 365 Email] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Microsoft Office 365 Email] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [メッセージ](#message)
* [下書きメッセージ](#draft-message)
* [添付](#attachment)
* [その他](#other)

### メッセージ

* [[!UICONTROL メッセージを見る]](#watch-messages)
* [[!UICONTROL メッセージを検索]](#search-messages)
* [[!UICONTROL メッセージを取得]](#get-a-message)
* [[!UICONTROL メッセージの作成と送信]](#create-and-send-a-message)
* [[!UICONTROL メッセージの移動]](#move-a-message)
* [[!UICONTROL メッセージの削除]](#delete-a-message)

#### [!UICONTROL メッセージを見る]

トリガー：新しい電子メールメッセージが送信または受信されたとき。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL メッセージを監視 ]</p> </td> 
   <td> <p>監視するメッセージを選択：</p> 
    <ul> 
     <li>[!UICONTROL 未読のみ ]</li> 
     <li>[!UICONTROL 読み取り専用 ]</li> 
     <li>[!UICONTROL すべて ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メールフォルダ ]</td> 
   <td> <p>監視するメッセージを含むフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 検索 ]</td> 
   <td>検索クエリを入力します。 検索クエリの作成方法について詳しくは、 [!DNL Microsoft] サポート記事 <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">でのメールと担当者の検索 [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ] </td> 
   <td> <p>メッセージの最大数を入力 [!DNL Workfront Fusion] は、1 回のシナリオ実行サイクルで返されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メッセージを検索]

特定の条件に基づいてメッセージを検索します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メールフォルダ ]</td> 
   <td> <p>検索するメッセージを含むフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 検索 ]</td> 
   <td>検索クエリを入力します。 検索クエリの作成方法について詳しくは、 [!DNL Microsoft] サポート記事 <a href="https://support.microsoft.com/en-us/office/search-mail-and-people-in-outlook-com-88108edf-028e-4306-b87e-7400bbb40aa7?ui=en-us&amp;rs=en-us&amp;ad=us">でのメールと担当者の検索 [!DNL Outlook.com]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order by]</td> 
   <td> <p>結果の並べ替え方法を選択します。</p> 
    <ul> 
     <li>[!UICONTROL 件名（昇順または降順）]</li> 
     <li>[!UICONTROL 作成日時（昇順または降順）]</li> 
     <li>[!UICONTROL 最終変更日時（昇順または降順）]</li> 
     <li>[!UICONTROL 受信日時（昇順または降順）]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>メッセージの最大数を入力 [!DNL Workfront Fusion] は、1 回のシナリオ実行サイクルで返されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メッセージを取得]

特定のメッセージのメタデータを取得します

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メッセージ ID]</td> 
   <td> <p> メタデータを取得するメッセージの ID を選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL MIME コンテンツを取得 ]</td> 
   <td>メッセージの MIME コンテンツに関するデータを取得するには、このオプションを有効にします。 [!UICONTROL MIME] コンテンツには、画像、オーディオ、ビデオ、その他のタイプのファイルが含まれる場合があります。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メッセージの作成と送信]

電子メールメッセージを作成して送信します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 件名 ]</td> 
   <td> <p>メッセージの件名行を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 本文コンテンツタイプ ]</td> 
   <td>メッセージの本文の内容を「HTML」と「テキスト」のどちらにするかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文コンテンツ ]</td> 
   <td> <p>メールのメッセージ本文テキストを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 重要度 ]</td> 
   <td> <p>メールの重要度を選択</p> 
    <ul> 
     <li>[!UICONTROL 低 ]</li> 
     <li>[!UICONTROL 標準 ]</li> 
     <li>[!UICONTROL 高 ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL から受信者へ ]</p> </td> 
   <td> <p>メッセージの送信先の電子メールアドレスを追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 名前 ]</strong> </p> <p>連絡先の名前を入力</p> </li> 
     <li> <p><strong>[!UICONTROL 電子メールアドレス ]</strong> </p> <p>連絡先のメールアドレスを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC 受信者 ]</p> </td> 
   <td> <p>メッセージのコピーを受信する受信者を追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 名前 ]</strong> </p> <p>連絡先の名前を入力</p> </li> 
     <li> <p><strong>[!UICONTROL 電子メールアドレス ]</strong> </p> <p>連絡先のメールアドレスを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Bcc 受信者 ]</p> </td> 
   <td> <p>他の受信者に名前や E メールアドレスの表示を許可することなく、メッセージにコピーする受信者を追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 名前 ]</strong> </p> <p>連絡先の名前を入力</p> </li> 
     <li> <p><strong>[!UICONTROL 電子メールアドレス ]</strong> </p> <p>連絡先のメールアドレスを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 添付ファイル ]</p> </td> 
   <td> <p>添付ファイルを E メールに追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL ファイル名 ]</strong> </p> <p>ファイル名を入力します。 例: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL データ ]</strong> </p> <p>フィールドにファイルデータを入力するか、ファイルのソースをマッピングします。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL インターネットメッセージヘッダー ]</td> 
   <td> <p>E メールのメッセージヘッダーを追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 名前 ]</strong> </p> <p>ヘッダーの名前を入力</p> </li> 
     <li> <p><strong>[!UICONTROL 電子メールアドレス ]</strong> </p> <p>ヘッダーの値を入力します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メッセージの移動]

メールメッセージをメールボックス内の選択したフォルダに移動します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メッセージ ID]</td> 
   <td> <p> 別のフォルダーに移動するメッセージの ID を選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メールフォルダ ] </td> 
   <td> <p>メッセージを移動するフォルダーの ID を選択またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メッセージの削除]

既存の電子メールメッセージを削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メッセージ ID]</td> 
   <td> <p> 削除するメッセージの ID を選択またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### 下書きメッセージ

* [下書きメッセージの作成](#create-a-draft-message)
* [下書きメッセージの送信](#send-a-draft-message)
* [メッセージの更新](#update-a-message)

#### [!UICONTROL 下書きメッセージの作成]

新しい電子メールメッセージを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 件名 ]</td> 
   <td> <p>メッセージの件名行を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文コンテンツタイプ ]</td> 
   <td>メッセージの本文の内容を「HTML」と「テキスト」のどちらにするかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文コンテンツ ]</td> 
   <td> <p>E メールのメッセージ本文テキストを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 重要度 ]</td> 
   <td> <p>メールの重要度を選択</p> 
    <ul> 
     <li>[!UICONTROL 低 ]</li> 
     <li>[!UICONTROL 標準 ]</li> 
     <li>[!UICONTROL 高 ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL から受信者へ ]</p> </td> 
   <td> <p>メッセージの送信先となる受信者を追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 名前 ]</strong> </p> <p>連絡先の名前を入力</p> </li> 
     <li> <p><strong>[!UICONTROL 電子メールアドレス ]</strong> </p> <p>連絡先のメールアドレスを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC 受信者 ]</p> </td> 
   <td> <p>受信者を追加メッセージのコピーを受け取る受信者：</p> 
    <ul> 
     <li> <p><strong>名前</strong> </p> <p>連絡先の名前を入力</p> </li> 
     <li> <p><strong>E メール アドレス</strong> </p> <p>連絡先のメールアドレスを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Bcc 受信者</p> </td> 
   <td> <p>他の受信者に名前や E メールアドレスの表示を許可することなく、メッセージにコピーする受信者を追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 名前 ]</strong> </p> <p>連絡先の名前を入力</p> </li> 
     <li> <p><strong>[!UICONTROL 電子メールアドレス ]</strong> </p> <p>連絡先のメールアドレスを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 添付ファイル ]</p> </td> 
   <td> <p>添付ファイルを E メールに追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL ファイル名 ]</strong> </p> <p>ファイル名を入力します。 例: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL データ ]</strong> </p> <p>フィールドにファイルデータを入力するか、ファイルのソースをマッピングします。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下書きメッセージの送信]

現在下書きになっている電子メールメッセージを送信します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 下書きメッセージ ID]</td> 
   <td> <p> 送信する下書きのメッセージ ID を選択またはマッピングします。</p> </td> 
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
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メッセージ ID を入力 ]</td> 
   <td> <p>更新するメッセージを識別する方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>メッセージ ID を入力またはマッピングします。</p> </li> 
     <li> <p><strong>[!UICONTROL リストから選択 ]</strong> </p> <p>更新するメッセージを含むフォルダーを選択し、メッセージを選択します</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 件名 ]</td> 
   <td> <p>メッセージの件名行を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文コンテンツ ]</td> 
   <td> <p>E メールのメッセージ本文テキストを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 重要度 ]</td> 
   <td> <p>メールの重要度を選択</p> 
    <ul> 
     <li>[!UICONTROL 低 ]</li> 
     <li>[!UICONTROL 標準 ]</li> 
     <li>[!UICONTROL 高 ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL から受信者へ ]</p> </td> 
   <td> <p>メッセージの送信先の電子メールアドレスを追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 名前 ]</strong> </p> <p>連絡先の名前を入力</p> </li> 
     <li> <p><strong>[!UICONTROL 電子メールアドレス ]</strong> </p> <p>連絡先のメールアドレスを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL CC 受信者 ]</p> </td> 
   <td> <p>受信者を追加メッセージのコピーを受け取る受信者：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 名前 ]</strong> </p> <p>連絡先の名前を入力</p> </li> 
     <li> <p><strong>[!UICONTROL 電子メールアドレス ]</strong> </p> <p>連絡先のメールアドレスを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Bcc 受信者 ]</p> </td> 
   <td> <p>他の受信者に名前や E メールアドレスの表示を許可することなく、メッセージにコピーする受信者を追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 名前 ]</strong> </p> <p>連絡先の名前を入力</p> </li> 
     <li> <p><strong>[!UICONTROL 電子メールアドレス ]</strong> </p> <p>連絡先のメールアドレスを入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 添付ファイル ]</p> </td> 
   <td> <p>添付ファイルを E メールに追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL ファイル名 ]</strong> </p> <p>ファイル名を入力します。 例: <code>sample.doc</code></p> </li> 
     <li> <p><strong>[!UICONTROL データ ]</strong> </p> <p>フィールドにファイルデータを入力するか、ファイルのソースをマッピングします。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 読み取りとしてマーク ]</td> 
   <td>このオプションを有効にすると、更新されたメッセージを既読としてマークします。</td> 
  </tr> 
 </tbody> 
</table>

### 添付

* [[!UICONTROL 添付ファイルをリスト]](#list-attachments)
* [[!UICONTROL 添付ファイルのダウンロード]](#download-an-attachment)

#### [!UICONTROL 添付ファイルをリスト]

このモジュールは、指定されたメッセージに属する添付ファイルのリストを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メッセージ ID]</td> 
   <td> <p> 添付ファイルを取得するメッセージの ID を選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
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
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メッセージ ID]</td> 
   <td> <p> ダウンロードする添付ファイルを含むメッセージの ID を選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 添付ファイル ID]</td> 
   <td> <p>ダウンロードする添付ファイルの ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### その他

* [[!UICONTROL API 呼び出しを実行する]](#make-an-api-call)
* [[!UICONTROL 添付ファイルを追加]](#add-an-attachment)

#### [!UICONTROL API 呼び出しを実行する]

このモジュールでは、カスタム API 呼び出しを実行できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>相対パスを入力 <code>https://graph.microsoft.com</code>. 例:<code> /v1.0/me/messages</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL メソッド ]</p> </td> 
   td&gt; <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。例： <code>{"Content-type":"application/json"}</code>. [!DNL Workfront Fusion] によって、認証ヘッダーが追加されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ]</td> 
   <td> <p> 標準の JSON オブジェクトの形式で、API 呼び出しのクエリを追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文のコンテンツを追加します。</p> <p>メモ:  <p>条件文 ( <code>if</code> JSON で、条件文の外側に引用符を置きます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 添付ファイルを追加]

このモジュールは、メッセージに大きな添付ファイルを追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Office 365] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メッセージ ID]</td> 
   <td> <p> 添付ファイルを追加するメッセージの ID を選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td> <p>前のモジュールからファイルを選択するか、ソースファイルの名前とデータをマップします。</p> </td> 
  </tr> 
 </tbody> 
</table>
