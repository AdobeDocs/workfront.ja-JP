---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Frame.io モジュール
description: この [!DNL Adobe Workfront Fusion Frame].io modules enable you to monitor, create, update, retrieve, or delete assets and comments in your [!DNL Frame.io] アカウント
author: Becky
feature: Workfront Fusion
exl-id: 373a86f6-fbba-4914-b08d-a3a035ac0ae4
source-git-commit: 885d93dd4383945538e977fd3edbfd55bda88b70
workflow-type: tm+mt
source-wordcount: '2263'
ht-degree: 0%

---

# [!DNL Frame.io] モジュール

この [!DNL Adobe Workfront Fusion] [!DNL Frame.io] モジュールを使用して、 [!DNL Frame.io] アカウント

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

使用する [!DNL Frame.io] モジュールの場合、 [!DNL Frame.io] アカウント

## 接続 [!DNL Frame.io] から [!UICONTROL Adobe Workfront Fusion]

次に接続できます： [!DNL Frame.io] API トークンを使用するか、OAuth 2.0 を使用します。

[接続先 [!DNL Frame.io] API トークンの使用](#connect-to-frameio-using-an-api-token)

[接続先 [!DNL Frame.io] OAuth 2.0 PKCE の使用](#connect-to-frameio-using-oauth-20-pkce)

### 接続先 [!DNL Frame.io] API トークンの使用

次の手順で [!DNL Frame.io] アカウント [!DNL Workfront Fusion] API トークンを使用して、 [!DNL Frame.io] アカウントに追加し、 [!DNL Workfront Fusion] [!DNL Frame.io] [!UICONTROL 接続の作成] ダイアログ。

1. にログインします。 [!DNL Frame.io] アカウント
1. 次に移動： **[!UICONTROL トークン]** ページの [!DNL Frame.io] 開発者。
1. クリック **[!UICONTROL 新規]**.
1. トークンの名前を入力し、使用するスコープを選択して、 **[!UICONTROL 作成]**.
1. 提供されたトークンをコピーします。
1. に移動します。 [!DNL Workfront Fusion] をクリックし、 [!DNL Frame.io] モジュール **[!UICONTROL 接続の作成]** ダイアログ。
1. 内 **[!UICONTROL 接続タイプ]** フィールド、選択 **[!DNL Frame.io]**.
1. 手順 5 で **[!UICONTROL お使いの [!DNL Frame.io] API キー]** フィールドとクリック **[!UICONTROL 続行]** 接続を確立するために。

接続が確立されました。 モジュールの設定に進むことができます。

### 接続先 [!DNL Frame.io] OAuth 2.0 PKCE の使用

次への接続を作成できます： [!DNL Frame.io] オプションのクライアント ID で OAuth 2.0 PKCE を使用します。 接続にクライアント ID を含める場合は、 [!DNL Frame.io] アカウント

* [接続先 [!DNL Frame.io] OAuth 2.0 PKCE（クライアント ID なし）の使用](#connect-to-frameio-using-using-oauth-20-pkce-without-client-id)
* [接続先 [!DNL Frame.io] OAuth 2.0 PKCE（クライアント ID を使用）の使用](#connect-to-frameio-using-using-oauth-20-pkce-with-client-id)

#### 接続先 [!DNL Frame.io] OAuth 2.0 PKCE（クライアント ID なし）の使用

1. に移動します。 [!DNL Workfront Fusion] をクリックし、 [!DNL Frame.io] モジュール **[!UICONTROL 接続の作成]** ダイアログ。
1. 内 **[!UICONTROL 接続タイプ]** フィールド、選択 **[!UICONTROL [!DNL Frame.io]OAuth 2.0 PKCE]**.
1. 新しい接続の名前を **[!UICONTROL 接続名]** フィールドに入力します。
1. クリック **[!UICONTROL 続行]** 接続を確立するために。

接続が確立されました。 モジュールの設定に進むことができます。

#### 接続先 [!DNL Frame.io] OAuth 2.0 PKCE（クライアント ID を使用）の使用

1. での OAuth 2.0 アプリの作成 [!DNL Frame.io]. 手順については、 [!DNL Frame.io] ドキュメント [!UICONTROL OAuth 2.0 コード承認フロー].

   >[!IMPORTANT]
   >
   >OAuth 2.0 アプリを [!DNL Frame.io]:
   >
   >* リダイレクト URI として次のように入力します。
   >   
   >  南北アメリカ/APAC `https://app.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >  EMEA `https://app-eu.workfrontfusion.com/oauth/cb/frame-io5`
   >
   >* 「 PCKE 」オプションを有効にします。



1. 提供されたをコピーします。 `client_id`.
1. に移動します。 [!DNL Workfront Fusion] をクリックし、 [!DNL Frame.io] モジュール **[!UICONTROL 接続の作成]** ダイアログ。
1. 内 **[!UICONTROL 接続タイプ]** フィールド、選択 **[!UICONTROL [!DNL Frame.io]OAuth 2.0 PKCE]**.
1. 新しい接続の名前を **[!UICONTROL 接続名]** フィールドに入力します。
1. クリック **[!UICONTROL 詳細設定を表示]**.
1. 次を入力します。 `client_id` 手順 2 でをにコピーしました。 **[!UICONTROL クライアント ID]** フィールドに入力します。
1. クリック **[!UICONTROL 続行]** 接続を確立するために。

接続が確立されました。 モジュールの設定に進むことができます。

## [!DNL Frame.io] モジュールとそのフィールド

設定時に [!DNL Frame.io] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Frame.io] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Assets](#assets)
* [コメント](#comments)
* [プロジェクト](#projects)
* [その他](#other)

### Assets

* [[!UICONTROL アセットの作成]](#create-an-asset)
* [[!UICONTROL アセットの削除]](#delete-an-asset)
* [[!UICONTROL アセットの取得]](#get-an-asset)
* [[!UICONTROL アセットのリスト]](#list-assets)
* [[!UICONTROL アセットの更新]](#update-an-asset)
* [[!UICONTROL アセットの削除を監視]](#watch-asset-deleted)
* [[!UICONTROL アセットラベルを更新済みで監視]](#watch-asset-label-updated)
* [[!UICONTROL 新しいアセットを見る]](#watch-new-asset)

#### [!UICONTROL アセットの作成]

このアクションモジュールは、新しいアセットを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td>への接続を作成する手順 [!DNL Frame.io]を参照してください。 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Frame.io] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL チーム ID] </td> 
   <td> <p>アセットを作成するプロジェクトを所有するチームを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>アセットを作成するプロジェクトを選択するか、プロジェクトの ID をマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ID] </td> 
   <td> <p>フォルダーを選択するか、アセットを作成するフォルダーの ID をマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL の種類 ] </td> 
   <td> <p>フォルダーを作成するか、ファイルを作成するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 名前 ] </td> 
   <td> <p>新しいファイルまたはフォルダの名前を入力します。</p> </td> 
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
   <td role="rowheader">[!UICONTROL ソース URL] </td> 
   <td> <p>アップロードするファイルの URL を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 説明 ] </td> 
   <td> <p>アセットの簡単な説明を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アセットの削除]

このアクションモジュールは、指定したアセットを削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td>への接続を作成する手順 [!DNL Frame.io]を参照してください。 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Frame.io] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL チーム ID] </td> 
   <td> <p>削除するアセットが含まれるプロジェクトを所有するチームを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p> 削除するアセットを含むプロジェクトまたはを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ID] </td> 
   <td> <p>削除するアセットを含むフォルダーを選択します</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>削除するアセットを選択またはマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アセットの取得]

このアクションモジュールは、アセットの詳細を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td>への接続を作成する手順 [!DNL Frame.io]を参照してください。 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Frame.io] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL チーム ID] </td> 
   <td> <p>詳細を取得するアセットを含むプロジェクトを所有するチームを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p> 詳細を取得するアセットを含むプロジェクトを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ID] </td> 
   <td> <p>詳細を取得するアセットを含むフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>詳細を取得するアセットを選択するか、アセットの ID をマッピングします。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アセットのリスト]

