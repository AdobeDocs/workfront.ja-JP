---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: ' [!DNL Microsoft] Teams からの [!DNL Adobe Workfront] タスクの作成'
description: チーム所有者がチームに [!DNL Workfront] for Microsoft Teams をインストールし設定してある場合、Microsoft Teams から Workfront にログインすると、Microsoft Teams から Adobe [!DNL Workfront] に個人タスクを作成できます。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 31b86c8d-967a-446a-86f2-3d38e44c45e1
TQID: https://experienceleague.adobe.com/EGXeEO-HU8813eA-dyVAuKSv6rAQg8tsDiDT5leVee0
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: a7ef0b24-c866-4849-a368-53678af2dfe5
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 449
ht-degree: 100%

---

# [!DNL Microsoft Teams] からの [!DNL Adobe Workfront] タスクの作成

>[!IMPORTANT]
>
>[Microsoft が New Teams クライアントに移行すると](https://learn.microsoft.com/ja-jp/microsoftteams/teams-classic-client-end-of-availability)、Classic Teams クライアントは 2025年7月1日（PT）以降は使用できなくなります。 Microsoft Teams や Workfront などの統合アプリを引き続き使用するには、この日付までに New Teams クライアントに移行する必要があります。
>
>アップデートされた Workfront 統合が利用可能になりました。この統合には、New Teams エクスペリエンスとの完全な互換性があります。 ほとんどの場合、ユーザーが移行すると、Workfront が自動的に表示されます。 表示されない場合は、Microsoft Teams App Store から手動で統合をインストールできます。 New Teams クライアントで Workfront 統合をインストールまたは検証するには、Workfront for Microsoft Teams](/help/quicksilver/workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) の[インストール [!DNL Adobe Workfront] を参照してください。



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
   <td> <p>標準</p>
   <p>Work またはそれ以上</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

次の条件が満たされた場合、[!DNL Microsoft Teams] から [!DNL Adobe Workfront] に個人タスクを作成できます。

* チーム所有者がチームに [!DNL Workfront for Microsoft Teams] をインストールし設定してある。
* ユーザーが [!DNL Microsoft Teams] から [!DNL Workfront] にログインしている。

>[!NOTE]
>
>[!DNL Microsoft Teams] では [!DNL Internet Explorer] のサポートを終了しました。 [!DNL Adobe Workfront for Microsoft Teams] 統合を使用するには、[!DNL Internet Explorer] 以外の web ブラウザーを使用する必要があります。

[!DNL Workfront for Microsoft Teams] のインストールと [!DNL Microsoft Teams] からの [!UICONTROL Workfront] へのログインについては、[ [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) のインストールを参照してください。

## [!DNL Microsoft Teams] から個人タスクを作成

1. [!DNL Microsoft Teams] から [!DNL Workfront] にログインします。

   [!DNL Workfront] へのログインについては、[ [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md) のインストールを参照してください。

1. **[!UICONTROL 新規タスク]**&#x200B;カードを開くには

   * [!DNL Workfront] ボットチャットチャネルを使用している場合は、「[!UICONTROL 会話]」フィールドに&#x200B;**[!UICONTROL 新規タスク]**&#x200B;と入力して、新しいタスクを作成します。
   * [!DNL Workfront] ボットチャットチャネル以外のチャットチャネルを使用している場合：

      * 「[!UICONTROL 会話]」フィールドに **[!DNL @workfront]** と入力していき、目的の [!DNL Workfront] ボットチャネルを選択します。
      * 引き続き「[!UICONTROL 会話]」フィールドに&#x200B;**[!UICONTROL 新規タスク]**&#x200B;と入力して、新しいタスクを作成します。

        [!DNL Workfront] ボットチャネルに[!UICONTROL 新規タスク]カードが表示されます。

        ![ms_teams_new_task_card.png](assets/ms-teams-new-task-card-350x181.png)

1. [!UICONTROL Workfront] ボットチャネルの[!UICONTROL 新規タスク]カードで、次の情報を指定します。

   * 「**[!UICONTROL タスクのタイトルをここに書き込みます]**」フィールドにタスク名を入力します。
   * 「**[!UICONTROL タスクの説明を書き込みます]**」フィールドにタスクの説明を入力します。
   * タスクの完了期限の日付を「**[!UICONTROL 期限日]**」フィールドに入力します。

1. 「**[!UICONTROL 保存]」をクリックします。**

   新しい個人タスクが [!DNL Workfront] に作成されます。 [!UICONTROL 参照番号]がタスクに割り当てられ、[!UICONTROL 新規タスク]カードに表示されます。

   参照番号については、[ [!DNL Adobe Workfront]](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) のオブジェクトについての記事のオブジェクトの[[!UICONTROL 参照番号]](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-reference-numbers-of-objects)の節を参照してください。

1. （オプション）「**[!UICONTROL 編集]**」をクリックして、タスクの情報をさらに編集します。
1. （オプション）「**[!UICONTROL [!DNL Workfront]]** で表示」をクリックして [!DNL Workfront] の新しいタブにタスクを開き、さらに編集して、プロジェクトに移動するか、他のユーザーに割り当てます。
