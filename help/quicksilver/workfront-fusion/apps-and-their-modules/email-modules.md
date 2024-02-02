---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: メールモジュール
description: ' [!DNL Adobe Workfront Fusion]  のシナリオでは、メールアカウントを複数のサードパーティアプリケーションやサービスに接続できます。これにより、IMAP 経由でメールをダウンロードしたり、SMTP 経由でメールを送信したり、新しい下書きを作成したり、フォルダー間でメールを移動およびコピーしたり、メールを既読または未読としてマークしたり、メールを削除したりすることができます。'
author: Becky
feature: Workfront Fusion
exl-id: 384ba60a-d79e-4126-a247-6d67b5154ede
source-git-commit: 8b4182ae2b32488a02cacc16fcb6a246fcb571fd
workflow-type: ht
source-wordcount: '2626'
ht-degree: 100%

---

# メールモジュール

[!DNL Adobe Workfront Fusion] のシナリオでは、メールアカウントを複数のサードパーティアプリケーションやサービスに接続できます。これにより、IMAP 経由でメールをダウンロードしたり、SMTP 経由でメールを送信したり、新しい下書きを作成したり、フォルダー間でメールを移動およびコピーしたり、メールを既読または未読としてマークしたり、メールを削除したりすることができます。

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
   <p>現在のライセンス要件：[!DNL Workfront Fusion] ライセンス要件はありません。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランがある場合、この記事で説明する機能を使用するには、組織は [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。[!DNL Workfront Fusion] は、[!UICONTROL Ultimate] [!DNL Workfront] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明する機能を使用するには、組織は [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] のライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion]  のライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## Workfront Fusion にメールを接続 {#connect-your-email-to-workfront-fusion}

* [Google に接続](#connect-to-google)
* [他のメールサービス（SMAP）に接続](#connect-to-other-email-services-smap)

### [!DNL Google] に接続

[!DNL Google] アカウントへの接続を必要とするメールモジュールを含むシナリオを作成するには、このオプションを使用します。これは、スコープが制限されたアカウントです。

[!DNL Google] アカウントへの接続を、メールモジュール内から直接作成できます。

1. 任意のメールモジュールで、[!UICONTROL 接続]フィールドの横にある「**[!UICONTROL 追加]**」をクリックします。
1. 接続タイプとして「**[!DNL Google]**」を選択します。
1. 接続に名前を入力します。
1. （オプション）[!UICONTROL [!DNL Google] クライアント ID] および[!UICONTROL クライアントシークレット]を入力します。
1. 「**[!UICONTROL 続行]**」をクリックし、接続を作成して、モジュールに戻ります。

### 他のメールサービス（SMAP）に接続

SMAP 接続を使用すると、メールボックスにリモートでアクセスし、メールボックス内のメッセージを読み取ったり操作したりできます。SMAP 接続は、ほとんどのメールモジュールで使用されます。

1. 任意のメールモジュールで、[!UICONTROL 接続]フィールドの横にある「**[!UICONTROL 追加]**」をクリックします。
1. 接続タイプとして「**[!UICONTROL その他（SMTP）]**」を選択します。
1. 接続の&#x200B;**[!UICONTROL 名前]**&#x200B;を入力します。
1. リストから&#x200B;**[!UICONTROL メールプロバイダー]**&#x200B;を選択します。メールプロバイダーがリストにない場合は、「その他」を選択します。
1. **[!UICONTROL メールアドレス]**、**[!UICONTROL 氏名]**、**[!UICONTROL ユーザー名]**、**[!UICONTROL パスワード]**&#x200B;を入力します。
1. （条件付き）プロバイダーがリストにない場合は、「**[!UICONTROL SMTP サーバー]**」および「**[!UICONTROL ポート]**」を入力し、**[!UICONTROL セキュア接続（TLS）を使用]**&#x200B;するかどうかを指定します。この情報を見つけるには、メールボックスの「[!UICONTROL ヘルプ]」セクションを確認してください。この情報が不明な場合は、メールサービスプロバイダーにお問い合わせください。
1. 「**[!UICONTROL 続行]**」をクリックし、接続を作成して、モジュールに戻ります。

## [!UICONTROL メール]モジュールとそのフィールド

[!UICONTROL メール]モジュールを設定すると、[!DNL Workfront Fusion] には次のフィールドが表示されます。これらと共に、アプリやサービスのアクセスレベルなどの要因に応じて、追加のフィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

シナリオの別のモジュールで一部のメールフィールドを使用した場合、それらのメールフィールドには既にデータが含まれている場合があります。詳しくは、メールのヘルプドキュメントを参照してください。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) で、あるモジュールから別のモジュールに情報をマッピングを参照してください。

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>[!UICONTROL メール ID（UID）]と呼ばれる一意のメール ID は、メールの識別子です。メール ID は、メールの各フォルダーに固有です。

* [トリガー](#triggers)
* [アクション](#actions)
* [イテレータ](#iterators)

### トリガー

#### [!UICONTROL メールを監視]

指定された条件に従って処理するために、新しいメールを受け取ったときにトリガーされます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>メールアカウントを [!UICONTROL Workfront Fusion] に接続する方法について詳しくは、この記事の <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">[!UICONTROL Workfront Fusion] にメールを接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] </td> 
   <td> <p>監視するメールを含むフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Criteria]</p> </td> 
   <td> <p>メールを監視する条件を選択します。</p> 
    <ul> 
     <li>[!UICONTROL All Emails]</li> 
     <li>[!UICONTROL Only Read Emails]</li> 
     <li>[!UICONTROL Only Unread Emails]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sender Email Address] </td> 
   <td> <p>監視するメールの送信者のメールアドレスを入力します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Recipient Email Address]</td> 
   <td> <p> 監視するメールの受信者のメールアドレスを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>監視するメールの件名を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Phrase] </td> 
   <td> <p>キーワードを入力して、特定のフレーズを含むメールのみを監視します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mark message(s) as read when fetched]</td> 
   <td> <p>詳細を取得した後、未読のメールを既読としてマークするには、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of results]</td> 
   <td> <p> 1 回のシナリオ実行サイクルで [!DNL Workfront Fusion] が返す必要のある最大メール数。</p> </td> 
  </tr> 
 </tbody> 
