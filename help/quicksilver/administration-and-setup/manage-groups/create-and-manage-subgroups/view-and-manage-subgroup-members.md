---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: サブグループメンバーの表示と管理
description: 管理対象のグループを表示している場合、グループのサブグループ内のすべてのユーザーを表示および管理できます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8f7b0183-6035-4dd4-8e42-fd65485449bf
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 0%

---

# サブグループメンバーの表示と管理

管理対象のグループを表示している場合、グループのサブグループ内のすべてのユーザーを表示および管理できます。

管理するグループの上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。 Workfront管理者（すべてのグループ）も同様です。

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
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>「ユーザー管理者（すべてのユーザー） 」オプションを選択して、ユーザーへのアクセスを編集</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスタイプ、アクセスレベル設定を確認するには、Workfront管理者に問い合わせてください。

## グループの下のサブグループのメンバーを表示および管理

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **グループ**.

   表示されるリストで、管理しているグループと、そのグループに含まれているサブグループを確認できます。 Adobe Workfront管理者は、すべてのグループを表示できます。

1. サブグループメンバーを表示または管理するグループの名前をクリックします。
1. 左側のパネルで、 **サブグループメンバー**.

   この左のパネル項目は、グループにサブグループが含まれている場合にのみ使用できます。

1. 次のいずれかの操作を行います。

   * リスト内のメンバーを選択し、「編集」をクリックします。 ![](assets/edit-icon.png) をクリックして、そのユーザーのユーザープロファイルを変更します。

      詳しくは、 [ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md) または [ユーザープロファイルの一括編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md).

   * リスト内の任意の数のメンバーを選択し、「更新」をクリックします ![](assets/comment-icon.png) をクリックして、ユーザープロファイルにコメントを追加します。

      ユーザーには、アプリ内通知と、コメントが記載された電子メール通知が送信されます。 コメントは、ユーザーのプロファイルの「更新」領域に表示されます。

   * リスト内の任意の数のメンバーを選択し、「非アクティブ化」をクリックします ![](assets/deactivate-user.png) またはアクティブ化 ![](assets/activate-user.png).

      詳しくは、 [ユーザーを非アクティブ化または再アクティブ化する](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md).

   * 書き出し ![](assets/export.png) メンバーのリスト。
