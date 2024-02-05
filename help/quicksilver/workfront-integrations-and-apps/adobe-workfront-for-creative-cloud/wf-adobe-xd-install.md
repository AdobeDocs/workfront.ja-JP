---
product-area: workfront-integrations;setup
navigation-topic: adobe-workfront-for-creative-cloud
title: Adobe Workfront for XD をインストールして開きます。
description: Adobe Workfront for XD プラグインは、Adobe Marketplace からインストールできます。
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
exl-id: d4971977-b5bd-4bb4-a1c2-44829a67d32d
source-git-commit: 78a6cee213887c72aedc14bbb4552f28fc27625d
workflow-type: tm+mt
source-wordcount: '458'
ht-degree: 93%

---

# [!DNL Adobe Workfront for XD] をインストールして開く

[!DNL Adobe Workfront for XD] プラグインは、Adobe Marketplace からインストールできます。このプラグインでは、次の言語をサポートしています。

* 英語
* フランス語
* ドイツ語
* イタリア語
* スペイン語
* ポルトガル語
* 日本語
* 簡体字中国語
* 繁体字中国語
* 韓国語

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
 <!-- <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!UICONTROL Pro] or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>[!UICONTROL Work] or [!UICONTROL Plan]</p> </td> 
  </tr> -->
  <tr> 
   <td role="rowheader">製品</td> 
   <td><p>[!DNL Workfront] ライセンスに加えて [!DNL Adobe Creative Cloud] ライセンスが必要です。</p><p>詳しくは、<a href="https://helpx.adobe.com/jp/support/programs/cc-support-policy.html#cce" class="MCXref xref" xrefformat="{para}">Creative Cloud サポートポリシー</a>を参照してください。</p></td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 前提条件

* Workfront プラグインをインストールする前に、[!DNL Adobe XD] アプリをインストールする必要があります。

## をインストールします。 [!DNL Adobe Workfront for XD] 組織のプラグイン

[!DNL Adobe Admin Console] 管理者は、プラグインを [!DNL Creative Cloud] デプロイメントパッケージに含めることができます。詳しくは、[パッケージへのプラグインの追加](https://helpx.adobe.com/jp/enterprise/using/manage-extensions.html)を参照してください。

[こちらからビデオチュートリアルをご覧いただけます](https://www.youtube.com/watch?v=zzvXNLIBzrc){target=_blank}。

[!DNL Adobe Admin Console] 管理者は、ユーザーに配布するプラグイン専用のパッケージを作成することもできます。 詳しくは、 [[!UICONTROL [!DNL Adobe Workfront] 対象： [!DNL Creative Cloud]] ユーザー向けのパッケージを [!DNL Adobe Admin Console]](/help/quicksilver/administration-and-setup/configure-integrations/create-plugin-only-packages.md)

## [!DNL Adobe Workfront for XD] プラグインの個別インストール

[!DNL Adobe Exchange] から自分用に [!DNL Adobe Workfront for XD] プラグインをインストールできます。

1. Adobe Exchange の [Adobe Workfront for XD のインストールページ](https://exchange.adobe.com/apps/cc/4c3566f9?pluginId=4c3566f9&amp;workflow=share)に移動します。
1. 表示されるダイアログで、「**[!DNL Adobe Creative Cloud] デスクトップアプリを開く**」をクリックします。
1. [!DNL Adobe XD] プラグインマネージャーを開いたら、「**[!UICONTROL インストール]**」をクリックします。
1. ダイアログボックスの情報を読み、「**[!UICONTROL OK]**」をクリックします。
1. プラグインを開く方法については、次の節を参照してください。

## [!DNL Adobe Workfront for XD] プラグインを開きます。

1. 開く [!DNL Adobe XD].

1. 新規ファイルを作成するか、既存のファイルを開きます。

1. 左下隅で、**プラグイン**&#x200B;アイコンをクリックします。

![](assets/xd-plugin-window-350x620.png)

1. **[!UICONTROL プラグインパネル]**&#x200B;で、**[!UICONTROL Adobe Workfront for XD]** を検索します。

1. プラグインへのログイン方法については、次の節を参照してください。

## [!DNL Adobe Workfront for XD] にログイン

1. プラグインパネルが開いていることを確認し、「**[!DNL Adobe Workfront for XD]**」をクリックします。
1. ドメインを入力し、「**[!UICONTROL ログイン]**」をクリックします。ブラウザーページが開きます。

   >[!TIP]
   >
   >* ドメインを検索するには、ブラウザーを開いて [!DNL Workfront] インスタンスに移動し、次の URL の最初の部分をコピーします。\
   >![](assets/domain-350x50.png)
   >
   > * Workfront インスタンスが Experience Cloud と統合されている場合は、Admin Console の製品／Workfront の下に Workfront ドメインが表示されるように管理者に依頼してください。

1. ブラウザーで、[!DNL Workfront] 資格情報を入力し、「**[!DNL Log in]**」をクリックします。会社がシングルサインオン（SSO）を使用している場合は、SSO プロバイダーのページにリダイレクトされ、そこからログインします。

   >[!NOTE]
   >
   >最近ログインした場合は、[!DNL Workfront] の資格情報の入力を求められない場合があります。

   画面の指示に従って、[!DNL Workfront] にログインします。

   >[!NOTE]
   >
   >* [!DNL Workfront] と [!DNL Adobe Creative Cloud] との接続には OAuth 2.0 を使用します。これはほとんどの Web ベースの統合で、ユーザーの認証と承認に使用される安全な規格です。
   >* [!DNL Workfront] アカウントの [ ドメインまたはホスト ] を入力するよう求められた場合は、*yourCompany&#39;sDomain.my.workfront.com* の形式で入力します。会社のドメインは通常、会社の名前です。

1. 「**[!UICONTROL アクセスを許可]**」をクリックしてログインを完了し、[!DNL Adobe XD] に戻って自分の作業を確認します。

 
