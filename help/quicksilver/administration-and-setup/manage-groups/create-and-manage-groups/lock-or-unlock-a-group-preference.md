---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: サブグループのプロジェクト、タスク、または問題の環境設定をロックまたはロック解除する
description: Workfrontの管理者がシステムレベルでロックを解除した場合は、グループ管理者がプロジェクト、タスクまたは問題の環境設定を設定してからロックできます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 05c32b6f-52e1-46a7-9011-633713422f3d
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '600'
ht-degree: 0%

---

# サブグループのプロジェクト、タスク、または問題の環境設定をロックまたはロック解除する

Workfrontの管理者がシステムレベルでロックを解除した場合は、グループ管理者がプロジェクト、タスクまたは問題の環境設定を設定してからロックできます。

レベルで設定したプロジェクト、タスク、または問題の環境設定をロックすると、グループ内の全員とサブグループ内の全員が同じ設定をその環境設定に使用するようになります。 グループに対してロックした環境設定を再構成することはできますが、グループ管理者はグループに対して再設定できません。

反対に、プロジェクト、タスク、または問題の環境設定をロック解除すると、グループ管理者は、グループがそれらの項目に対してどのように機能するかを柔軟に管理できます。 プリファレンスをロック解除すると、グループ管理者はそれらのサブグループに対して再設定できます。

これは、Workfront管理者がシステム内のすべてのユーザーに対して環境設定をロックまたはロック解除する必要がある機能と並行して実行できます。

Workfront管理者がシステム内のすべてのグループの環境設定をロックまたはロック解除する方法について詳しくは、 [システム内のすべてのグループのプロジェクト環境設定をロックまたはロック解除します](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
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

## グループプロジェクト、タスク、または問題の環境設定をロックまたはロック解除する

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **グループ**.
1. プロジェクト環境設定をロックまたはロック解除するグループの名前をクリックします。
1. 左側のパネルで、 **プロジェクト環境設定** または **タスクと問題の環境設定**.

1. 表示されるページで、システムレベルでロックが解除されているプリファレンス、またはグループの上のグループのプリファレンスに対して、次のいずれかの操作を行います。

   * グループの下のグループの管理者がグループの環境設定を構成できるようにするには、グループのロックを解除します ![](assets/unlock-toggle-button.png).
   * 下のすべてのグループで設定を使用して環境設定を行う場合は、ロックされていることを確認してください ![](assets/lock-toggle-button.png).

      >[!IMPORTANT]
      >
      >ロックされた環境設定を設定する際に、すべてのニーズが確実に考慮されるように、以下のグループの管理者やユーザーとコミュニケーションを取ることが重要です。 ロックすると、その設定は下のサブグループに継承されます。 また、環境設定のロックが一定期間解除されている場合は、下位サブグループ内の管理者が作成したグループ管理者を設定で置き換えます。

1. 「**保存**」をクリックします。