</table>

### アクション

* [[!UICONTROL メールの送信]](#send-an-email)
* [[!UICONTROL 下書きの作成]](#create-a-draft)
* [[!UICONTROL メールを既読としてマーク]](#mark-an-email-as-read)
* [[!UICONTROL メールを未読としてマーク]](#mark-an-email-as-unread)
* [[!UICONTROL メールの移動]](#move-an-email)
* [[!UICONTROL メールのコピー]](#copy-an-email)
* [[!UICONTROL メールの削除]](#delete-an-email)
* [[!UICONTROL メールの取得]](#get-emails)

#### [!UICONTROL メールの送信]

新しいメールを送信します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>メールアカウントを [!DNL Workfront Fusion] に接続する方法について詳しくは、この記事の<a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">[!UICONTROL Workfront Fusion] へのメールの接続</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Save Message after Sending]</td> 
   <td>メールメッセージが送信されると、メールボックスに保存されます。[!DNL Workfront Fusion] を使用して送信されたメールを <i>[!UICONTROL Sent mail]</i> フォルダーまたはメールボックス内の別のフォルダーに保存する場合は、このオプションを有効にします。一部のメールサービス（[!DNL Gmail] など）では、送信したメッセージが自動的に保存されます。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL To] </td> 
   <td> <p>メールの送信先のメールアドレスを追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>メールの件名行を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Content Type]</p> </td> 
   <td> <p>メールの [!UICONTROL content] タイプを選択します。</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL Plaintext]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content] </td> 
   <td> <p>「[!UICONTROL Content Type]」フィールドで選択した内容に応じて、HTML タグを使用してHTML 形式で、またはプレーンテキストでメールコンテンツを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>添付ファイルの追加：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>ファイル名を入力します。例えば、sample.doc のように指定します。</p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>添付ファイルをアップロードするフォルダーのパスを入力します。</p> </li> 
     <li> <p><strong>[!UICONTROL Content-ID]</strong> </p> <p>[!UICONTROL content ID] を入力して、コンテンツに添付ファイル（画像）を挿入します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copy Recipient] </td> 
   <td> <p>このメールのコピーを送信する 1 つ以上のメールアドレスを入力またはマッピングします。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Blind Copy Recipient]</td> 
   <td> <p> メールアドレスをメールに表示せずに、このメールのコピーを送信する 1 つ以上のメールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL From] </td> 
   <td> <p>メールの「[!UICONTROL From]」フィールドに表示されるメールアドレス（および必要に応じて名前）を入力またはマッピングします。 </p> <p>重要：正しい構文を使用してください（<code>name@email.com</code> または <code>"Name" name@email.com</code>）。</p> <p>メモ：通常は、[!DNL Workfront Fusion] は、接続を作成する際に入力したメールアドレスを送信者のアドレスとして使用します。他のメールアドレスを入力すると、メッセージの送信時にエラーが発生する場合があります。これは、お使いのアカウントに、自身のアドレスとは異なるアドレスからメールを送信する権限がない可能性があるためです。（例：<code>test@mail.com</code> または "<code>John Bush" test@email.com</code>）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Sender]</p> </td> 
   <td> <p>メールの「[!UICONTROL Sender]」フィールドに表示されるメールアドレスを入力またはマッピングします。</p> <p>ヒント：このフィールドと「送信者」フィールドのどちらを使用するかが不明な場合は、「送信者」フィールドを選択することをお勧めします。</p> <p>重要：正しい構文を使用してください（<code>name@email.com</code> または <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reply-To]</td> 
   <td> <p> このメールに対する返信を「送信者」アドレスとは別のアドレスに送信する場合は、このメールに対する返信先のメールアドレスを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL In-Reply-To]</td> 
   <td> <p> 特定のメールに返信する場合は、返信先のメールの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL References] </td> 
   <td> <p>スレッド内のすべての返信のメッセージ ID を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Priority]</p> </td> 
   <td> <p>メールの優先度を選択します。</p> 
    <ul> 
     <li>[!UICONTROL High]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Low]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
   <td> <p>ヘッダーを追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Key]</strong> </p> <p>キーを追加します。例えば、[!UICONTROL Sender]、[!UICONTROL Date]、[!UICONTROL To] などです。</p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>キーの値を入力します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ドラフトの作成]

