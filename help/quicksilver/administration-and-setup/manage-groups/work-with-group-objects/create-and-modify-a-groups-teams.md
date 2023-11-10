---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: グループのチームの作成と変更
description: '[ グループ ] 領域で管理するグループを表示している場合、グループとそのサブグループに関連付けられたチームを表示し、操作できます。'
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 51967cd7-962e-4354-a04b-6df4e31e70c6
source-git-commit: 6f9eddd46430990e11d5d661ea09f0595a9acebc
workflow-type: tm+mt
source-wordcount: '1014'
ht-degree: 3%

---

# グループのチームの作成と変更

[ グループ ] 領域で管理するグループを表示している場合、グループとそのサブグループに関連付けられたチームを表示し、操作できます。

グループの上にグループがある場合は、その管理者がグループに対してこれらの操作を実行することもできます。 Workfront管理者（すべてのグループ）も同様です。

プランライセンスを持つユーザーがチームを作成する方法については、 [チームの作成](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).

Workfront管理者によるチームの作成方法について詳しくは、 [[ 設定 ] 領域からチームを作成する](../../../administration-and-setup/add-users/create-and-manage-teams/create-a-team-from-setup.md).

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> <p>グループのグループ管理者またはWorkfront管理者である必要があります。 詳しくは、 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref" data-mc-variable-override="">グループ管理者</a> および <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref" data-mc-variable-override="">ユーザーに完全な管理アクセス権を付与する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランまたはライセンスの種類を確認する必要がある場合は、Workfront管理者にお問い合わせください。

## 「グループ」領域で、グループのチームを表示、操作、作成します。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **グループ** ![](assets/groups-icon.png).

1. チームを作成または変更するグループの名前をクリックします。
1. 左側のパネルで、 **チーム** ![](assets/teams.png) グループに関連するチームと、そのグループに含まれるサブグループを一覧表示します。

1. 次のいずれかの操作を行います。

   * **チームを追加**：クリック **新規チーム**&#x200B;を設定するには、次のオプションを使用します。

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
       <td> <p> 新しいチームの「グループ」フィールドが、表示しているグループで入力されます。 チームを別のグループに関連付ける場合は、グループの名前を入力し、表示されたら名前を選択します。</p> <p>適切なグループにカーソルを合わせ、情報アイコンをクリックすると、適切なグループがチームに関連付けられていることを確認できます。 <img src="assets/info-icon.png"> その横に表示されます。 グループの上位のグループの階層や管理者など、グループに関する情報が一覧表示されるツールチップが表示されます。</p> <p><b>注意</b>：チームがグループまたはサブグループに割り当てられると、そのグループまたはサブグループのグループ管理者は、チームのメンバーにならずにチームを管理できます。 グループ管理者は、メインメニューから「チーム」領域に移動し、「チームを切り替え」矢印をクリックします。 <img src="assets/switch-team-icon.png" alt="チームを切り替えアイコン"> ：管理するグループに割り当てられているすべてのチームのリストを表示します。</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">チームメンバー</td> 
       <td> <p>チームに参加するユーザーの名前を入力し始め、ドロップダウンリストにが表示されたら、名前を選択します。 複数のユーザーをチームに追加するには、この手順を繰り返します。</p> <p>チームに追加できるユーザー数に制限はありません。 ただし、1 つのチームの作業管理が複雑すぎる可能性があるので、1 つのチームに過度に多くのユーザーを含めないようにすることをお勧めします。</p> </td> 
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
       <td>「作業」ボタンを「開始」ボタンに変更します。 ユーザーが「開始」をクリックすると、項目のステータスが自動的に更新されます。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">「完了」ボタン</td> 
       <td>[ 完了 ] ボタンをクリックしたときにアイテムに設定するステータスを選択します。</td> 
       </tr> 
      </tbody> 
     </table>

   * **チームの編集**：少なくとも 1 つのチームを選択し、「 **の** 編集アイコン ![](assets/edit-icon.png)を設定するには、次のオプションを使用します。

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
       <td> <p>チームをグループに関連付けます。 グループの名前を入力し、表示されたら名前を選択します。</p> <p>適切なグループにカーソルを合わせ、情報アイコンをクリックすると、適切なグループがチームに関連付けられていることを確認できます。 <img src="assets/info-icon.png"> その横に表示されます。 グループの上位のグループの階層や管理者など、グループに関する情報が一覧表示されるツールチップが表示されます。</p> <p><b>注意</b>：チームがグループまたはサブグループに割り当てられると、そのグループまたはサブグループのグループ管理者は、チームのメンバーにならずにチームを管理できます。 グループ管理者は、メインメニューから「チーム」領域に移動し、「チームを切り替え」矢印をクリックします。 <img src="assets/switch-team-icon.png" alt="チームを切り替えアイコン"> ：管理するグループに割り当てられているすべてのチームのリストを表示します。</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">所有者</td> 
       <td>チームの所有者を選択します。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">チームメンバー</td> 
       <td> <p>とチームメンバーを追加します。 ユーザーの名前の入力を開始し、表示されたら名前を選択します。 複数のユーザーをチームに追加するには、この手順を繰り返します。</p> <p><b>ヒント</b>：チームに追加できるユーザー数に制限はありません。 ただし、1 つのチームの作業管理が複雑すぎる可能性があるので、1 つのチームに過度に多くのユーザーを含めないようにすることをお勧めします。</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">説明</td> 
       <td>チームの説明を入力します。</td> 
       </tr> 
       <tr> 
       <td role="rowheader">レイアウトテンプレート</td> 
       <td> <p>チームが使用するレイアウトテンプレートの名前を入力し、表示されたらクリックします。</p> <p>このレイアウトテンプレートを持つチームをホームユーザーチームとして指定すると、このチームのすべてのユーザーは、このレイアウトテンプレートのカスタマイズを表示します。<br>個々のレイアウトテンプレートの設定は、ホームチームのレイアウトテンプレートの設定に優先します。 </p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">アジャイル</td> 
       <td>これがアジャイルチームかどうかを指定します。 アジャイルチームとその作業の管理方法について詳しくは、 <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">アジャイルチームの作成</a>.</td> 
       </tr> 
       <tr> 
       <td role="rowheader">作業</td> 
       <td> <p>「作業」ボタンを「開始」ボタンに変更します。 ユーザーが「開始」をクリックすると、項目のステータスが自動的に更新されます。</p> <p>「開始」ボタンの設定方法について詳しくは、「 <a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">「作業対象」ボタンを「開始」ボタンに置き換えます</a>.</p> </td> 
       </tr> 
       <tr> 
       <td role="rowheader">「完了」ボタン</td> 
       <td> <p>「完了」ボタンをカスタマイズします。 詳しくは、以下を参照してください。</p> 
       <ul> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md" class="MCXref xref">タスクの「完了」ボタンの設定</a> </li> 
       <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md" class="MCXref xref">問題が発生しないように「完了」ボタンを設定します</a> </li> 
       </ul> </td> 
       </tr> 
      </tbody> 
     </table>

   * **チームを削除**：少なくとも 1 つのチームを選択して、削除アイコンをクリックします。 ![](assets/delete.png).
   * **チームのリストをエクスポート**：クリック **書き出し** ![](assets/export.png)次に、書き出すリストのファイル形式を選択します。
