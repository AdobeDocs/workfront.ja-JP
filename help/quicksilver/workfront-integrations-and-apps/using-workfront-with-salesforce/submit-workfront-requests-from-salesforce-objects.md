---
product-area: workfront-integrations
navigation-topic: workfront-for-salesforce
title: 送信 [!DNL Adobe Workfront] からのリクエスト [!DNL Salesforce] オブジェクト
description: インストール後 [!DNL Adobe Workfront] 対象 [!DNL Salesforce], you can submit [!DNL Workfront] からのリクエスト [!DNL Salesforce] 商談とアカウント。 この機能は、Classic と Lightning Experience の両方のフレームワークに存在します。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 84f8cb15-4840-4fe1-bf60-93bc4283b564
source-git-commit: 5b889633a96d634a359181bfd53ec106b0f3705c
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 1%

---

# 送信 [!DNL Adobe Workfront] からのリクエスト [!DNL Salesforce] オブジェクト

インストール後 [!DNL Adobe Workfront for Salesforce]を送信し、 [!DNL Workfront] からのリクエスト [!DNL Salesforce] 商談とアカウント。 この機能は、 [!DNL Classic] および [!DNL Lightning Experience] フレームワーク

## アクセス要件

この記事で説明する機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] 計画*</p></td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>[!DNL Adobe Workfront] ライセンス*</p></td> 
   <td> <p>[!UICONTROL プラン ]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## 前提条件

次の手順で [!DNL Workfront] からのリクエスト [!DNL Salesforce] オポチュニティまたはアカウントは、お客様の環境に以下が存在することを確認します。

* お使いの [!DNL Workfront] 管理者がインストール済み [!DNL Workfront for Salesforce].\
   インストールの詳細 [!DNL Workfront for Salesforce]を参照してください。 [インストール [!DNL Adobe Workfront for Salesforce]](../../workfront-integrations-and-apps/using-workfront-with-salesforce/install-workfront-for-salesforce.md)

* お使いの [!DNL Workfront] 管理者が [!DNL Workfront] セクションで [!UICONTROL 商談] および [!UICONTROL アカウント] ページレイアウト。\
   詳しくは、 [!DNL Workfront] セクションをページレイアウトに追加する場合は、 [の設定 [!DNL Adobe Workfront] セクション [!DNL Salesforce] ユーザー](../../workfront-integrations-and-apps/using-workfront-with-salesforce/configure-wf-section-for-salesforce-users.md).

* 次の条件を満たしている： [!DNL Workfront] アカウントを使用し、 [!DNL Workfront] 」セクションを使用して、商談またはアカウント内で設定します。\
   ログインすると、 [!UICONTROL 新しいリクエスト] 」タブを開きます。

## 送信 [!DNL Workfront] からのリクエスト [!DNL Salesforce]

1. Salesforce の商談またはアカウントに移動します。
1. 次に移動： [!DNL Workfront] 」セクションに入力します。
1. 内 **[!UICONTROL 新しいリクエスト]** 」タブで、 **[!UICONTROL リクエストタイプを選択]** ドロップダウンメニュー。

   Workfrontで表示できるのと同じリクエストキューを確認できます。

1. リクエストに使用可能なフィールドの入力を開始します。

   からのリクエストの送信 [!DNL Salesforce] は、 [!DNL Workfront] web アプリケーション。

   >[!NOTE]
   >
   >を使用したドキュメントのアップロード [!DNL Workfront] プラグイン [!DNL Salesforce] は一時的に使用できなくなっています。

   引き続き、 [作成して送信 [!DNL Adobe Workfront] リクエスト](../../manage-work/requests/create-requests/create-submit-requests.md).

1. クリック **[!UICONTROL 送信]**.

## 表示 [!DNL Workfront] リクエスト

1. 次の商談またはアカウントに移動： [!DNL Salesforce].
1. 次に移動： **[!DNL Workfront]** 」セクションに入力します。

   >[!NOTE]
   >
   >使用する [!DNL Workfront] 管理者がこのセクションを設定しました。別の名前を使用している可能性があります。

1. を選択します。 **[!UICONTROL 送信されたリクエスト]** タブをクリックします。

   このタブで、この商談またはアカウントから自分または他の人が送信したすべてのリクエストを表示できます。Web アプリケーションのこのリクエストキューに送信されたリクエストは、このリストには表示されません。 [!DNL Salesforce].

   >[!NOTE]
   >
   >Web アプリケーションのこのリクエストキューに送信されたリクエストは、Salesforce のこのリストには表示されません。

   ![salesforce_submitted_requests.png](assets/salesforce-submitted-requests-350x58.png)

   送信されたリクエストに関する次の情報を表示できます。

   * リクエスト名 ( [!UICONTROL 件名] 列 )
   * 参照番号
   * リクエストタイプ
   * ステータス
   * 送信日
   * 名前でリクエスト
   * 名前に割り当て済み\

      この情報が [!DNL Workfront]の場合は、このリストでも更新されます。

1. （オプション）リクエストの名前をクリックして開きます。 [!DNL Workfront].

1. （オプション）「 **[!UICONTROL に移動します。[!DNL Salesforce]]** Workfrontの次の領域から発生した問題の商談またはアカウントにアクセスするには：

   * 内 [!UICONTROL 詳細] 問題のセクション
   * リストで問題を選択する際に、「Summary」パネルで「 [!UICONTROL 概要を開く] ![](assets/summary-panel-icon.png) 」をクリックします。
   * イシューヘッダーで、 [!UICONTROL 統合] フィールドが使用可能です。 システム管理者またはグループ管理者が [!UICONTROL 統合] フィールドに入力して、問題ヘッダーの「 Salesforce に移動」リンクを表示します。 詳しくは、 [レイアウトテンプレートを使用したオブジェクトヘッダーのカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

   >[!NOTE]
   >
   >この [!UICONTROL Salesforce に移動] リンクはすべてのに対して表示されます [!DNL Workfront] 問題を表示できるユーザー。 次をお持ちの場合は、 [!DNL Salesforce] 次にアクセスできるアカウント [!DNL Salesforce] 問題が記録された商談またはアカウント。
