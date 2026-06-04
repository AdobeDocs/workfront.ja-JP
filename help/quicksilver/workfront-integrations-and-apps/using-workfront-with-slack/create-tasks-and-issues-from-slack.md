---
product-area: workfront-integrations;projects
navigation-topic: workfront-for-slack
title: Slack からのタスクとイシューの作成
description: Slack 向け  [!DNL Adobe Workfront]  のインストールと設定が完了したら、Slack からタスクとイシューを作成し、Workfront のプロジェクトに関連付けることができます。
author: Becky
feature: Workfront Integrations and Apps
exl-id: cf4a514a-fe69-4c2f-8e35-5738dfaab24e
TQID: https://experienceleague.adobe.com/IVleUkmG-O8tjYeup3EiKB5DQIidKr9GaAVhRJHVZ3U
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
subfeature_v2:
  - id: e4fedd42-4a54-4109-859f-13c7f0366a72
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 428
ht-degree: 100%

---

# [!DNL Slack] からのタスクとイシューの作成

[!DNL Adobe Workfront for Slack] のインストールと設定が完了したら、[!DNL Slack] からタスクとイシューを作成し、[!DNL Workfront] のプロジェクトに関連付けることができます。

[!DNL Slack] を用いた [!DNL Workfront] の設定に関して詳しくは、[ [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md) の設定を参照してください。

アクセスレベルでタスクとイシューを作成するアクセス権と、関連付けているプロジェクトに対する[!UICONTROL 参加]権限が必要です。

アクセスレベルの詳細については、[アクセスレベルの概要](../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md)を参照してください。 オブジェクトに対する権限について詳しくは、[オブジェクトに対する共有権限の概要](../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

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
   <td> <p>任意</p>
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

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
   >コマンドでは大文字と小文字が区別されます。 `/workfront` の代わりに `/wf` でコマンドを開始できます。
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
   >コマンドでは大文字と小文字が区別されます。 コマンドは、「/workfront」ではなく「/wf」を使用して開始できます。 \
   >イシュー名は、[!DNL Workfront] インターフェイスに表示されるとおりに、括弧や引用符を付けずに入力する必要があります。

1. （オプション）新しいイシューを関連付けるプロジェクトの名前の入力を開始し、リストに表示されたら選択します。\
   選択したプロジェクトにイシューが追加されたことを示す確認メッセージが表示されます。
1. （オプション）確認メッセージに表示されるイシューの名前をクリックすると、[!DNL Workfront]（新しいブラウザータブ）で開きます。
