---
product-area: workfront-integrations
navigation-topic: workfront-for-slack
title: お気に入りと最近使用した項目にアクセスするには、 [!DNL Slack] を使用
description: Slack の  [!DNL Adobe Workfront]  をインストールし、設定したら、Workfront のお気に入りと最近使用した項目を表示し、Slack のどちらかのリストから項目にアクセスできます。
author: Becky
feature: Workfront Integrations and Apps
exl-id: 4bf62192-66fe-42a7-b8c0-23b7bdef45e8
TQID: https://experienceleague.adobe.com/Fqy-Tqgyza2C4STR6qD78-HsyKDiydUM1NTnzLY1-FE
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
source-wordcount: 323
ht-degree: 95%

---

# [!DNL Slack] からお気に入りと最近使用した項目にアクセス

[!DNL Adobe Workfront for Slack] のインストールと設定が完了したら、[!UICONTROL Workfront] のお気に入りと最近使用した項目を表示でき、[!DNL Slack] のリストからいずれかの項目にアクセスできます。

[!DNL Workfront with Slack] の設定に関して詳しくは、[&#x200B; [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md) の設定を参照してください。

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

* [!DNL Workfront for Slack] の設定\
   [!DNL Workfront for Slack] の設定の手順については、[&#x200B; [!DNL Adobe Workfront for Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/configure-workfront-for-slack.md) の設定を参照してください。

## [!DNL Slack] から[!UICONTROL お気に入り]リストにアクセス

1. お使いの [!DNL Slack] インスタンスにログインして、[!DNL Slack] から [!DNL Workfront] にログインします。\
   [!DNL Slack] から [!DNL Workfront] へのログインについて詳しくは、[&#x200B; [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) から  [!DNL Adobe Workfront]  にアクセスの「[!DNL Slack] から [!DNL Workfront] へのログイン」の節を参照してください。

1. 任意のチャネルから、[!UICONTROL メッセージ]フィールドに次のコマンドの入力を開始します：`/workfront favorites`

   >[!NOTE]
   >
   >コマンドでは大文字と小文字が区別されます。 `/workfront` の代わりに `/wf` でコマンドを開始できます。

   お気に入りのリストが表示されます。

1. （オプション）「**[!UICONTROL 詳細を表示]**」をクリックして、さらにお気に入りをリストします。
1. お気に入りの名前をクリックして新規のブラウザータブの [!DNL Workfront] で開きます。

## [!DNL Slack] から最近使用した項目の一覧にアクセス

1. お使いの [!DNL Slack] インスタンスにログインして、Slack から [!DNL Workfront] にログインします。\
   [!DNL Slack] から [!DNL Workfront] へのログインについて詳しくは、[&#x200B; [!DNL Slack]](../../workfront-integrations-and-apps/using-workfront-with-slack/access-workfront-from-slack.md) から  [!DNL Adobe Workfront]  にアクセスの[!DNL Slack] から [!DNL Workfront] にログインの節を参照してください。

1. 任意のチャネルから、[!UICONTROL メッセージ]フィールドに次のコマンドの入力を開始します：`/workfront recent`

   >[!NOTE]
   >
   >コマンドでは大文字と小文字が区別されます。 `/workfront` の代わりに `/wf` でコマンドを開始できます。

   最近使用した項目のリストが、最後にアクセスした順序で表示され、一番上に最新の項目が表示されます。 アイテムは一度に3つずつリストされ、オブジェクトタイプ別にグループ化されます。\

1. （オプション）「**[!UICONTROL 詳細を表示]**」をクリックして、最近使用した項目の一覧を表示します。
1. （オプション）最近アクセスした項目の名前をクリックして、新規のブラウザータブの [!DNL Workfront] で開きます。
