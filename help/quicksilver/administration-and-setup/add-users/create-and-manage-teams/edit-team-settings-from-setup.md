---
title: '[ 設定 ] 領域でチームの設定を編集する'
description: Adobe Workfrontの管理者は、「設定」領域でチームの設定を編集できます。 チームにユーザーを追加し、チームのレイアウトテンプレートを設定し、チームが作業項目を完了したときのステータスの記録方法を設定できます。
author: Caroline, Courtney
feature: System Setup and Administration
role: Admin
exl-id: 648a36ce-5793-472f-9fee-9dedf71991ef
source-git-commit: 7fa4791e19a84d7215e341e8bbde8dd4d4d8ccc6
workflow-type: tm+mt
source-wordcount: '621'
ht-degree: 3%

---

# [ 設定 ] 領域でチームの設定を編集する

Adobe Workfrontの管理者は、「設定」領域でチームの設定を編集できます。 チームにユーザーを追加し、チームのレイアウトテンプレートを設定し、チームが作業項目を完了したときのステータスの記録方法を設定できます。

チームについて詳しくは、 [チームの概要](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* グループ管理者は、管理するグループのチーム設定を編集できます。 詳しくは、 [グループのチームの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* プランライセンスを持つユーザーは、「担当者」領域でチームの設定を編集できます。 詳しくは、 [チーム設定を編集](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
>


## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront管理者である。</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## チームの設定を編集する

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **チーム** をクリックします。
1. チームを選択し、「 **編集** ![](assets/edit-icon.png).

1. 次の変更を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">チーム名</td> 
      <td>チームの名前を入力します。</td> 
     </tr>
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">アクティブ </td> 
       <td>このオプションは、新規チームと既存チームに対して、デフォルトで有効になっています。 無効にしてチームを非アクティブ化します。 詳しくは、 <a href="../../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md" class="MCXref xref">チームを非アクティブ化</a> </td> 
      </tr>
     <tr> 
      <td role="rowheader">グループ</td> 
      <td> <p>チームをグループに関連付けます。 グループの名前を入力し、表示されたら名前を選択します。</p> <p><b>注意</b>:チームがグループまたはサブグループに割り当てられると、そのグループまたはサブグループのグループ管理者は、チームのメンバーにならずにチームを管理できます。 グループ管理者は、メインメニューから「チーム」領域に移動し、「チームを切り替え」矢印をクリックします。 <img src="assets/switch-team-icon.png" alt="チームを切り替えアイコン"> ：管理するグループに割り当てられているすべてのチームをリストします。</p> <p>適切なグループにカーソルを合わせ、情報アイコンをクリックすると、適切なグループがチームに関連付けられていることを確認できます <img src="assets/info-icon.png"> その横に表示されます。 グループの上位のグループの階層や管理者など、グループに関する情報が一覧表示されるツールチップが表示されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">所有者</td> 
      <td>チームの所有者を選択します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">チームメンバー</td> 
      <td> <p>チームメンバーを追加します。 ユーザーの名前の入力を開始し、表示されたら名前を選択します。 複数のユーザーをチームに追加するには、この手順を繰り返します。</p> 
      <p><b>ヒント</b>:1 つのチームに任意の数のユーザーを追加できます。 ただし、1 つのチームの作業管理が複雑すぎる可能性があるので、1 つのチームに過度に大きな数を追加しないことをお勧めします。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td>チームの説明を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">レイアウトテンプレート</td> 
      <td> <p>チームが使用するレイアウトテンプレートの名前を入力し、表示されたらクリックします。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">アジャイル</td> 
      <td>これがアジャイルチームかどうかを指定します。 アジャイルチームとその作業の管理方法について詳しくは、 <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">アジャイルチームの作成</a>.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">作業する</td> 
      <td> <p>「作業」ボタンを「開始」ボタンに変更します。 ユーザーが「開始」をクリックすると、項目のステータスが自動的に更新されます。</p> <p>「開始」ボタンの設定方法について詳しくは、 <a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">「作業対象」ボタンを「開始」ボタンに置き換えます</a>.</p> </td> 
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

1. クリック **変更を保存**.
