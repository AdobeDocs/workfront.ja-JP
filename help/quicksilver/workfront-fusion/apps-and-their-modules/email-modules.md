---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: E メールモジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオの場合は、電子メールアカウントを複数のサードパーティのアプリケーションやサービスに接続できます。IMAP 経由での電子メールのダウンロード、SMTP 経由での電子メールの送信、新しい下書きの作成、別のフォルダへの電子メールの移動とコピー、電子メールの削除が可能です。
author: Becky
feature: Workfront Fusion
exl-id: 384ba60a-d79e-4126-a247-6d67b5154ede
source-git-commit: ea19c2a58bac322c804fca3f6bb7d7147efa4d9a
workflow-type: tm+mt
source-wordcount: '2578'
ht-degree: 0%

---

# E メールモジュール

内 [!DNL Adobe Workfront Fusion] シナリオの場合は、電子メールアカウントを複数のサードパーティのアプリケーションやサービスに接続できます。IMAP 経由での電子メールのダウンロード、SMTP 経由での電子メールの送信、新しい下書きの作成、別のフォルダへの電子メールの移動とコピー、電子メールの削除が可能です。

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

## 電子メールをWorkfront Fusion に接続 {#connect-your-email-to-workfront-fusion}

* [Googleに接続](#connect-to-google)
* [他の電子メールサービス (SMAP) に接続](#connect-to-other-email-services-smap)

### 接続先 [!DNL Google]

このオプションを使用して、 [!DNL Google] アカウント これは、スコープが制限されたアカウントです。

次に、 [!DNL Google] アカウントを電子メールモジュール内から直接アクセスできます。

1. 任意の電子メールモジュールで、 **[!UICONTROL 追加]** の横 [!UICONTROL 接続] フィールドに入力します。
1. 選択 **[!DNL Google]** 接続タイプとして。
1. 接続の名前を入力します。
1. （オプション） [!UICONTROL [!DNL Google] クライアント ID] および [!UICONTROL クライアント秘密鍵].
1. クリック **[!UICONTROL 続行]** 接続を作成し、モジュールに戻ります。

### 他の電子メールサービス (SMAP) に接続

SMAP 接続を使用すると、メールボックスにリモートでアクセスし、メールボックス内のメッセージを読み取ったり操作したりできます。 SMAP 接続は、ほとんどの E メールモジュールで使用されます。

1. 任意の電子メールモジュールで、 **[!UICONTROL 追加]** の横 [!UICONTROL 接続] フィールドに入力します。
1. 選択 **[!UICONTROL その他 (SMTP)]** 接続タイプとして。
1. を入力します。 **[!UICONTROL 名前]** 接続に対して。
1. を選択します。 **[!UICONTROL E メールプロバイダー]** を選択します。 電子メールプロバイダーがリストにない場合は、「その他」を選択します。
1. を入力します。 **[!UICONTROL 電子メールアドレス]**, **[!UICONTROL 氏名]**、 **[!UICONTROL ユーザー名]**、および **[!UICONTROL パスワード]**.
1. （条件付き）プロバイダーがリストにない場合は、 **[!UICONTROL SMTP サーバー]** および **[!UICONTROL ポート]**&#x200B;をクリックし、 **[!UICONTROL セキュア接続 (TLS) を使用]**. この情報を見つけるには、 [!UICONTROL ヘルプ] メールボックスのセクション。 この情報が不明な場合は、電子メールサービスプロバイダーにお問い合わせください。
1. クリック **[!UICONTROL 続行]** 接続を作成し、モジュールに戻ります。

## [!UICONTROL 電子メール] モジュールとそのフィールド

設定時に [!UICONTROL 電子メール] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、アプリやサービスでのアクセスレベルなどの要因に応じて、追加のフィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

シナリオの別のモジュールで使用したので、一部の E メールフィールドには既にデータが含まれている場合があります。 詳しくは、電子メールのヘルプドキュメントを参照してください。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

>[!NOTE]
>
>「 」と呼ばれる一意の電子メール ID[!UICONTROL 電子メール ID (UID)]「 」は E メールの識別子です。 電子メール ID は、電子メールのフォルダーごとに固有です。

* [トリガー](#triggers)
* [アクション](#actions)
* [イテレータ](#iterators)

### トリガー

#### [!UICONTROL メールを見る]

トリガー：指定された条件に従って処理するために新しい E メールを受け取ったとき。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>電子メールアカウントを [!UICONTROL Workfront Fusion] に接続する手順については、 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">電子メールを [!UICONTROL Workfront Fusion] に接続</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ] </td> 
   <td> <p>監視する電子メールを含むフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 条件 ]</p> </td> 
   <td> <p>E メールを監視する条件を選択します。</p> 
    <ul> 
     <li>[!UICONTROL すべての電子メール ]</li> 
     <li>[!UICONTROL 電子メールの読み取りのみ ]</li> 
     <li>[!UICONTROL 未読メールのみ ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 送信者の電子メールアドレス ] </td> 
   <td> <p>監視するメールの送信者のメールアドレスを入力します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 受信者の電子メールアドレス ]</td> 
   <td> <p> 監視する E メールの受信者の E メールアドレスを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 件名 ] </td> 
   <td> <p>視聴する電子メールの件名を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フレーズ ] </td> 
   <td> <p>キーワードを入力して、特定のフレーズを含む電子メールのみを視聴します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 取得時にメッセージを既読としてマーク ]</td> 
   <td> <p>詳細を取得した後、未読のメールを既読としてマークするには、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 結果の最大数 ]</td> 
   <td> <p> 電子メールの最大数 [!DNL Workfront Fusion] は、1 回のシナリオ実行サイクルで返されます。</p> </td> 
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

