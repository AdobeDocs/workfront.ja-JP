---
title: '[ 設定 ] 領域からチームを作成する'
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-teams-admin
description: Adobe Workfront管理者は、「設定」領域からチームを作成できます。
author: Caroline, Courtney
feature: System Setup and Administration
role: Admin
exl-id: 29a84e52-0bd3-45c2-a8b8-80bfec894196
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '567'
ht-degree: 4%

---

# [ 設定 ] 領域からチームを作成する

Adobe Workfront管理者は、「設定」領域からチームを作成できます。 チームについて詳しくは、 [チームの概要](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md).

>[!NOTE]
>
>* グループ管理者は、管理するグループのチームを「設定」領域から作成できます。 詳しくは、 [グループのチームの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).
>* プランライセンスを持つユーザーは、「人」領域からチームを作成することもできます。 詳しくは、 [チームの作成](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
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

## チームの作成

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **チーム**&#x200B;を選択し、「 **新規チーム**.

1. 内 **新規チーム** 表示されるボックスで、次の情報を指定します。

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
      <td> <p>チームをグループに関連付ける場合は、グループの名前を入力し、表示されたら名前を選択します。</p> <p>適切なグループにカーソルを合わせ、情報アイコンをクリックすると、適切なグループがチームに関連付けられていることを確認できます <img src="assets/info-icon.png"> その横に表示されます。 グループの上位のグループの階層や管理者など、グループに関する情報が一覧表示されるツールチップが表示されます。</p> <p><b>注意</b>:チームがグループまたはサブグループに割り当てられると、そのグループまたはサブグループのグループ管理者は、チームのメンバーにならずにチームを管理できます。 グループ管理者は、メインメニューから「チーム」領域に移動し、「チームを切り替え」矢印をクリックします。 <img src="assets/switch-team-icon.png" alt="チームを切り替えアイコン"> ：管理するグループに割り当てられているすべてのチームをリストします。</p> </td> 
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
     <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
      <td role="rowheader">これはアジャイル チームです</td> 
      <td>この新しいチームをアジャイルチームに設定する場合は、この項目を選択します。 アジャイルチームについて詳しくは、 <a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">アジャイルチームの作成</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">作業する</td> 
      <td>「作業」ボタンを「開始」ボタンに変更します。 ユーザーが「開始」をクリックすると、項目のステータスが自動的に更新されます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">「完了」ボタン</td> 
      <td>[ 完了 ] ボタンをクリックしたときにアイテムに設定するステータスを選択します。</td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **チームを作成**.

## チーム所有者

チームを作成すると、デフォルトでチームの所有者になります。

チームのレポートを作成し、レポートに所有者名フィールドを含めると、すべてのチームのチーム所有者を表示できます。 ( レポートの作成について詳しくは、 [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).)
