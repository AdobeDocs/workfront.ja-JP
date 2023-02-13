---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: グループのタイムシートと時間の優先順位をロックまたはロック解除する
description: グループ管理者は、Workfront管理者がシステムレベルでグループをロック解除した後で、グループのタイムシートと時間の優先設定を構成し、ロックすることができます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5b36106f-d521-4cc1-9f1f-647415c282b4
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '627'
ht-degree: 0%

---

# グループのタイムシートと時間の優先順位をロックまたはロック解除する

グループ管理者は、Workfront管理者がシステムレベルでグループをロック解除した後で、グループのタイムシートと時間の優先設定を構成し、ロックすることができます。

Adobe Workfrontの環境設定をロックすると、グループ内の全員とサブグループ内の全員が同じ設定をその環境設定で使用するようになります。 ロックした環境設定は再構成できますが、グループ管理者は下位のサブグループに対しては再構成できません。

逆に、グループレベルでプリファレンスをロック解除すると、サブグループ管理者は、グループがそれらのアイテムを扱う方法をより柔軟に管理できます。 プリファレンスをロック解除すると、グループ管理者はそれらのサブグループに対して再設定できます。

これは、Workfront管理者がシステム内のすべてのユーザーに対して環境設定をロックまたはロック解除する必要がある機能と並行して実行できます。

Workfront管理者がタイムシートをロックまたはロック解除する方法、およびシステム内のすべてのグループの時間の優先順位については、 [タイムシートと時間の基本設定を構成する](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md).

タイムシートの構成とグループの時間優先の詳細については、「 [グループのタイムシートと時間の基本設定を構成する](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-timesheet-hour-preferences-group.md).

<!--
Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
-->

>[!NOTE]
>
>* グループのロックが解除された環境設定を構成しても、グループの下にあるサブグループの環境設定には影響しません。
>
>  ただし、新しいサブグループを作成すると、その直上のグループのプリファレンス設定とロックまたはロック解除状態が継承されます。
>
>* ロックされたプリファレンスを持つグループの下にグループを移動すると、移動されたグループはそのプリファレンスを継承し、移動されたグループに対してロックされます。
>* ロックが解除されたプリファレンスを持つグループの下にグループを移動しても、そのプリファレンスの影響は受けません。
>
>  移動時に移動グループ内のプリファレンスがロックされた場合、そのプリファレンスはロックされたままになりますが、親グループのロックが解除されているので、グループ管理者は今すぐロックを解除できます。

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
   <td> <p>計画 </p> <p>グループのグループ管理者またはWorkfront管理者である必要があります。 詳しくは、 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a> および <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランまたはライセンスの種類を確認する必要がある場合は、Workfront管理者にお問い合わせください。

## グループのタイムシートと時間の優先順位をロックまたはロック解除する

>[!TIP]
>
>Workfrontの管理者は、[ 設定 ] > [ タイムシートと時間 ] > [ 環境設定 ] に移動して、ページ上部のボックスでグループの名前を検索することで、手順 1 ～ 4 をスキップできます。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **グループ**.
1. タイムシートと時間の優先順位をロックまたはロック解除するグループの名前をクリックします。
1. 左側のパネルで、 **タイムシートと時間の環境設定**.

1. 表示されるページで、次のいずれかの操作を行います。

   * グループの下のグループの管理者がグループの環境設定を構成できるようにするには、グループのロックを解除します ![](assets/unlock-toggle-button.png).
   * 下のすべてのグループで設定を使用して環境設定を行う場合は、ロックされていることを確認してください ![](assets/lock-toggle-button.png) （これはデフォルト）。

      >[!IMPORTANT]
      >
      >ロックされた環境設定を設定する際に、すべてのニーズが確実に考慮されるように、以下のグループの管理者やユーザーとコミュニケーションを取ることが重要です。 ロックすると、その設定は下のサブグループに継承されます。 また、環境設定のロックが一定期間解除されている場合は、下位サブグループ内の管理者が作成したグループ管理者を設定で置き換えます。

1. 「**保存**」をクリックします。
