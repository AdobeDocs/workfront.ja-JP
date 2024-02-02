---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Slack からのタスクとイシューの作成
description: Slack 向け  [!DNL Adobe Workfront]  のインストールと設定が完了したら、Slack からタスクとイシューを作成し、Workfront のプロジェクトに関連付けることができます。
author: Becky
feature: Workfront Integrations and Apps
exl-id: cf4a514a-fe69-4c2f-8e35-5738dfaab24e
source-git-commit: 65bfeafe67a10c72e87a02e0ece285df619fcb81
workflow-type: ht
source-wordcount: '431'
ht-degree: 100%

---

# [!DNL Slack] からのタスクとイシューの作成

[!DNL Adobe Workfront for Slack] のインストールと設定が完了したら、[!DNL Slack] からタスクとイシューを作成し、[!DNL Workfront] のプロジェクトに関連付けることができます。

[!DNL Slack] を用いた [!DNL Workfront] の設定に関して詳しくは、[ [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md) の設定を参照してください。

アクセスレベルでタスクとイシューを作成するアクセス権と、関連付けているプロジェクトに対する[!UICONTROL 参加]権限が必要です。

アクセスレベルの詳細については、[アクセスレベルの概要](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)を参照してください。オブジェクトに対する権限について詳しくは、[オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">[!DNL [!DNL Adobe Workfront] プラン]</a>*</td> 
   <td> <p>[!UICONTROL Pro] 以降</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## 前提条件

[!DNL Slack] からタスクとイシューを作成する前に、次を実行する必要があります。

* Slack 向け [!DNL Workfront] を設定する\
   [!DNL Workfront for Slack] の設定手順については、[設定 [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md)を参照してください。

## [!DNL Slack] からのタスクの作成

1. [!DNL Slack] インスタンスにログインして、[!DNL Slack] から [!DNL Workfront] にログインします。\
   [!DNL Slack] から Workfront へのログインについて詳しくは、[ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) から  [!DNL Adobe Workfront]  にアクセスの「[!DNL Slack] から [!DNL Workfront] へのログイン」の節を参照してください。

1. 任意のチャネルから、メッセージフィールドに次のコマンドを入力します。

   `/workfront add task <Task Name>`

   >[!NOTE]
   >
   >コマンドでは大文字と小文字が区別されます。`/workfront` の代わりに `/wf` でコマンドを開始できます。
   >  
   >タスク名は、[!DNL Workfront] インターフェイスに表示されるとおりに、括弧や引用符を付けずに入力する必要があります。

1. （オプション）新しいタスクを関連付けるプロジェクトの名前の入力を開始し、リストに表示されたら選択します。\
   選択したプロジェクトにタスクが追加されたことを示す確認メッセージが表示されます。
1. （オプション）確認メッセージに表示されるタスクの名前をクリックすると、[!DNL Workfront]（新しいブラウザータブ）で開きます。

## [!DNL Slack] からのイシュー作成

1. [!DNL Slack] インスタンスにログインして、[!DNL Slack] から [!DNL Workfront] にログインします。\
   [!DNL Slack] から [!DNL Workfront] へのログインに関して詳しくは、[ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) から  [!DNL Adobe Workfront]  にアクセスにある「[!DNL Slack]から[!DNL Workfront]へのログイン」の節を参照してください。

1. 任意のチャネルから、メッセージフィールドに次のコマンドを入力します。

   `/workfront add issue <Issue Name>`

   >[!NOTE]
   >
   >コマンドでは大文字と小文字が区別されます。コマンドは、「/workfront」ではなく「/wf」を使用して開始できます。 \
   >イシュー名は、[!DNL Workfront] インターフェイスに表示されるとおりに、括弧や引用符を付けずに入力する必要があります。

1. （オプション）新しいイシューを関連付けるプロジェクトの名前の入力を開始し、リストに表示されたら選択します。\
   選択したプロジェクトにイシューが追加されたことを示す確認メッセージが表示されます。
1. （オプション）確認メッセージに表示されるイシューの名前をクリックすると、[!DNL Workfront]（新しいブラウザータブ）で開きます。
