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
source-git-commit: 63c2206905f4ebbc35cb162ae6e895b98b5d20eb
workflow-type: tm+mt
source-wordcount: '384'
ht-degree: 87%

---

# サブグループのメンバーの表示と管理

管理対象のグループを表示している場合、グループのサブグループ内のすべてのユーザーを表示および管理できます。

管理するグループ上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。Workfront 管理者（すべてのグループ）も同様です。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：プラン</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>次のいずれかが必要です。</p> 
    <ul> 
     <li> <p>システム管理者のアクセス レベルです。 </li> 
     <li> <p><b>編集</b>アクセスに設定されたアクセスレベルでの<b>ユーザー</b>設定には、<b>作成</b>および<b>設定を微調整</b> <img src="assets/gear-icon-settings.png">の下で有効となる少なくとも 2 つのうち 1 つの<b>ユーザー管理者</b>オプションがあります。 </p> <p>これら 2 つのオプションのうち、<b> ユーザー管理者（グループユーザー） </b> が有効になっている場合、ユーザーがメンバーになっているグループのグループ管理者である必要があります。</p> </li> 
    </ul> </td> 
  </tr>  
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## グループの下のサブグループのメンバーを表示および管理

{{step-1-to-setup}}

1. 「**グループ**」をクリックします。

   表示されるリストで、管理しているグループと、その中のサブグループを確認できます。Adobe Workfront 管理者は、すべてのグループを表示できます。

1. サブグループメンバーを表示または管理するグループの名前をクリックします。
1. 左側のパネルで、「**サブグループメンバー**」をクリックします。

   この左のパネル項目は、グループにサブグループが含まれている場合にのみ使用できます。

1. 次のいずれかの操作を行います。

   * リスト内のメンバーを選択し、「編集」![](assets/edit-icon.png) をクリックして、そのユーザーのユーザープロファイルを変更します。

     詳しくは、[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)または[ユーザープロファイルの一括編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-user-profiles-in-bulk.md)を参照してください。

   * リスト内の任意の数のメンバーを選択し、「更新」![](assets/comment-icon.png) をクリックして、ユーザープロファイルにコメントを追加します。

     ユーザーには、アプリ内通知と、コメントが記載されたメール通知が送信されます。コメントは、ユーザーのプロファイルの「更新」エリアに表示されます。

   * リスト内の任意の数のメンバーを選択し、「非アクティブ化」![](assets/deactivate-user.png) または「アクティブ化」![](assets/activate-user.png) をクリックします。

     詳しくは、[ユーザーを非アクティブ化または再アクティブ化](../../../administration-and-setup/add-users/create-and-manage-users/deactivate-a-user.md)を参照してください。

   * メンバーのリスト ![](assets/export.png) を書き出します。
