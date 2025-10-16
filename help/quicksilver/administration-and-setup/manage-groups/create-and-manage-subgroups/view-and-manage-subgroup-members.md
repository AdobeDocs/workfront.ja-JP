---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: サブグループのメンバーの表示と管理
description: 管理対象のグループを表示している場合、グループのサブグループ内のすべてのユーザーを表示および管理できます。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 8f7b0183-6035-4dd4-8e42-fd65485449bf
source-git-commit: a42a167447d2f11b5502e4a0953b5e7eec2e67b1
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 67%

---

# サブグループのメンバーの表示と管理

管理対象のグループを表示している場合、グループのサブグループ内のすべてのユーザーを表示および管理できます。

管理するグループ上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。Workfront 管理者（すべてのグループ）も同様です。

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
   <td> <p>次のいずれかが必要です。</p> 
    <ul> 
     <li> <p>システム管理者のアクセス レベルです。 </li> 
     <li> <p><b>編集</b>アクセスに設定されたアクセスレベルでの<b>ユーザー</b>設定には、<b>作成</b>および<b>設定を微調整</b> <img src="assets/gear-icon-settings.png">の下で有効となる少なくとも 2 つのうち 1 つの<b>ユーザー管理者</b>オプションがあります。 </p> <p>これら 2 つのオプションのうち、<b> ユーザー管理者（グループユーザー） </b> が有効になっている場合、ユーザーがメンバーになっているグループのグループ管理者である必要があります。</p> </li> 
    </ul> </td> 
  </tr>  
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## グループの下のサブグループのメンバーを表示および管理

{{step-1-to-setup}}

1. 「**グループ**」をクリックします。

   表示されるリストで、管理しているグループと、その中のサブグループを確認できます。Adobe Workfront 管理者は、すべてのグループを表示できます。

1. サブグループメンバーを表示または管理するグループの名前をクリックします。
1. 左側のパネルで、「**サブグループメンバー**」をクリックします。

   この左のパネル項目は、グループにサブグループが含まれている場合にのみ使用できます。

1. 次のいずれかの操作を行います。

   * リストでメンバーを選択し、編集 ![&#x200B; 編集アイコン &#x200B;](assets/edit-icon.png) をクリックして、そのユーザーのユーザープロファイルを変更します。

     詳しくは、[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)または[ユーザープロファイルの一括編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md)を参照してください。

   * リスト内の任意の数のサブグループメンバーを選択し、「**ユーザーに更新を送信**」をクリックして、ユーザープロファイルにコメントを追加します。

     ユーザーには、アプリ内通知と、コメントが記載されたメール通知が送信されます。コメントは、ユーザーのプロファイルの「更新」エリアに表示されます。

     詳しくは、[&#x200B; 他のユーザーへのダイレクトメッセージの送信 &#x200B;](/help/quicksilver/people-teams-and-groups/work-directly-with-others/send-direct-messages-to-other-users.md) を参照してください。

   * リスト内の任意の数のメンバーを選択し、「非アクティブ化 ![&#x200B; ユーザーの非アクティブ化 &#x200B;](assets/deactivate-user.png) または「アクティブ化 ![&#x200B; ユーザーのアクティブ化 &#x200B;](assets/activate-user.png)」をクリックします。

     詳しくは、[ユーザーの非アクティブ化または再アクティブ化](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)を参照してください。

   * Export![Export](assets/export.png) メンバーのリスト。