新しい電子メールを送信します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>電子メールアカウントをに接続する手順については、 [!DNL Workfront Fusion]を参照してください。 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">電子メールを [!UICONTROL Workfront Fusion] に接続</a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 送信後にメッセージを保存 ]</td> 
   <td>電子メールメッセージが送信されると、メールボックスに保存されます。 次を使用して送信したメールを保存する場合は、このオプションを有効にします： [!DNL Workfront Fusion] から <i>[!UICONTROL 送信済みメール ]</i> フォルダー、またはメールボックス内の別のフォルダー。 一部の電子メールサービス ( 例： [!DNL Gmail]、送信したメッセージを自動的に保存します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL から ] </td> 
   <td> <p>E メールの送信先の E メールアドレスを追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 件名 ] </td> 
   <td> <p>電子メールの件名行を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL コンテンツタイプ ]</p> </td> 
   <td> <p>E メールの [!UICONTROL コンテンツ ] タイプを選択します。</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL 平文 ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL コンテンツ ] </td> 
   <td> <p>「[!UICONTROL コンテンツタイプ ]」フィールドで選択した内容に応じて、HTMLタグを使用してHTML形式で、またはプレーンテキストで E メールコンテンツを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 添付ファイル ]</p> </td> 
   <td> <p>添付ファイルの追加：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL ファイル名 ]</strong> </p> <p>ファイル名を入力します。 例えば、sample.doc のように指定します。</p> </li> 
     <li> <p><strong>[!UICONTROL データ ]</strong> </p> <p>添付ファイルをアップロードするフォルダーのパスを入力します。</p> </li> 
     <li> <p><strong>[!UICONTROL Content-ID]</strong> </p> <p>[!UICONTROL コンテンツ ID] を入力して、コンテンツに添付ファイル（画像）を挿入します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 受信者をコピー ] </td> 
   <td> <p>このメールのコピーを送信する 1 つ以上のメールアドレスを入力またはマッピングします。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ブラインドコピーの受信者 ]</td> 
   <td> <p> 電子メールアドレスを電子メールに表示せずに、この電子メールのコピーを送信する 1 つ以上の電子メールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 元 ] </td> 
   <td> <p>電子メールの [!UICONTROL 送信者 ] フィールドに表示される電子メールアドレス（および必要に応じて名前）を入力またはマッピングします。 </p> <p>重要：正しい構文を使用します。 <code>name@email.com</code> または <code>"Name" name@email.com</code>.</p> <p>注意：通常、 [!DNL Workfront Fusion] は、接続を作成する際に入力した電子メールアドレスを送信者のアドレスとして使用します。 他の電子メールアドレスを入力すると、自分のアドレスとは異なるアドレスから電子メールを送信する権限がアカウントにない可能性があるので、メッセージの送信時にエラーが発生する場合があります。 例： <code>test@mail.com</code> または"<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Sender]</p> </td> 
   <td> <p>電子メールの [!UICONTROL Sender] フィールドに表示される電子メールアドレスを入力またはマッピングします。</p> <p>ヒント：このフィールドと「開始日」フィールドのどちらを使用するかが不明な場合は、「開始日」フィールドを選択することをお勧めします。</p> <p>重要：正しい構文を使用します。 <code>name@email.com</code> または <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 返信先 ]</td> 
   <td> <p> このメールに対する返信を「差出人」アドレスとは別のアドレスに送信する場合は、このメールに対する返信先のメールアドレスを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL In-Reply-To]</td> 
   <td> <p> 特定の電子メールに返信する場合は、返信先の電子メールの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 参照 ] </td> 
   <td> <p>スレッド内のすべての返信のメッセージ ID を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 優先度 ]</p> </td> 
   <td> <p>E メールの優先度を選択：</p> 
    <ul> 
     <li>[!UICONTROL 高 ]</li> 
     <li>[!UICONTROL 標準 ]</li> 
     <li>[!UICONTROL 低 ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
   <td> <p>ヘッダーを追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL キー ]</strong> </p> <p>キーを追加します。 例えば、[!UICONTROL Sender]、[!UICONTROL Date]、[!UICONTROL To] などです。</p> </li> 
     <li> <p><strong>[!UICONTROL 値 ]</strong> </p> <p>キーの値を入力します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 下書きの作成]

