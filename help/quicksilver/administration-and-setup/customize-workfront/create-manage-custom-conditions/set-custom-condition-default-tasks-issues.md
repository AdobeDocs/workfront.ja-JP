---
title: タスクおよび問題の既定としてカスタム条件を設定する
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: ユーザーが「作業」をクリックしたとき、または割り当てられた新規タスクにアップデートコメントを追加したとき（タスクの状況を手動で設定せずに）、Adobe Workfront に（「設定」で指定された）タスクのデフォルトの条件が表示されます。同じことがイシューにも当てはまります。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 40b426f4-0a9c-49a6-91c7-b5f8aa48bd37
source-git-commit: a54200ceeaadfeaac6767f06676cb11814959601
workflow-type: tm+mt
source-wordcount: '403'
ht-degree: 94%

---

# タスクとイシューのデフォルトとしてカスタム状況を設定

ユーザーが「作業」をクリックしたとき、または割り当てられた新規タスクにアップデートコメントを追加したとき（タスクの状況を手動で設定せずに）、Adobe Workfront に（「設定」で指定された）タスクのデフォルトの条件が表示されます。同じことがイシューにも当てはまります。

Workfront は、組み込みの状況「順調」をタスクのデフォルトの状況として使用し、別途、イシューのデフォルト条件として使用します。Workfront の管理者は、これらの両方のオブジェクトタイプのデフォルトの条件を、作成したカスタム条件に変更できます。

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
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## カスタム状況をタスクとイシューのデフォルト状況として設定します。

{{step-1-to-setup}}

1. **プロジェクト環境設定**／**条件**&#x200B;をクリックします。

1. 「**タスク**」タブまたは「**イシュー**」タブをクリックします。

1. 「**デフォルトの条件をセット**」をクリックします。
1. ドロップダウンメニューで、タスク（またはイシュー）のデフォルト状況として使用するカスタム状況をクリックします。
1. 「**保存**」をクリックします。

>[!NOTE]
>
>* タスクまたはイシューに割り当てられているユーザー、またはタスクまたはイシューに対する管理権限を持つユーザーは、手動で状況を変更できます。詳しくは、[タスクおよびイシューの状況を更新](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md)を参照してください。
>* Workfront に伴うタスクとイシューの 3 つのデフォルト状況は、「順調」、「やや心配」、「深刻な障害」です。これらの状況は、非表示に、または削除できませんが、名前と色は変更できます。または、詳しくは、[カスタムフォームを作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)で説明されているように、新しいものを作成して代わりに使用することもできます。
>

カスタム状況をプロジェクトのデフォルト状況として設定する方法については、[カスタム状況をプロジェクトのデフォルトとして設定](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md)を参照してください。

カスタム状況について詳しくは、[カスタム状況](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md)を参照してください。
