---
user-type: administrator
product-area: system-administration
navigation-topic: create-custom-status-and-priority-labels
title: カスタムステータスの削除
description: カスタムシステムステータスが組織にとって不要になった場合は、削除できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 73c4eb87-94f6-47bf-b447-eb02a703f7ef
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 96%

---

# カスタムステータスの削除

カスタムシステムステータスが組織にとって不要になった場合は、削除できます。

ステータスがロックされているかロック解除されているかによって、システム内のすべてのグループのステータスが削除されるかどうかが決まります。

* 現在ロックされているシステムステータスを削除すると、グループの名前が変更されているかどうかに関係なく、システム内のすべてのグループのステータスが削除されます。
* 逆に、現在ロック解除されているシステムステータスを削除しても、そのステータスはシステム内のすべてのグループで維持されます。


>[!NOTE]
>
>以下のものは削除できません。
>
>* システムの承認プロセスで使用される、ロックまたはロック解除されたシステムステータス。システム内の 1 つ以上のオブジェクトに対して承認を現在保留中です。
>
>  ただし、単一使用または現在承認保留中のグループレベルの承認プロセスで使用され、ロックが解除されたシステムステータスは削除できます。
>
>  レポートを実行してオブジェクトを検索し、承認保留中を解決してから、ステータスの削除を再試行できます。手順については、[特定のステータスを使用した承認保留中プロセスのオブジェクトを一覧表示](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/list-objects-pending-approval-certain-status.md)を参照してください。
>
>* システム内の 1 つ以上のオブジェクトに対して現在承認保留中の承認プロセスで使用されるステータス。

グループステータスの削除手順については、[グループステータスを削除](../../../administration-and-setup/manage-groups/manage-group-statuses/delete-a-group-status.md)を参照してください。

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
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
     <p>新規：標準</p>
     <p>または</p>
     <p>現在：プラン</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## カスタムシステムステータスを削除

{{step-1-to-setup}}

1. 左側のパネルで、**プロジェクト環境設定**／**ステータス**&#x200B;をクリックします。

1. システム全体（個別のグループを含む）のステータスを削除するには、ステータスの上にマウスを移動して、「**編集**」クリックし、「**すべてのグループに対してロック**」が選択されていることを確認します。「**保存**」をクリックします。

   または

   システムステータスを削除しても個別のグループに対して保持するには、ステータスの上にマウスを移動して、「**編集**」をクリックし、「**すべてのグループに対してロック**」が選択されていないことを確認します。「**保存**」をクリックします。

1. 削除するステータスの上にポインタを合わせて、「**削除**」をクリックします。
1. 表示されるメッセージで、「**ステータスを削除**」をクリックします。
1. 表示される&#x200B;**ステータスを削除**&#x200B;ボックスで、「**現在このステータスを持つすべてのプロジェクトを設定**」というラベルが付いたフィールドでステータスを選択します。

   削除するステータスを使用していたプロジェクトは、選択したステータスに設定されます。

   ステータスは、削除するステータスと同じステータスである場合にのみ、ドロップダウンリストで使用できます。

   例えば、「現在」と同じステータスを削除する場合、「現在」と同じステータスのみを選択できます。

1. 「**ステータスを削除**」をクリックします。
