---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: カスタムステータスの削除
description: カスタムシステムステータスが組織で役立たなくなった場合は、削除できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 73c4eb87-94f6-47bf-b447-eb02a703f7ef
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 1%

---

# カスタムステータスの削除

カスタムシステムステータスが組織で役立たなくなった場合は、削除できます。

ステータスがロックされているかロック解除されているかによって、システム内のすべてのグループのステータスが削除されているかどうかが決まります。

* 現在ロックされているシステムステータスを削除すると、そのグループの名前が変更されているかどうかに関係なく、システム内のすべてのグループのステータスが削除されます。
* 逆に、現在ロック解除されているシステムステータスを削除しても、システム内のすべてのグループのステータスは維持されます。


>[!NOTE]
>
>次の項目は削除できません。
>
>* システムの承認プロセスで使用される、ロックまたはロック解除されたシステムステータス。システム内の少なくとも 1 つのオブジェクトの承認を現在保留中です。
>
>  ただし、単一使用または現在承認待ちのグループレベルの承認プロセスで使用されている、ロックが解除されたシステムステータスを削除することはできます。
>
>  レポートを実行してオブジェクトを検索し、承認待ちを解決してから、ステータスを削除してもう一度試すことができます。 手順については、 [特定のステータスを使用した保留中の承認プロセスのオブジェクトのリスト](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/list-objects-pending-approval-certain-status.md).
>
>* システム内の 1 つ以上のオブジェクトに対して現在承認を保留中の承認プロセスで使用されるステータス。


グループステータスの削除手順については、 [グループステータスの削除](../../../administration-and-setup/manage-groups/manage-group-statuses/delete-a-group-status.md).

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
   <td> <p>Workfront管理者である。</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## カスタムシステムステータスの削除

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **プロジェクト環境設定** > **ステータス**.

1. （個々のグループを含む）システム全体のステータスを削除するには、ステータスの上にマウスを移動して、 **編集**&#x200B;を選択し、 **すべてのグループに対してロック** が選択されている。 「**保存**」をクリックします。

   または

   システムステータスを削除して、個々のグループに対して保持するには、ステータスの上にマウスを移動して、 **編集**&#x200B;を選択し、 **すべてのグループに対してロック** が選択されていない。 「**保存**」をクリックします。

1. 削除するステータスの上にマウスポインターを置いて、「 **削除**.
1. 表示されるメッセージで、 **ステータスを削除**.
1. 内 **ステータスを削除** 表示されるボックスで、ラベル付きのフィールドでステータスを選択します **現在このステータスのすべてのプロジェクトをに設定**.

   削除しようとしていたステータスを使用していたプロジェクトは、選択したステータスに設定されます。

   ステータスは、削除中のステータスと同じステータスである場合にのみ、ドロップダウンリストで使用できます。

   例えば、現在のステータスを削除する場合、現在のステータスと同じステータスのみを選択できます。

1. クリック **ステータスを削除**.
