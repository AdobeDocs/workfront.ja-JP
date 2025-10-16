---
product-area: workfront-integrations
keywords: google,doc,ドキュメント,シート,スライド
navigation-topic: workfront-for-g-suite
title: Google Workspaceから  [!DNL Adobe Workfront]  ホームコンテンツへのアクセス
description: Google Workspaceから離れることなく、割り当てられたすべてのタスク、イシュー、承認およびアクセス要求を含む  [!DNL Adobe Workfront]  ホームコンテンツにアクセスできます。
author: Becky
feature: Workfront Integrations and Apps
exl-id: da2ecaf1-5cfb-470e-90a1-fbb386db8670
source-git-commit: 1e5b3c7d087c34870ccb0f4e65021358f08b81bf
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 38%

---

# [!DNL Google Workspace] から [!DNL Adobe Workfront] [!UICONTROL ホーム] コンテンツへのアクセス

>[!IMPORTANT]
>
>より安定したスケーラブルな統合を実現するために、アドビでは、Workfront Automation and Integration （Fusion）を使用した最新の柔軟な統合アプローチに移行しています。 この移行プロセスの一環として、Google Workspaceの次のWorkfront機能は、**2026 年 2 月 28 日** 以降は使用できなくなります。
>
>* Workfront内からのGoogle Workspace機能へのアクセス
>
>* Gmail またはWorkfrontのカレンダーサイトパネルからのGoogle タスクの表示と管理
>
>Google Workspaceを使用した組織の統合のニーズに対しては、Workfront Automation and Integration を使用することをお勧めします。
>
>Workfrontの自動処理と統合の概要については、[Adobe Workfront Fusion の概要 &#x200B;](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/workfront-fusion-overview) を参照してください。
>
>Google WorkspaceのWorkfront Automation and Integration モジュールの具体的な機能については、{Gmail モジュール [&#x200B; および &#x200B;](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/gmail-modules)2}Google カレンダーモジュール [&#x200B; を参照してください。](https://experienceleague.adobe.com/ja/docs/workfront-fusion/using/references/apps-and-their-modules/third-party-app-connectors/google-calendar-modules)

Google Workspaceから離れることなく、割り当てられたすべてのタスク、イシュー、承認、アクセスリクエストを含む [!DNL Adobe Workfront] [!UICONTROL &#x200B; ホーム &#x200B;] コンテンツにアクセスできます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p><p>ワークまたはそれ以上</p>
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

[!DNL Google Workspace] から [!UICONTROL ホーム]コンテンツにアクセスする前に、次の操作を実行する必要があります。

* [!DNL Workfront for Google Workspace] をインストール\
   手順について詳しくは、[インストール [!DNL Adobe Workfront for Google Workspace]](../../workfront-integrations-and-apps/workfront-for-g-suite/install-workfront-for-gsuite.md)を参照してください。

## [!DNL Google Workspace] から [!DNL Workfront] [!UICONTROL ホーム]へのアクセス

1. [!DNL Workfront] にログインしていることを確認します。
1. Google Workspaceの [!UICONTROL Workfront] パネルが表示されない場合は、ページの右端にあるア [!DNL Workfront] オンサイドバーの ![&#x200B; アイコン &#x200B;](assets/wf-lion-icon.png)3&rbrace;Workfront アイコン &rbrace; をクリックします。[!DNL Google Workspace]
1. [!DNL Google Workspace] の [!DNL Workfront] 上部に左向き矢印が表示される場合、[!UICONTROL ホーム]エリアに移動する矢印をクリックします。

1. **[!UICONTROL 並べ替え]** 領域で、展開する矢印 ![&#x200B; 展開する矢印 &#x200B;](assets/dropdown-arrow.png) をクリックし、作業アイテムのグループ化方法を指定するオプションをクリックして、目的の作業アイテムを見つけることができます。

   **[!UICONTROL コミット日]**&#x200B;または&#x200B;**[!UICONTROL 完了予定]**&#x200B;日で並べ替えする場合、最も古い作業アイテムが一番上に表示されます。

   **[!UICONTROL プロジェクト]**&#x200B;で並び替えする場合、作業アイテムは親プロジェクトの順に表示され、アルファベット順に A から Z の順に表示されます。親プロジェクトのない作業アイテムは、**[!UICONTROL プロジェクトなし]**&#x200B;の下に表示されます。

1. 表示するグループ化の展開矢印 ![&#x200B; 展開矢印 &#x200B;](assets/dropdown-arrow.png) をクリックします。

   各グループ内に含まれる項目の数は括弧で囲まれて表示されます。[!UICONTROL 展開]矢印をクリックすると、グループ内のすべての作業アイテムが表示されます。

   作業アイテムは次のように表示されます。

   * ![&#x200B; タスクアイコン &#x200B;](assets/task-icon.png)**タスク** 親プロジェクト名、タスク名および予定完了日を表示します。

   * ![&#x200B; イシューアイコン &#x200B;](assets/issue-icon.png)**イシュー** 親プロジェクト名、イシュー名および予定完了日を表示します。

   * ![&#x200B; ドキュメントアイコン &#x200B;](assets/document-icon.png)**承認** 要求者の名前、ドキュメント名、送信日が表示されます。
   * **アクセスリクエスト**&#x200B;は、リクエスターの名前、オブジェクト名および送信日を表示します。オブジェクトタイプのアイコンが左側に表示されます。

1. 作業アイテムの任意の場所をクリックして、その詳細、更新およびドキュメントを表示します。
