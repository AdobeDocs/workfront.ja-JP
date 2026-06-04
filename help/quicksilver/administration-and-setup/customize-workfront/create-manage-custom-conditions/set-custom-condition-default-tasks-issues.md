---
title: タスクとイシューのデフォルトとしてカスタム条件を設定する
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: ユーザーが「作業」をクリックしたとき、または割り当てられた新規タスクにアップデートコメントを追加したとき（タスクの状況を手動で設定せずに）、Adobe Workfront に（「設定」で指定された）タスクのデフォルトの条件が表示されます。 同じことがイシューにも当てはまります。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 40b426f4-0a9c-49a6-91c7-b5f8aa48bd37
TQID: https://experienceleague.adobe.com/1pmI09IkVMY3r4YIy4RjaIeUVsQvFNtlyYLxeT-fBII
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 350
ht-degree: 95%

---

# タスクとイシューのデフォルトとしてカスタム状況を設定

ユーザーが「作業」をクリックしたとき、または割り当てられた新規タスクにアップデートコメントを追加したとき（タスクの状況を手動で設定せずに）、Adobe Workfront に（「設定」で指定された）タスクのデフォルトの条件が表示されます。 同じことがイシューにも当てはまります。

Workfront は、ビルトインの状況「順調」をタスクのデフォルトの状況として使用し、別途、イシューのデフォルト条件として使用します。 Workfront の管理者は、これらの両方のオブジェクトタイプのデフォルトの条件を、作成したカスタム条件に変更できます。

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
   <td>システム管理者</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## カスタム状況をタスクとイシューのデフォルト状況として設定します。

{{step-1-to-setup}}

1. **プロジェクト環境設定**／**条件**&#x200B;をクリックします。

1. 「**タスク**」タブまたは「**イシュー**」タブをクリックします。

1. 「**デフォルト条件を設定**」をクリックします。
1. ドロップダウンメニューで、タスク（またはイシュー）のデフォルト状況として使用するカスタム状況をクリックします。
1. 「**保存**」をクリックします。

>[!NOTE]
>
>* タスクまたはイシューに割り当てられているユーザー、またはタスクまたはイシューに対する管理権限を持つユーザーは、手動で状況を変更できます。 詳しくは、[タスクおよびイシューの状況を更新](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md)を参照してください。
>* Workfront に伴うタスクとイシューの 3 つのデフォルト状況は、「順調」、「やや心配」、「深刻な障害」です。 これらの状況は、非表示に、または削除できませんが、名前と色は変更できます。 または、詳しくは、[カスタムフォームを作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)で説明されているように、新しいものを作成して代わりに使用することもできます。

カスタム状況をプロジェクトのデフォルト状況として設定する方法については、[カスタム状況をプロジェクトのデフォルトとして設定](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md)を参照してください。