選択したフォルダーに新しいドラフトを作成して追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>メールアカウントを [!UICONTROL Workfront Fusion] に接続する方法について詳しくは、この記事の <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">[!UICONTROL Workfront Fusion] へのメールの接続</a>を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>ドラフトメールを作成するフォルダーを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL To] </td> 
   <td> <p>メールの送信先となるメールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>メールの件名行を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Content Type]</p> </td> 
   <td> <p>メールのコンテンツタイプを選択します。</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL Plain Text]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Content] </td> 
   <td> <p>「[!UICONTROL Content Type]」フィールドで選択した内容に応じて、HTML タグを使用してHTML 形式で、またはプレーンテキストでメールコンテンツを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachments]</p> </td> 
   <td> <p>添付ファイルの追加：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File name]</strong> </p> <p>ファイル名を入力します。例えば、sample.doc のように指定します。</p> </li> 
     <li> <p><strong>[!UICONTROL Data]</strong> </p> <p>添付ファイルをアップロードするフォルダーのパスを入力します。</p> </li> 
     <li> <p><strong>[!UICONTROL Content-ID]</strong> </p> <p>コンテンツ ID を入力して、添付ファイル（画像）をコンテンツに挿入します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copy Recipient] </td> 
   <td> <p>このメールのコピーを送信する 1 つ以上のメールアドレスを入力またはマッピングします。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Blind Copy Recipient]</td> 
   <td> <p> メールアドレスをメールに表示せずに、このメールのコピーを送信する 1 つ以上のメールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL From] </td> 
   <td> <p>メールの「[!UICONTROL From]」フィールドに表示されるメールアドレス（および必要に応じて名前）を入力またはマッピングします。 </p> <p>重要：正しい構文を使用してください（<code>name@email.com</code> または <code>"Name" name@email.com</code>）。</p> <p>注意：通常は、[!DNL Workfront Fusion] は、接続を作成する際に入力したメールアドレスを送信者のアドレスとして使用します。他のメールアドレスを入力すると、メッセージの送信時にエラーが発生する場合があります。これは、お使いのアカウントに、自身のアドレスとは異なるアドレスからメールを送信する権限がない可能性があるためです。（例：<code>test@mail.com</code> または "<code>John Bush" test@email.com</code>）。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Sender]</p> </td> 
   <td> <p>メールの「[!UICONTROL Sender]」フィールドに表示されるメールアドレスを入力またはマッピングします。</p> <p>ヒント：このフィールドと「送信者」フィールドのどちらを使用するかが不明な場合は、「送信者」フィールドを選択することをお勧めします。</p> <p>重要：正しい構文を使用してください（<code>name@email.com</code> または <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Reply-To]</td> 
   <td> <p> このメールに対する返信を「[!UICONTROL from]」アドレスとは別のアドレスに送信する場合は、このメールに対する返信先のメールアドレスを入力します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL In-Reply-To]</td> 
   <td> <p> 特定のメールに返信する場合は、返信先のメールの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL References] </td> 
   <td> <p>スレッド内のすべての返信のメッセージ ID を入力します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Priority]</p> </td> 
   <td> <p>メールの優先度を選択します。</p> 
    <ul> 
     <li>[!UICONTROL High]</li> 
     <li>[!UICONTROL Normal]</li> 
     <li>[!UICONTROL Low]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
   <td> <p>ヘッダーを追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Key]</strong> </p> <p>キーを追加します。例えば、「送信者」、「日付」、「宛先」などです。</p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>キーの値を入力します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メールを既読としてマーク]

