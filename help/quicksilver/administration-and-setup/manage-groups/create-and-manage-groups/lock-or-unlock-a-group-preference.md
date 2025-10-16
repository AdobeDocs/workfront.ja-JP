---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: create-and-manage-groups
title: サブグループのプロジェクト、タスクまたはイシューの環境設定のロックまたはロック解除
description: Workfront の管理者がシステムレベルでロックを解除した場合は、グループ管理者がプロジェクト、タスクまたはイシューの環境設定を設定してからロックできます。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 05c32b6f-52e1-46a7-9011-633713422f3d
source-git-commit: a42a167447d2f11b5502e4a0953b5e7eec2e67b1
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 85%

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

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td><p>標準</p>
       <p>プラン</p></td>
  </tr>
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>グループのグループ管理者またはシステム管理者である必要があります。</td>
  </tr>
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## グループプロジェクト、タスク、イシューの環境設定のロックまたはロック解除

{{step-1-to-setup}}

1. 左側のパネルで、「**グループ**」をクリックします。
1. プロジェクト環境設定をロックまたはロック解除するグループの名前をクリックします。
1. 左側のパネルで、「**プロジェクト環境設定**」または「**タスクとイシューの環境設定**」をクリックします。

1. 表示されるページで、システムレベルでロックが解除されている環境設定、または自身のグループの上にあるグループの環境設定に対して、次のいずれかの操作を行います。

   * グループの下のグループの管理者がグループの環境設定を設定できるようにするには、そのロックを解除します ![&#x200B; ロック解除切替スイッチ &#x200B;](assets/unlock-toggle-button.png)。
   * 以下のすべてのグループを環境設定で使用する場合は、ロックされていることを確認してください ![&#x200B; ロック切り替え &#x200B;](assets/lock-toggle-button.png)。

     >[!IMPORTANT]
     >
     >ロックされた設定を構成する方法ですべてのニーズが確実に考慮されるように、管理者および自分の下のグループのユーザーと通信することが重要です。ロックすると、その構成は以下のサブグループに継承されます。また、設定が一定期間ロック解除されていた場合、その設定は、下位のサブグループのグループ管理者が作成した設定を置き換えます。

1. 「**保存**」をクリックします。
