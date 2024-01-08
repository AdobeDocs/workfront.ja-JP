---
user-type: administrator
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: スケジュールの作成
description: スケジュールを使用して、ユーザーの作業週を定義できます。 スケジュールは、ユーザーまたはプロジェクトに関連付けることができます。 これにより、 [!DNL Workfront] をクリックして、タイムラインとユーザーの可用性を計算します。
author: Lisa, Alina
feature: System Setup and Administration
role: Admin
exl-id: f7347ba6-68bf-45d8-b5d2-6136f3e696c9
source-git-commit: 9d2165cdc9399273a4f79b90d4049f50097cadee
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 0%

---

# スケジュールの作成

<!--Audited: 01/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
Linked to Editing Users, Editing Projects, Creating and managing groups
-->

As an [!DNL Adobe Workfront] 管理者は、スケジュールを使用して作業週を定義できます。 スケジュールは、ユーザーまたはプロジェクトに関連付けることができます。 これにより、 [!DNL Workfront] をクリックして、タイムラインとユーザーの可用性を計算します。

異なるタイムゾーンで作業するユーザーがいる場合、各タイムゾーンでスケジュールを作成し、それらのユーザーに関連付けると、作業が必ず次の場所に記録されます。 [!DNL Workfront] リアルタイムで実行でき、動作するタイミングに応じて常に正確に使用できること。

スケジュールとユーザーおよびプロジェクトの関連付けについて詳しくは、 [ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) および [プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md).

また、グループ管理者は、管理するグループに関連付けられたスケジュールを作成することもできます。 詳しくは、 [グループのスケジュールを作成および変更する](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

スケジュールを使用して、 [!DNL Workfront] タイムゾーンを超える場合： [タイムゾーンをまたいでの作業](../../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md).

生産資源計画でのスケジュールの使用方法の詳細は、「 [スケジュールの概要](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/schedules-overview.md) および [リソースプランナーの概要](/help/quicksilver/resource-mgmt/resource-planning/get-started-resource-planner.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>新規： [!UICONTROL Standard]</p>
       <p>または</p>
       <p>現在： [!UICONTROL プラン ]</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>次の条件を満たす必要があります。 [!DNL Workfront] 管理者。 </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## スケジュールの作成

{{step-1-to-setup}}

1. クリック **[!UICONTROL スケジュール]**.
1. クリック **[!UICONTROL 新しいスケジュール]**.
1. スケジュールの名前を入力します。
1. （オプション）「 」を選択します。 **[!UICONTROL デフォルトのスケジュール]** をクリックして、このスケジュールをデフォルトとして指定します。

   に少なくとも 1 つのスケジュールを設定する必要があります [!DNL Workfront]. 1 つのみの場合は、デフォルトのスケジュールに指定されます。

   複数のスケジュールを設定できますが、既定のスケジュールは 1 つだけにすることができます。

   >[!NOTE]
   >
   >グループ管理者は、スケジュールをデフォルトのスケジュールとして指定できません。 a のみ [!DNL Workfront] 管理者は、スケジュールをシステムのデフォルトとして指定できます。

   ![新しいスケジュール](assets/new-schedule.png)

1. 次の日： **[!UICONTROL スケジュール]** 「 」タブで、時間ブロック間の青いアウトラインをドラッグしてハイライト表示し、日次スケジュールを選択します。

   9 時間の期間に 8 つの 1 時間ブロックを選択することをお勧めします。 昼食や休憩に対応。

   ![スケジュールに基づく時間ブロック](assets/new-schedule-with-exceptions.png)

1. 次の日： **[!UICONTROL 詳細]** 「 」タブで、次の情報を入力します。

   <table style="table-layout:auto">
    <tr>
     <td>[!UICONTROL 管理アクセス権を持つグループ ]</td>
     <td><p>このスケジュールを編集する権限を持つ管理者のグループを選択します。</p>
     <p><b>重要</b>:</p>
      <ul>
       <li>
       <p>スケジュールを作成するグループ管理者の場合、このフィールドは必須です。</p>
       <p>グループ管理者は、自分が管理者として指定されているグループまたはサブグループに対して指定されている場合にのみ、スケジュールを作成できます。</p>
       <p>1 つのグループのみを管理する場合、このフィールドではそのグループがデフォルトで選択されます。</p>
       <p>複数のグループを管理する場合は、スケジュールを保存する前に、このフィールドでグループを選択する必要があります。</p></li>
       <li>次の場合、 [!DNL Workfront] 管理者がスケジュールを作成する場合、このフィールドはオプションです。 スケジュールをグループに関連付けずに作成すると、そのスケジュールはシステムレベルのスケジュールとして保存され、どのグループのグループ管理者でも管理できなくなります。
       <p>アカウントまたはプロジェクトに割り当てられたスケジュールは、これらのオブジェクトを編集できるすべてのユーザーに表示されます。 これは、システムレベルのスケジュールとグループレベルのスケジュールの両方に当てはまります。</p>
       </li>
       <p>スケジュールに対して管理アクセス権を持つグループを指定しても、グループ内のユーザーにスケジュールは割り当てられません。グループ内のグループ管理者だけが、スケジュールを編集、削除、コピーできます。</p>
       <p>グループ管理者は、システムレベルのスケジュールを編集、削除、またはコピーできません。 詳しくは、 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a>.
     </td>
    </tr>
    <tr>
     <td>[!UICONTROL 表示アクセス権を持つグループ ]</td>
     <td><p>[!UICONTROL 表示 ] にアクセスし、このスケジュールを表示できるグループを選択します。</p>
     <p>ここで指定したグループのユーザーのみが、ユーザーまたはプロジェクトに割り当てる際に、ドロップダウンメニューでスケジュールを検索できます。</p></tr>
    <tr>
     <td>[!UICONTROL タイムゾーン ]</td>
     <td><p>スケジュールのタイムゾーンを選択します。</p>
     <p>スケジュールをユーザーに関連付ける場合、スケジュールのタイムゾーンがユーザーのタイムゾーンと一致することをお勧めします。 ユーザーのタイムゾーンについて詳しくは、 <a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">ユーザーのプロファイルを編集します。
     </td>
    </tr>
   </table>


1. 次の日： **[!UICONTROL 例外]** タブで、スケジュールに対する例外を指定します。

   例外は、休日や会社のイベントなど、スケジュールから除外する必要がある完全な日数または半日数です。

   >[!NOTE]
   >
   >定期スケジュールの例外が何かが既にわかっている場合は、将来の何年間もスケジュールの例外を定義できます。

   全日または一部の日は、作業スケジュールから除外できます。 日付をクリックして例外として選択し、「 **[!UICONTROL 終日]** フィールドを使用して、例外が 1 日であるかどうかを指定します。

   ![終日例外](assets/schedule-adding-an-all-day-exception.png)

1. 日の一部例外の開始および終了時間を入力します。

   ![日の一部例外](assets/partial-day-exception-on-schedules.png)

1. クリック **[!UICONTROL 保存]**&#x200B;を選択し、次に **[!UICONTROL 保存] 変更点**.

1. （オプション）スケジュールをユーザーに関連付けます。

   詳しくは、 [ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

1. （オプション）スケジュールをプロジェクトに関連付けます。

   詳しくは、 [プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md).
