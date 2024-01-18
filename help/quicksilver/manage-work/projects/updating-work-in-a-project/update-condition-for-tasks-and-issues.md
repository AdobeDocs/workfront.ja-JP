---
product-area: projects
navigation-topic: update-work-in-a-project
title: タスクおよび問題の条件を更新
description: タスクまたはイシューの条件は、タスクの進行状況を示すフラグがタスクまたはイシューに設定されます。 これは、作業項目の現在の開発段階を示す作業項目のステータスとは異なります。
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 0%

---

# タスクおよび問題の条件を更新

タスクまたはイシューの条件は、タスクの進行状況を示すフラグがタスクまたはイシューに設定されます。 これは、作業項目の現在の開発段階を示す作業項目のステータスとは異なります。

タスクまたはイシューの条件は、自動または手動で設定できます。

Adobe Workfront管理者は、 [カスタム条件の作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)

<!--You can manually update the Condition of a task or issue if you are assigned to it or if you have permissions to it, as described in the [Access requirements](#access-requirements) section of this article.-->

## アクセス要件 {#access-requirements}

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>

新しいライセンスの場合：
<ul><li><p>タスクの標準</p></li>
   <li><p>問題の寄稿者以上</p></li></ul>


現在のライセンスの場合：
<ul><li><p>タスクに関する作業以上</p></li>
   <li><p>問題に対するリクエスト以上</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトへの表示またはアクセス権の高さ</p> <p>タスクおよび問題へのアクセスを編集 </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>タスクおよびタスクの条件を表示するタスクに対する権限を表示または上限に設定します</p>
   <p>条件を更新するためのタスクおよび問題に関する権限を管理します</p>
  </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。 詳しくは、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## タスクと問題の条件を見つける

条件は、タスクまたは問題に関連付けられたフラグとして表示されます。 また、ラベルの代わりにレポートに表示できる数値に関連付けることもできます。 条件と数値の関連付けの詳細については、「 [カスタム条件の作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

タスクの条件と問題は、次の領域で確認できます。

* タスクまたはイシューに割り当てられた場合の、更新内のタスクおよびイシューの更新領域。 これは、新しいコメントエクスペリエンスではサポートされていません。 詳しくは、 [新しいコメントエクスペリエンス](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md).
* レポートとリストは、ビューまたはグループの「条件」フィールドを表示する際に使用されます。

>[!NOTE]
>
>ジャーナルエントリレポートの「フィールド名」フィールドに「条件」という単語が表示される場合は、アイテムの条件が更新されたことを示します。 仕訳レポートで「条件」フィールドが追跡される場合、新旧の数値には、名前ではなく、条件に関連付けられた数値が表示されます。 タスクまたはイシューに対して条件が最初に定義されていない状態で、後でその条件を更新した場合、更新を取り込むジャーナルエントリには、「条件」フィールドの「古い番号」の値が —2,147,483,648 と表示されます。

## ステータスを更新して条件を自動的に更新

タスクまたはタスクを割り当てられ、「 **作業する** 、タスクを開始またはタスクを開始またはステータスを更新すると、タスクまたはタスクの条件は、 **スムーズに進む**.

カスタム条件をデフォルトの条件として使用する方法については、  [タスクとタスクのデフォルトとしてカスタム条件を設定する](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md) および [カスタム条件をプロジェクトのデフォルトとして設定する](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md).

タスクのステータスの変更について詳しくは、 [タスクステータスを更新](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md).

問題ステータスの変更について詳しくは、 [問題ステータスを更新](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md).

[ 作業開始 ] ボタンを [ タスクの開始 ] または [ タスクの開始 ] ボタンに設定する方法については、 [「作業対象」ボタンを「開始」ボタンに置き換えます](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).

## 手動での条件の更新

条件を設定するには、タスクまたはタスクに割り当てられているか、タスクに対する管理権限が必要です。

ビューに「条件」フィールドを表示するときに、タスクまたはタスクまたはイシューのタスクまたはイシューの条件を手動で更新することができます。


<!--old Condition update - in the commenting stream: 
Updating the Condition of a task or issue differs depending on whether you are assigned to it or not:

* If you are using the legacy commenting experience, you can update the Condition in the Updates tab or in a list of tasks or issues if you are assigned to them. This is not supported in the new commenting experience. For information, see [New commenting experience](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
* You can update the Condition in a list of tasks or issues if you are not assigned to them, only if you have Manage permissions to them. In this case, you cannot update the Condition in the Update tab of the task or issue. -->

タスクまたはイシューの条件を手動で更新するには、次の手順に従います。

1. 管理権限を持つタスクまたは問題の一覧に移動します。 次を確認します。 **条件** フィールドがリストの表示に表示されます。

1. を更新します。 **条件** イシューまたはタスクをインラインで表示する場合は、既存の条件をダブルクリックし、ドロップダウンメニューから新しい値を選択します。

   ![](assets/condition-drop-down-values-in-task-list.png)

   >[!NOTE]
   >
   >条件は、お使いの環境に合わせてカスタマイズできるので、お使いの環境で条件に対して 3 つ以上のオプションを検索できます。 条件の名前は、上記の名前とは異なる場合があります。 Workfrontの条件のカスタマイズについて詳しくは、 [カスタム条件の作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).


1. 押す **入力** キーボードでクリックするか、[ 条件 ] フィールドの外側をクリックして、新しいタスクまたは問題の条件を保存します。

   <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md" class="MCXref xref">Views overview in Adobe Workfront</a>.</p></li>   
     -->
