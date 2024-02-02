---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: アジャイルストーリーを作成する
description: 様々な方法を使って、1 つの反復で 1 つのアジャイルストーリーを作成できます。アジャイルストーリーを作成したら、ストーリーにサブタスクを追加できます。
author: Lisa
feature: Agile
exl-id: d16ee940-3551-44da-8fe6-093f4fcac070
source-git-commit: 11009f24cd482e83319ed9f1ecf3f7a2f4e79d52
workflow-type: ht
source-wordcount: '756'
ht-degree: 100%

---

# アジャイルストーリーを作成する

様々な方法を使って、1 つの反復で 1 つのアジャイルストーリーを作成できます。アジャイルストーリーを作成したら、ストーリーにサブタスクを追加できます。

ストーリーまたはサブタスクを反復に追加すると、期間タイプが「[!UICONTROL シンプル]」に設定されます。また、タスクの制約が「固定日付」に設定され、日付は反復内でロックされます。反復期間のタイプやタスクの制約は変更できません。また、タスクの期間は 0 分を超える値にする必要があります。

反復に追加された後のストーリーの管理方法について詳しくは、[反復](../../agile/use-scrum-in-an-agile-team/iterations/iterations.md)を参照してください。

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
   <td> <p>[!UICONTROL Worker] 以上</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか [!DNL Workfront] 管理者にお問い合わせください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>ストーリーが存在するプロジェクトへの[!UICONTROL Manage]アクセス権</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## イテレーションでのアジャイルストーリーの作成

1. ストーリーを作成するアジャイルなイテレーションに移動します。

   1. [!DNL Adobe Workfront] の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png)、「**[!UICONTROL ボード]**」の順にクリックします。

   1. （オプション）**[!UICONTROL チームの切り替え]**&#x200B;アイコン ![チームの切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索します。

   1. 左のパネルで、「**[!UICONTROL 反復]**」を選択して特定の反復を選択するか、または「**[!UICONTROL 進行中の反復]**」を選択します。
   1. ストーリーを作成する特定のイテレーションの名前をクリックします。

   ![反復への新しいストーリーの追加](assets/iteration-add-story.png)

1. 「**[!UICONTROL 新規ストーリー]」をクリックします。**
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
      <td>ストーリーをイテレーションに追加する準備が整ったら、このオプションを選択します。 このオプションを選択すると、バックログ内のイテレーションに追加する準備ができているストーリーをユーザーに示します。<br>ストーリーは、<strong>[!UICONTROL Ready] とマークされているかどうかに関わらず、反復に追加できます。</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimate]（ポイント）</strong></td>
      <td>ストーリーの見積りを指定します。 アジャイルチームがストーリーをポイント単位で推定するように設定されている場合、デフォルトでは1ポイントが8時間になります。見積もりは、ストーリーに[!UICONTROL Planned Hours]として追加されます。<br>例えば、ストーリーを 3 ポイントと見積もる場合、デフォルトの動作では、24 [!UICONTROL Planned Hours] がストーリーに追加されます。<br>ストーリーにサブタスクが含まれる場合は、すべてのサブタスクの合計見積もりで親ストーリーの見積もりが決まることに注意してください。詳しくは、<a href="../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md" class="MCXref xref">既存の反復へのストーリーの追加</a>を参照してください。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Project]</strong></td>
      <td>このストーリーを関連付けるプロジェクトの名前を入力します。<br>デフォルトでは、ストーリーの色は、このプロジェクトの他のストーリーと同じ色で表示されます。<br>プロジェクトのステータスは [!UICONTROL Current] に設定する必要があります。プロジェクトのステータスが [!UICONTROL Current] 以外の場合は、ドロップダウンメニューには表示されません。</td>
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

## バックログにアジャイルストーリーを作成

[アジャイルバックログの管理](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)の記事の、[バックログに新規ストーリーを作成](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#creating-new-stories)節で説明されているように、アジャイルバックログからアジャイルストーリーを作成できます。

## タスクまたはイシューをアジャイルストーリーとして追加

既存のタスクやイシューをストーリーとしてイテレーションに追加できます。詳しくは、[既存のイテレーションへのストーリーの追加](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md)または[[!UICONTROL スクラム]ボードからのストーリーとイシューの追加](../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md)を参照してください。

## アジャイルストーリーにサブタスクを作成

次のどちらかの方法を使用して、アジャイルストーリーにサブタスクを作成できます。

* 「**[!UICONTROL サブタスク]**」タブを使用する（[サブタスクの作成](../../manage-work/tasks/create-tasks/create-subtasks.md)の[サブタスクを作成](../../manage-work/tasks/create-tasks/create-subtasks.md#creating-subtasks)で説明）

* ストーリーボードから直接（[イテレーションの作成](../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md)で説明）