選択したフォルダー内のメールまたは下書きを既読としてマークするには、[!UICONTROL 既読]フラグを設定します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>メールアカウントを [!UICONTROL Workfront Fusion] に接続する方法について詳しくは、この記事の <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">[!UICONTROL Workfront Fusion] へのメールの接続</a>を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>既読としてマークするメールのフォルダーを選択します。（例：プライマリ）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Email ID (UID)]</p> </td> 
   <td> <p>既読としてマークするメールの UID を入力します。</p> <p>メールの UID は、[!UICONTROL Email]／[!UICONTROL Watch Email] モジュールまたは [!UICONTROL Search Email] モジュールを使用して取得できます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メールを未読としてマーク]

選択したフォルダー内のメールまたは下書きを未読としてマークするには、「未読」フラグを設定します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>メールアカウントを [!UICONTROL Workfront Fusion] に接続する方法について詳しくは、この記事の <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">[!UICONTROL Workfront Fusion] へのメールの接続</a>を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>未読としてマークするメールのフォルダーを選択します。（例：プライマリ）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Email ID (UID)]</p> </td> 
   <td> <p>未読としてマークするメールの UID を入力します。</p> <p>メールの UID は、[!UICONTROL Email]／[!UICONTROL Watch Email] モジュールまたは [!UICONTROL Search Email] モジュールを使用して取得できます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メールの移動]

選択したメールまたは下書きを選択したフォルダーに移動します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>メールアカウントを [!UICONTROL Workfront Fusion] に接続する方法について詳しくは、この記事の <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">[!UICONTROL Workfront Fusion] へのメールの接続</a>を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Folder]</td> 
   <td>移動元のメールを含むフォルダーを選択します。（例：プライマリ）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination Folder]</td> 
   <td> <p> メールを追加するフォルダーを選択します。（例： ワーク）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Email ID (UID)]</p> </td> 
   <td> <p>宛先フォルダーに移動するメールの UID を入力します。</p> <p>メールの UID は、[!UICONTROL Email]／[!UICONTROL Watch Email] モジュールまたは [!UICONTROL Search Email] モジュールを使用して取得できます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メールのコピー]

