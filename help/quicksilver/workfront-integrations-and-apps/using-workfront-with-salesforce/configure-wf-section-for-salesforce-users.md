---
product-area: workfront-integrations;setup;user-management
navigation-topic: workfront-for-salesforce
title: ' [!DNL Salesforce]  ユーザー用  [!DNL Adobe Workfront]  セクションの設定'
description: ' [!DNL Workfront]  管理者は、 [!DNL Adobe Workfront]  for Salesforce をインストールした後に、Salesforce の新しいセクションで商談ページレイアウトとアカウントページレイアウトに追加することにより、ユーザーがそれを使用できるようになります。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 81481813-74db-4408-8c85-c3b5b844f932
source-git-commit: f9af669b023309abc132421f35a2ece974e796b0
workflow-type: tm+mt
source-wordcount: '790'
ht-degree: 89%

---

# [!DNL Salesforce] ユーザー用 [!DNL Adobe Workfront] セクションの設定

>[!IMPORTANT]
>
>より安定したスケーラブルな統合を実現するために、アドビでは、Workfront Automation and Integration （Fusion）を使用した最新の柔軟な統合アプローチに移行しています。 この移行プロセスの一環として、Workfront for Salesforce統合は **2026 年 2 月 28 日** 以降は使用できなくなります。
>
>組織のSalesforceとの統合のニーズに応じて、Workfront Automation and Integration を使用することをお勧めします。
>
>Workfrontの自動処理と統合の概要については、[Adobe Workfront Fusion の概要 &#x200B;](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview) を参照してください。
>
>SalesforceのWorkfront Automation and Integration モジュールの具体的な機能については、[Salesforce モジュール &#x200B;](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/salesforce-modules) を参照してください。

この機能を使用するには、[!UICONTROL Pro] [!DNL Workfront] プランが必要です。利用可能な様々なプランについて詳しくは、[[!DNL Workfront]  プラン](https://business.adobe.com/jp/products/workfront/pricing.html)を参照してください。

[!DNL Workfront] 管理者は、[!DNL Adobe Workfront] for [!DNL Salesforce] をインストールした後に、[!UICONTROL Salesforce] の新しいセクションで[!UICONTROL 商談]ページレイアウトおよび[!UICONTROL アカウント]
ページレイアウトに追加することにより、ユーザーがそれを使用できるようになります。

[!DNL Workfront for Salesforce] のインストールについて詳しくは、[&#x200B; [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md) のインストールを参照してください。

ユーザーが [!DNL Classic] フレームワークと [!DNL Lightning Experience] フレームワークの両方で [!DNL Workfront] を使用できるようにするために、[!DNL WorkfrontOpportunities] と [!DNL WorkfrontAccounts] [!UICONTROL Visualforce] ページを[!UICONTROL 商談]ページレイアウトおよび[!UICONTROL アカウント]ページレイアウトにそれぞれ追加する必要があります。

## アクセス要件

この記事で説明されている機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 前提条件

* システム管理者アカウントにアクセスできる [!DNL Salesforce] インスタンスが必要です。
* システム管理者アカウントにアクセスできる [!DNL Workfront] インスタンスが必要です。

## [!DNL Salesforce Classic] フレームワークで [!DNL Workfront] セクションを設定

1. Workfront 管理者として [!DNL Salesforce] にログインします。
1. 「**[!UICONTROL 設定]」**&#x200B;をクリックします。
1. 「**[!UICONTROL ビルド]**」セクションで、**[!UICONTROL カスタマイズ]**&#x200B;を展開します。

1. **[!UICONTROL 商談]**&#x200B;を展開し、次に「**[!UICONTROL ページレイアウト]**」をクリックして、[!DNL Workfront] セクションを商談に追加します。

   または

   **[!UICONTROL アカウント]**&#x200B;を展開し、次に「**[!UICONTROL ページレイアウト]**」をクリックして、[!DNL Workfront] セクションをアカウントに追加します。


1. 既存のレイアウト上の「**[!UICONTROL 編集]**」をクリックします。

   または

   「**[!UICONTROL 新規]**」をクリックして、新しいレイアウトを追加します。

1. （オプション）**[!UICONTROL セクション]**&#x200B;コンポーネントをレイアウトにドラッグし、希望の位置にドロップします。

1. （オプション）新しいセクションの名前を指定します。

   このセクションに「**[!DNL Workfront]**」と名前を付けることをお勧めします。

1. （オプション）新しいセクションの目的の&#x200B;**[!UICONTROL レイアウト]**&#x200B;および&#x200B;**[!UICONTROL タブキーの順序]**&#x200B;を指定します。

   **[!UICONTROL [!DNL Workfront] セクションの 1 列]**&#x200B;レイアウトを選択することをお勧めします。

1. 「**[!UICONTROL OK]**」をクリックします。
1. **[!UICONTROL レイアウト]**&#x200B;領域で、**[!UICONTROL Visualforce ページ]**&#x200B;をクリックします。

1. **[!UICONTROL WorkfrontOpportunities]** コンポーネントを&#x200B;**[!UICONTROL 商談]**&#x200B;レイアウトの新しいセクションにドラッグ＆ドロップします。

   または

   **[!UICONTROL WorkfrontAccounts]** コンポーネントを&#x200B;**[!UICONTROL アカウント]**&#x200B;レイアウトの新しいセクションにドラッグ＆ドロップします。

1. 新しく追加されたコンポーネントの右上にある「**[!UICONTROL プロパティ]**」アイコンをクリックします。

1. 最適な表示を実現するには、[!DNL Workfront Visualforce] ページに次のプロパティを指定します。

   * **[!UICONTROL 幅（ピクセル単位または％）]**：100％
   * **[!UICONTROL 高さ（ピクセル単位）]**：600
   * 「**[!UICONTROL スクロールバーを表示]**」を選択します。

1. 「**[!UICONTROL OK]**」をクリックします。
1. 「**[!UICONTROL 保存]**」をクリックしてレイアウトを保存します。

   このレイアウトを割り当てたすべてのユーザーが、[!UICONTROL 商談]オブジェクトまたは[!UICONTROL アカウント]オブジェクトで [!DNL Workfront] セクションを参照できるようになりました。

   ユーザーには、[!DNL Workfront] セクションで [!DNL Workfront] ログイン画面が表示されます。[!DNL Workfront] アカウントを持っていない場合は、セクションを折りたたむことはできますが、レイアウトから削除できません。

## [!DNL Salesforce Lightning Experience] フレームワークで [!DNL Workfront] セクションを設定

[!UICONTROL 設定]領域にアクセスするか、アカウントまたは[!UICONTROL 商談]オブジェクトからアクセスすることで、
[!DNL Salesforce Lightning Experience] フレームワークの [!DNL Salesforce] の[!UICONTROL 商談]またはアカウントのレイアウトに [!DNL Workfront] セクションを追加できます。

* [[!UICONTROL 設定]レベルで  [!DNL Workfront]  セクションを設定](#configure-the-workfront-section-at-the-setup-level-configure-the-workfront-section-at-the-setup-level)
* [商談またはアカウントレベルで  [!DNL Workfront]  セクションを設定](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)

### [!UICONTROL 設定]レベルで [!DNL Workfront] セクションを設定 {#configure-the-workfront-section-at-the-setup-level}

1. システム管理者として [!DNL Salesforce] にログインします。
1. **[!UICONTROL 設定]**&#x200B;アイコン、「**[!UICONTROL 設定]**」の順にクリックします。

1. **[!UICONTROL オブジェクトとフィールド]**&#x200B;を展開し、「**[!UICONTROL オブジェクトマネージャー]**」をクリックします。

1. 「**[!UICONTROL 機会]**」をクリックして、機会のレイアウトをカスタマイズします。

   または

   「**[!UICONTROL アカウント]**」をクリックして、アカウントのレイアウトをカスタマイズします。

1. 「**[!UICONTROL ページレイアウト]**」をクリックします。
1. 既存のページレイアウトの名前をクリックして編集します。

   または

   「**[!UICONTROL 新規]**」をクリックして、新しいページレイアウトを作成します。

1. 以下の[機会レベルまたはアカウント レベルでの  [!DNL Workfront]  セクションの設定](#configure-the-workfront-section-at-the-opportunity-or-account-level-configure-the-workfront-section-at-the-opportunity-or-account-level)に進みます。

### 機会またはアカウントレベルでの [!DNL Workfront] セクションの設定 {#configure-the-workfront-section-at-the-opportunity-or-account-level}

1. システム管理者として [!DNL Salesforce] にログインします。
1. 「**[!UICONTROL 機会]**」または「**[!UICONTROL アカウント]**」に移動します。

1. **[!UICONTROL 設定]**&#x200B;アイコンをクリックし、「**[!UICONTROL ページを編集]**」をクリックします。

1. 「**[!UICONTROL カスタム管理]**」セクションを展開します。
1. 「[!UICONTROL 機会]」または「アカウント」ページに
**[!DNL Workfront]** コンポーネントをドラッグ ＆ドロップします。

   [!DNL Workfront] セクションには、レイアウトの 1 つの列ではなく、ページの全幅を使用することをお勧めします。

1. 「**[!UICONTROL 保存]**」をクリックします。

   このレイアウトが割り当てられているすべてのユーザーが、「[!UICONTROL 機会]」または「[!UICONTROL アカウント]」のオブジェクトで「[!DNL Workfront]」セクションを表示できるようになりました。

   >[!NOTE]
   >
   >ユーザーには、「[!DNL Workfront]」セクションに [!DNL Workfront] ログイン画面が表示されます。[!DNL Workfront] アカウントを持っていない場合、セクションを折りたたむことはできますが、レイアウトから削除することはできません。ユーザーは、有効にした認証方法（強化認証または Security Assertion Markup Language（SAML）URL）を使用してログインできます。