選択したフォルダーに新しい下書きを作成して追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>電子メールアカウントを [!UICONTROL Workfront Fusion] に接続する手順については、 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">電子メールを [!UICONTROL Workfront Fusion] に接続</a> 」を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ]</td> 
   <td>下書きメールを作成するフォルダーを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL から ] </td> 
   <td> <p>電子メールを送信する電子メールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 件名 ] </td> 
   <td> <p>電子メールの件名行を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL コンテンツタイプ ]</p> </td> 
   <td> <p>E メールのコンテンツタイプを選択します。</p> 
    <ul> 
     <li>HTML</li> 
     <li>[!UICONTROL プレーンテキスト ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL コンテンツ ] </td> 
   <td> <p>「[!UICONTROL コンテンツタイプ ]」フィールドで選択した内容に応じて、HTMLタグを使用してHTML形式で、またはプレーンテキストで E メールコンテンツを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 添付ファイル ]</p> </td> 
   <td> <p>添付ファイルの追加：</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL ファイル名 ]</strong> </p> <p>ファイル名を入力します。 例えば、sample.doc のように指定します。</p> </li> 
     <li> <p><strong>[!UICONTROL データ ]</strong> </p> <p>添付ファイルをアップロードするフォルダーのパスを入力します。</p> </li> 
     <li> <p><strong>[!UICONTROL Content-ID]</strong> </p> <p>コンテンツ ID を入力して、添付ファイル（画像）をコンテンツに挿入します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 受信者をコピー ] </td> 
   <td> <p>このメールのコピーを送信する 1 つ以上のメールアドレスを入力またはマッピングします。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ブラインドコピーの受信者 ]</td> 
   <td> <p> 電子メールアドレスを電子メールに表示せずに、この電子メールのコピーを送信する 1 つ以上の電子メールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 元 ] </td> 
   <td> <p>電子メールの [!UICONTROL 送信者 ] フィールドに表示される電子メールアドレス（および必要に応じて名前）を入力またはマッピングします。 </p> <p>重要：正しい構文を使用します。 <code>name@email.com</code> または <code>"Name" name@email.com</code>.</p> <p>注意：通常、 [!DNL Workfront Fusion] は、接続を作成する際に入力した電子メールアドレスを送信者のアドレスとして使用します。 他の電子メールアドレスを入力すると、自分のアドレスとは異なるアドレスから電子メールを送信する権限がアカウントにない可能性があるので、メッセージの送信時にエラーが発生する場合があります。 例： <code>test@mail.com</code> または"<code>John Bush" test@email.com</code>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Sender]</p> </td> 
   <td> <p>電子メールの [!UICONTROL Sender] フィールドに表示される電子メールアドレスを入力またはマッピングします。</p> <p>ヒント：このフィールドと「開始日」フィールドのどちらを使用するかが不明な場合は、「開始日」フィールドを選択することをお勧めします。</p> <p>重要：正しい構文を使用します。 <code>name@email.com</code> または <code>"Name" name@email.com</code></p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 返信先 ]</td> 
   <td> <p> この電子メールに対する返信を「[!UICONTROL from]」アドレスとは別のアドレスに送信する場合は、この電子メールに対する返信を送信する電子メールアドレスを入力します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL In-Reply-To]</td> 
   <td> <p> 特定の電子メールに返信する場合は、返信先の電子メールの ID を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 参照 ] </td> 
   <td> <p>スレッド内のすべての返信のメッセージ ID を入力します。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL 優先度 ]</p> </td> 
   <td> <p>E メールの優先度を選択：</p> 
    <ul> 
     <li>[!UICONTROL 高 ]</li> 
     <li>[!UICONTROL 標準 ]</li> 
     <li>[!UICONTROL 低 ]</li> 
    </ul> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Headers]</p> </td> 
   <td> <p>ヘッダーを追加します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL キー ]</strong> </p> <p>キーを追加します。 例えば、「送信者」、「日付」、「終了日」などです。</p> </li> 
     <li> <p><strong>[!UICONTROL 値 ]</strong> </p> <p>キーの値を入力します。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メールを既読としてマーク]

