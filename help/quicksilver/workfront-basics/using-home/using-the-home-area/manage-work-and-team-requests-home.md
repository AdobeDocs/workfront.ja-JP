---
product-area: projects;agile-and-teams
navigation-topic: use-the-home-area
title: ホームエリアでの作業リクエストとチームリクエストの管理
description: 作業タスクとイシューが割り当てられると、それらは自分の作業ウィジェット、自分のタスクウィジェット、自分のイシューウィジェットにリストされます。  作業項目と要求を表示、作業、または削除できます。
author: Courtney
feature: Get Started with Workfront, Work Management
exl-id: 79826743-eeb9-4849-b46f-cc3f086e3194
source-git-commit: fddb927f2c9639b4c26d590bbea7dba684ed2b6c
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 42%

---


# [!UICONTROL  ホーム ] エリアの作業項目とチームリクエストの管理

作業タスクとイシューが割り当てられると、それらは自分の作業ウィジェット、自分のタスクウィジェット、自分のイシューウィジェットにリストされます。  作業項目と要求を表示、作業、または削除できます。

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Work] 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>タスクとイシューに対する[!UICONTROL Edit]アクセス権</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されているか [!DNL Workfront] 管理者に確認してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>作業が必要なタスクやイシューに対する参加以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト </a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

+++

## 自分の作業ウィジェットでの作業項目の表示

自分に割り当てられた作業項目は、[!UICONTROL  ホーム ] の自分の作業ウィジェットに表示されます。 ウィジェット [!UICONTROL  ワークリスト ] の上部にあるフィルターを使用して、自分の作業ウィジェットに表示する作業項目を設定できます。

作業の準備ができた項目または現在作業中の項目を表示するフィルターを選択できます。

この記事では、[!UICONTROL ホーム]エリアのフィルターを使用して、現在作業中の項目、または作業を開始することを検討している項目を表示する方法について説明します。[!UICONTROL  ホーム ] エリアでフィルターを使用する方法について詳しくは、[ ホーム [!UICONTROL  エリアの [!UICONTROL  ワークリスト ] の項目を表示 ]](/help/quicksilver/workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md) を参照してください。

自分の作業ウィジェットに作業項目を表示するには：

1. 右上隅の **[!UICONTROL メインメニュー]**![ メインメニューアイコン ](assets/main-menu-icon.png) をクリックし、**[!UICONTROL ホーム]** をクリックします。
1. （条件付き） **カスタマイズ** をクリックして **担当作業** ウィジェットを追加します。

1. ウィジェットワークリストの左上隅にある **フィルター** アイコン ![ フィルターアイコン ](assets/filter-nwepng.png) をクリックします。

1. タスクに対して、次のいずれかのオプションまたは両方をクリックします。

   **[!UICONTROL 準備完了]：**&#x200B;開始する準備ができたタスクとイシューのみを表示します。以下の条件の両方が成り立つ必要があります。

   * タスクとその親には、作業を妨げる先行タスクやタスク制約がない。
   * タスクまたはイシューの[!UICONTROL 予定開始日]は過去、または最大 2 週間先です。

   **[!UICONTROL 準備未完了]**：まだ開始する準備ができていないタスクとイシューのみを表示します。以下の条件のいずれか 1 つが成り立つ必要があります。

   * タスクとその親に、作業を妨げる先行タスクやタスク制約がある可能性がある。
   * タスクまたはイシューの[!UICONTROL 予定開始日]は 2 週間以上先です。

1. [!UICONTROL タスク]または[!UICONTROL イシュー]の下にある「**[!UICONTROL 作業中]**」をクリックして、現在取り組んでいるタスクとイシューを表示します。
1. [!UICONTROL イシュー]の下の「**[!UICONTROL 要求済み]**」をクリックすると、要求された（割り当てられている）が、まだ作業を承諾していないイシューが表示されます。

## チームリクエストウィジェットのチームリクエストにアクセスします

チームに割り当てられたリクエストには、[!UICONTROL  ホーム ] エリアのチームリクエスト ウィジェットから直接アクセスできます。 チームリクエストについて詳しくは、[チームリクエストの概要](../../../people-teams-and-groups/work-with-team-requests/team-requests-overview.md)を参照してください。

チームリクエストにアクセスするには：