この検索モジュールは、指定されたプロジェクトのフォルダ内のすべてのアセットを取得します。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td>への接続を作成する手順 [!DNL Frame.io]を参照してください。 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Frame.io] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL チーム ID] </td> 
   <td> <p>アセットを取得するフォルダーを含むプロジェクトを所有するチームを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p> アセットを取得するフォルダーを含むプロジェクトを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ID] </td> 
   <td> <p>アセットのリストを表示するフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ] </td> 
   <td> <p>アセットの最大数の設定 [!DNL Workfront Fusion] は、1 回の実行サイクルで返されます。</p> </td> 
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
    <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td>への接続を作成する手順 [!DNL Frame.io]を参照してください。 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Frame.io] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL チーム ID] </td> 
   <td> <p>アセットを更新するプロジェクトを所有するチームを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>アセットを更新するプロジェクトを選択するか、プロジェクトの ID をマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ID] </td> 
   <td> <p>アセットを更新するフォルダーを選択するか、フォルダーの ID をマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 名前 ] </td> 
   <td> <p>更新したファイルの名前を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 説明 ] </td> 
   <td> <p>更新したアセットの簡単な説明を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アセットの削除を監視]

このトリガーモジュールは、アセットが削除されたときにシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook 名 ]</td> 
   <td> <p> ウェブフックの名前（例：削除済みアセット）を入力します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td>への接続を作成する手順 [!DNL Frame.io]を参照してください。 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Frame.io] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL チーム ID] </td> 
   <td> <p>この Webhook を作成するチームを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL アセットラベルを更新済みで監視]

