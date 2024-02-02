---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: グループのタイムシートと時間の優先順位をロックまたはロック解除
description: グループ管理者の場合は、Workfront 管理者がシステムレベルでロックを解除した後、グループのタイムシートと時間設定を構成してロックできます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5b36106f-d521-4cc1-9f1f-647415c282b4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '627'
ht-degree: 100%

---

# グループのタイムシートと時間の優先順位をロックまたはロック解除

グループ管理者の場合は、Workfront 管理者がシステムレベルでロックを解除した後、グループのタイムシートと時間設定を構成してロックできます。

Adobe Workfront 環境設定をロックすると、グループおよびそのサブグループ内の全員がその環境設定に対して同じ設定を使用するようになります。ロックした設定を再構成することはできますが、グループ管理者は下位のサブグループに対して再構成を行うことはできません。

逆に、グループレベルで設定のロックを解除すると、サブグループ管理者は、グループがそれらの項目を操作する方法をより柔軟に管理できるようになります。設定のロックが解除されると、グループ管理者はそれらのサブグループに対して設定を再設定できます。

これは、Workfront 管理者がシステム内のすべてのユーザーの設定をロックまたはロック解除する必要がある機能と同じです。

Workfront 管理者がシステム内のすべてのグループのタイムシートと時間設定をロックまたはロック解除する方法については、[タイムシートと時間設定を構成する](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)を参照してください。

グループのタイムシートと時間設定の構成については、[グループのタイムシートと時間設定を構成する](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md)を参照してください。

<!--
Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
-->

>[!NOTE]
>
>* グループのロック解除された設定を構成しても、そのグループの下のサブグループの設定には影響しません。
>
>  ただし、新しいサブグループが作成されると、そのすぐ上のグループの基本設定とロックまたはロック解除の状態が継承されます。
>
>* ロックされた設定を持つグループの下にグループを移動すると、移動されたグループはその設定を継承し、移動されたグループに対してロックされます。
>* ロックが解除された環境設定を持つグループの下にグループを移動した場合、移動されたグループはその環境設定の影響を与えません。
>
>  移動されたグループの設定が移動時にロックされている場合、その設定はロックされたままになりますが、親グループではロックが解除されているため、グループ管理者はここでロックを解除できます。
>

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
   <td> <p>プラン </p> <p>グループのグループ管理者または Workfront 管理者である必要があります。詳しくは、<a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a>と<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類を確認するには、Workfront 管理者にお問い合わせください。

## グループのタイムシートと時間の優先順位をロックまたはロック解除

>[!TIP]
>
>Workfront 管理者は、設定／タイムシートと時間／環境設定に移動して、ページ上部のボックスでグループの名前を検索することで、手順 1～4 をスキップできます。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)をクリックし、「**設定**」![](assets/gear-icon-settings.png) をクリックします。

1. 左側のパネルで、「**グループ**」をクリックします。
1. タイムシートと時間設定をロックまたはロック解除するグループの名前をクリックします。
1. 左側のパネルで、「**タイムシートと時間の設定**」をクリックします。

1. 表示されるページで、次のいずれかの操作を行います。

   * 自身のグループの下にあるグループの管理者が自身のグループの環境設定を構成できるようにするには、ロックを解除します ![](assets/unlock-toggle-button.png)。
   * 自分の下のすべてのグループに設定を使用させたい場合は、その設定がロック ![](assets/lock-toggle-button.png) であることを確認してください（これがデフォルトの設定です）。

     >[!IMPORTANT]
     >
     >ロックされた設定を構成する方法ですべてのニーズが確実に考慮されるように、管理者および自分の下のグループのユーザーと通信することが重要です。ロックすると、その構成は以下のサブグループに継承されます。また、設定が一定期間ロック解除されていた場合、その設定は、下位のサブグループのグループ管理者が作成した設定を置き換えます。

1. 「**保存**」をクリックします。
