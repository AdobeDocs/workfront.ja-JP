---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: グループのチームの作成および変更
description: 管理するグループをグループエリアに表示している場合、グループとそのサブグループに関連付けられたチームを表示して操作できます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51967cd7-962e-4354-a04b-6df4e31e70c6
source-git-commit: 6f9eddd46430990e11d5d661ea09f0595a9acebc
workflow-type: tm+mt
source-wordcount: '1014'
ht-degree: 98%

---

# グループのチームの作成および変更

管理するグループをグループエリアに表示している場合、グループとそのサブグループに関連付けられたチームを表示して操作できます。

グループの上にグループがある場合は、その管理者がグループに対してこれらの操作を実行することもできます。Workfront 管理者（すべてのグループ）も同様です。

Plan ライセンスのあるユーザーがチームを作成する方法について詳しくは、[チームの作成](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md)を参照してください。

Workfront 管理者がチームを作成する方法について詳しくは、[設定エリアからのチームの作成](../../../administration-and-setup/add-users/create-and-manage-teams/create-a-team-from-setup.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront プラン*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> <p>グループのグループ管理者または Workfront 管理者である必要があります。詳しくは、<a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">グループ管理者</a>および<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類を確認するには、Workfront 管理者にお問い合わせください。

## グループエリアでのグループのチームの表示、操作、作成

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)をクリックし、「**設定**」![](assets/gear-icon-settings.png) をクリックします。

1. 左パネルで、**グループ** ![](assets/groups-icon.png) をクリックします。

1. チームを作成または変更するグループの名前をクリックします。
1. 左パネルで&#x200B;**チーム** ![](assets/teams.png) をクリックして、グループおよびそのサブグループに関連付けられているチームを一覧表示します。

1. 次のいずれかの操作を行います。

   * **チームを追加**：**新しいチーム**&#x200B;をクリックし、次のオプションを使用して設定します。

   <!-- WRITER please check table below. I stripped out wonky conditions-->

   <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
       <td role="rowheader">チーム名</td> 
       <td>チームの名前を入力します。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">グループ</td> 
       <td> <p> 新しいチームの「グループ」フィールドが、表示しているグループで入力されます。 チームを別のグループに関連付ける場合は、グループの名前を入力し始め、表示されたら名前を選択します。</p> <p>チームに適切なグループが関連付けられていることを確認するには、そのグループにポインタを合わせ、その横に表示される情報アイコン <img src="assets/info-icon.png"> をクリックします。グループの上位のグループの階層や管理者など、グループに関する情報が一覧表示されるツールチップが表示されます。</p> <p><b>メモ</b>：チームがグループまたはサブグループに割り当てられると、そのグループまたはサブグループのグループ管理者は、チームのメンバーにならずにチームを管理することができます。グループ管理者は、メインメニューからチーム領域に移動し、チームを切り替え矢印 <img src="assets/switch-team-icon.png" alt="チームを切り替えアイコン"> をクリックすると、管理するグループに割り当てられているすべてのチームのリストを表示できます。</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">チームメンバー</td> 
       <td> <p>チームに参加するユーザーの名前の入力を開始し、ドロップダウンリストに表示されたら、名前を選択します。複数のユーザーをチームに追加するには、このプロセスを繰り返します。</p> <p>チームに追加できるユーザー数に制限はありません。ただし、1 つのチームの作業管理が複雑すぎる可能性があるので、1 つのチームに過度に多くのユーザーを含めないようにすることをお勧めします。</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">説明</td> 
       <td>チームの説明を入力します。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">カレンダー</td> 
       <td>このチームに表示するカレンダータブの選択</td> 
       </tr> 
       <tr> 
       <td role="rowheader">作業</td> 
       <td>「作業」ボタンを「開始」ボタンに変更します。ユーザーが「開始」をクリックすると、項目のステータスが自動的に更新されます。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">「完了」ボタン</td> 
       <td>「完了」ボタンをクリックしたときに項目に設定するステータスを選択します。</td> 
       </tr> 
      </tbody> 
     </table>

   * **チームを編集**：少なくとも 1 つのチームを選択して&#x200B;**編集**&#x200B;アイコン ![](assets/edit-icon.png) をクリックし、次のオプションを使用して設定します。

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
       <td role="rowheader">チーム名</td> 
       <td>チームの名前を入力します。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">グループ</td> 
       <td> <p>チームをグループに関連付けます。グループ名を入力し、表示されたら名前を選択します。</p> <p>適切なグループをチームに関連付けていることを確認するには、そのグループにポインタを合わせ、その横に表示される情報アイコン <img src="assets/info-icon.png"> をクリックします。グループの上位のグループの階層や管理者など、グループに関する情報が一覧表示されるツールチップが表示されます。</p> <p><b>メモ</b>：チームがグループまたはサブグループに割り当てられると、そのグループまたはサブグループのグループ管理者は、チームのメンバーにならずにチームを管理することができます。グループ管理者は、メインメニューからチームエリアに移動し、チームを切り替え矢印 <img src="assets/switch-team-icon.png" alt="チームを切り替えアイコン"> をクリックして、管理するグループに割り当てられているすべてのチームのリストを表示します。</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">所有者</td> 
       <td>チームの所有者を選択します。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">チームメンバー</td> 
       <td> <p>チームメンバーを追加します。ユーザー名を入力し、表示されたら名前を選択します。複数のユーザーをチームに追加するには、このプロセスを繰り返します。</p> <p><b>ヒント</b>：チームに追加できるユーザー数に制限はありません。ただし、1 つのチームの作業管理が複雑すぎる可能性があるので、1 つのチームに過度に多くのユーザーを含めないようにすることをお勧めします。</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">説明</td> 
       <td>チームの説明を入力します。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">レイアウトテンプレート</td> 
       <td> <p>チームが使用するレイアウトテンプレートの名前を入力し、表示されたらクリックします。</p> <p>このレイアウトテンプレートを使用するチームをユーザーのホームチームとして指定すると、チームのすべてのユーザーにこのレイアウトテンプレートのカスタマイズが表示されます。<br>個々のレイアウトテンプレートの設定は、ホームチームのレイアウトテンプレートの設定よりも優先されます。 </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">アジャイル</td> 
       <td>これがアジャイルチームかどうかを指定します。アジャイルチームとその作業の管理方法について詳しくは、<a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">アジャイルチームの作成</a>を参照してください。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">作業</td> 
       <td> <p>「作業」ボタンを「開始」ボタンに変更します。ユーザーが「開始」をクリックすると、項目のステータスが自動的に更新されます。</p> <p>「開始」ボタンの設定方法について詳しくは、<a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">「作業」ボタンと「開始」ボタンの置き換え</a>を参照してください。</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">「完了」ボタン</td> 
       <td> <p>「完了」ボタンをカスタマイズします。詳しくは、以下を参照してください。</p> 
       <ul> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md" class="MCXref xref">タスクの「完了」ボタンの設定</a> </li> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md" class="MCXref xref">イシューへの「完了」ボタンの設定</a> </li> 
       </ul> </td> 
       </tr> 
      </tbody> 
     </table>

   * **チームを削除**：少なくとも 1 つのチームを選択して、削除アイコン ![](assets/delete.png) をクリックします。
   * **チームのリストを書き出し**：**書き出し** ![](assets/export.png) をクリックし、書き出すリストのファイル形式を選択します。
