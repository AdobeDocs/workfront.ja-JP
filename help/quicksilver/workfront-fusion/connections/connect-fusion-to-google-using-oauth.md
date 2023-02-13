---
product-previous: workfront-fusion
product-area: workfront-integrations;setup
navigation-topic: connections-annd-webhooks
title: 接続 [!DNL Adobe Workfront Fusion] から [!DNL Google Services] カスタム OAuth クライアントの使用
description: 以下を使用できます。 [!DNL Adobe Workfront Fusion] 接続する [!DNL Google Services] カスタム OAuth クライアントを使用します。 この手順には、既存の [!DNL Google] アカウント
author: Becky
feature: Workfront Fusion
exl-id: 5efc0001-a8cd-4ffc-b074-3536f095727b
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 0%

---

# 接続 [!DNL Adobe Workfront Fusion] から [!DNL Google Services] カスタム OAuth クライアントの使用

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

既存の [!DNL Google] この接続を確立するアカウント。

## でプロジェクトを作成する [!DNL Google Cloud Platform]

以下の手順は、を対象としています。

* 個人用 ([!DNL @gmail.com] および [!DNL @googlemail.com] ユーザー )
* 内部使用 ([!DNL G Suite] カスタム OAuth クライアントの使用を希望するユーザー )

にプロジェクトを作成するには [!DNL Google Cloud] プラットフォーム：

1. ログイン先 [[!DNL Google Cloud] Platform](https://console.developers.google.com/projectselector2/apis/dashboard?supportedpurview=project) を使用して、 [!DNL Google] 資格情報。
1. 左側のパネルで、 **[!UICONTROL ダッシュボード]**.
1. クリック **[!UICONTROL プロジェクトを作成]** をクリックします。
1. 次を入力します。 **[!UICONTROL プロジェクト名]**&#x200B;を選択し、「 **[!UICONTROL 作成]**.

1. 次をクリック： **[!UICONTROL API とサービスの有効化]** タブをクリックします。
1. 内 **[!UICONTROL API とサービスの検索]** 画面上部のフィールドに、使用するサービスの名前 ( [!DNL Gmail] API または [!DNL Google Drive] API) を参照してください。
1. API が表示されたら、接続先の API またはサービスをクリックします [!DNL Workfront Fusion].
1. クリック **[!UICONTROL 有効にする]** 選択した API を有効にします。
1. 有効にする API ごとに、手順 6～8 を繰り返します。

   >[!NOTE]
   >
   >有効にする必要があります [!DNL Google Drive] API と、すべての [!DNL Google] 使用するアプリ ( [!DNL Google Sheets] API) を参照してください。

1. 表示される画面で、 **[!UICONTROL 資格情報の作成]** をクリックします。
1. 「 」セクションに進みます。 [OAuth の同意設定を構成します](#configure-oauth-consent-settings) 」を参照してください。

## 設定 [!UICONTROL OAuth 同意] 設定

1. 左側のパネルで、 **[!UICONTROL OAuth 同意画面]**.
1. 選択 **[!UICONTROL 外部]**&#x200B;を選択し、「 **[!UICONTROL 作成]**.

   >[!NOTE]
   >
   >このオプションを選択すると、課金されなくなります。 詳しくは、 [!DNL Google]検証要件の例外に関するの情報。

1. 次のように、必須フィールドに入力します。

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL アプリ名 ]</p> </td> 
      <td> <p>同意を要求するアプリの名前を入力します。</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>例: </b></span></span>[!DNL Adobe Workfront Fusion] </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ユーザーサポート電子メール ]</td> 
      <td>ユーザーがこのアプリに接続する際の同意に関する質問を連絡するための電子メールアドレスを入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 電子メールアドレス ]</td> 
      <td>Googleがプロジェクトに対する変更を通知する際に使用できる電子メールアドレスを 1 つ以上入力します。</td> 
     </tr> 
    </tbody> 
   </table>

1. の下 [!UICONTROL 承認済みドメイン]をクリックし、 **[!UICONTROL ドメインを追加]**、と入力します。 `workfrontfusion.com`.

1. クリック **[!UICONTROL 保存して続行]**.
1. クリック **[!UICONTROL スコープを追加または削除]**.
1. 右側のパネルで、次のスコープを有効にします。

<table style="table-layout:auto">
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th>サービス/API</th> 
      <th>必須スコープ</th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td> <p>[!DNL Gmail]</p> </td> 
      <td> <p>https://mail.google.com/</p> <p>https://www.googleapis.com/auth/gmail.labels</p> <p>https://www.googleapis.com/auth/gmail.send</p> <p>https://www.googleapis.com/auth/gmail.readonly</p> <p>https://www.googleapis.com/auth/gmail.compose</p> <p>https://www.googleapis.com/auth/gmail.insert</p> <p>https://www.googleapis.com/auth/gmail.modify</p> <p>https://www.googleapis.com/auth/gmail.metadata</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!DNL Google Drive]</p> </td> 
      <td> <p>https://www.googleapis.com/auth/drive</p> <p>https://www.googleapis.com/auth/drive.readonly</p> </td> 
     </tr> 
    </tbody> 
   </table>

リストを展開するか、リストの次のページに移動して、すべてを表示する必要が生じる場合があります。

