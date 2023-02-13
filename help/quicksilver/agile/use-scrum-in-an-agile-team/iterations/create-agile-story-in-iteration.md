---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: 反復での俊敏なストーリーの作成
description: この記事では、既に反復している場合に、新しい俊敏なストーリーを作成する方法について説明します。
author: Lisa
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 0%

---

# 反復での俊敏なストーリーの作成

この記事では、既に反復している場合に、新しい俊敏なストーリーを作成する方法について説明します。 タスク、問題、または [!DNL Adobe Workfront]を参照してください。 [既存の反復にストーリーを追加する](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計画*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Work] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>[!UICONTROL Worker] 以降</p> <p>注意：まだアクセス権がない場合は、 [!DNL Workfront] 管理者（アクセスレベルに追加の制限を設定している場合） を参照してください。 [!DNL Workfront] 管理者はアクセスレベルを変更できます。詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>[!UICONTROL ストーリーが存在するプロジェクトへの [!UICONTROL 管理 ] アクセス権</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## 反復での俊敏なストーリーの作成

1. ストーリーを作成するアジャイルな反復に移動します。

   1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe] Workfront、 **[!UICONTROL チーム]**.

   1. （オプション） **[!UICONTROL チームの切り替え]** アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png)をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索します。

   1. 左のパネルで、「 」を選択します。 **[!UICONTROL 反復]**.
   1. ストーリーを作成する特定の反復の名前をクリックします。
   1. 左のパネルで、「 」を選択します。 **[!UICONTROL ストーリー]**.

1.  クリック **[!UICONTROL 新しいストーリー].**
1. 次の情報を指定します。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL ストーリー名 ]</strong></td>
      <td>ストーリーの名前を入力します。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 説明 ]</strong></td>
      <td>ストーリーの説明を入力します。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 準備完了 ]</strong></td>
      <td>ストーリーを反復に追加する準備が整ったら、このオプションを選択します。 このオプションを選択すると、バックログ内のどのストーリーを反復に追加する準備ができているかをユーザーに示します。<br>ストーリーは、マークされているかどうかに関わらず、繰り返しに追加できます <strong>[!UICONTROL 準備完了 ]。</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 予測 ] （ポイント）</strong></td>
      <td>ストーリーの推定を指定します。 アジャイルチームがストーリーをポイント単位で推定するように設定されている場合、デフォルトでは 1 ポイントが 8 時間になります。 見積もりは、ストーリーに [!UICONTROL 予定時間 ] として追加されます。<br>例えば、ストーリーを 3 ポイントと見積もる場合、デフォルトの動作では、ストーリーに 24 時間計画を追加します。<br>ストーリーにサブタスクが含まれる場合は、すべてのサブタスクの合計見積もりで親ストーリーの見積もりが決まることに注意してください。 詳しくは、 <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/add-a-subtask-to-an-existing-story-scrum.md" class="MCXref xref">[!UICONTROL スクラム ] ボード上の既存のストーリーにサブタスクを追加</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 親プロジェクト ]</strong></td>
      <td>このストーリーを関連付けるプロジェクトの名前を入力します。<br>デフォルトでは、ストーリーの色は、このプロジェクトの他のストーリーと同じ色で表示されます。<br>プロジェクトのステータスは [!UICONTROL Current] に設定する必要があります。 プロジェクトのステータスが [!UICONTROL Current] 以外の場合は、ドロップダウンメニューに表示されません。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 親タスク ]</strong></td>
      <td>親プロジェクトを選択した後で、親タスクを選択することもできます。 親タスクを選択すると、ストーリーは、選択したプロジェクトの親タスクのサブタスクとして作成されます。<br>ストーリーの親タスクの名前を入力し、ドロップダウンリストに表示されたらクリックします。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL カスタムForms]</strong></td>
      <td>ストーリーに追加するカスタムフォームを選択します。</td>
     </tr>
    </tbody>
   </table>

1. クリック **[!UICONTROL ストーリーを保存]**.