このトリガーモジュールは、アセットのステータスが設定、変更または削除されたときにシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook 名 ]</td> 
   <td> <p> Webhook の名前を入力します（例：アセットのステータス更新）。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td>への接続を作成する手順 [!DNL Frame.io]を参照してください。 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Frame.io] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL チーム ID] </td> 
   <td> <p>この Webhook を作成するチームを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 新しいアセットを見る]

このトリガーモジュールは、新しいアセットが作成される際にシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook 名 ]</td> 
   <td> <p> Webhook の名前を入力します（例：作成されたアセット）。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td>への接続を作成する手順 [!DNL Frame.io]を参照してください。 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Frame.io] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL チーム ID] </td> 
   <td> <p>この Webhook を作成するチームを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

### コメント

* [[!UICONTROL コメントの作成]](#create-a-comment)
* [[!UICONTROL コメントの削除]](#delete-a-comment)
* [[!UICONTROL コメントを取得]](#get-a-comment)
* [[!UICONTROL コメントをリスト]](#list-comments)
* [[!UICONTROL コメントの更新]](#update-a-comment)
* [[!UICONTROL ウォッチコメントの更新]](#watch-comment-updated)
* [[!UICONTROL 新しいコメントを見る]](#watch-new-comment)

#### [!UICONTROL コメントの作成]

このアクションモジュールは、新しいコメントまたは返信をアセットに追加します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td>への接続を作成する手順 [!DNL Frame.io]を参照してください。 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Frame.io] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL の種類 ] </td> 
   <td> <p>コメントを作成するか、コメントに返信するかを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL チーム ID] </td> 
   <td> <p>コメントを追加するアセットを含むプロジェクトを所有するチームを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>プロジェクトを選択するか、コメントを追加するアセットが含まれるプロジェクトの ID をマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ID] </td> 
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
   <td role="rowheader">[!UICONTROL テキスト ]</td> 
   <td> <p> コメントまたは返信のテキスト内容を入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL タイムスタンプ ] </td> 
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
    <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td>への接続を作成する手順 [!DNL Frame.io]を参照してください。 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Frame.io] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL チーム ID]</td> 
   <td> <p> コメントを削除するアセットを含むプロジェクトを所有するチームを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID]</td> 
   <td> <p> コメントを削除するアセットを含むプロジェクトを選択するか、プロジェクトの ID をマップします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ID]</td> 
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
    <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td>への接続を作成する手順 [!DNL Frame.io]を参照してください。 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Frame.io] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL チーム ID] </td> 
   <td> <p>アセットを取得するフォルダーを含むプロジェクトを所有するチームを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>アセットを取得するフォルダーを含むプロジェクトを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ID] </td> 
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
    <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td>への接続を作成する手順 [!DNL Frame.io]を参照してください。 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Frame.io] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL チーム ID] </td> 
   <td> <p>コメントを取得するフォルダを含むプロジェクトを所有するチームを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>コメントを取得するフォルダーを含むプロジェクトを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ID] </td> 
   <td> <p>コメントのリストを表示するアセットを含むフォルダーを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID] </td> 
   <td> <p>コメントのリストを表示するアセットを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ] </td> 
   <td> <p>コメントの最大数を設定 [!DNL Workfront Fusion] は、1 回の実行サイクルで返されます。</p> </td> 
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
    <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td>への接続を作成する手順 [!DNL Frame.io]を参照してください。 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Frame.io] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL チーム ID] </td> 
   <td> <p>コメントを更新するアセットを含むプロジェクトを所有するチームを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project ID] </td> 
   <td> <p>コメントを更新するアセットを含むプロジェクトを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL フォルダー ID] </td> 
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
   <td role="rowheader">[!UICONTROL テキスト ]</td> 
   <td> <p> コメントのテキストコンテンツを入力します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL タイムスタンプ ] </td> 
   <td> <p>コメントのリンク先となるビデオのフレーム番号を入力します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL ウォッチコメントの更新]