1. クリック **[!UICONTROL 更新]**.
1. クリック **[!UICONTROL 保存して続行]**.
1. （オプション）テストユーザーをプロジェクトに追加します。
1. クリック **[!UICONTROL 保存して続行]**.
1. 情報の正確性を確認し、 **[!UICONTROL ダッシュボードに戻る]**.

   >[!NOTE]
   >
   >次の方法で確認を行うために、同意画面や申請を送信する必要はありません。 [!DNL Google].

1. 続行 [OAuth 資格情報を作成](#create-oauth-credentials).

## OAuth 資格情報を作成

1. 左側のパネルで、 **[!UICONTROL 資格情報]**.

   >[!NOTE]
   >
   >これが最初の API またはサービス ([!DNL Gmail] または [!DNL Google Drive]) を有効にしている場合、新しい資格情報を作成する必要はありません。

1. クリック **[!UICONTROL 資格情報の作成]** 画面の上部付近にある「 」を選択し、 **[!UICONTROL OAuth クライアント ID]** を選択します。

1. 次のように、必須フィールドに入力します。

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL アプリケーションタイプ ]</td> 
      <td> <p> [!UICONTROL Web アプリケーション ]</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 名前 ]</td> 
      <td>[!DNL Workfront Fusion] </td> 
     </tr> 
    </tbody> 
   </table>

1. の下 [!UICONTROL 承認済みのリダイレクト URI]をクリックし、 **[!UICONTROL URI を追加]** と入力します。 **1 つ** 次のうちの 1 つ：

   * の場合 [!DNL Gmail] または [!DNL Google Drive]: `https://app.workfrontfusion.com/oauth/cb/google-restricted`

   * その他の場合 [!DNL Google] アプリ： `https://app.workfrontfusion.com/oauth/cb/google`

1. 「**[!UICONTROL 作成]**」をクリックします。

   この [!UICONTROL クライアント ID] および [!UICONTROL クライアント秘密鍵] 表示。

1. を [!UICONTROL クライアント ID] および [!UICONTROL クライアント秘密鍵] を安全な場所に移動します。 これらを使用してで接続を作成します。 [!DNL Workfront Fusion].
1. 続行 [接続先 [!DNL Google] in [!DNL Workfront Fusion]](#connect-to-google-in-workfront-fusion).

## 接続先 [!DNL Google] in [!DNL Workfront Fusion]

への接続を作成するプロセス [!DNL Google] は、 [!DNL Google] サービス ( [!DNL Google Sheets] または [!DNL Google Docs])、または [!DNL Google] 経由 [!UICONTROL HTTP] >[!UICONTROL OAuth2.0 を作成] リクエストモジュール。

* [接続先 [!DNL Google] 内 [!DNL Google] サービス](#connect-to-google-in-a-google-service)
* [接続先 [!DNL Google] 内 [!UICONTROL HTTP] > [!UICONTROL OAuth2.0 リクエストを作成] モジュール](#connect-to-google-in-the-http--make-an-oauth20-request-module)

### 接続先 [!DNL Google] 内 [!DNL Google] サービス

1. In [!DNL Workfront Fusion]、 [!DNL Google] 接続を作成する必要があるモジュール。
1. クリック **[!UICONTROL 接続の作成]**&#x200B;を選択し、「 **[!UICONTROL 詳細設定を表示]**.

1. 次を入力します。 [!UICONTROL クライアント ID] および [!UICONTROL クライアント秘密鍵] で取得した [[!UICONTROL OAuth 資格情報を作成]](#create-oauth-credentials) 各フィールドで、 **[!UICONTROL 続行]**.

1. ログイン [!DNL Google] アカウント

   この **[!UICONTROL このアプリは検証されていません]** ウィンドウが表示されます。 ウィンドウのタイトルに表示される「アプリ」は、上で作成した OAuth クライアントです。

1. クリック **[!UICONTROL 詳細]**&#x200B;を選択し、「 **[!UICONTROL に移動します。 [!DNL Workfront Fusion] （安全でない）]** ：カスタム OAuth クライアントを使用したアクセスを許可します。

1. クリック **[!UICONTROL 許可]** 付与する [!DNL Workfront Fusion] 権限。
1. 表示されるウィンドウで、 **[!UICONTROL 許可]** を再度クリックして、選択内容を確認します。

   目的の [!DNL Google] カスタム OAuth クライアントを使用するサービスが確立されます。

### 接続先 [!DNL Google] 内 [!UICONTROL HTTP] > [!UICONTROL OAuth2.0 リクエストを作成] モジュール {#connect-to-google-in-the-http--make-an-oauth20-request-module}

への接続手順 [!DNL Google] 内 [!UICONTROL HTTP] > [!UICONTROL OAuth2.0 リクエストを作成] モジュール、詳しくは、 [への接続を作成する手順 [!DNL Google] 内 [!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 リクエストを作成] モジュール](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md#instruct) in [[!UICONTROL HTTP] > [!UICONTROL OAuth 2.0 リクエストを作成] モジュール](../../workfront-fusion/apps-and-their-modules/http-modules/http-module-make-an-oauth-2-request.md).

## 考えられるエラーメッセージ：[!UICONTROL [403] アクセスが設定されていません]

この [!UICONTROL [403] アクセスが設定されていません] エラーメッセージが表示される場合は、Google Cloud Platform で対応する API を有効にする必要があります。 API を有効にするには、の節の手順に従います [でプロジェクトを作成する [!DNL Google Cloud Platform]](#create-a-project-on-google-cloud-platform) 」を参照してください。
