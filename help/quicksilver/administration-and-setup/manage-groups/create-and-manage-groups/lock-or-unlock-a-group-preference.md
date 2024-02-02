---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: サブグループのプロジェクト、タスク、またはイシューの環境設定のロックまたはロック解除
description: Workfront の管理者がシステムレベルでロックを解除した場合は、グループ管理者がプロジェクト、タスクまたはイシューの環境設定を設定してからロックできます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 05c32b6f-52e1-46a7-9011-633713422f3d
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: ht
source-wordcount: '600'
ht-degree: 100%

---

# サブグループのプロジェクト、タスク、またはイシューの環境設定のロックまたはロック解除

Workfront の管理者がシステムレベルでロックを解除した場合は、グループ管理者がプロジェクト、タスクまたはイシューの環境設定を設定してからロックできます。

レベルで設定したプロジェクト、タスク、またはイシューの環境設定をロックすると、グループ内とサブグループ内の全員が同じ設定をその環境設定に使用するようになります。グループに対してロックした環境設定を再設定することはできますが、グループ管理者はグループに対して再設定できません。

反対に、プロジェクト、タスク、またはイシューの環境設定をロック解除すると、グループ管理者は、それらの項目を使用してグループがどのように機能するかを柔軟に管理できます。環境設定をロック解除すると、グループ管理者はそれらのサブグループに対して再設定できます。

これは、Workfront 管理者がシステム内のすべてのユーザーの設定をロックまたはロック解除する必要がある機能と同じです。

Workfront 管理者がシステム内のすべてのグループの環境設定をロックまたはロック解除する方法について詳しくは、[システム内のすべてのグループのプロジェクト環境設定のロックまたはロック解除](../../../administration-and-setup/set-up-workfront/configure-system-defaults/lock-or-unlock-project-preferences-for-groups-system.md)を参照してください。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Unlike other Lock/Unlock articles that start just like this one, we need the steps here. In other areas, the lock/unlock step is part of the article about setting preferences or creating statuses.</p>
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
   <td> <p>プラン </p> <p>グループのグループ管理者または Workfront 管理者である必要があります。詳しくは、<a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a>および<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランまたはライセンスの種類を確認する必要がある場合は、Workfront 管理者にお問い合わせください。

## グループプロジェクト、タスク、イシューの環境設定のロックまたはロック解除

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックして、**設定** ![](assets/gear-icon-settings.png) をクリックします。

1. 左側のパネルで、「**グループ**」をクリックします。
1. プロジェクト環境設定をロックまたはロック解除するグループの名前をクリックします。
1. 左側のパネルで、「**プロジェクト環境設定**」または「**タスクとイシューの環境設定**」をクリックします。

1. 表示されるページで、システムレベルでロックが解除されている環境設定、または自身のグループの上にあるグループの環境設定に対して、次のいずれかの操作を行います。

   * 自身のグループの下にあるグループの管理者が自身のグループの環境設定を構成できるようにするには、ロックを解除します ![](assets/unlock-toggle-button.png)。
   * 自身のグループの下にあるすべてのグループで環境設定の設定を使用する場合は、ロックされていることを確認してください。![](assets/lock-toggle-button.png)

     >[!IMPORTANT]
     >
     >ロックされた設定を構成する方法ですべてのニーズが確実に考慮されるように、管理者および自分の下のグループのユーザーと通信することが重要です。ロックすると、その構成は以下のサブグループに継承されます。また、設定が一定期間ロック解除されていた場合、その設定は、下位のサブグループのグループ管理者が作成した設定を置き換えます。

1. 「**保存**」をクリックします。
