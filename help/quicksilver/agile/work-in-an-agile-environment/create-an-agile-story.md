---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: アジャイルストーリーの構築
description: イテレーションでは、さまざまな方法でアジャイルストーリーを作成できます。 アジャイルストーリーを作成したら、ストーリーにサブタスクを追加できます。
author: Courtney
feature: Agile
exl-id: d16ee940-3551-44da-8fe6-093f4fcac070
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/eIcQnZTyB60Uox-XSXGxoy-PmbsVvqkTJnX4wNofuuY
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 689
ht-degree: 65%

---

# アジャイルストーリーの作成

イテレーションでは、さまざまな方法でアジャイルストーリーを作成できます。 アジャイルストーリーを作成したら、ストーリーにサブタスクを追加できます。

ストーリーまたはサブタスクを反復に追加すると、期間タイプが「[!UICONTROL シンプル]」に設定されます。また、タスクの制約が「固定日付」に設定され、日付は反復内でロックされます。 反復期間のタイプやタスクの制約は変更できません。 また、タスクの期間は 0 分を超える値にする必要があります。

反復に追加された後のストーリーの管理方法について詳しくは、[反復](../../agile/use-scrum-in-an-agile-team/iterations/iterations.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p> 
   <p>Work またはそれ以上</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td>ストーリーが進行しているプロジェクトへのアクセスを管理 </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## イテレーションでのアジャイルストーリーの作成

1. ストーリーを作成するアジャイルイテレーションに移動します。

   {{step1-to-team}}

   1. （オプション）**[!UICONTROL チームを切り替え]**&#x200B;アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索します。

   1. 左パネルで、「**[!UICONTROL 反復]**」を選択して特定の反復を選ぶか、「**[!UICONTROL 進行中の反復]**」を選択します。
   1. ストーリーを作成する特定のイテレーションの名前をクリックします。

   ![反復への新しいストーリーの追加](assets/iteration-stories-list.png)

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
      <td>ストーリーをイテレーションに追加する準備が整ったら、このオプションを選択します。 このオプションを選択すると、バックログ内のどのストーリーをイテレーションに追加する準備ができているかをユーザーに示します。<br> ストーリーは、<strong>[!UICONTROL Ready]とマークされているかどうかに関係なく、イテレーションに追加できます。</strong></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimate]（ポイント）</strong></td>
      <td>ストーリーの見積りを指定します。 アジャイルチームがストーリーをポイントで見積もるように設定されている場合、デフォルトでは1 ポイントは8時間に相当します。 見積もりは、ストーリーに[!UICONTROL Planned Hours]として追加されます。<br>例えば、ストーリーを 3 ポイントと見積もる場合、デフォルトの動作では、24 [!UICONTROL Planned Hours] がストーリーに追加されます。<br>ストーリーにサブタスクが含まれる場合は、すべてのサブタスクの合計見積もりで親ストーリーの見積もりが決まることに注意してください。 詳しくは、<a href="../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md" class="MCXref xref">既存の反復へのストーリーの追加</a>を参照してください。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Project]</strong></td>
      <td>このストーリーを関連付けるプロジェクトの名前を入力します。<br>デフォルトでは、ストーリーの色は、このプロジェクトの他のストーリーと同じ色で表示されます。<br>プロジェクトのステータスは [!UICONTROL Current] に設定する必要があります。 プロジェクトのステータスが [!UICONTROL Current] 以外の場合は、ドロップダウンメニューには表示されません。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Parent Task]</strong></td>
      <td>親プロジェクトを選択した後で、親タスクを選択することもできます。 親タスクを選択すると、選択したプロジェクトの親タスクのサブタスクとしてストーリーが作成されます。<br> ストーリーの親タスクの名前を入力し始め、ドロップダウンリストに表示されたらクリックします。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom Forms]</strong></td>
      <td>ストーリーに追加するカスタムフォームを選択します。</td>
     </tr>
    </tbody>
   </table>

1. 「**[!UICONTROL ストーリーを保存]**」をクリックします。

## バックログでのアジャイルストーリーの構築

アジャイルバックログからアジャイルストーリーを作成できます。詳しくは、[[!UICONTROL &#x200B; アジャイルバックログの管理]記事](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md)の「[&#x200B; バックログに新しいストーリーを作成](../../agile/work-in-an-agile-environment/manage-the-agile-backlog.md#creating-new-stories)」を参照してください。

## タスクまたは問題をアジャイルストーリーとして追加

既存のタスクやイシューをストーリーとしてイテレーションに追加できます。 詳しくは、[既存のイテレーションへのストーリーの追加](../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md)または[[!UICONTROL スクラム]ボードからのストーリーとイシューの追加](../../agile/use-scrum-in-an-agile-team/scrum-board/add-story-from-scrum-board.md)を参照してください。

## アジャイルストーリーへのサブタスクの作成

次のいずれかの方法を使用して、アジャイルストーリーのサブタスクを作成できます。

* 「**[!UICONTROL サブタスク]**」タブを使用する（[サブタスクの作成](../../manage-work/tasks/create-tasks/create-subtasks.md)の[サブタスクを作成](../../manage-work/tasks/create-tasks/create-subtasks.md#creating-subtasks)で説明）

* ストーリーボードから直接（[イテレーションの作成](../../agile/use-scrum-in-an-agile-team/iterations/create-an-iteration.md)で説明）
