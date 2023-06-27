---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: 署名モジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Bynder]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。
author: Becky
feature: Workfront Fusion
exl-id: e4dc9588-334a-41a3-85d1-996cb819c3fa
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1664'
ht-degree: 1%

---

# [!DNL Bynder] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Bynder]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

シナリオの作成手順については、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

モジュールについて詳しくは、 [のモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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

使用する [!DNL Bynder] モジュールの場合、 [!DNL Bynder] アカウント

## 接続 [!DNL Bynder] Workfront Fusion  {#connect-bynder-to-workfront-fusion}

* [への接続の作成 [!DNL Bynder] から [!DNL Workfront Fusion]](#create-a-connection-to-bynder-from-workfront-fusion)
* [を生成する [!UICONTROL クライアント ID] および [!UICONTROL クライアント秘密鍵] in [!DNL Bynder] （オプション）](#generate-a-client-id-and-client-secret-in-bynder-optional)

### への接続の作成 [!DNL Bynder] から [!DNL Workfront Fusion]

接続は、 [!DNL Workfront Fusion] を [!DNL Bynder] 内部から直接アカウントを取得する [!DNL Bynder] モジュール。

1. 任意の [!DNL Bynder] モジュール、クリック **[!UICONTROL 追加]** の横 [!UICONTROL 接続] フィールドに入力します。
1. を選択します。 [!DNL Bynder] 接続先のドメイン。
1. （オプション）「 **[!UICONTROL 詳細設定]**&#x200B;を選択し、 [!UICONTROL クライアント ID] および [!UICONTROL クライアント秘密鍵].

   クライアント ID とクライアント秘密鍵の生成手順については、 [でのクライアント ID とクライアント秘密鍵の生成 [!DNL Bynder] （オプション）](#generate-a-client-id-and-client-secret-in-bynder-optional) 」を参照してください。

1. 内 [!UICONTROL ログイン] ウィンドウで、ユーザー名（電子メールアドレス）とパスワードを入力します。
1. クリック **[!UICONTROL 続行]** 接続を作成し、モジュールに戻ります。

### を生成する [!UICONTROL クライアント ID] および [!UICONTROL クライアント秘密鍵] in [!DNL Bynder] （オプション）

クライアント ID とクライアント秘密鍵を使用して接続を作成する場合は、 [!DNL Bynder] アカウント クライアント ID とクライアント秘密鍵は、 [!DNL Bynder].

でのアプリの作成手順については、 [!DNL Bynder]を参照してください。 [Oauth 2.0 アプリ](https://developer-docs.bynder.com/api/authentication-oauth2-oauth-apps/) 内 [!DNL Bynder] ドキュメント。

>[!NOTE]
>
>でアプリを作成する場合 [!DNL Bynder]を使用する場合は、次のように入力します。 `redirect uri`:
>
>`https://app.workfrontfusion.com/oauth/cb/workfront-bynder`

## [!DNL Bynder] モジュールとそのフィールド

設定時に [!DNL Bynder] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Bynder] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [アクション](#actions)
* [検索](#searches)
* [トリガー](#triggers)

### アクション

* [[!UICONTROL カスタム API 呼び出し]](#custom-api-call)
* [[!UICONTROL アセットメタデータの読み取り]](#read-asset-metadata)
* [[!UICONTROL アセットメタデータの更新]](#update-asset-metadata)
* [[!UICONTROL コレクションへのアセットの追加]](#add-assets-to-a-collection)
* [[!UICONTROL コレクションからアセットを削除]](#remove-assets-from-collection)
* [[!UICONTROL アセットへのタグの追加]](#add-a-tag-to-assets)
* [[!UICONTROL タグの削除] アセットから](#remove-a-tag-from-assets)
* [[!UICONTROL アセットをダウンロード]](#download-asset)
* [[!UICONTROL アセットをアップロード]](#upload-asset)

#### [!UICONTROL カスタム API 呼び出し]

このアクションモジュールを使用すると、 [!DNL Bynder] API これにより、他のユーザーが達成できないデータフローの自動化を作成できます [!DNL Bynder] モジュール。

このモジュールを設定する際には、次のフィールドが表示されます。

このモジュールは、ステータスコードと共に、API 呼び出しのヘッダーと本文を返します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Bynder] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">接続 [!DNL Bynder] から [!DNL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td>相対パスを入力 <code>https://{your-bynder-domain}/api/{api-version}/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メソッド ]</td> 
   td&gt; <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>例： <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion は、認証ヘッダーを追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しのクエリを追加します。</p> <p>例： <code>{"name":"something-urgent"}</code></p> </td> 
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

#### [!UICONTROL アセットメタデータの読み取り]

このアクションモジュールは、アセットのメタデータを読み取ります。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Bynder] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">接続 [!DNL Bynder] から [!DNL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td>メタデータを取得するアセットの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td> <p>このモジュールの出力バンドルに含める情報を選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アセットメタデータの更新]

このアクションモジュールは、既存のアセットのメタデータを更新します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Bynder] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">接続 [!DNL Bynder] から [!DNL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td>メタデータを更新するアセットの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フィールド ]</td> 
   <td> <p>情報を入力するフィールドを選択し、メタデータを更新する情報をこれらのフィールドに入力またはマッピングします。 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL メタプロパティ ]</p> </td> 
   <td>更新するオプションを選択し、情報を入力するか、これらのプロパティにマッピングします。 メタプロパティは、アセット内の特定のフィールドを表さないアセットに関する情報です。</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL コレクションへのアセットの追加]

このアクションモジュールは、1 つ以上のアセットをコレクションに追加します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Bynder] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">接続 [!DNL Bynder] から [!DNL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL コレクション ID]</td> 
   <td> <p>アセットを追加するコレクションの ID を入力またはマッピングします。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アセット ID]</td> 
   <td> <p>コレクションに追加するアセットごとに、 <strong>[!UICONTROL 項目を追加 ]</strong>をクリックし、アセット ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL コレクションからアセットを削除]

このアクションモジュールは、1 つ以上のアセットをコレクションから削除します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Bynder] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">接続 [!DNL Bynder] から [!DNL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL コレクション ID]</td> 
   <td> <p>アセットを削除するコレクションの ID を入力またはマッピングします。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アセット ID]</td> 
   <td> <p>コレクションから削除するアセットごとに、 <strong>[!UICONTROL 項目を追加 ]</strong>をクリックし、アセット ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アセットへのタグの追加]

1 つ以上のアセットにタグを追加する

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Bynder] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">接続 [!DNL Bynder] から [!DNL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL タグ ID]</td> 
   <td> <p>アセットに追加するタグの ID を入力またはマッピングします。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アセット ID]</td> 
   <td> <p>タグを付ける各アセットに対して、 <strong>[!UICONTROL 項目を追加 ]</strong>をクリックし、アセット ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アセットからタグを削除する]

1 つ以上のアセットからタグを削除する

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Bynder] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">接続 [!DNL Bynder] から [!DNL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL タグ ID]</td> 
   <td> <p>アセットから削除するタグの ID を入力またはマッピングします。</p> <p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アセット ID]</td> 
   <td> <p>タグを削除する各アセットに対して、 <strong>[!UICONTROL 項目を追加 ]</strong>をクリックし、アセット ID を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アセットをダウンロード]