選択したフォルダーにメールまたは下書きをコピーします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>メールアカウントを [!UICONTROL Workfront Fusion] に接続する方法について詳しくは、この記事の <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">[!UICONTROL Workfront Fusion] へのメールの接続</a>を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Folder]</td> 
   <td>メールのコピー元のフォルダーを選択します。（例：プライマリ）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Destination Folder]</td> 
   <td> <p> メールのコピー先のフォルダーを選択します。（例： ワーク）。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Email ID (UID)]</p> </td> 
   <td> <p>宛先フォルダーにコピーするメールのメール UID を入力します。</p> <p>メールの UID は、[!UICONTROL Email]／[!UICONTROL Watch Email] モジュールまたは [!UICONTROL Search Email] モジュールを使用して取得できます。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メールの削除]

選択したフォルダーからメールまたはドラフトを削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>メールアカウントを [!UICONTROL Workfront Fusion] に接続する方法について詳しくは、この記事の <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">[!UICONTROL Workfront Fusion] へのメールの接続</a>を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td>削除するメールのフォルダーを選択します。（例：プライマリ）。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Email ID (UID)]</p> </td> 
   <td> <p>削除するメールのメール UID を入力します。</p> <p>メールの UID は、[!UICONTROL Email]／[!UICONTROL Watch Email] モジュールまたは [!UICONTROL Search Email] モジュールを使用して取得できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expunge]</td> 
   <td> <p>このオプションを有効にすると、モジュールは現在開いているメールボックスで [!UICONTROL Deleted] としてフラグ付けされたすべてのメッセージを完全に削除できます。</p> <p>メモ：[!DNL Gmail] の場合、この動作は [!UICONTROL Settings]／「[!UICONTROL Forwarding POP/IMAP in IMAP access]」セクションの設定によって決まります。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メールの取得]

指定された条件に一致するメールを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>メールアカウントを [!UICONTROL Workfront Fusion] に接続する方法について詳しくは、この記事の <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">[!UICONTROL Workfront Fusion] へのメールの接続</a>を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder] </td> 
   <td> <p>取得するメールを含むフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Mark message(s) as read when fetched] </td> 
   <td> <p>詳細を取得した後、未読のメールを既読としてマークするには、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Criteria]</p> </td> 
   <td> <p>メールを取得する条件を選択します。</p> 
    <ul> 
     <li>[!UICONTROL All Emails]</li> 
     <li>[!UICONTROL Only Read Emails]</li> 
     <li>[!UICONTROL Only Unread Emails]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sender Email Address] </td> 
   <td> <p>メールを取得する送信者のメールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Recipient Email Address]</td> 
   <td> <p> メールを取得する受信者のメールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL From date] </td> 
   <td> <p>指定した日付以降に処理されるメールを取得する日付を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Before date]</td> 
   <td> <p> 指定した日付以前に処理されたメールを取得する日付を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subject] </td> 
   <td> <p>取得するメールの件名を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Phrase] </td> 
   <td> <p>キーワードを入力またはマッピングして、特定の語句を含むメールのみを取得します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email ID (UID)]</td> 
   <td> <p> 詳細を取得するメールのメール ID（UID）を入力します。</p> <p>メールの UID は、[!DNL Workfront Fusion] の[!UICONTROL  Watch Email] モジュールまたは [!UICONTROL Search Email] モジュールを使用して取得できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of results]</td> 
   <td> <p> 1 回のシナリオ実行サイクルで [!DNL Workfront Fusion] が返す必要のある最大メール数。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Continue the execution of the route even if the module returns no results]</td> 
   <td> <p> 結果が返されない場合でもモジュールの実行を続行する場合は、選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### イテレータ

#### [!UICONTROL 添付ファイルの反復]

受け取った添付ファイルを 1 つずつ繰り返します。

メールイテレーターモジュールを使用すると、メールの添付ファイルを個別に管理できます。例えば、メールを監視して添付ファイル付きのメールを繰り返し処理し、アラートを受け取るように設定できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source module]</td> 
   <td> <p>繰り返し処理を行う添付ファイルが含まれるメールを出力するモジュールを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

イテレーターの詳細については、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) のイテレーターモジュールを参照してください。
