---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: イテレーションでのアジャイルストーリーの作成
description: この記事では、既にイテレーションを行っている場合に、新しいアジャイルストーリーを作成する方法について説明します。
author: Lisa
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
source-git-commit: 094a9d453476418cbe1b065930eb3a179e4cf73a
workflow-type: ht
source-wordcount: '572'
ht-degree: 100%

---

# イテレーションでのアジャイルストーリーの作成

この記事では、既にイテレーションを行っている場合に、新しいアジャイルストーリーを作成する方法について説明します。[!DNL Adobe Workfront] のタスク、イシュー、その他の領域からのアジャイルストーリーついて詳しくは、[既存のイテレーションにストーリーを追加](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md)を参照してください。 

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] プラン*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Work] 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>[!UICONTROL Worker] 以上</p> <p>メモ：アクセス権がない場合は、アクセスレベルに追加の制限が設定されているかどうかを [!DNL Workfront] 管理者に確認してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>ストーリーが存在するプロジェクトへの[!UICONTROL Manage]アクセス権</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## イテレーションでのアジャイルストーリーの作成

1. ストーリーを作成するアジャイルなイテレーションに移動します。

   1. [!DNL Adobe] Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、「**[!UICONTROL チーム]**」をクリックします。

   1. （オプション）「**[!UICONTROL チームの切り替え]**」アイコン「![チームを切り替え」アイコン](assets/switch-team-icon.png)をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索します。

   1. 左側のパネルで、「**[!UICONTROL イテレーション]**」を選択します。
   1. ストーリーを作成する特定のイテレーションの名前をクリックします。
   1. 左側のパネルで、「**[!UICONTROL ストーリー]**」を選択します。

1. 「**[!UICONTROL 新しいストーリー]」をクリックします。**
1. 次の情報を指定します。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Story Name]</strong></td>
      <td>ストーリーの名前を入力します。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td>
      <td>ストーリーの説明を入力します。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Ready]</strong></td>
      <td>ストーリーをイテレーションに追加する準備が整ったら、このオプションを選択します。 このオプションを選択すると、バックログ内のイテレーションに追加する準備ができているストーリーをユーザーに示します。<br>ストーリーは、<strong>[!UICONTROL Ready] とマークされているかどうかに関わらず、イテレーションに追加できます。</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimate]（ポイント）</strong></td>
      <td>ストーリーの見積りを指定します。 アジャイルチームがストーリーをポイント単位で推定するように設定されている場合、デフォルトでは1ポイントが8時間になります。見積もりは、ストーリーに[!UICONTROL Planned Hours]として追加されます。<br>例えば、ストーリーを 3 ポイントと見積もる場合、デフォルトの動作では、24 予定時間数がストーリーに追加されます。<br>ストーリーにサブタスクが含まれる場合は、すべてのサブタスクの合計見積もりで親ストーリーの見積もりが決まることに注意してください。詳しくは、<a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/add-a-subtask-to-an-existing-story-scrum.md" class="MCXref xref">[!UICONTROL Scrum] ボード上の既存のストーリーにサブタスクを追加</a>を参照してください。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Project]</strong></td>
      <td>このストーリーを関連付けるプロジェクトの名前を入力します。<br>デフォルトでは、ストーリーの色は、このプロジェクトの他のストーリーと同じ色で表示されます。<br>プロジェクトのステータスは [!UICONTROL Current] に設定する必要があります。 プロジェクトのステータスが [!UICONTROL Current] 以外の場合は、ドロップダウンメニューには表示されません。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Task]</strong></td>
      <td>親プロジェクトを選択した後で、親タスクを選択することもできます。 親タスクを選択すると、選択したプロジェクトの親タスクのサブタスクとしてストーリーが作成されます。<br>ストーリーの親タスクの名前を入力し、ドロップダウンリストに表示されたらクリックします。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td>ストーリーに追加するカスタムフォームを選択します。</td>
     </tr>
    </tbody>
   </table>

1. 「**[!UICONTROL ストーリーを保存]**」をクリックします。
