---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: ブループリントへのアクセスを設定
description: システム管理者は、要求キューを設定して要求を保存することで、ユーザーがブループリントのインストールを要求するアクセスを有効にできます。 そこで、リクエストを追跡して更新する場所は 1 つです。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d85f363f-2ab4-45cb-b851-a7f33e1ca905
source-git-commit: d46eb98c443a421f340b1021972ddb89eda1966b
workflow-type: tm+mt
source-wordcount: '510'
ht-degree: 0%

---

# ブループリントへのアクセスを設定

すべて [!DNL Adobe Workfront] ユーザーはブループリントのカタログを参照できます。

システム管理者は、次の操作を実行できます。

* 追加 [!UICONTROL ブループリント] をレイアウトテンプレートのメインメニューに追加し、レイアウトテンプレートをユーザーまたはグループに割り当てます。 詳しくは、 [のカスタマイズ [!UICONTROL メインメニュー] レイアウトテンプレートの使用](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md) および [レイアウトテンプレートにユーザーを割り当てる](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md).

   >[!NOTE]
   >
   >* レイアウトテンプレートが割り当てられていないユーザーには、 [!UICONTROL ブループリント] アイコン [!UICONTROL メインメニュー].
   >* 新しいレイアウトテンプレートを作成する場合、 [!UICONTROL ブループリント] アイコンが [!UICONTROL アクティブな項目] リスト [!UICONTROL メインメニュー] デフォルトでは。



* 要求キューを設定して要求を保存することで、ユーザーがブループリントのインストールを要求できるようにします。 そこで、リクエストを追跡して更新する場所は 1 つです。 詳しくは、以下の手順に従ってください。
* ブループリントをインストールします。 詳しくは、 [ブループリントのインストール](../../administration-and-setup/blueprints/blueprints-install.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計画</strong></td> 
   <td> <p> 任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe [!DNL Workfront] ライセンス</strong></td> 
   <td>[!UICONTROL プラン ]</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>[!UICONTROL システム管理者 ]</p> </td> 
  </tr> 
 </tbody> 
</table>

## 前提条件 {#prerequisites}

* ブループリントリクエストを保存するには、既存のリクエストキューを使用する必要があります。 プロジェクトはリクエストキューとして保存する必要があります。また、次の場所に保存する必要があります。 [!UICONTROL 現在] ステータス。
* リクエストキューはパブリックにする必要があります。 リクエストキューの詳細で、[!UICONTROL このキューにリクエストを追加できるのは誰ですか？]&quot;は次の値に設定する必要があります： **[!UICONTROL 全員]**.

>[!TIP]
>
>ブループリントリクエストの新しいリクエストキューを作成する場合は、ブループリントアクセスを設定する前にキューを作成する必要があります。 リクエストキューの作成について詳しくは、 [リクエストキューの作成](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

## ブループリントリクエストを保存するリクエストキューを選択

ユーザーがブループリントのインストールをリクエストする前に、それらのリクエストのリクエストキューを選択する必要があります。 リクエストキューが定義されるまで、ユーザーはブループリントカタログのみを参照できます。

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL ブループリント]**.
1. クリック **[!UICONTROL ブループリントリクエストを設定]** をクリックします。

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>In the <strong>Configure blueprints</strong> dialog, ensure that the <strong>Configure request queues</strong> tab is selected.</p> </li>
   -->

1. の **[!UICONTROL ブループリントを設定]** ダイアログで、アクティブなリクエストキューの名前を入力し始め、検索結果に表示されたら選択します。

   >[!IMPORTANT]
   >
   >このリストに表示されるのはパブリックリクエストキューのみです。 リクエストキューを公開するには、 [前提条件](#prerequisites) 」の節を参照してください。

   リクエストキューの環境設定が設定され、ユーザーはブループリントのインストールをリクエストできるようになりました。

   ![リクエストキューの設定](assets/Blueprints_access_setup_request_queue.png)

1. （オプション）実際のリクエストキューを変更するには、 **[!UICONTROL このリクエストキューを編集]**.

   リクエストキュープロジェクトが新しいブラウザータブで開き、必要に応じて更新できます。

1. （オプション）リクエストキューにトピックグループまたはキュートピックが含まれている場合は、リストから選択できます。
1. ブループリントカタログに戻るには、 **[!UICONTROL 閉じる]**.

>[!NOTE]
>
>要求されたブループリントをインストールする場合は、問題のステータスを「 **[!UICONTROL クローズ]** または **[!UICONTROL 解決済み]** リクエストキュー内で要求者に通知を送信する。 ブループリントのインストールについて詳しくは、 [ブループリントのインストール](../../administration-and-setup/blueprints/blueprints-install.md).
