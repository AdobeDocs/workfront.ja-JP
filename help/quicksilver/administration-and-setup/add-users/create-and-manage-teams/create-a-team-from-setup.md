---
title: 設定エリアからのチームの作成
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-teams-admin
description: Adobe Workfront 管理者は、設定エリアからチームを作成できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 29a84e52-0bd3-45c2-a8b8-80bfec894196
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 96%

---

# 設定エリアからのチームの作成

Adobe Workfront 管理者は、設定エリアからチームを作成できます。チームについて詳しくは、[チームの概要](../../../people-teams-and-groups/create-and-manage-teams/teams-overview.md)を参照してください。

>[!NOTE]
>
>* グループ管理者は、管理するグループのチームを設定エリアから作成できます。詳しくは、[グループのチームの作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md)を参照してください。
>* プランライセンスを持つユーザーは、ユーザーエリアからチームを作成することもできます。詳しくは、[チームの作成](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md)を参照してください。
>

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

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
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：プラン</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## チームの作成

{{step-1-to-setup}}

1. 「**チーム**」を選択し、次に「**新規チーム**」をクリックします。

1. 表示される「**新規チーム**」ボックスで、次の情報を指定します。

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
      <td> <p>チームをグループに関連付ける場合は、グループの名前を入力し、表示されたら名前を選択します。</p> <p>適切なグループにポインタを合わせ、その横に表示される情報アイコン <img src="assets/info-icon.png"> をクリックすると、適切なグループがチームに関連付けられていることを確認できます。グループの上位のグループの階層や管理者など、グループに関する情報が一覧表示されるツールチップが表示されます。</p> <p><b>メモ</b>：チームがグループまたはサブグループに割り当てられると、そのグループまたはサブグループのグループ管理者は、チームのメンバーにならずにチームを管理することができます。グループ管理者は、メインメニューからチーム領域に移動し、チームを切り替え矢印 <img src="assets/switch-team-icon.png" alt="チームを切り替えアイコン"> をクリックすると、管理するグループに割り当てられているすべてのチームのリストを表示できます。</p> </td> 
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
     <tr data-mc-conditions="SnippetConditions-wf-groups.system-level"> 
      <td role="rowheader">これはアジャイルチームです</td> 
      <td>この新しいチームをアジャイルチームに設定する場合は、この項目を選択します。アジャイルチームについて詳しくは、<a href="../../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md" class="MCXref xref">アジャイルチームの作成</a>を参照してください。</td> 
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

1. 「**チームの作成**」をクリックします。

## チーム所有者

チームを作成すると、デフォルトでチームの所有者になります。

チームのレポートを作成し、レポートに「所有者名」フィールドを含めると、すべてのチームのチーム所有者を表示できます。（レポートの作成について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。）
