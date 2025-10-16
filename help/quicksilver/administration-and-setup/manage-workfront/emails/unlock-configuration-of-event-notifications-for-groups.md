---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: すべてのグループのイベント通知の設定のロック解除またはロック
description: Adobe Workfront の管理者は、管理するトップレベルのグループに対してグループ管理者がイベント通知を設定できるようにロック解除または再ロックできます。イベント通知の設定は、その設定の有効化と無効化で構成されます。
author: Lisa, Nolan
feature: System Setup and Administration
role: Admin
exl-id: 056d76c1-7e9b-49b9-974a-75765e53b7fd
source-git-commit: e34abb5ff1068de99eaba33dc95287164e556742
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 95%

---

# すべてのグループのイベント通知の設定をロック解除またはロックします。

Adobe Workfront の管理者は、管理するトップレベルのグループに対してグループ管理者がイベント通知を設定できるようにロック解除または再ロックできます。イベント通知の設定は、その設定の有効化と無効化で構成されます。

管理するグループ上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。Workfront 管理者（すべてのグループ）も同様です。

管理者がグループのイベント通知を設定すると、グループ、またはそのサブグループの 1 つがホームグループになるユーザーに影響が及びます。ユーザープロファイルには、システム全体でアクティブ化されたイベント通知ではなく、ホームグループに対してアクティブ化されたイベント通知が表示されます。詳しくは、[グループのイベント通知を表示および設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)を参照してください。

>[!NOTE]
>
>* Workfront の管理者は、Adobe Workfront Classic と新しい Adobe Workfront エクスペリエンスの両方で、イベント通知の設定のロックを解除および再ロックできます。ただし、グループ管理者は、新しい Adobe Workfront エクスペリエンスでのみ、そのイベント通知をグループに設定できます。Adobe Workfront Classic を使用するグループ管理者は、新しい Adobe Workfront エクスペリエンスに切り替えて、グループのロックが解除されたイベント通知を設定した後、Adobe Workfront Classic に戻って実際の変更内容を確認できます。
>* サブグループは、グループレベルのイベント通知設定を上位のグループからすぐ上に継承します。
>

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
   <p>標準</p>
   <p>プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>システム管理者</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## イベント通知を設定する機能のロックを解除または再度ロック

>[!IMPORTANT]
>
>通知を再度ロックすると、システム内のすべてのグループが、設定した通知を正確に継承します。これは、グループ管理者がグループに対して行った変更を上書きするので、最初にグループ管理者に相談することをお勧めします。

{{step-1-to-setup}}

1. **メール**／**通知**&#x200B;をクリックします。

1. 「**イベント通知**」タブが開くことを確認します。
1. 通知の右側にあるアイコンをクリックして、ロック ![ロックアイコン](assets/lock-toggle-button.png) またはロックが解除 ![ロック解除アイコン](assets/unlock-toggle-button.png) の位置に切り替えます。

   または

   複数の通知を一度にロック解除またはロックしたい場合は、通知を選択し、リストの上のツールバーに表示されるロック解除 ![ロック解除アイコン](assets/unlock-icon-toolbar.png) またはロック ![ロックアイコン](assets/lock-icon-locked-qs.png) のボタンをクリックします。

1. 「**保存**」をクリックします。
1. （オプション）このタスクをグループの管理者に任せる代わりに、トップレベルのグループに対するイベント通知を設定する場合は、次のいずれかの操作を実行できます。

   * 通知のリストの上にある検索ボックスで&#x200B;**システムイベント通知**&#x200B;を削除し、上位レベルのグループの名前を検索および選択します。その後、表示されるリストでロック解除済みの通知を有効化または無効化します。
   * 左側のメニューで、「**グループ**」をクリックしてから、トップレベルのグループの名前を選択します。左側のパネルで、「**イベント通知**」をクリックし、[グループのイベント通知を表示および設定](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md)で説明したように、ロック解除済みのイベント通知を設定します。
