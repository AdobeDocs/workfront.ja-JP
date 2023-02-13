---
product-area: workfront-integrations;agile-and-teams;user-management
navigation-topic: workfront-for-microsoft-teams
title: 作成 [!DNL Adobe Workfront] タスク [!DNL Microsoft] チーム
description: 個人用タスクはAdobeで作成できます [!DNL Workfront] Microsoft Teamsの所有者がインストールおよび設定済みの場合は、チームから [!DNL Workfront] チームのMicrosoft Teamsの場合は、Workfrontにログインしている状態をMicrosoft Teamsから削除します。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 31b86c8d-967a-446a-86f2-3d38e44c45e1
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '351'
ht-degree: 1%

---

# 作成 [!DNL Adobe Workfront] タスク [!DNL Microsoft Teams]

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Work]、[!UICONTROL Plan]</p> </td> 
  </tr>
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## 前提条件

個人用タスクは、 [!DNL Adobe Workfront] から [!DNL Microsoft Teams] 次の条件が満たされた場合：

* チーム所有者がインストールおよび設定しました [!DNL Workfront for Microsoft Teams] チームのために。
* ログインしています [!DNL Workfront] から [!DNL Microsoft Teams].

>[!NOTE]
>
>[!DNL Microsoft Teams] は、 [!DNL Internet Explorer]. 次の手順で [!DNL Adobe Workfront for Microsoft Teams] 統合の場合、 [!DNL Internet Explorer].

インストールに関する情報 [!DNL Workfront for Microsoft Teams] にログインし、 [!UICONTROL Workfront] から [!DNL Microsoft Teams]を参照してください。 [インストール [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

## 個人用タスクの作成元 [!DNL Microsoft Teams]

1. にログインします。 [!DNL Workfront] から [!DNL Microsoft Teams].

   へのログインについて [!DNL Workfront]を参照してください。 [インストール [!DNL Adobe Workfront for Microsoft Teams]](../../workfront-integrations-and-apps/using-workfront-with-microsoft-teams/install-workfront-ms-teams.md).

1. を開くには **[!UICONTROL 新規タスク]** カード：

   * 次の場合、 [!DNL Workfront] ボットチャットチャネル、タイプ **[!UICONTROL 新規タスク]** 内 [!UICONTROL 会話] 新しいタスクを作成するフィールド
   * 次のチャットチャネルに属している場合、 [!DNL Workfront] ボットチャットチャネル：

      * 入力を開始 **[!DNL @workfront]** 内 [!UICONTROL 会話] 「 」フィールドで、 [!DNL Workfront] 使用するボットチャネル。
      * 入力を続行 **[!UICONTROL 新規タスク]** 内 [!UICONTROL 会話] 新しいタスクを作成するフィールド

         この [!UICONTROL 新規タスク] カードが [!DNL Workfront] ボットチャネル。

         ![ms_teams_new_task_card.png](assets/ms-teams-new-task-card-350x181.png)

1. 内 [!UICONTROL Workfront] ボットチャネル ( [!UICONTROL 新規タスク] カード：

   * 内のタスク名 **[!UICONTROL タスクのタイトルを書き込む]** フィールドに入力します。
   * タスクの説明 ( **[!UICONTROL タスクの説明を書き込む]** フィールドに入力します。
   * タスクを完了する必要がある日付 ( **[!UICONTROL 期限]** フィールドに入力します。

1. 「**[!UICONTROL 保存]」をクリックします。**

   新しい個人用タスクがに作成されます [!DNL Workfront]. A [!UICONTROL 参照番号] が割り当てられ、 [!UICONTROL 新規タスク] カード。

   参照番号の詳細については、 [[!UICONTROL 参照番号] オブジェクトの](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md#understanding-reference-numbers-of-objects) セクション [でのオブジェクトについて [!DNL Adobe Workfront]](../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md) 記事。

1. （オプション）「 **[!UICONTROL 編集]** をクリックして、タスク情報をさらに編集します。
1. （オプション）「 **[!UICONTROL 表示場所[!DNL Workfront]]** タスクを [!DNL Workfront] タスクをさらに編集し、プロジェクトに移動するか、他のユーザーに割り当てます。
