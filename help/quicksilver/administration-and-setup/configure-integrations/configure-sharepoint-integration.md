---
title: の設定 [!DNL SharePoint] 統合
user-type: administrator
product-area: system-administration;workfront-integrations;setup
navigation-topic: administrator-integrations
description: 統合可能な [!DNL Workfront] と [!DNL SharePoint] オンラインで、ユーザーが移動、リンク、追加できる機能を提供 [!DNL SharePoint] Workfront内のドキュメント。 提供される機能は他の機能と似ています [!DNL Workfront] 統合 (Google Drive、Box、Dropboxなど )。
author: Becky, Caroline
feature: System Setup and Administration, [!DNL Workfront] Integrations and Apps, Digital Content and Documents
role: Admin
exl-id: fd45e1bc-9a35-4960-a73a-ff845216afe4
source-git-commit: 5292069412a73f824dbcd967d47737cff5ef58fa
workflow-type: tm+mt
source-wordcount: '2515'
ht-degree: 0%

---

# レガシーの設定 [!DNL SharePoint] 統合

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

>[!IMPORTANT]
>
>新しい [!DNL SharePoint] 統合は、22.3 リリース（2022 年 7 月）で実稼動環境にリリースされました。 ユーザーは、従来の [!DNL SharePoint] 統合の場合、新しい [!DNL SharePoint] SharePointからドキュメントをリンクするための統合
>
>* 新しいSharePoint統合は、管理者が設定する必要はなく、個々のユーザーが設定できます。 ただし、新しいSharePoint統合にスムーズに移行できるように、Workfront管理者は、Workfrontのセットアップ領域で小さな設定を変更する必要があります。
   >
   >    詳細および手順については、 [ドキュメントに引き続きアクセスするための従来のSharePoint統合の設定](#configure-the-legacy-sharepoint-integration-for-continued-access-to-documents) 」を参照してください。
>    
>* 現在レガシーの [!DNL SharePoint] 新しい統合による統合。
   >    
   >    ドキュメントをリンクする手順については、 [外部アプリケーションからドキュメントをリンク](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).


統合可能な [!DNL Workfront] と [!DNL SharePoint Online]を使用して、ユーザーが移動、リンク、および追加できるようにする [!DNL SharePoint] Workfront内のドキュメント。 提供される機能は他の機能と似ています [!DNL Workfront] 統合（例： ） [!DNL Google Drive], [!DNL Box]、および [!DNL Dropbox].

この統合は、 [!DNL SharePoint Online]. のオンプレミスインスタンス [!DNL SharePoint] はサポートされていません。

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>[!UICONTROL プラン ]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>次の条件を満たす必要があります。 [!DNL Workfront] 管理者。 詳しくは、 [!DNL Workfront] 管理者向け： <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## 前提条件

で必要なアクセス権または権限を持っている。 [!DNL SharePoint] 組織の [!DNL SharePoint].

## 新しいSharePoint統合によるドキュメントのリンク

個々のユーザーは、新しい [!DNL SharePoint] 統合とも呼ばれます。 統合には管理者設定は必要ありません。 代わりに、ユーザーが [!DNL Microsoft] ドキュメントをリンクする際にアカウントを作成します。これにより、統合でユーザーの [!DNL SharePoint].

ユーザーが [!DNL Workfront] [!DNL SharePoint] 統合と [!DNL SharePoint] アカウントを使用する場合、 [!DNL Workfront] は、 [!UICONTROL SharePoint] アカウント 読み取り権限許可 [!DNL Workfront] 次のファイルを表示してアクセスする： [!DNL SharePoint]、および書き込み権限を持つユーザーは、にファイルをアップロードできます。 [!DNL SharePoint].

新しい [!DNL SharePoint] 統合については、 [外部ドキュメントを次にリンク： [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#link-an-external-document-to-workfront)

>[!NOTE]
>
>* A [!DNL SharePoint] 統合は、 [!DNL SharePoint] インスタンス。 したがって、ユーザーは、 [!DNL SharePoint]を設定する必要がありますが、1 秒に対する統合を設定することはできません [!DNL SharePoint](2 番目の [!DNL SharePoint].
>
>* ユーザーは、 [!DNL Workfront] [!DNL SharePoint] の統合と同様に、 [!DNL SharePoint] アカウント


## ドキュメントに引き続きアクセスするための従来のSharePoint統合の設定

従来のSharePoint統合を使用して、Workfrontにリンクされたドキュメントにユーザーが引き続きアクセスできるようにするには、従来のSharePoint統合へのアクセスを再設定し、SharePoint Client Secret を最新の状態に保つ必要があります。

* [従来の [!DNL SharePoint] 統合](#reconfigure-access-to-the-legacy-dnl-sharepoint-integration)
* [従来の [!DNL SharePoint] 統合](#configure-the-client-secret-for-continued-access-to-the-legacy-dnl-sharepoint-integration)

### 従来の [!DNL SharePoint] 統合

レガシーを使用してリンクされたドキュメントに確実にアクセスするには [!DNL SharePoint] 統合では、ユーザーがその統合を通じて新しいドキュメントをリンクできないようにしますが、次の手順を実行します。

>[!NOTE]
>
> * レガシー [!DNL SharePoint] 統合に「[!DNL SharePoint].&quot;
> * 新しい [!DNL SharePoint] 統合に「[!UICONTROL [!DNL SharePoint] （グラフ API）].&quot;


1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **[!UICONTROL 設定]** ![設定](../get-started-wf-administration/assets/gear-icon-settings.png).
1. 選択 **[!UICONTROL ドキュメント]** 左側のナビゲーションで、「 **[!UICONTROL クラウドプロバイダー]**.
1. 必ず **[!DNL SharePoint]** オプションと **[!UICONTROL [!DNL SharePoint]（グラフ API）]** オプションは両方とも有効です。
1. 「**[!UICONTROL 保存]**」をクリックします。
1. 選択 **[!UICONTROL ドキュメント]** 左側のナビゲーションで、「 **[!UICONTROL [!DNL SharePoint]統合]**.
1. リストの左側にあるすべての既存の統合のチェックマークを選択し、「 」を選択します。 **[!UICONTROL 無効にする]**.


### 従来の [!DNL SharePoint] 統合

お使いの [!DNL SharePoint] クライアントシークレットは、1 年に 1 回期限切れになります。 レガシーのドキュメントに引き続きアクセスできるようにするには [!DNL SharePoint] 統合のために、 [!DNL SharePoint] クライアントシークレットが最新です。

>[!IMPORTANT]
>
> 理由： [!DNL SharePoint] クライアントシークレットは、 [!DNL Microsoft]、クライアントシークレットの機能および手順は、 [!DNL SharePoint] 作成元 [!DNL Microsoft]. 常に [!DNL Microsoft] の手順と機能に関する最新の情報に関するドキュメント [!DNL SharePoint].

<!--1. Go to the site that your [!DNL SharePoint] integration uses. This may be a site that you created when setting up the integrations, or it may be your organization's root site.

1. Add `/_layouts/15/appregnew.aspx` to the end of the URL in the search bar at the top of your browser window.-->

1. 新しいクライアント秘密鍵を生成します。詳しくは、 [の期限が切れるクライアント秘密鍵を置き換える [!DNL SharePoint] アドイン](https://docs.microsoft.com/en-us/sharepoint/dev/sp-add-ins/replace-an-expiring-client-secret-in-a-sharepoint-add-in#generate-a-new-secret)
1. このクライアント秘密鍵を安全な場所にコピーします。
1. ログイン [!DNL Workfront] 管理者として。
1. Workfrontで、 **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).
1. 左側のパネルで、 **[!UICONTROL ドキュメント]** > **[!UICONTROL [!DNL SharePoint]統合]**.
1. をクリックします。 [!DNL SharePoint] 統合を更新し、「 **[!UICONTROL 編集]**.
1. 新しいクライアント秘密鍵を **[!UICONTROL クライアント秘密鍵]** フィールドに入力します。
1. 「**[!UICONTROL 保存]**」をクリックします。



## 従来のSharePoint統合の設定手順

>[!IMPORTANT]
>
>この統合は非推奨（廃止予定）となりました。 ここで説明する内容は情報提供のみで、近い将来に削除されます。


Workfrontが [!DNL SharePoint] OAuth 2.0 を使用したオンライン。これは、ほとんどの Web ベースの統合で、ユーザーの認証と承認に使用される標準です。

OAuth を設定するには、 [!DNL SharePoint] サイトと、 [!DNL SharePoint]. このプロセスについては、以降の節で説明します。

OAuth について詳しくは、 [http://oauth.net](http://oauth.net/).

>[!TIP]
>
>情報のコピーと貼り付けを簡単に行う [!DNL Workfront] および [!DNL SharePoint] この手順では、両方のアプリケーションを別々のタブで開いたままにすることをお勧めします。

* [の作成と設定 [!DNL SharePoint] サイト](#create-and-configure-a-sharepoint-site)
* [サイトアプリに対する書き込み権限を付与する](#grant-write-permissions-to-the-site-app)
* [の作成 [!DNL Workfront] [!DNL SharePoint] 統合インスタンス](#create-a-workfront-sharepoint-integration-instance)
* [統合の完了](#complete-your-integration)
* [ドキュメントを追加します](#add-documents)

### の作成と設定 [!DNL SharePoint] サイト  {#create-and-configure-a-sharepoint-site}

次のために [!DNL Workfront] 認証を受ける [!DNL SharePoint], [!DNL Workfront] ユーザーが [!UICONTROL フルコントロール] 権限レベルまたは特定の Manage 権限。 このマスターサイトは、 [!DNL Workfront].

を作成して設定するには、以下を実行します。 [!DNL SharePoint] サイト：

1. （オプション）組織のルートサイトを使用しない場合は、 [!DNL SharePoint].

   手順については、 [サイトの作成](https://docs.microsoft.com/en-us/sharepoint/create-site-collection) 内 [!DNL Microsoft] ドキュメント。

   * を選択します。 **[!UICONTROL チームサイト]** オプションを使用して、サイトを作成できます。

1. （条件付き）手順 1 でサイトを作成した場合は、作成したサイトに移動します。

   または

   手順 1 でサイトを作成しなかった場合は、組織のルートサイトに移動します。

1. 追加 `/_layouts/15/appregnew.aspx` を追加します。
1. 次のフィールドを設定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL クライアント ID]</p> </td> 
      <td> <p>クリック <strong>[!UICONTROL 生成 ]</strong> をクリックしてクライアント ID を生成します。 この ID を安全な場所にコピーします。 後で [!DNL SharePoint] 統合 [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL クライアント秘密鍵 ]</p> </td> 
      <td> <p>クリック <strong>[!UICONTROL 生成 ]</strong> をクリックして、クライアントシークレットを生成します。 このシークレットを安全な場所にコピーします。 後で [!DNL SharePoint] 統合 [!DNL Workfront].</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>タイトル</p> </td> 
      <td> <p>タイトルを入力します（例： ）。 [!DNL Workfront] サイトアプリ。 ユーザーがドキュメントを追加すると、このタイトルが表示されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL App Domain]</p> </td> 
      <td> <p><code>my.workfront.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL リダイレクト URI]</p> </td> 
      <td> <p><code>https://oauth.my.workfront.com/oauth2/redirect</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **[!UICONTROL 作成]**
1. 続行 [サイトアプリに対する書き込み権限を付与する](#grant-write-permissions-to-the-site-app).

### サイトアプリに対する書き込み権限を付与する  {#grant-write-permissions-to-the-site-app}

この時点で、Site アプリが正常に作成され、内で登録されました。 [!DNL Workfront]. このサイトアプリは、 [!DNL SharePoint]. テナント内に存在します。 新しいサイトアプリは、テナント内のサイトコレクションに自動的にアクセスできません。 権限は、各サイトコレクションに対して明示的に付与する必要があります。 以下の手順では、新しい Site App にサイトコレクションへの書き込み権限を付与する方法を示します。 以下に追加した各サイトコレクションに対して、これらの手順を繰り返します。 [!UICONTROL 表示されるサイトコレクション] 上記の手順で説明します。

このサイトアプリには [!UICONTROL 書き込み] ユーザーがアクセスする必要があるすべてのサイトコレクションへの権限 [!DNL Workfront].

1. URL に「/_layouts/15/appinv.aspx」を [!DNL Sharepoint].

   **例:**

   ```
   https://mycompany.sharepoint.com/sites/mysite/_layouts/15/appinv.aspx
   ```

1. 次のフィールドを設定します

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL アプリ ID]</td> 
      <td> <p>作成したクライアント ID を追加します。 <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">の作成と設定 [!DNL SharePoint] サイト </a>をクリックし、 <strong>[!UICONTROL 参照 ]</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL クライアント ] / [!UICONTROL アプリドメイン ] / [!UICONTROL リダイレクト URL]</p> </td> 
      <td> <p>[!UICONTROL ルックアップ ] をクリックすると、これらは自動的に入力されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 権限リクエスト XML]</td> 
      <td> <p>次の XML を「[!UICONTROL 権限リクエスト XML]」フィールドにコピーします。 追加のスペースなしで、表示されたとおりに追加されていることを確認します。 エラーを回避するために。</p> 
      <div></a> 
      <div style="mc-code-lang: XML;" class="codeSnippetBody" data-mc-continue="False" data-mc-line-number-start="1" data-mc-use-line-numbers="False"> 
       <pre></pre></div></div></td></tr></tbody></table>

1. 「**[!UICONTROL 作成]**」をクリックします。
1. 表示されるダイアログで、 **[!UICONTROL 信頼する]**.
1. サイトアプリがサイトコレクションにアクセスできることを確認するには、 **[!UICONTROL サイトコレクションアプリの権限]** リンクイン [!UICONTROL サイト設定].
1. 残りのサイトコレクションに対して上記の手順を繰り返し、次に続行します。 [の作成 [!DNL Workfront] [!DNL SharePoint] 統合インスタンス](#create-a-workfront-sharepoint-integration-instance).

### の作成 [!DNL Workfront] [!DNL SharePoint] 統合インスタンス {#create-a-workfront-sharepoint-integration-instance}

サイトアプリを [!DNL SharePoint]を使用すると、サイトアプリから [!DNL Workfront]. サイトアプリはアプリのプリンシパルで、サイトコレクション内のドキュメントにアクセスするために OAuth 要求が行われるコンジットとして機能します。

1. ログイン [!DNL Workfront] 管理者として。
1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **[!UICONTROL ドキュメント]** > **[!UICONTROL [!DNL SharePoint]統合]**.
1. クリック **[!UICONTROL 追加[!DNL SharePoint]]**.
1. 次のフィールドを設定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL 名前 ]</p> </td> 
      <td> <p>名前を入力 [!DNL SharePoint] 統合とも呼ばれます。 ユーザーは、[!UICONTROL 追加 ] / [!UICONTROL 元 ] 「統合名」をクリックすると、この名前が表示されます。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL SharePoint] ホストインスタンス ]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.sharepoint.com</code> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL [!DNL Azure] ドメインにアクセス ]</p> </td> 
      <td> <p><code>&lt;YourDomain&gt;.onmicrosoft.com</code> </p> <p>これは、ユーザーがマスターを通じて認証する際に使用する認証サイトを指します。 [!UICONTROL [!DNL SharePoint] ホストインスタンス ]。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>
      </p> </td> 
      <td> <b>重要</b> サイトコレクションはレガシー [!DNL SharePoint] 統合。
       <ul> 
        <li> <p><b>組織のルートサイトを使用している場合</b><b>:</b> </p> <p>入力 <code>/</code></p> </li> 
        <li> <p><b>マスター・サイトとサブサイトを使用している場合：</b> </p> <p><b>重要</b>: [!DNL Microsoft SharePoint] では、サブサイトの使用をお勧めしていません。</p> <p>上記のセクションで作成したサイトコレクションの URL ステムを入力します。</p> <p>これは、.com の後の URL のセクションです。</p> <p>例：（URL の） <code>https://mycompany.sharepoint.com/sites/mysite</code>の場合、ステムは <code>/sites/mysite</code>.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] クライアント ID]</td> 
      <td>生成したクライアント ID を <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">の作成と設定 [!DNL SharePoint] サイト </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL [!DNL SharePoint] クライアント秘密鍵 ]</td> 
      <td>生成したクライアント秘密鍵を入力します。 <a href="#create-and-configure-a-sharepoint-site" class="MCXref xref">の作成と設定 [!DNL SharePoint] サイト </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 表示可能なサイトコレクション ]</td> 
      <td> <b>重要</b> サイトコレクションはレガシー [!DNL SharePoint] 統合とも呼ばれます。
       <ul> 
        <li> <p><b> 組織のルートサイトを使用している場合</b><b>:</b> </p> <p>入力 <code>/</code></p> </li> 
        <li> <p><b>マスター・サイトとサブサイトを使用している場合：</b> </p> <p><b>重要</b>: [!DNL Microsoft SharePoint] では、サブサイトの使用をお勧めしていません。</p> <p>を [!DNL SharePoint] 統合の場合は、サブサイトのステムを入力します。</p> <p>例：（URL の）<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>の場合、ステムは <code>/sites/mysite/mysubsite</code>.</p> <p><b>メモ</b>:   <p>設定のみをテストする場合（サブサイトを使用しない場合）は、マスターサイトのステムを入力します。 </p> <p>例：（URL の） <code> https://mycompany.sharepoint.com/sites/mysite</code>の場合、ステムは <code>/sites/mysite</code>.</p> <p>設定をテストしたとき ( <a href="#complete-your-integration" class="MCXref xref">統合の完了</a>の場合は、マスターサイトを削除してサブサイトを入力する必要があります。</p> 
          <ol> 
           <li value="1">次をクリック： <strong>[!UICONTROL メインメニュー ]</strong> アイコン <img src="assets/main-menu-icon.png"> 右上隅に [!DNL Adobe Workfront]を選択し、「 <strong>[!UICONTROL 設定 ]</strong> <img src="assets/gear-icon-settings.png">.<li><p>左側のパネルで、 <strong>[!UICONTROL ドキュメント ]</strong> &gt; <strong>[!UICONTROL [!DNL SharePoint] 統合 ]</strong>.</p></li><li><p>次をクリック： [!DNL SharePoint] 統合を設定して、「編集」をクリックします。</p></li><li><p>「[!UICONTROL 表示可能なサイトコレクション ]」フィールドからマスターサイトのステムを削除します。</p></li><li><p>を [!DNL SharePoint] 統合の場合は、サブサイトのステムを入力します。</p></li><p>例：（URL の）<code>https://mycompany.sharepoint.com/sites/mysite/mysubsite</code>の場合、ステムは <code>/sites/mysite/mysubsite</code>.</p></li> 
          </ol> </p> </li> 
       </ul> <p> </p> <p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **[!UICONTROL 保存]**
1. 続行 [統合の完了](#complete-your-integration).

### 統合の完了 {#complete-your-integration}

基本設定はほぼ完了です。

1. Workfrontで、 **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **[!UICONTROL ドキュメント]** ![](assets/document-icon.png).
1. クリック **[!UICONTROL 新規追加]**.
1. クリック **[!UICONTROL 送信者]`<title of your [!DNL SharePoint] site>`** 」と入力します。

   [ このサイトを信頼する ] を選択するように促すダイアログが表示されます。

   >[!NOTE]
   >
   >このダイアログが表示されない場合は、 [!DNL SharePoint] 統合が正しく設定されていません。

1. クリック **[!UICONTROL 信頼する]**.

### ドキュメントを追加します {#add-documents}

これで、 [!DNL SharePoint] サイト。

手順については、 [外部ドキュメントを次にリンク： [!DNL Workfront]](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md#linking-existing-documents) in [外部アプリケーションからドキュメントをリンク](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)

>[!IMPORTANT]
>
>フォルダーをリンクしたユーザーが外部アプリケーションにアクセスできなくなった場合、 [!DNL Workfront] では、フォルダーのコンテンツにアクセスできなくなりました。 この問題は、例えば、フォルダーを最初にリンクしたユーザーが会社を離れた場合に発生する可能性があります。 引き続きアクセスできるように、フォルダーへのアクセス権を持つユーザーは、フォルダーを再リンクする必要があります。

## トラブルシューティング

* [問題：ユーザーは、 [!DNL SharePoint] 統合とも呼ばれます。](#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration)
* [問題：As a [!DNL Workfront] ユーザー、新しいをプロビジョニングできません [!DNL SharePoint] インスタンス。 この操作を行うと、エラーが表示されます。](#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error)
* [問題：参照しようとしたとき [!DNL SharePoint] ファイル [!DNL Workfront]の場合、サイトコレクションが表示されません。](#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections)
* [問題：以前リンクしたフォルダやドキュメントには、 [!DNL SharePoint].](#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint)

### 問題：ユーザーは、 [!DNL SharePoint] 統合とも呼ばれます。 {#problem-users-experience-authentication-based-errors-when-using-the-sharepoint-integration}

解決策：

ユーザーは、 [!DNL SharePoint] サイト。

次を持つユーザー： [!UICONTROL フルコントロール] には、お客様に必要な権限がすべて付与されています [!DNL SharePoint] 統合とも呼ばれます。 ユーザーにフルコントロールアクセス権を付与したくない場合は、次の権限を付与する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL デザイン ]</p> </td> 
   <td> <p>表示、追加、更新、削除、承認およびカスタマイズが可能</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 編集 ]</p> </td> 
   <td> <p>リストの追加、編集、削除が可能リストの項目とドキュメントの表示、追加、更新、削除を行うことができます</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Contribute]</p> </td> 
   <td> <p>リストの項目とドキュメントを表示、追加、更新、削除できます</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 表示のみ ]</p> </td> 
   <td> <p>ページ、リスト項目、およびドキュメントを表示できます（サーバー側のファイルハンドラーを持つドキュメントタイプは、ブラウザーで表示できますが、ダウンロードできません）</p> </td> 
  </tr> 
 </tbody> 
</table>

権限レベルの作成および編集手順については、 [権限レベルの作成および編集方法](https://docs.microsoft.com/en-us/sharepoint/how-to-create-and-edit-permission-levels) (Microsoftドキュメント ) を参照してください。

### 問題：As a [!DNL Workfront] ユーザー、新しいをプロビジョニングできません [!DNL SharePoint] インスタンス。 この操作を行うと、エラーが表示されます。 {#problem-as-a-workfront-user-i-am-unable-to-provision-a-new-sharepoint-instance-when-i-attempt-to-do-i-see-an-error}

解決策：

これは、次のいずれかに由来する多くのものによって引き起こされます。 [!DNL Workfront] または [!DNL SharePoint]&#39;s 設定。 以下を確認します。

* クライアント ID、クライアント秘密鍵、戻り URL およびその他の設定フィールドが、 [!DNL Workfront] [!DNL SharePoint] 統合インスタンスと [!DNL SharePoint] サイトアプリ。
* ユーザーが [!UICONTROL フルコントロール] 認証に使用されるサイトコレクションへの権限。
* Site App がの下に表示されます。 [!UICONTROL サイトアプリの権限] の [!UICONTROL サイトコレクション] 認証に使用されます。

### 問題：参照しようとしたとき [!DNL SharePoint] ファイル [!DNL Workfront]の場合、サイトコレクションが表示されません。 {#problem-when-attempting-to-browse-sharepoint-files-in-workfront-i-do-not-see-any-or-all-of-my-site-collections}

解決策：

でサイトコレクションを表示するには [!DNL Workfront]の場合は、次の条件を満たす必要があります。

* サイトコレクションは、 [!DNL Workfront] [!DNL SharePoint] 統合インスタンス。

   次の手順でこれを検証します。 [!DNL Workfront]:

   1. に移動します。 [!UICONTROL 設定] > [!UICONTROL ドキュメント] > [!UICONTROL [!DNL SharePoint] 統合].
   1. を編集します。 [!DNL SharePoint] 統合インスタンスの情報。
   1. サイトコレクションがの下に表示されていることを確認します。 [!UICONTROL 表示されるサイトコレクション].

* ユーザーは、のサイトコレクションに対するビューアクセス権を持っている必要があります。 [!DNL SharePoint].
* 次の手順でこれを検証します。 [!DNL SharePoint]に移動します。 [!DNL SharePoint]を開き、サイトコレクションを開きます。 [!UICONTROL 設定] > [!UICONTROL サイトの権限].
* この [!DNL SharePoint] サイトアプリは、サイトコレクションにアクセスできる必要があります。

   次の手順でこれを検証します。 [!DNL SharePoint]:

   1. サイトコレクションに移動します ( > [!UICONTROL 設定] > [!UICONTROL サイトアプリの権限].
   1. 次を確認します。 [!UICONTROL サイトアプリ] 使用者 [!DNL Workfront] をここにリストします。
   1. （条件付き） Site App が一覧に表示されない場合は、_layouts/15/appinv.aspxを使用してサイトコレクションに追加します。

      サイトコレクションの追加については、「 Site App に対する書き込み権限の付与」を参照してください。

### 問題：以前リンクしたフォルダやドキュメントには、 [!DNL SharePoint]. {#problem-i-cannot-access-previously-linked-folders-and-documents-in-sharepoint}

解決策：

リンクしたユーザーが [!DNL SharePoint] フォルダーは認証できなくなりました [!DNL Workfront] では、フォルダーのコンテンツにアクセスできなくなりました。 この問題は、例えば、フォルダーを最初にリンクしたユーザーが会社を離れた場合に発生する可能性があります。

引き続きアクセスできるように、フォルダーへのアクセス権を持つユーザーは、フォルダーを再リンクする必要があります。

外部プロバイダーからのフォルダーのリンクについて詳しくは、 [外部アプリケーションからドキュメントをリンク](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

### 問題：からドキュメントを追加しようとすると、「404 が見つかりません」というエラーが表示される [!DNL Sharepoint]

#### 解決策：

このエラーは、 [!UICONTROL 表示されるサイトコレクション] リストが SharePoint で削除されました。 次を確認します。 [!UICONTROL 表示されるサイトコレクション] SharePoint で削除されたサイトの一覧を表示し、削除します。
