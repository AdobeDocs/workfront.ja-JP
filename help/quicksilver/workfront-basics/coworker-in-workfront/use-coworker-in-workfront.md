---
title: WorkfrontでのCX Coworkerの使用
content-type: reference
description: WorkfrontでCX Coworkerを利用する方法を学びましょう。
author: Becky
feature: Get Started with Workfront
source-git-commit: b88f894ad1d30382e9cb62e680d8eb87a858610f
workflow-type: tm+mt
source-wordcount: '611'
ht-degree: 7%

---

# WorkfrontでのCX Coworkerの使用

{{preview-fast-release-general}}

>[!IMPORTANT]
>
>CX Coworkerは現在、ヘルスケアや金融など、機密データを扱う業界の企業には利用できません。 AI アシスタントは、これらの組織で利用できます。 詳しくは、[AI アシスタントの概要](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md)を参照してください。

WorkfrontからCX Coworkerにアクセスできます。

WorkfrontでCoworkerを使用する場合、次のような情報とオブジェクトを操作できます。

* WorkfrontまたはWorkfront Planningにあります。
* に対する権限があります。

Coworkerは大規模なAdobe CX Enterprise エコシステムの一部であるため、Coworkerを使用して、Workfrontの右側のパネルにある他のAdobe製品の情報やオブジェクトを操作したり、WorkfrontからAdobe CX Coworker インターフェイスに移動したりできます。

Workfront以外でのCoworkerとその機能について詳しくは、[Adobe CX Enterprise Coworker Chatの概要](https://experienceleague.adobe.com/en/docs/cx-enterprise-coworker/content/chat/overview)を参照してください。


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
   <td><p>標準</p>
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

* CX CoworkerでWorkfront オブジェクトを操作する前に、そのオブジェクトに対する既存のアクセス権と権限が必要です。 例えば、Coworkerでプロジェクトに関する情報を表示するには、少なくともプロジェクトへの表示アクセス権が必要です。
* CX Coworkerを通じてWorkfrontに変更を加える前に、Workfront管理者が組織のシステム環境設定で「MCP ツールを書き込む」オプションを有効にする必要があります。 デフォルトでは、CX Coworkerには読み取り専用の機能があります。

  詳細と手順については、[&#x200B; システム環境設定の設定](/help/quicksilver/administration-and-setup/manage-workfront/security/configure-security-preferences.md)を参照してください。


## WorkfrontでのCX Coworkerの使用

1. Workfront ページの上部で、CX Coworker アイコン ![AI アイコン &#x200B;](assets/ai-icon.png)をクリックします。
1. 質問を入力するか、画面の右側にあるパネルにプロンプトを表示します。

1. Coworkerが必要な回答を提供しない場合は、プロンプトを調整して、もう一度試してください。

   プロンプトの例については、[Adobe Workfront MCP サーバーの使用](/help/quicksilver/workfront-basics/workfront-mcp-server/use-workfront-mcp-server.md)の記事のプロンプトを参照してください。
1. チャット入力ボックスのアクションのいずれかを使用します。

   * **+ （添付）**：添付メニューを開いて、メッセージにファイルまたはデータオブジェクトを追加します。
   * **プランモード**：共同作業者チャットにステップバイステップのプランを提案するよう依頼し、承認のために一時停止してから実行します。 これをオフにすると、同僚チャットが直接動作します。
   * **文字起こしビュー**:Coworker Chatの内部アクティビティ（標準、フォーカス、詳細）の表示量を制御します。
   * **マイク**：音声入力でメッセージを指示します。 録音を停止するには、もう一度選択します。
   * **送信**: メッセージを送信します。 同僚のチャットが応答している間、これは割り込みに使用できる停止制御になります。

   これらのアクションについて詳しくは、Adobe CX Coworker ドキュメントの[&#x200B; チャット入力ボックス &#x200B;](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/ui-guide#the-chat-input-box)を参照してください。

1. 以前のチャットを表示および管理するには、CX同僚パネルのチャットアイコン ![&#x200B; チャットアイコン &#x200B;](assets/ai-icon.png)をクリックします。

   チャットについて詳しくは、Adobe CX Coworker ドキュメントの[&#x200B; チャットの管理](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/ui-guide#manage-your-chats)を参照してください。
1. 出力リストなどのチャットアーティファクトを表示および管理するには、アーティファクトアイコン ![&#x200B; アーティファクトアイコン &#x200B;](assets/artifacts-icon.png)をクリックします。

   CX Coworkerのアーティファクトについて詳しくは、Adobe CX Coworker ドキュメントの[&#x200B; アーティファクト &#x200B;](https://experienceleague.adobe.com/en/docs/cx-enterprise-ai/experience-cloud-ai/coworker/chat/ui-guide#artifacts)を参照してください。
1. 同僚の設定を管理するには、設定アイコン ![設定](assets/coworker-settings-icon.png)をクリックします。
1. 同僚パネルを展開するには、展開アイコン ![展開アイコン &#x200B;](assets/coworker-expand-icon.png)をクリックします。
1. Adobe CX Coworker インターフェイスに移動するには、ページの右上隅にあるアプリアイコン ![&#x200B; アプリアイコン &#x200B;](assets/apps-icon.png)をクリックし、使用可能なアプリケーションのリストから「Coworker」を選択します。