選択したフォルダー内のメールまたは下書きを既読としてマークするには、 [!UICONTROL 読み取り] フラグ。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>電子メールアカウントを [!UICONTROL Workfront Fusion] に接続する手順については、 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">電子メールを [!UICONTROL Workfront Fusion] に接続</a> 」を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ]</td> 
   <td>既読としてマークする電子メールのフォルダを選択します。 例：プライマリ。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 電子メール ID (UID)]</p> </td> 
   <td> <p>既読としてマークする電子メールの電子メール UID を入力します。</p> <p>電子メールの UID を取得するには、[!UICONTROL 電子メールを監視 ] モジュールまたは [!UICONTROL 電子メールを検索 ] モジュールを使用します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メールを未読としてマーク]

[ 未読 ] フラグを設定すると、選択したフォルダ内のメールまたは下書きを未読としてマークします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>電子メールアカウントを [!UICONTROL Workfront Fusion] に接続する手順については、 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">電子メールを [!UICONTROL Workfront Fusion] に接続</a> 」を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ]</td> 
   <td>未読としてマークする電子メールのフォルダを選択します。 例：プライマリ。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 電子メール ID (UID)]</p> </td> 
   <td> <p>未読としてマークするメールの E メール UID を入力します。</p> <p>電子メールの UID を取得するには、[!UICONTROL 電子メールを監視 ] モジュールまたは [!UICONTROL 電子メールを検索 ] モジュールを使用します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メールの移動]

選択したメールまたは下書きを選択したフォルダに移動します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>電子メールアカウントを [!UICONTROL Workfront Fusion] に接続する手順については、 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">電子メールを [!UICONTROL Workfront Fusion] に接続</a> 」を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースフォルダー ]</td> 
   <td>電子メールを移動する元の電子メールを含むフォルダーを選択します。 例：プライマリ。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 保存先フォルダー ]</td> 
   <td> <p> 電子メールを追加するフォルダーを選択します。 例：仕事。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 電子メール ID (UID)]</p> </td> 
   <td> <p>宛先フォルダーに移動する電子メールの電子メール UID を入力します。</p> <p>電子メールの UID を取得するには、[!UICONTROL 電子メールを監視 ] モジュールまたは [!UICONTROL 電子メールを検索 ] モジュールを使用します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メールのコピー]

選択したフォルダーに電子メールまたは下書きをコピーします。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>電子メールアカウントを [!UICONTROL Workfront Fusion] に接続する手順については、 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">電子メールを [!UICONTROL Workfront Fusion] に接続</a> 」を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースフォルダー ]</td> 
   <td>電子メールのコピー元のフォルダーを選択します。 例：プライマリ。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 保存先フォルダー ]</td> 
   <td> <p> 電子メールをコピーするフォルダーを選択します。 例：仕事。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 電子メール ID (UID)]</p> </td> 
   <td> <p>宛先フォルダーにコピーする電子メールの電子メール UID を入力します。</p> <p>電子メールの UID を取得するには、[!UICONTROL 電子メールを監視 ] モジュールまたは [!UICONTROL 電子メールを検索 ] モジュールを使用します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メールの削除]

