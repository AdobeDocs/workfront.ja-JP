---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Frame.io モジュール
description: ' [!DNL Adobe Workfront Fusion Frame].io modules enable you to monitor, create, update, retrieve, or delete assets and comments in your [!DNL Frame.io]  アカウント'
author: Becky
feature: Workfront Fusion
exl-id: 373a86f6-fbba-4914-b08d-a3a035ac0ae4
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '2338'
ht-degree: 99%

---

# [!DNL Frame.io] モジュール

[!DNL Adobe Workfront Fusion] [!DNL Frame.io] モジュールでは、[!DNL Frame.io] アカウント内のアセットとコメントを監視、作成、更新、取得、削除できます。

Frame.io コネクタのビデオの紹介については、以下を参照してください。

* [Frame.io](https://video.tv.adobe.com/v/3427032/){target=_blank}

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
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] [!DNL Adobe Workfront] プランをご利用の場合、この記事で説明されている機能を使用するには、組織は [!DNL Adobe Workfront] に加えて [!DNL Adobe Workfront Fusion] も購入する必要があります。[!DNL Workfront Fusion] は、[!DNL Workfront] [!UICONTROL Ultimate] プランに含まれています。</p>
   <p>または</p>
   <p>従来の製品要件：この記事で説明している機能を使用するには、[!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront]を組織で購入する必要があります。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

## 前提条件

[!DNL Frame.io] モジュールを使用するには、[!DNL Frame.io] アカウントが必要です。

## [!DNL Frame.io] から [!UICONTROL Adobe Workfront Fusion] への接続

[!DNL Frame.io] には、API トークンまたは OAuth 2.0 を使用して接続できます。