このトリガーモジュールは、コメントが編集されたときにシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook 名 ] </td> 
   <td> <p>Webhook の名前を入力します（例：「編集されたコメント」）。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td>への接続を作成する手順 [!DNL Frame.io]を参照してください。 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Frame.io] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL チーム ID] </td> 
   <td> <p>この Webhook を作成するチームを選択します。</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL 新しいコメントを見る]

このトリガーモジュールは、新しいコメントまたは返信が作成されたときにシナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook 名 ] </td> 
   <td> <p>Webhook の名前（「新しいコメント」など）を入力します。</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td>への接続を作成する手順 [!DNL Frame.io]を参照してください。 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Frame.io] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL チーム ID] </td> 
   <td> <p>この Webhook を作成するチームを選択します。</p> </td> 
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
    <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td>への接続を作成する手順 [!DNL Frame.io]を参照してください。 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Frame.io] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL チーム ID] </td> 
   <td> <p>プロジェクトを取得するチームを選択またはマッピングします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ] </td> 
   <td> <p>プロジェクトの最大数を設定 [!DNL Workfront Fusion] は、1 回の実行サイクルで返されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

### その他

#### [!UICONTROL API 呼び出しを実行する]

このモジュールでは、カスタム API 呼び出しを実行できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td>への接続を作成する手順 [!DNL Frame.io]を参照してください。 <a href="#connect-frame-io-to-adobe-workfront-fusion" class="MCXref xref">接続 [!DNL Frame.io] から [!DNL Adobe Workfront Fusion]</a> 」を参照してください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL URL]</p> </td> 
   <td> <p>相対パスを入力 <code>https://api.frame.io</code>. 例: <code> /v2/teams</code></p> <p>注意：使用可能なエンドポイントの一覧については、 [!DNL Frame.io] API リファレンス。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL メソッド ]</p> </td> 
   <td> <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> <p>[!DNL Workfront Fusion] は、認証ヘッダーを自動的に追加します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ] </td> 
   <td> <p>リクエストクエリ文字列を入力します。 クエリ文字列に含める各パラメーターに対して、 <b>[!UICONTROL 項目を追加 ]</b> フィールドの名前と値を入力します。</p> </td> 
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

**例：** 次の API 呼び出しは、すべてのチームとその詳細を [!DNL Frame.io] アカウント：

URL: `/v2/teams`

メソッド: `GET`

![](assets/api-call-example.png)

結果は、モジュールの Output の Bundle > Body にあります。

この例では、1 チームの詳細が返されました。

![](assets/api-call-output.png)
