---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: ' [!DNL Salesforce] オブジェクトからの [!DNL Adobe Workfront] リクエストの送信'
description: インストール後 [!DNL Adobe Workfront] 対象： [!DNL Salesforce], you can submit [!DNL Workfront] からのリクエスト [!DNL Salesforce] 商談とアカウント。 この機能は、Classic と Lightning Experience の両方のフレームワークに存在します。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 84f8cb15-4840-4fe1-bf60-93bc4283b564
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: ht
source-wordcount: '546'
ht-degree: 100%

---

# [!DNL Salesforce] オブジェクトからの [!DNL Adobe Workfront] リクエストの送信

[!DNL Adobe Workfront for Salesforce] をインストールすると、[!DNL Salesforce] の商談およびアカウントから [!DNL Workfront] リクエストを送信できるようになります。この機能は、[!DNL Classic] と [!DNL Lightning Experience] の両方のフレームワークに存在します。

## アクセス要件

この記事で説明されている機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] プラン*</p></td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] ライセンス*</p></td> 
   <td> <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 前提条件

[!DNL Salesforce] の商談やアカウントから [!DNL Workfront] リクエストを送信するには、お使いの環境が以下の条件を満たしていることを確認してください。

* [!DNL Workfront] 管理者が [!DNL Workfront for Salesforce] をインストールしてある。\
   [!DNL Workfront for Salesforce] のインストールについて詳しくは、[ [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md) のインストールを参照してください。

* [!DNL Workfront] 管理者が、[!UICONTROL 商談]ページと[!UICONTROL アカウント]ページのレイアウトに「[!DNL Workfront]」セクションを追加してある。\
   ページレイアウトへの「[!DNL Workfront]」セクションの追加について詳しくは、[ [!DNL Salesforce] ユーザーに対する「 [!DNL Adobe Workfront] 」セクションの設定](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md)を参照してください。

* [!DNL Workfront] アカウントがあり、商談またはアカウント内の「[!DNL Workfront]」セクションからログインできる。\
   ログインすると「[!UICONTROL 新しい要求]」タブが表示され、リクエストを入力できるようになります。

## [!DNL Salesforce] からの [!DNL Workfront] リクエストの送信

1. Salesforce で商談またはアカウントに移動します。
1. 「[!DNL Workfront]」セクションに移動します。
1. 「**[!UICONTROL 新しい要求]**」タブで、**[!UICONTROL リクエストタイプを選択]**&#x200B;ドロップダウンメニューからリクエストタイプを選択します。

   Workfront で表示されるリクエストキューと同じものが表示されます。

1. リクエストに使用できるフィールドに入力していきます。

   [!DNL Salesforce] からのリクエストの送信は、[!DNL Workfront] web アプリケーションでのリクエストの送信と同じです。

   >[!NOTE]
   >
   >[!DNL Salesforce] の [!DNL Workfront] プラグインを使用したドキュメントのアップロードは、一時的に利用できなくなっています。

   引き続き、[ [!DNL Adobe Workfront] リクエストの作成と送信](../../manage-work/requests/create-requests/create-submit-requests.md)で説明されている手順に従います。

1. 「**[!UICONTROL 送信]**」をクリックします。

## [!DNL Workfront] リクエストの表示

1. [!DNL Salesforce] で商談またはアカウントに移動します。
1. 「**[!DNL Workfront]**」セクションに移動します。

   >[!NOTE]
   >
   >[!DNL Workfront] 管理者によるこのセクションの設定によっては、別の名前が付けられている場合があります。

1. 「**[!UICONTROL 送信済みの要求]**」タブを選択します。

   このタブには、自分または他のユーザーがこの商談またはアカウントから送信したすべてのリクエストが表示されきます。Web アプリケーションでこのリクエストキューに送信されたリクエストは、[!DNL Salesforce] のこのリストには表示されません。

   >[!NOTE]
   >
   >Web アプリケーションでこのリクエストキューに送信されたリクエストは、Salesforce のこのリストには表示されません。

   ![salesforce_submitted_requests.png](assets/salesforce-submitted-requests-350x58.png)

   送信済みのリクエストに関する次の情報が表示されます。

   * リクエスト名（[!UICONTROL 件名]列）
   * 参照番号
   * リクエストタイプ
   * ステータス
   * 送信日
   * 要求者名
   * 割り当て先の名前

     この情報が [!DNL Workfront] で更新されると、このリストでも更新されます。

1. （オプション）リクエストの名前をクリックして [!DNL Workfront] で開きます。

1. （オプション）「**[!UICONTROL [!DNL Salesforce]]**&#x200B;に移動」をクリックして、Workfront の以下のエリアからイシューが発生した商談またはアカウントにアクセスします。

   * イシューの[!UICONTROL 詳細]セクション
   * 概要パネル（リスト内のイシューを選択するときに、リストのツールバーで[!UICONTROL 概要を開く]![](assets/summary-panel-icon.png) をクリックしたとき）。
   * イシューヘッダー（[!UICONTROL 統合]フィールドが使用可能なとき）。システム管理者またはグループ管理者が、レイアウトテンプレートに[!UICONTROL 統合]フィールドを追加して、イシューヘッダーに「Salesforce に移動」リンクを表示する必要があります。詳しくは、[レイアウトテンプレートを使用したオブジェクトヘッダーのカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md)を参照してください。

   >[!NOTE]
   >
   >「[!UICONTROL Salesforce に移動]」リンクは、イシューを表示できるすべての [!DNL Workfront] ユーザーに表示されます。イシューが記録された [!DNL Salesforce] の商談またはアカウントに移動するには、[!DNL Salesforce] アカウントが必要です。
