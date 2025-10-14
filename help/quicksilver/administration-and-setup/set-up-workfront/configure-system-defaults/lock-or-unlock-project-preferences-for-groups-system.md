---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: システム内のすべてのグループのプロジェクト環境設定のロックまたはロック解除
description: 組織内の各グループでは、一意のワークフローに合わせて、それぞれのプロジェクト環境設定が必要になる場合があります。組織全体のすべてのグループの環境設定をロック解除すると、各グループで独自に設定できるようになります。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: f5a94eaf-ebb8-424b-80ff-ba40cc985a6e
source-git-commit: 612243e928c6053d9b02715d9fcfef4dae25cb7a
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 86%

---

# システム内のすべてのグループに対するプロジェクト環境設定をロックまたはロック解除

組織内の各グループでは、一意のワークフローに合わせて、それぞれのプロジェクト環境設定が必要になる場合があります。組織全体のすべてのグループの環境設定をロック解除すると、各グループで独自に設定できるようになります。

プリファレンスのロックが解除され、グループ管理者が変更すると、グループに関連付けられたプロジェクトは、システムレベルの設定ではなく、グループレベルの設定からそのプリファレンスの設定を取得します。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>新規：[!UICONTROL Standard]</p>
   または
   <p>現在：[!UICONTROL Plan]</p>
   </td> 
  </tr>
  <tr> 
   <td role="rowheader">アクセスレベル設定</td>
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ロックおよびロック解除の環境設定について

システムレベルで設定したプロジェクト、タスク、またはイシューの環境設定をロックすると、すべてのユーザーが同じ環境設定で使用できるようになります。ロックした環境設定は再構成できますが、グループ管理者はグループ用に再設定できません。

反対に、プロジェクト、タスク、またはイシューの環境設定をロック解除すると、グループ管理者は、それらの項目を使用してグループがどのように機能するかを柔軟に管理できます。プリファレンスをロック解除すると、グループ管理者はそのプリファレンスをグループ用に再設定できます。

フィールドにロック/ロック解除の切り替えスイッチがない場合、グループ管理者がグループレベルで設定を指定するためにロックを解除することはできません。 設定は、システムレベルでのみ使用できます。

システムレベルのプロジェクト、タスク、またはイシューの環境設定をロックまたはロック解除する手順については、[システム全体のタスクとイシューの環境設定を行う](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

>[!NOTE]
>
>[!DNL Workfront] 管理者がシステムレベルで環境設定のロックを解除した後、グループ管理者なら誰でもその設定を行い、自身のグループおよび下位のサブグループのメンバー全員が同じ設定を使用するようにロックできます。これは、[!DNL Workfront] 管理者がシステム内のすべてのユーザーに対して環境設定を指定およびロックする操作と同じです。詳しくは、[グループのプロジェクト環境設定の指定](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)および[サブグループのプロジェクト、タスクまたはイシューの環境設定をロックまたはロック解除](../../../administration-and-setup/manage-groups/create-and-manage-groups/lock-or-unlock-a-group-preference.md)を参照してください。

## プロジェクトの環境設定をロック解除して、グループで設定できるようにする

{{step-1-to-setup}}

1. 「**[!UICONTROL プロジェクト環境設定]**」、「**[!UICONTROL プロジェクト]**」の順にクリックします。

1. 次のいずれかの操作を行います。

   * グループ管理者がグループの環境設定を設定できるようにするには、ロックを解除します ![&#x200B; ロック解除切替スイッチ &#x200B;](assets/unlock-toggle-button.png)。
   * すべてのグループで環境設定を使用する場合は、環境設定がロックされていることを確認します（これがデフォルトの設定です）。

     >[!IMPORTANT]
     >
     >ロックされた環境設定を指定する際にすべてのニーズが考慮されるように、システム全体の管理者やグループ内のユーザーとコミュニケーションを取ることをお勧めします。ロックすると、その設定がシステム内のすべてのグループに継承されます。また、環境設定のロックが一定期間解除されている場合、設定はグループ管理者が指定した設定と置き換えられます。

1. 「**[!UICONTROL 保存]**」をクリックします。
