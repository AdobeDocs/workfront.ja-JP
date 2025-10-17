---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: スケジュールの作成
description: スケジュールを使用して、ユーザーの週労働時間を定義できます。ユーザーやプロジェクトに、スケジュールを関連付けることができます。これにより、 [!DNL Workfront]  がタイムラインとユーザーの空き時間を計算します。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f7347ba6-68bf-45d8-b5d2-6136f3e696c9
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '794'
ht-degree: 98%

---

# スケジュールの作成

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
Linked to Editing Users, Editing Projects, Creating and managing groups
-->

[!DNL Adobe Workfront] 管理者は、スケジュールを使用して週労働時間を定義できます。ユーザーやプロジェクトに、スケジュールを関連付けることができます。これにより、[!DNL Workfront] がタイムラインとユーザーの空き時間を計算できるようになります。

異なるタイムゾーンで作業するユーザーがいる場合、各タイムゾーンでスケジュールを作成し、それらのユーザーに関連付けると、作業が [!DNL Workfront] にリアルタイムで記録され、作業する時間帯に従って空き時間が常に正確であることが保証されます。

ユーザーやプロジェクトへのスケジュールの関連付けについては、[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)および[プロジェクトの編集](../../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。

グループ管理者は、自分が管理するグループに関連付けられているスケジュールを作成することもできます。詳しくは、[グループのスケジュールの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md)を参照してください。

スケジュールを使用してユーザーがタイムゾーンをまたいで [!DNL Workfront] で共同作業できるようにする方法については、[タイムゾーンをまたいだ作業](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md)を参照してください。

リソース計画でのスケジュールの使用方法については、[スケジュールの概要](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md)および[リソースプランナーの概要](/help/quicksilver/resource-mgmt/resource-planning/get-started-resource-planner.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## スケジュールの作成

{{step-1-to-setup}}

1. 「**[!UICONTROL スケジュール]**」をクリックします。
1. 「**[!UICONTROL 新規スケジュール]**」をクリックします。
1. スケジュールの名前を入力します。
1. （オプション）「**[!UICONTROL デフォルトのスケジュール]**」を選択して、このスケジュールをデフォルトとして指定します。

   少なくとも 1 つのスケジュールが [!DNL Workfront] に存在する必要があります。1 つのみの場合は、それがデフォルトのスケジュールに指定されます。

   複数のスケジュールを設定できますが、デフォルトのスケジュールは 1 つだけです。

   >[!NOTE]
   >
   >グループ管理者は、スケジュールをデフォルトのスケジュールとして指定できません。スケジュールをシステムのデフォルトとして指定できるのは、[!DNL Workfront] 管理者だけです。

   ![新規スケジュール](assets/new-schedule.png)

1. 「**[!UICONTROL スケジュール]**」タブで、青いアウトラインを時間ブロックをまたいでドラッグしてハイライト表示することで、日次スケジュールを選択します。

   9 時間の期間内に 1 時間ブロックを 8 つ選択することをお勧めします。これにより、昼食やその他の休憩に対応できます。

   ![スケジュールでの時間ブロック](assets/new-schedule-with-exceptions.png)

1. 「**[!UICONTROL 詳細]**」タブで、以下の情報を入力します。

   <table style="table-layout:auto">
    <tr>
     <td>[!UICONTROL Group with Administration Access]</td>
     <td><p>このスケジュールを編集する権限を持つ管理者が所属するグループを選択します。</p>
     <p><b>重要</b>：</p>
      <ul>
       <li>
       <p>グループ管理者がスケジュールを作成する場合、このフィールドは必須です。</p>
       <p>グループ管理者は、自分が管理者として指定されているグループまたはサブグループにスケジュールが指定されている場合にのみ、スケジュールを作成できます。</p>
       <p>1 つのグループのみを管理する場合、このフィールドでは、そのグループがデフォルトで選択されます。</p>
       <p>複数のグループを管理する場合は、スケジュールを保存する前に、このフィールドで 1 つのグループを選択する必要があります。</p></li>
       <li>[!DNL Workfront] 管理者がスケジュールを作成する場合、このフィールドはオプションです。スケジュールをグループに関連付けずに作成すると、そのスケジュールはシステムレベルのスケジュールとして保存され、どのグループのグループ管理者でも管理できなくなります。
       <p>アカウントまたはプロジェクトに割り当てられたスケジュールは、これらのオブジェクトを編集できるすべてのユーザーに表示されます。これは、システムレベルのスケジュールとグループレベルのスケジュールの両方に当てはまります。</p>
       </li>
       <p>スケジュールの管理アクセス権を持つグループを指定しても、そのスケジュールはこのグループ内のユーザーには割り当てられません。グループ内のグループ管理者だけが、スケジュールの編集、削除およびコピーを行えます。</p>
       <p>グループ管理者は、システムレベルのスケジュールを編集、削除またはコピーできません。詳しくは、<a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a>を参照してください。
     </td>
    </tr>
    <tr>
     <td>[!UICONTROL Groups with View Access]</td>
     <td><p>このスケジュールが表示される、[!UICONTROL View]アクセス権を持つグループを選択します。</p>
     <p>スケジュールがユーザーまたはプロジェクトに割り当てられたときに、ここで指定したグループのユーザーのみが、ドロップダウンメニューでそのスケジュールを見つけることができます。</p></tr>
    <tr>
     <td>[!UICONTROL Time Zone]</td>
     <td><p>スケジュールのタイムゾーンを選択します。</p>
     <p>スケジュールをユーザーに関連付ける場合は、スケジュールのタイムゾーンをユーザーのタイムゾーンと一致させることをお勧めします。ユーザーのタイムゾーンについては、<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">ユーザーのプロファイルの編集を参照してください。
     </td>
    </tr>
   </table>


1. 「**[!UICONTROL 例外]**」タブで、スケジュールの例外を指定します。

   例外は、休日や会社のイベントなど、スケジュールから除外する必要がある全日または半日の数です。

   >[!NOTE]
   >
   >繰り返しスケジュールの例外の内容が既にわかっている場合は、今後の何年にもわたってスケジュールの例外を定義できます。

   全日または 1 日の一部を作業スケジュールから除外できます。例外として選択する日付をクリックし、「**[!UICONTROL 一日中]**」フィールドを選択して、例外が全日であるかどうかを指定します。

   ![一日中の例外](assets/schedule-adding-an-all-day-exception.png)

1. 1 日のある時間帯の例外については、開始時刻と終了時刻を入力します。

   ![1 日のある時間帯の例外](assets/partial-day-exception-on-schedules.png)

1. 「**[!UICONTROL 保存]**」に続いて、「**[!UICONTROL 変更を]保存**」をクリックします。

1. （オプション）スケジュールをユーザーに関連付けます。

   詳しくは、[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

1. （オプション）スケジュールをプロジェクトに関連付けます。

   詳しくは、[プロジェクトの編集](../../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。
