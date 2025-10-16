---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: お気に入りと最近使用した項目にアクセスするには、 [!DNL Slack] を使用
description: Slack の  [!DNL Adobe Workfront]  をインストールし、設定したら、Workfront のお気に入りと最近使用した項目を表示し、Slack のどちらかのリストから項目にアクセスできます。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4bf62192-66fe-42a7-b8c0-23b7bdef45e8
source-git-commit: 6178cabbf021fbf92bd8795c5c2bd0346801d64d
workflow-type: tm+mt
source-wordcount: '326'
ht-degree: 95%

---

# [!DNL Slack] からお気に入りと最近使用した項目にアクセス

[!DNL Adobe Workfront for Slack] のインストールと設定が完了したら、[!UICONTROL Workfront] のお気に入りと最近使用した項目を表示でき、[!DNL Slack] のリストからいずれかの項目にアクセスできます。

[!DNL Workfront with Slack] の設定に関して詳しくは、[ [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md) の設定を参照してください。

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

[!DNL Slack] からお気に入りと最近使用した項目にアクセスする前に、以下を行います

* [!DNL Workfront for Slack] を設定\
   [!DNL Workfront for Slack] の設定の手順については、[ [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md) の設定を参照してください。

## [!DNL Slack] から[!UICONTROL お気に入り]リストにアクセス

1. お使いの [!DNL Slack] インスタンスにログインして、[!DNL Slack] から [!DNL Workfront] にログインします。\
   [!DNL Slack] から [!DNL Workfront] へのログインについて詳しくは、[ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) から  [!DNL Adobe Workfront]  にアクセスの「[!DNL Slack] から [!DNL Workfront] へのログイン」の節を参照してください。

1. 任意のチャネルから、[!UICONTROL メッセージ]フィールドに次のコマンドの入力を開始します：`/workfront favorites`

   >[!NOTE]
   >
   >コマンドでは大文字と小文字が区別されます。`/workfront` の代わりに `/wf` でコマンドを開始できます。

   お気に入りのリストが表示されます。

1. （オプション）「**[!UICONTROL 詳細を表示]**」をクリックして、さらにお気に入りをリストします。
1. お気に入りの名前をクリックして新規のブラウザータブの [!DNL Workfront] で開きます。

## [!DNL Slack] から最近使用した項目の一覧にアクセス

1. お使いの [!DNL Slack] インスタンスにログインして、Slack から [!DNL Workfront] にログインします。\
   [!DNL Slack] から [!DNL Workfront] へのログインについて詳しくは、[ [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) から  [!DNL Adobe Workfront]  にアクセスの[!DNL Slack] から [!DNL Workfront] にログインの節を参照してください。

1. 任意のチャネルから、[!UICONTROL メッセージ]フィールドに次のコマンドの入力を開始します：`/workfront recent`

   >[!NOTE]
   >
   >コマンドでは大文字と小文字が区別されます。`/workfront` の代わりに `/wf` でコマンドを開始できます。

   最近使用した項目のリストが、最後にアクセスした順序で表示され、一番上に最新の項目が表示されます。項目は一度に 3 つずつリストされ、オブジェクトタイプ別にグループ化されます。\

1. （オプション）「**[!UICONTROL 詳細を表示]**」をクリックして、最近使用した項目の一覧を表示します。
1. （オプション）最近アクセスした項目の名前をクリックして、新規のブラウザータブの [!DNL Workfront] で開きます。