このアクションモジュールは、1 つのアセットをダウンロードします。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Bynder] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">接続 [!DNL Bynder] から [!DNL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td>ダウンロードするアセットの ID を入力またはマッピングします。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL アセットのバージョン ]</td> 
   <td> <p>ダウンロードするアセットのバージョンを入力またはマッピングします。 アセットの最新バージョンをダウンロードするには、「 」フィールドを空のままにします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アセットをアップロード]

このアクションモジュールは、1 つのアセットをアップロードします。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Bynder] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">接続 [!DNL Bynder] から [!DNL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 名前を付けて保存 ]</td> 
   <td> <p>アップロードするファイルの保存方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 新しいアセット ]</strong> </p> <p>情報を入力するフィールドおよびメタプロパティを選択し、それらのフィールドに情報を入力します。</p> <p>アップロードしたアセットに使用するブランドの ID を入力またはマッピングします。</p> </li> 
     <li> <p><strong>[!UICONTROL 新しいアセットバージョン ]</strong> </p> <p>新しいバージョンをアップロードするアセットの ID を入力します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ソースファイル ]</td> 
   <td>前のモジュールからソースファイルを選択するか、ソースファイルの名前とデータをマップします。</td> 
  </tr> 
 </tbody> 
</table>

### 検索

* [[!UICONTROL レコードをリスト]](#list-record)
* [[!UICONTROL アセットの検索]](#search-for-assets)

#### [!UICONTROL レコードをリスト]

この検索モジュールは、特定のタイプのすべての項目を取得します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Bynder] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">接続 [!DNL Bynder] から [!DNL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL レコードタイプ ]</td> 
   <td> <p>リストするレコードのタイプを選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL すべてのコレクションを読み取る ]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL すべてのタグに関する情報を読む ]</strong> </p> </li> 
     <li> <p><strong>[!UICONTROL コレクションのすべてのアセットを読み取る ]</strong> </p> <p>アセットのリストを表示するコレクションの ID を入力またはマッピングします。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td> <p>モジュールの出力に含めるフィールドを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すアセットの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アセットの検索]

