---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: manage-group-statuses
title: グループステータスの削除
description: グループ管理者は、自分が管理するグループのステータスが、システムレベルまたは階層内の上位グループで必須ステータスまたはロックステータスとして設定されていない場合、そのステータスを削除できます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: bfce0325-fe6e-459f-96ca-9a5c94c61ed3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '572'
ht-degree: 100%

---

# グループステータスの削除

グループ管理者は、自分が管理するグループのステータスが、システムレベルまたは階層内の上位グループで必須ステータスまたはロックステータスとして設定されていない場合、そのステータスを削除できます。

管理するグループ上にグループがある場合は、その管理者がグループに対してこの操作を行うこともできます。Workfront 管理者（すべてのグループ）も同様です。

>[!NOTE]
>
>以下のものは削除できません。
>
>* 組み込みステータスは、計画、現在、および完了です。名前の更新、色の編集、ロックまたはロック解除は可能ですが、削除することはできません。
>* グループに関連付けられた 1 つ以上のオブジェクトまたはそのサブグループの 1 つに対して、承認待ち状態のステータス。

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

&#42;ご利用のプランまたはライセンスタイプを確認する必要がある場合は、Workfront 管理者にお問い合わせください。

## グループステータスの削除

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックして、**設定** ![](assets/gear-icon-settings.png) をクリックします。

1. 左側のパネルで、「**グループ**」をクリックします。
1. 最上位グループの名前をクリックします。
1. 左側のパネルで、「**ステータス**」をクリックします。
1. 表示されるステータスのリストで、削除するステータスの上にポインタを合わせ、右端に表示されたら「**削除**」をクリックします。

   ![](assets/hover-click-delete.jpg)

1. 表示されるボックスで、ステータスを選択して、削除するステータスを使用していたオブジェクト（プロジェクト、タスク、イシュー、承認プロセス）の置き換えステータスを指定します。

   削除しようとしているステータスに等しいステータスのみを使用できます。例えば、現在と同等のステータスを削除する場合は、現在と同等のステータスのみが表示されます。

   また、表示されるステータスは、削除するステータスのロックが解除されているかロックされているかによって異なります。

   * **ロックが解除されている場合**：非表示のロック済みステータスとロック解除済みステータスを使用できます。

     サブグループに対して作成されたステータスとともに、システムレベルと上位レベルのグループから継承されたステータスも含まれます。

   * **ロックされている場合**：次のいずれかが該当します。

      * 他にロックされた非表示でないステータスがある場合は、それらのステータスのみが使用可能です。
      * ロックされた非表示でないステータスがない場合は、非表示またはロック解除されている場合でも、デフォルトの Workfront ステータスを使用できます。

        デフォルトの Workfront のステータスについて詳しくは、[システムプロジェクトステータスのリストへのアクセス](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/project-statuses.md)、[システムタスクステータスのリストへのアクセス](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/task-statuses.md)、および[システムのイシューステータスのリストへのアクセス](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/issue-statuses.md)の 4 つの必須のイシューステータスに関する情報を参照してください。

1. 「**ステータスを削除**」をクリックします。

   削除済みステータスがグループ内のそのタイプのデフォルトステータスの場合は、置き換えステータスがその代わりに使用されます。

   削除済みのステータスがプロジェクト環境設定でデフォルトのプロジェクトステータスに設定された場合、環境設定は置き換えステータスに設定されます。

## グループが削除された場合

グループが削除され、別のグループに置き換えられると、削除されたグループが持っていた固有のステータスが、置き換えグループのステータスに追加されます。詳しくは、[移動または削除されたグループのカスタムステータス](../../../administration-and-setup/manage-groups/manage-group-statuses/custom-statuses-in-group-moved-or-deleted.md)を参照してください。
