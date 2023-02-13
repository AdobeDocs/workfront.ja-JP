---
title: タスクとタスクのデフォルトとしてカスタム条件を設定
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: ユーザーが「作業」をクリックしたとき、または割り当てられた新しいタスクに更新コメントを追加したとき（タスクの条件を手動で設定せずに）、Adobe Workfrontにタスクのデフォルトの条件が表示されます（セットアップで設定）。 同じことが問題にも当てはまります。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 40b426f4-0a9c-49a6-91c7-b5f8aa48bd37
source-git-commit: a3cb3d9d340d377e301c98480324bfe8bf507382
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# タスクとタスクのデフォルトとしてカスタム条件を設定

ユーザーが「作業」をクリックしたとき、または割り当てられた新しいタスクに更新コメントを追加したとき（タスクの条件を手動で設定せずに）、Adobe Workfrontにタスクのデフォルトの条件が表示されます（セットアップで設定）。 同じことが問題にも当てはまります。

Workfrontは、組み込みの条件 Going Smousle をタスクのデフォルト条件として使用し、別途、問題のデフォルト条件として使用します。 Workfrontの管理者は、これらの両方のオブジェクトタイプのデフォルトの条件を、作成したカスタム条件に変更できます。

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

## タスクまたは問題のデフォルト条件としてカスタム条件を設定します。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **プロジェクト環境設定** > **条件**.

1. 次をクリック： **タスク** または **問題** タブをクリックします。

1. クリック **デフォルト条件の設定**.
1. ドロップダウンメニューで、タスク（またはタスク）のデフォルト条件として使用するカスタム条件をクリックします。
1. 「**保存**」をクリックします。

>[!NOTE]
>
>* タスクまたはイシューに割り当てられているユーザー、またはタスクまたはイシューに対する管理権限を持つユーザーは、手動で条件を変更できます。 詳しくは、 [タスクおよび問題の条件を更新](../../../manage-work/projects/updating-work-in-a-project/update-condition-for-tasks-and-issues.md).
>* Workfrontに付属するタスクと問題に関する 3 つのデフォルト条件は、スムーズに進むこと、いくつかの懸念事項、主要な障害要因です。 これらの条件は、非表示または削除できませんが、名前と色は変更できます。 または、新しいものを作成して代わりに使用することもできます。詳しくは、 [カスタム条件の作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).
>


カスタム条件をプロジェクトのデフォルト条件として設定する方法については、 [カスタム条件をプロジェクトのデフォルトとして設定する](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

カスタム条件について詳しくは、 [カスタム条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