[API トークンを使用した  [!DNL Frame.io]  への接続](#connect-to-frameio-using-an-api-token)

[OAuth 2.0 PKCE を使用した  [!DNL Frame.io]  への接続](#connect-to-frameio-using-oauth-20-pkce)

### API トークンを使用した [!DNL Frame.io] への接続

API トークンを使用して [!DNL Frame.io] アカウントを [!DNL Workfront Fusion] に接続するには、[!DNL Frame.io] アカウントで API トークンを作成して [!DNL Workfront Fusion] [!DNL Frame.io] の「[!UICONTROL 接続を作成]」ダイアログに挿入する必要があります。

1. [!DNL Frame.io] アカウントにログインします。
1. [!DNL Frame.io] Developer の「**[!UICONTROL トークン]**」ページに移動します。
1. 「**[!UICONTROL 新規]**」をクリックします。
1. トークンの名前を入力して使用する範囲を選択し、「**[!UICONTROL 作成]**」をクリックします。
1. 提供されたトークンをコピーします。
1. [!DNL Workfront Fusion] に移動して、[!DNL Frame.io] モジュールの「**[!UICONTROL 接続を作成]**」ダイアログを開きます。
1. 「**[!UICONTROL 接続タイプ]**」フィールドで「**[!DNL Frame.io]**」を選択します。
1. 手順 5 でコピーしたトークンを「**[!UICONTROL [!DNL Frame.io] API キー]**」フィールドに入力し、「**[!UICONTROL 続行]**」をクリックして接続を確立します。

接続が確立されました。モジュールの設定に進むことができます。

### OAuth 2.0 PKCE を使用した [!DNL Frame.io] への接続

OAuth 2.0 PKCE とオプションのクライアント ID を使用して、[!DNL Frame.io] への接続を作成できます。接続にクライアント ID を含める場合は、[!DNL Frame.io] アカウントで OAuth 2.0 アプリを作成する必要があります。

* [OAuth 2.0 PKCE（クライアント ID なし）を使用した  [!DNL Frame.io]  への接続](#connect-to-frameio-using-using-oauth-20-pkce-without-client-id)
* [OAuth 2.0 PKCE（クライアント ID あり）を使用した  [!DNL Frame.io]  への接続](#connect-to-frameio-using-using-oauth-20-pkce-with-client-id)

#### OAuth 2.0 PKCE（クライアント ID なし）を使用した [!DNL Frame.io] への接続

1. [!DNL Workfront Fusion] に移動して、[!DNL Frame.io] モジュールの「**[!UICONTROL 接続を作成]**」ダイアログを開きます。
1. 「**[!UICONTROL 接続タイプ]**」フィールドで「**[!UICONTROL [!DNL Frame.io]OAuth 2.0 PKCE]**」を選択します。
1. 新しい接続の名前を「**[!UICONTROL 接続名]**」フィールドに入力します。
1. 「**[!UICONTROL 続行]**」をクリックして接続を確立します。

接続が確立されました。モジュールの設定に進むことができます。

#### OAuth 2.0 PKCE（クライアント ID あり）を使用した [!DNL Frame.io] への接続

1. [!DNL Frame.io] で OAuth 2.0 アプリを作成します。手順については、[!DNL Frame.io] ドキュメントの [!UICONTROL OAuth 2.0 コード承認フロー] を参照してください。

   >[!IMPORTANT]
   >
   >[!DNL Frame.io] で OAuth 2.0 アプリを作成する際には：
   >
   >* リダイレクト URI として次のように入力します。
   >   
   >  南北アメリカ / APAC `https://app.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >  EMEA `https://app-eu.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >* 「PCKE」オプションを有効にします。


1. 提供された `client_id` をコピーします。
1. [!DNL Workfront Fusion] に移動して、[!DNL Frame.io] モジュールの「**[!UICONTROL 接続を作成]**」ダイアログを開きます。
1. 「**[!UICONTROL 接続タイプ]**」フィールドで「**[!UICONTROL [!DNL Frame.io]OAuth 2.0 PKCE]**」を選択します。
1. 新しい接続の名前を「**[!UICONTROL 接続名]**」フィールドに入力します。
1. 「**[!UICONTROL 詳細設定を表示]**」をクリックします。
1. 手順 2 でコピーした `client_id` を「**[!UICONTROL クライアント ID]**」フィールドに入力します。
1. 「**[!UICONTROL 続行]**」をクリックして接続を確立します。

接続が確立されました。モジュールの設定に進むことができます。

## [!DNL Frame.io] モジュールとそのフィールド

[!DNL Frame.io] モジュールを設定する際、[!DNL Workfront Fusion] に以下のフィールドが表示されます。これらに加えて、アプリまたはサービスのアクセスレベルなどの要因に応じて、追加の [!DNL Frame.io] フィールドが表示される場合があります。モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用すると、そのフィールドの変数や関数を設定できます。詳しくは、[ [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md) でのモジュールから別のモジュールへの情報のマッピングを参照してください。

![](assets/map-toggle-350x74.png)

* [アセット](#assets)
* [コメント](#comments)
* [プロジェクト](#projects)
* [その他](#other)

### アセット

* [[!UICONTROL アセットの作成]](#create-an-asset)
* [[!UICONTROL アセットの削除]](#delete-an-asset)
* [[!UICONTROL アセットの取得]](#get-an-asset)
* [[!UICONTROL アセットの一覧表示]](#list-assets)
* [[!UICONTROL アセットの更新]](#update-an-asset)
* [[!UICONTROL 削除されたアセットの監視]](#watch-asset-deleted)
* [[!UICONTROL 更新されたアセットラベルの監視]](#watch-asset-label-updated)
* [[!UICONTROL 新しいアセットの監視]](#watch-new-asset)

#### [!UICONTROL アセットの作成]

このアクションモジュールでは、新しいアセットを作成できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>[!DNL Frame.io] への接続を作成する手順については、この記事にある<a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> への [!DNL Frame.io] の接続を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>アセットを作成するプロジェクトを所有するチームを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>アセットを作成するプロジェクトを選択するか、プロジェクトの ID をマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>アセットを作成するフォルダーを選択するか、フォルダーの ID をマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type] </td> 
   <td> <p>フォルダーを作成するか、ファイルを作成するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>新規ファイルまたはフォルダーの名前を入力します。</p> </td> 
  </tr> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">File Type </td> 
    <td> <p>Select the type of file you want to upload.</p> </td> 
   </tr>
  --> <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td role="rowheader">File Size </td> 
    <td> <p>The file size in bytes.</p> </td> 
   </tr>
  --> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source URL] </td> 
   <td> <p>アップロードするファイルの URL を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description] </td> 
   <td> <p>アセットの簡単な説明を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アセットを削除]

このアクションモジュールは、指定したアセットを削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>[!DNL Frame.io] への接続を作成する手順については、この記事にある<a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> への [!DNL Frame.io] の接続を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>削除するアセットが含まれるプロジェクトを所有するチームを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p> 削除するアセットが含まれるプロジェクトまたはプロジェクトを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>削除するアセットを含むフォルダーを選択</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>削除するアセットを選択またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アセットを取得]

このアクションモジュールは、アセットの詳細を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>[!DNL Frame.io] への接続を作成する手順については、この記事にある<a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> への [!DNL Frame.io] の接続を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>詳細を取得するアセットを含むプロジェクトを所有するチームを、選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p> 詳細を取得するアセットを含むプロジェクトを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>詳細を取得するアセットを含むフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>詳細を取得するアセットを選択するか、そのアセットの ID をマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アセットを一覧表示]

この検索モジュールは、指定されたプロジェクトのフォルダー内のすべてのアセットを取得します。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>[!DNL Frame.io] への接続を作成する手順については、この記事にある<a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> への [!DNL Frame.io] の接続を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>アセットを取得するフォルダーを含む、プロジェクトを所有するチームを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p> アセットを取得するフォルダーを含むプロジェクトを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>アセットのリストを表示するフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>[!DNL Workfront Fusion] が 1 回の実行サイクルで返すアセット数の上限を設定します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### `[!UICONTROL Update an Asset]`

このアクションモジュールを使用すると、既存のアセットの名前、説明、またはカスタムフィールドを更新できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>[!DNL Frame.io] への接続を作成する手順については、この記事にある<a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> への [!DNL Frame.io] の接続を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>アセットを更新するプロジェクトを所有する、チームを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>アセットを更新するプロジェクトを選択するか、プロジェクトの ID をマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>アセットを更新するフォルダーを選択するか、フォルダーの ID をマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>更新したファイルの名前を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description] </td> 
   <td> <p>更新したアセットの簡単な説明を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 削除されたアセットを監視]

このトリガーモジュールは、アセットが削除されたときにシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p> Web フックの名前（例：削除済みアセット）を入力します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>[!DNL Frame.io] への接続を作成する手順については、この記事にある<a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> への [!DNL Frame.io] の接続を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>この Web フックが作成されるチームを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新されたアセットラベルを監視]

このトリガーモジュールは、アセットのステータスが設定、変更または削除されたときにシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p> Web フックの名前を入力します（例：更新されたアセットステータス）。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>[!DNL Frame.io] への接続を作成する手順については、この記事にある<a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> への [!DNL Frame.io] の接続を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>この Web フックが作成されるチームを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 新しいアセットを見つける]

このトリガーモジュールは、新しいアセットが作成される際にシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name]</td> 
   <td> <p> Web フックの名前を入力します（例：作成されたアセット）。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>[!DNL Frame.io] への接続を作成する手順については、この記事にある<a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> への [!DNL Frame.io] の接続を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>この Web フックが作成されるチームを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### コメント

* [[!UICONTROL コメントを作成]](#create-a-comment)
* [[!UICONTROL コメントを削除]](#delete-a-comment)
* [[!UICONTROL コメントを取得]](#get-a-comment)
* [[!UICONTROL コメントをリスト]](#list-comments)
* [[!UICONTROL コメントをアップデート]](#update-a-comment)
* [[!UICONTROL 更新されたコメントを監視]](#watch-comment-updated)
* [[!UICONTROL 新規コメントを監視]](#watch-new-comment)

#### [!UICONTROL コメントを作成]

このアクションモジュールは、新しいコメントまたは返信をアセットに追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>[!DNL Frame.io] への接続を作成する手順については、この記事にある<a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Frame.io] を [!DNL Adobe Workfront Fusion]</a> に接続を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type] </td> 
   <td> <p>コメントを作成するか、コメントに返信するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>コメントを追加するアセットを含むプロジェクトを所有するチームを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>プロジェクトを選択するか、コメントを追加するアセットが含まれるプロジェクトの ID をマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>フォルダーを選択するか、コメントを追加するアセットが含まれるフォルダーの ID をマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>コメントを追加するアセットを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment ID] </td> 
   <td> <p>返信を追加するコメントを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text]</td> 
   <td> <p> コメントまたは返信のテキスト内容を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timestamp] </td> 
   <td> <p>コメントのリンク先となるビデオのフレーム番号を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL コメントの削除]

このアクションモジュールは、既存のコメントを削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>[!DNL Frame.io] への接続を作成する手順については、この記事にある<a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> への [!DNL Frame.io] の接続を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID]</td> 
   <td> <p> コメントを削除するアセットを含むプロジェクトを所有するチームを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p> コメントを削除するアセットを含むプロジェクトを選択するか、プロジェクトの ID をマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID]</td> 
   <td> <p> コメントを削除するアセットを含むフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>削除するコメントが含まれているアセットを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment ID] </td> 
   <td> <p>削除するコメントを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL コメントを取得]

このアクションモジュールは、指定されたコメントの詳細を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>[!DNL Frame.io] への接続を作成する手順については、この記事にある<a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> への [!DNL Frame.io] の接続を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>アセットを取得するフォルダーを含む、プロジェクトを所有するチームを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>アセットを取得するフォルダーを含むプロジェクトを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>アセットのリストを表示するフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>取得するコメントを含むアセットを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment ID] </td> 
   <td> <p>詳細を取得するコメントを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL コメントをリスト]

この検索モジュールは、指定されたアセットのすべてのコメントを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>[!DNL Frame.io] への接続を作成する手順については、この記事にある<a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> への [!DNL Frame.io] の接続を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>コメントを取得するフォルダーを含む、プロジェクトを所有するチームを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>コメントを取得するフォルダーを含むプロジェクトを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>コメントのリストを表示するアセットを含むフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>コメントのリストを表示するアセットを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>[!DNL Workfront Fusion] が 1 回の実行サイクルで返すコメントの最大数を設定します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL コメントの更新]

