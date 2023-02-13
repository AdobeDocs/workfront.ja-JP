---
user-type: administrator
product-area: system-administration
navigation-topic: emails-administration
title: すべてのグループのイベント通知の設定をロック解除またはロックします
description: Adobe Workfrontの管理者は、管理するトップレベルのグループに対してイベント通知を設定するために、グループ管理者がイベント通知をロック解除または再ロックできます。 イベント通知の設定は、イベント通知のアクティブ化と非アクティブ化で構成されます。
author: Lisa, Caroline
feature: System Setup and Administration
role: Admin
exl-id: 056d76c1-7e9b-49b9-974a-75765e53b7fd
source-git-commit: 730932f6c8d4658273dd943e464a038828d288e9
workflow-type: tm+mt
source-wordcount: '540'
ht-degree: 0%

---

# すべてのグループのイベント通知の設定をロック解除またはロックします

Adobe Workfrontの管理者は、管理するトップレベルのグループに対してイベント通知を設定するために、グループ管理者がイベント通知をロック解除または再ロックできます。 イベント通知の設定は、イベント通知のアクティブ化と非アクティブ化で構成されます。

管理するグループの上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。 Workfront管理者（すべてのグループ）も同様です。

管理者がグループのイベント通知を設定すると、そのグループのユーザー、またはそのサブグループの 1 つがホームグループになるユーザーに影響が及びます。 ユーザープロファイルには、システム全体でアクティブ化されたイベント通知の代わりに、ホームグループに対してアクティブ化されたイベント通知が表示されます。 詳しくは、 [グループのイベント通知を表示および設定する](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

>[!NOTE]
>
>* Workfrontの管理者は、Adobe Workfront Classic と新しいAdobe Workfrontエクスペリエンスの両方で、イベント通知の設定のロックを解除および再ロックできます。 ただし、グループ管理者は、新しいAdobe Workfrontエクスペリエンスでのみ、そのイベント通知をグループに設定できます。 Adobe Workfront Classic を使用するグループ管理者は、新しいAdobe Workfrontエクスペリエンスに切り替えて、グループのロックが解除されたイベント通知を設定した後、Adobe Workfront Classic に戻って変更内容を確認できます。
>* サブグループは、グループレベルのイベント通知設定を上位のグループから継承します。
>


## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>システム管理者</p> </td> 
  </tr> 
 </tbody> 
</table>

## イベント通知を設定する機能のロックを解除または再度ロック

>[!IMPORTANT]
>
>通知を再度ロックすると、システム内のすべてのグループが、設定した通知を正確に継承します。 これは、グループ管理者がグループに対しておこなった変更を上書きするので、最初にグループ管理者に相談することをお勧めします。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **電子メール** > **通知**.

1. 次を確認します。 **イベント通知** 」タブが開きます。
1. 通知の右側のアイコンをクリックして、ロック解除済みの ![](assets/lock-toggle-button.png) またはロック済み ![](assets/unlock-toggle-button.png) 位置。

   または

   複数の通知を一度にロックまたはロック解除する場合は、通知を選択し、「ロック解除」 ![](assets/unlock-icon-toolbar.png) またはロック ![](assets/lock-icon-locked-qs.png) ボタンをクリックします。

1. 「**保存**」をクリックします。
1. （オプション）このタスクをグループの管理者に任せる代わりに、トップレベルのグループに対するイベント通知を設定する場合は、次のいずれかを実行できます。

   * 削除 **システムイベント通知** 通知のリストの上の検索ボックスで、通知を検索して最上位グループの名前を選択し、表示されるリストでロック解除済みの通知をアクティブ化または非アクティブ化します。
   * クリック **グループ** 左側のメニューで、最上位グループの名前をクリックします。 クリック **イベント通知** 左側のパネルで、ロック解除されたイベント通知を設定します。詳しくは、 [グループのイベント通知を表示および設定する](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
