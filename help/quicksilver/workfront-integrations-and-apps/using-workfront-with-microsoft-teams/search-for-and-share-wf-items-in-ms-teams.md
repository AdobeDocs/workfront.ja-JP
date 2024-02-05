---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: ' [!DNL Microsoft Teams] での  [!DNL Adobe Workfront]  項目の検索および共有'
description: ' [!DNL Microsoft Teams] の任意の [!DNL Adobe WorkfrontWorkfront] チャネルで [!DNL Workfront] 項目を検索し、これらの項目をチームのメンバーと共有できます。'
author: Becky
feature: Workfront Integrations and Apps
exl-id: 71d83723-daea-4b7b-8e5b-cfcf414611fe
source-git-commit: 1f2655c0e88a5cc918501e2a0ef830758111ded8
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 95%

---

# [!DNL Microsoft Teams] での [!DNL Adobe Workfront] 項目の検索および共有

>[!NOTE]
>
>Adobe WorkfrontとMicrosoft Teamsの統合は、現在、クラシックMicrosoft Teamsエクスペリエンスでのみサポートされています。

[!DNL Microsoft Teams] の任意の [!DNL Adobe Workfront] チャネルで [!DNL Workfront] 項目を検索し、これらの項目をチームのメンバーと共有できます。

* [ [!DNL Microsoft Teams] で  [!DNL Workfront]  項目を共有するための前提条件](#prerequisites-for-sharing-workfront-items-in-microsoft-teams-prerequisites-for-sharing-workfront-items-in-microsoft-teams)
* [ [!DNL Microsoft Teams] での  [!DNL Workfront]  項目の検索および共有](#search-for-and-share-adobe-workfront-items-in-microsoft-teams)

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Work]、[!UICONTROL Plan]</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## [!DNL Microsoft Teams] で [!DNL Workfront] 項目を共有するための前提条件 {#prerequisites-for-sharing-workfront-items-in-microsoft-teams}

次の条件が満たされた場合、[!DNL Microsoft Teams] で [!DNL Workfront] 項目を検索して共有できます。

* チーム所有者がチームに対して [!DNL Workfront for Microsoft Teams] をインストールおよび設定している。
* [!UICONTROL Microsoft Teams]. から [!DNL Workfront] にログインしている。

[!UICONTROL Workfront for Microsoft Teams] のインストールと、[!DNL Microsoft Teams] から [!UICONTROL Workfront] へのログインについては、[Adobe Workfront for Microsoft Teams のインストール](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) を参照してください。

>[!NOTE]
>
>[!DNL Microsoft Teams] は、[!DNL Internet Explorer] のサポートを終了しました。[!DNL Adobe Workfront for Microsoft Teams integration] を使用する場合は、[!DNL Internet Explorer] 以外の web ブラウザーを使用する必要があります。


## [!DNL Microsoft Teams] での [!DNL Workfront] 項目の検索および共有 {#search-for-and-share-workfront-items-in-microsoft-teams}

[!DNL Microsoft Teams] チャネルから次の [!DNL Workfront] 項目を検索できます。

* プロジェクト
* タスク

  >[!NOTE]
  >
  >個人のタスクは検索できません。

* イシュー

検索した項目が見つかったら、[!DNL Microsoft Teams] で他のユーザーと共有できます。

[!DNL Microsoft Teams] から [!DNL Workfront] 項目を検索して他のユーザーと共有するには：

1. [!DNL Microsoft Teams] で任意のチャットチャネルに移動し、**[!DNL Workfront]** アイコンをクリックします。
1. 次のいずれかの操作を行って、[!DNL Workfront] 項目を検索します。

   * 会話フィールドの下にある [!DNL Workfront] アイコンをクリックします。\

     ![ms_teams_workfront_pinned_icon_highlight.png](assets/ms-teams-workfront-pinned-icon-highlight-350x69.png)\
      設定によっては、このアイコンは&#x200B;**[!UICONTROL その他]**&#x200B;アイコンの下に表示されます。\
      ![more_icon.png](assets/more-icon-52x34.png)\
      「**[!UICONTROL 検索]**」ボックスがデフォルトで表示されます。

   * 任意のチャネルから「*@[!DNL Workfront]*」と入力し、Workfront を選択して、「**[!UICONTROL 検索]」を選択します。**

     ![ms_teams_search_from_command.png](assets/ms-teams-search-from-command-350x74.png)

1. 「[!UICONTROL 検索]」ボックスに、プロジェクト、タスク、またはイシューの名前または参照番号を入力し始めて、リストに表示されたらクリックします。\
   ![ms_teams_searching_for_items.png](assets/ms-teams-searching-for-items-350x359.png)\
   これにより、チャットフィールドに [!DNL Workfront] 項目を含むカードが追加されます。カードには、項目の名前、親オブジェクト、ステータス、優先度、完了率など、項目に関する情報が含まれます。

1. （オプション）[!DNL Workfront] カードの下にコメントを追加し、「**[!UICONTROL 送信]**」または Enter キーを押します。\
   これにより、[!DNL Workfront] 項目を含むメッセージがチャネルに送信されます。\
   チャネルのすべてのメンバーが、このメッセージを表示できます。これには、[!DNL Workfront] カードの情報が含まれます。

1. 「**[!UICONTROL Workfrontで表示]**」をクリックすると、[!DNL Workfront] に項目が表示されます。\
   [!DNL Workfront] ライセンスを持つユーザーのみが、[!DNL Workfront] で項目を表示できます。