1. 右上隅の **[!UICONTROL メインメニュー]**![ メインメニューアイコン ](assets/main-menu-icon.png) をクリックし、**[!UICONTROL ホーム]** をクリックします。
1. （条件付き） **カスタマイズ** をクリックして **チームリクエスト** ウィジェットを追加します。

   このウィジェットは、チームのグループ化の下にチームリクエストを表示します。 **[!UICONTROL チームリクエスト]** ウィジェットが表示され、自分が参加しているチームに割り当てられたすべてのリクエストが表示されます。 チームリクエストの作業について詳しくは、[作業とチームリクエストを管理](../../../people-teams-and-groups/work-with-team-requests/manage-work-and-team-requests.md)を参照してください。

   ![ チームリクエストウィジェット ](assets/team-request-widget.png)

## 自分の作業ウィジェットでの作業項目の操作

「[!UICONTROL  作業対象 ]」ボタンをクリックすると、作業項目を送信したユーザーと、作業を開始する作業項目に割り当てられている可能性のある他のユーザーに示されます。

作業項目を作業する手順は、次のとおりです。

1. 右上隅の **[!UICONTROL メインメニュー]**![ メインメニューアイコン ](assets/main-menu-icon.png) をクリックし、**[!UICONTROL ホーム]** をクリックします。
1. （条件付き） **カスタマイズ** をクリックして **担当作業** ウィジェットを追加します。

1. ウィジェットの **[!UICONTROL ワークリスト]** エリアで、作業するリクエストを選択し、「**[!UICONTROL 作業]**」をクリックします。
1. 作業項目の上にマウスポインターを置いて「**概要** アイコンをクリックすると、作業項目に関する情報が表示されます。

   ![ 概要を開く ](assets/open-summary-new-home.png)


## 作業項目を削除

作業アイテムを作業しない場合は、リストから削除できます。

作業項目を削除する手順は、次のとおりです。

1. 右上隅の **[!UICONTROL メインメニュー]**![ メインメニューアイコン ](assets/main-menu-icon.png) をクリックし、**[!UICONTROL ホーム]** をクリックします。
1. （条件付き） **カスタマイズ** をクリックして **担当作業** ウィジェットを追加します。

1. ウィジェットのワークリストで、作業項目にポインタを合わせ、「**概要** アイコンをクリックすると、作業項目に関する情報が表示されます。
   ![ 概要を開く ](assets/open-summary-new-home.png)
1. 「**割り当て**」セクションで、自分の名前を削除します。
   ![ 割り当てを削除 ](assets/remove-assignment.png)



<!--
## Reassign a request

1. Click the **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **[!UICONTROL Home]**.
1. In the **[!UICONTROL Work List]** area, select the request you want to reassign.

1. Click on the **[!UICONTROL Assignments]** widget and remove yourself from the request, then type the name of the user you want to reassign the request to.

   >[!TIP]
   >
   >If the work request is still in the Ready to Start or Not Ready state, you can use the **[!UICONTROL Reassign]** button in the **[!UICONTROL More]** menu in the [!UICONTROL Work List].\
   >![Reassign button](assets/reassign-in-left-panel-350x204.png)

1. If a task's status is changed to [!UICONTROL New] or [!UICONTROL In Progress] after it was completed, you must unassign the user, save the task, then reassign the user in order for the task to reappear in their Home Work List.



## Reply to a request

You can reply to a request to further clarify the request or to propose a new date.

1. Click the **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **[!UICONTROL Home]**.
1. In the **[!UICONTROL Work List]** area, select the request you want to reply to.
1. Locate the individual who assigned the request to you.

   You can find this information on the [!UICONTROL Updates] tab of the task. Make sure the option to **[!UICONTROL Show System Updates]** is enabled.

1. Click **[!UICONTROL Start new update]** and begin typing your reply.
1. Enter the name of the recipient in the **[!UICONTROL Notify]** box, then click **[!UICONTROL Update]**.

   >[!TIP]
   >
   >If the work request is still in the Ready to Start or [!UICONTROL Not Ready] state, you can use the **[!UICONTROL Reply]** button in the **[!UICONTROL More]** menu in the [!UICONTROL Work List].\
   >![[!UICONTROL Reply button]](assets/reassign-in-left-panel-350x204.png)   

   -->
