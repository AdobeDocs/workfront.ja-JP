---
product-area: agile-and-teams;projects
navigation-topic: iterations
title: 反復でのアジャイルストーリーの作成
description: この記事では、既にイテレーションに参加している場合に新しいアジャイルストーリーを作成する方法について説明します。
author: Jenny
feature: Agile
exl-id: 9712e065-5fbf-4deb-a39f-36e0e918ed12
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 80%

---

# 反復でのアジャイルストーリーの作成

この記事では、既にイテレーションに参加している場合に新しいアジャイルストーリーを作成する方法について説明します。 タスク、イシュー、その他の [!DNL Adobe Workfront] ークフロー領域からアジャイルストーリーを作成する方法については、[&#x200B; 既存の反復にストーリーを追加 &#x200B;](../../../agile/use-scrum-in-an-agile-team/iterations/add-stories-to-existing-iteration.md) を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
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
   <td>ストーリーが含まれるプロジェクトへのアクセスの管理 </td> 
  </tr>
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 反復でのアジャイルストーリーの作成

1. ストーリーを作成するアジャイル イテレーションに移動します。

   {{step1-to-team}}

   1. （オプション）**[!UICONTROL チームの切り替え]**&#x200B;アイコン ![チームを切り替えアイコン](assets/switch-team-icon.png) をクリックし、ドロップダウンメニューから新しいスクラムチームを選択するか、検索バーでチームを検索します。

   1. 左側のパネルで、「**[!UICONTROL イテレーション]**」を選択します。
   1. ストーリーを作成する特定のイテレーションの名前をクリックします。
   1. 左側のパネルで、「**[!UICONTROL ストーリー]**」を選択します。

1.  **[!UICONTROL 新規ストーリー]** をクリックします。
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
