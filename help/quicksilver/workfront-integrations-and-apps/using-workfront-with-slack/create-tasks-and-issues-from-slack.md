---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: タスクとタスクのSlack
description: のインストールと設定が完了したら、 [!DNL Adobe Workfront] Slackに関しては、Slackからタスクとイシューを作成し、Workfrontのプロジェクトに関連付けることができます。
author: Becky
feature: Workfront Integrations and Apps
exl-id: cf4a514a-fe69-4c2f-8e35-5738dfaab24e
source-git-commit: 04782dfdb8c1ed24bb9c7399a01511c0cbd2dec3
workflow-type: tm+mt
source-wordcount: '440'
ht-degree: 0%

---

# タスクとタスクの作成元 [!DNL Slack]

のインストールと設定が完了したら、 [!DNL Adobe Workfront for Slack]を使用すると、次の場所からタスクや問題を作成できます： [!DNL Slack] でプロジェクトに関連付けます。 [!DNL Workfront].

設定に関する詳細 [!DNL Workfront] と [!DNL Slack]を参照してください。 [設定 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

アクセスレベルでタスクとイシューを作成するアクセス権があり、 [!UICONTROL 投稿] 関連付けるプロジェクトに対する権限。

アクセスレベルの詳細については、 [アクセスレベルの概要](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md). オブジェクトに対する権限の詳細については、 [オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] 計画]</a>*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。\

## 前提条件

タスクとタスクを作成する前に [!DNL Slack]を

* 設定 [!DNL Workfront] Slack\
   設定手順 [!DNL Workfront for Slack]を参照してください。 [設定 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md).

## タスクの作成元 [!DNL Slack]

1. にログインします。 [!DNL Slack] インスタンスとログイン [!DNL Workfront] から [!DNL Slack].\
   からWorkfrontにログインする方法について詳しくは、 [!DNL Slack]詳しくは、 [!DNL Workfront] から [!DNL Slack]」セクション内の [アクセス [!DNL Adobe Workfront] から [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. 任意のチャネルから、メッセージフィールドに次のコマンドを入力します。

   `/workfront add task <Task Name>`

   >[!NOTE]
   >
   >コマンドでは大文字と小文字が区別されます。 コマンドは、 `/wf` の代わりに `/workfront`.
   >  
   >タスク名は、 [!DNL Workfront] インターフェイスで使用できます。\
   >![add_task_to_project.png](assets/add-task-to-project-350x63.png)

1. （オプション）新しいタスクを関連付けるプロジェクトの名前の入力を開始し、リストに表示されたら選択します。\
   選択したプロジェクトにタスクが追加されたことを示す確認メッセージが表示されます。
1. （オプション）確認メッセージに表示されるタスクの名前をクリックして、 [!DNL Workfront]（新しいブラウザータブ）

## 問題の作成元 [!DNL Slack]

1. にログインします。 [!DNL Slack] インスタンスとログイン [!DNL Workfront] から [!DNL Slack].\
   へのログインの詳細 [!DNL Workfront] から [!DNL Slack]詳しくは、 [!DNL Workfront] から [!DNL Slack]」セクション内の [アクセス [!DNL Adobe Workfront] から [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md).

1. 任意のチャネルから、メッセージフィールドに次のコマンドを入力します。

   `/workfront add issue <Issue Name>`

   >[!NOTE]
   >
   >コマンドでは大文字と小文字が区別されます。 コマンドは、「/workfront」ではなく「/wf」を使用して開始できます。 \
   >問題名は、 [!DNL Workfront] インターフェイスで使用できます。\
   >![slack_add_issue_to_project.png](assets/slack-add-issue-to-project-350x88.png)

1. （オプション）新しいイシューを関連付けるプロジェクトの名前を入力し、リストに表示されたら選択します。\
   選択したプロジェクトに問題が追加されたことを示す確認メッセージが表示されます。
1. （オプション）確認メッセージに表示される問題の名前をクリックして、 [!DNL Workfront]（新しいブラウザータブ）