このアクションモジュールは、既存のコメントを編集します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>[!DNL Frame.io] への接続を作成する手順については、この記事にある<a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> への [!DNL Frame.io] の接続を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>コメントを更新するアセットを含むプロジェクトを所有するチームを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>コメントを更新するアセットを含むプロジェクトを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder ID] </td> 
   <td> <p>コメントを更新するアセットを含むフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>コメントを更新するアセットを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment ID] </td> 
   <td> <p>更新するコメントを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text]</td> 
   <td> <p> コメントのテキストコンテンツを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Timestamp] </td> 
   <td> <p>コメントのリンク先となるビデオのフレーム番号を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 更新されたコメントを監視]

このトリガーモジュールは、コメントが編集されたときにシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name] </td> 
   <td> <p>Web フックの名前（例：「編集されたコメント」）を入力します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>[!DNL Frame.io] への接続を作成する手順については、この記事にある<a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> への [!DNL Frame.io] の接続を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>この Web フックが作成されるチームを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 新規コメントを監視]

このトリガーモジュールは、新しいコメントまたは返信が作成されたときにシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook name] </td> 
   <td> <p>Web フックの名前（例：新規コメント）を入力します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>[!DNL Frame.io] への接続を作成する手順については、この記事にある<a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> への [!DNL Frame.io] の接続を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>この Web フックが作成されるチームを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### プロジェクト