選択したフォルダーからメールまたは下書きを削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>電子メールアカウントを [!UICONTROL Workfront Fusion] に接続する手順については、 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">電子メールを [!UICONTROL Workfront Fusion] に接続</a> 」を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ]</td> 
   <td>削除する電子メールのフォルダーを選択します。 例：プライマリ。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 電子メール ID (UID)]</p> </td> 
   <td> <p>削除する電子メールの電子メール UID を入力します。</p> <p>電子メールの UID を取得するには、[!UICONTROL 電子メールを監視 ] モジュールまたは [!UICONTROL 電子メールを検索 ] モジュールを使用します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expunge]</td> 
   <td> <p>このオプションを有効にすると、モジュールは現在開いているメールボックスで [!UICONTROL 削除済み ] としてフラグ付けされたすべてのメッセージを完全に削除できます。</p> <p>注意：In [!DNL Gmail]の場合、この動作は [!UICONTROL 設定 ] /[!UICONTROL IMAP アクセスでの POP/IMAP の転送 ] セクションの設定によって決まります。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL メールの取得]

指定された条件に一致する E メールを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>電子メールアカウントを [!UICONTROL Workfront Fusion] に接続する手順については、 <a href="#connect-your-email-to-workfront-fusion" class="MCXref xref">電子メールを [!UICONTROL Workfront Fusion] に接続</a> 」を参照してください。</p> </td>
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ] </td> 
   <td> <p>取得する電子メールが含まれているフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 取得時にメッセージを既読としてマーク ] </td> 
   <td> <p>詳細を取得した後で未読のメールを既読としてマークする場合は、このオプションを有効にします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 条件 ]</p> </td> 
   <td> <p>取得する E メールの条件を選択します。</p> 
    <ul> 
     <li>[!UICONTROL すべての電子メール ]</li> 
     <li>[!UICONTROL 電子メールの読み取りのみ ]</li> 
     <li>[!UICONTROL 未読メールのみ ]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 送信者の電子メールアドレス ] </td> 
   <td> <p>E メールを取得する送信者の E メールアドレスを入力またはマップします。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL 受信者の電子メールアドレス ]</td> 
   <td> <p> E メールを取得する受信者の E メールアドレスを入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 開始日 ] </td> 
   <td> <p>指定した日付以降に処理される E メールを取得する日付を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 日付の前 ]</td> 
   <td> <p> 指定した日付以前に処理された E メールを取得する日付を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 件名 ] </td> 
   <td> <p>取得する電子メールの件名を入力またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フレーズ ] </td> 
   <td> <p>キーワードを入力またはマッピングして、特定の語句を含む電子メールのみを取得します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 電子メール ID (UID)]</td> 
   <td> <p> 詳細を取得する電子メールの電子メール ID(UID) を入力します。</p> <p>E メールの UID は、 [!DNL Workfront Fusion]'s[!UICONTROL 電子メールを監視 ] モジュールまたは [!UICONTROL 電子メールを検索 ] モジュール。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 結果の最大数 ]</td> 
   <td> <p> 電子メールの最大数 [!DNL Workfront Fusion] は、1 回のシナリオ実行サイクルで返されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL モジュールが結果を返さない場合でも、ルートの実行を続行します ]</td> 
   <td> <p> 結果が返されない場合でもモジュールの実行を続行する場合に選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### イテレータ

#### [!UICONTROL 添付ファイルを繰り返し]

受け取った添付ファイルを 1 つずつ繰り返します。

email iterator モジュールを使用すると、E メールの添付ファイルを個別に管理できます。 例えば、電子メールを監視して添付ファイル付きの電子メールを繰り返し処理し、アラートを受け取るように設定できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースモジュール ]</td> 
   <td> <p>繰り返し処理をおこなう添付ファイルが含まれる E メールを出力するモジュールを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

イテレータの詳細については、 [の Iterator モジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md).
