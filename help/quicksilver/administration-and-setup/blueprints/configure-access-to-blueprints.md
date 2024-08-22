---
user-type: administrator
product-area: system-administration;workfront-integrations
navigation-topic: best-practices-catalog
title: ブループリントへのアクセスの設定
description: システム管理者は、リクエストを保存するリクエストキューを設定することで、ユーザーがブループリントのインストールをリクエストするためのアクセス権を有効にできます。そこで、リクエストの追跡と更新を一元的に行うことができます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: d85f363f-2ab4-45cb-b851-a7f33e1ca905
source-git-commit: 55c8a3e5d0041a0e975bfd979a2d2e38930fea8d
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 97%

---

# ブループリントへのアクセス権の設定

すべての [!DNL Adobe Workfront] ユーザーが、ブループリントのカタログを参照できます。

システム管理者は以下を行えます。

* [!UICONTROL ブループリント]をレイアウトテンプレートのメインメニューに追加し、レイアウトテンプレートをユーザーやグループに割り当てる。詳しくは、[レイアウトテンプレートを使用した[!UICONTROL メインメニュー]のカスタマイズ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)と[レイアウトテンプレートへのユーザーの割り当て](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)を参照してください。

  >[!NOTE]
  >
  >* レイアウトテンプレートが割り当てられていないユーザーには、[!UICONTROL メインメニュー]に[!UICONTROL ブループリント]アイコンが表示されます。
  >* 新規レイアウトテンプレートを作成すると、[!UICONTROL メインメニュー]の[!UICONTROL アクティブなアイテム]リストに[!UICONTROL ブループリント]アイコンが、デフォルトで含まれています。


* リクエストを保存するリクエストキューを設定することで、ユーザーがブループリントのインストールをリクエストするためのアクセス権を有効にする。そこで、リクエストの追跡と更新を一元的に行うことができます。詳しくは、以下の手順に従ってください。
* ブループリントをインストールする。詳しくは、[ブループリントのインストール](../../administration-and-setup/blueprints/blueprints-install.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>
   <p>新規：標準</p>
   <p>または</p>
   <p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!DNL Workfront] 管理者である必要があります。 </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件 {#prerequisites}

* ブループリントリクエストを保存するには、既存のリクエストキューを使用する必要があります。プロジェクトはリクエストキューとして保存する必要があります。また、[!UICONTROL 進行中]のステータスになっている必要があります。
* リクエストキューは公開されている必要があります。リクエストキューの詳細で、「[!UICONTROL このキューにリクエストを追加できるユーザー]」は&#x200B;**[!UICONTROL 全員]**&#x200B;に設定する必要があります。

>[!TIP]
>
>ブループリントリクエストのリクエストキューを新規作成する場合は、ブループリントへのアクセス権を設定する前に作成してください。リクエストキューの作成については、[リクエストキューの作成](../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)を参照してください。

## ブループリントリクエストを保存するリクエストキューを選択

ユーザーからブループリントのインストールをリクエストされる前に、そのリクエスト用のリクエストキューを選択する必要があります。リクエストキューが定義されるまで、ユーザーはブループリントカタログの参照のみ可能です。

{{step1-to-blueprints}}

1. カタログ画面の右上にある「**[!UICONTROL ブループリントリクエストを設定]**」をクリックします。

   <!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>In the <strong>Configure blueprints</strong> dialog, ensure that the <strong>Configure request queues</strong> tab is selected.</p> </li>
   -->

1. **[!UICONTROL ブループリントを設定]**&#x200B;ダイアログで、アクティブなリクエストキューの名前を入力していき、検索結果に表示されたら選択します。

   >[!IMPORTANT]
   >
   >このリストには、パブリックリクエストキューのみが表示されます。リクエストキューをパブリックにするには、上記の[前提条件](#prerequisites)の節を参照してください。

   リクエストキューの環境設定が指定され、ユーザーがブループリントのインストールをリクエストできるようになりました。

   ![リクエストキューの設定](assets/Blueprints_access_setup_request_queue.png)

1. （オプション）現行のリクエストキューに変更を加えるには、「**[!UICONTROL このリクエストキューを編集]**」をクリックします。

   リクエストキュープロジェクトが新しいブラウザータブで開き、リクエストキューを必要に応じて更新できます。

1. （オプション）リクエストキューにトピックグループまたはキュートピックが含まれている場合は、それらをリストから選択できます。
1. ブループリントカタログに戻るには、「**[!UICONTROL 閉じる]**」をクリックします。

>[!NOTE]
>
>リクエストされたブループリントをインストールする際は、リクエストキューでイシューステータスを&#x200B;**[!UICONTROL クローズ]**&#x200B;または&#x200B;**[!UICONTROL 解決済み]**&#x200B;に変更して、リクエスターに通知が届くようにする必要があります。ブループリントのインストールについては、[ブループリントのインストール](../../administration-and-setup/blueprints/blueprints-install.md)を参照してください。