#### [!UICONTROL プロジェクトのリスト]

この検索モジュールは、指定したチームのすべてのプロジェクトを取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>[!DNL Frame.io] への接続を作成する手順については、この記事にある<a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a> への [!DNL Frame.io] の接続を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Team ID] </td> 
   <td> <p>プロジェクトを取得するチームを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>[!DNL Workfront Fusion] が 1 回の実行サイクルで返すコメントの最大数を設定します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### その他

#### [!UICONTROL API 呼び出しの実行]

このモジュールでは、カスタム API 呼び出しを実行できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL Connection] </td> 
   <td>[!DNL Frame.io] への接続を作成する手順については、この記事にある<a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">[!DNL Frame.io] を [!DNL Adobe Workfront Fusion]</a> に接続を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p><code>https://api.frame.io</code> からの相対パスを入力します。例： <code> /v2/teams</code></p> <p>メモ：使用可能なエンドポイントの一覧については、[!DNL Frame.io] API リファレンスを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Method]</p> </td> 
   <td> <p>API 呼び出しの設定に必要な HTTP リクエストメソッドを選択します。詳しくは、<a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">[!DNL Adobe Workfront Fusion]</a>での HTTP リクエストメソッドを参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>リクエストのヘッダーを標準 JSON オブジェクトの形式で追加します。</p> <p>例： <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] 認証ヘッダーを自動的に追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String] </td> 
   <td> <p>リクエストクエリ文字列を入力します。クエリ文字列に含める各パラメーターに対して、<b>[!UICONTROL Add item]</b> をクリックして、フィールドの名前と必要な値を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文の内容を追加します。</p> <p>メモ：  <p><code>if</code> などの条件ステートメントを JSON で使用する場合は、条件ステートメントの外側に引用符を挿入します。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

**例：** 次の API 呼び出しは、[!DNL Frame.io] アカウントのすべてのチームとその詳細を返します。

URL：`/v2/teams`

メソッド：`GET`

![](assets/api-call-example.png)

結果は、モジュールの出力のバンドル／本文にあります。

この例では、1 チームの詳細が返されました。

![](assets/api-call-output.png)