この検索モジュールは、指定した条件に基づいてアセットを検索します。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Bynder] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">接続 [!DNL Bynder] から [!DNL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 条件 ]</td> 
   <td> <p>検索条件を入力します。 </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL フィールド ]</strong> </p> <p>検索で使用するフィールドを選択します</p> </li> 
     <li> <p><strong>[!UICONTROL 論理演算子 ]</strong> </p> <p>検索に使用する演算子を選択します。</p> </li> 
     <li> <p><strong>[!UICONTROL 値 ]</strong> </p> <p>選択したフィールドに、検索する値を入力またはマッピングします。 値のタイプは、選択したフィールドのデータタイプと同じである必要があります。 </p> <p>データタイプについて詳しくは、 <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">の項目データタイプ [!DNL Adobe Workfront Fusion]</a>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 結果セット ]</td> 
   <td>最初に一致したアセットを返すか、一致したすべてのアセットを返すかを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 並べ替え基準 ]</td> 
   <td> <p>並べ替えの基準となるフィールドを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 並べ替え方向 ]</td> 
   <td> <p>昇順と降順のどちらで並べ替えるかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 出力 ]</td> 
   <td> <p>モジュールの出力に含めるフィールドを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ]</td> 
   <td> <p>各シナリオの実行サイクル中に、モジュールが返すアセットの最大数を入力またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

### トリガー

#### [!UICONTROL アセットを見る]

このトリガーモジュールは、アセットが作成または更新されたときにシナリオを開始します。

<table style="table-layout:auto">
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
    <td role="rowheader"> <p>[!UICONTROL 接続 ]</p> </td> 
   <td> <p>接続方法 [!DNL Bynder] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="#connect-bynder-to-workfront-fusion" class="MCXref xref">接続 [!DNL Bynder] から [!DNL Workfront Fusion] </a> 」を参照してください。</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Event type</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select whether you want to start the scenario when a new asset is created or when an existing asset is updated.</td>
   --> 
  </tr> 
  <tr>
     <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL コレクション ]</td>
   <td> <p>新しいアセットを監視するコレクションを選択します。 すべてのコレクションを閲覧するには、このフィールドを空のままにします。</p> </td> 
  </tr> 
  <tr> <!--
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">Outputs</td>
   --> <!--
    <td data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the fields that you want to include in the output.</td>
   --> 
  </tr> 
  <tr> 
    <td role="rowheader" data-mc-conditions="QuicksilverOrClassic.Draft mode">[!UICONTROL 制限 ]</td>

<td> <p>各シナリオの実行サイクル中にモジュールが返すレコードの最大数を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>
