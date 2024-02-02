---
title: 設定領域におけるチームの設定の編集
description: Adobe Workfront の管理者は、設定領域からチームの設定を編集できます。チームにユーザーを追加し、チームのレイアウトテンプレートを設定して、チームが作業項目を完了したときのステータスの記録方法を設定できます。
author: Caroline, Courtney
feature: System Setup and Administration
role: Admin
exl-id: 648a36ce-5793-472f-9fee-9dedf71991ef
source-git-commit: 7fa4791e19a84d7215e341e8bbde8dd4d4d8ccc6
workflow-type: ht
source-wordcount: '621'
ht-degree: 100%

---

# 設定領域におけるチームの設定の編集

Adobe Workfront の管理者は、設定領域からチームの設定を編集できます。チームにユーザーを追加し、チームのレイアウトテンプレートを設定して、チームが作業項目を完了したときのステータスの記録方法を設定できます。

チームについて詳しくは、[チームの概要](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md)を参照してください。

>[!NOTE]
>
>* グループ管理者は、管理するグループのチームの設定を編集できます。詳しくは、[グループのチームの作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md)を参照してください。
>* プランライセンスを持つユーザーは、ユーザー領域からチームの設定を編集できます。詳しくは、[チーム設定の編集](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md)を参照してください。
>

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## チームの設定を編集

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、**設定** ![](assets/gear-icon-settings.png) の順にクリックします。

1. 左側のパネルで「**チーム**」をクリックします。
1. チームを選択し、「**編集**」![](assets/edit-icon.png)をクリックします。

1. 次のいずれかの変更を加えます。

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
       <td>このオプションは、新規チームと既存チームに対して、デフォルトで有効になっています。無効にしてチームを非アクティブ化します。詳しくは、<a href="../../../people-teams-and-groups/create-and-manage-teams/deactivate-a-team.md" class="MCXref xref">チームの非アクティブ化</a>を参照してください。 </td> 
      </tr>
     <tr> 
      <td role="rowheader">グループ</td> 
      <td> <p>チームをグループに関連付けます。グループ名を入力し、表示されたら名前を選択します。</p> <p><b>メモ</b>：チームがグループまたはサブグループに割り当てられると、そのグループまたはサブグループのグループ管理者は、チームのメンバーにならずにチームを管理することができます。グループ管理者は、メインメニューからチーム領域に移動し、チームを切り替え矢印 <img src="assets/switch-team-icon.png" alt="チームを切り替えアイコン"> をクリックすると、管理するグループに割り当てられているすべてのチームのリストを表示できます。</p> <p>グループにポインタを合わせ、その横に表示される情報アイコン <img src="assets/info-icon.png"> をクリックすると、適切なグループがチームに関連付けられていることを確認できます。グループの上位のグループの階層や管理者など、グループに関する情報が一覧表示されるツールチップが表示されます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">所有者</td> 
      <td>チームの所有者を選択します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">チームメンバー</td> 
      <td> <p>チームメンバーを追加します。ユーザー名を入力し、表示されたら名前を選択します。複数のユーザーをチームに追加するには、このプロセスを繰り返します。</p> 
      <p><b>ヒント</b>：チームには、任意の人数のユーザーを追加できます。ただし、チームの作業管理が複雑になりすぎる可能性があるため、1 つのチームに過剰な人数を追加しないことをお勧めします。</p> </td> 
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
      <td>これがアジャイルチームかどうかを指定します。アジャイルチームとその作業の管理方法について詳しくは、<a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">アジャイルチームの作成</a>を参照してください。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">作業</td> 
      <td> <p>「作業」ボタンを「開始」ボタンに変更します。ユーザーが「開始」をクリックすると、項目のステータスが自動的に更新されます。</p> <p>「開始」ボタンの設定方法について詳しくは、<a href="../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md" class="MCXref xref">「作業」ボタンと「開始」ボタンの置き換え</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">「完了」ボタン</td> 
      <td> <p>「完了」ボタンをカスタマイズします。詳しくは、以下を参照してください。</p> 
       <ul> 
        <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md" class="MCXref xref">タスクの「完了」ボタンの設定</a> </li> 
        <li><a href="../../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md" class="MCXref xref">イシューの「完了」ボタンの設定</a> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**変更を保存**」をクリックします。
