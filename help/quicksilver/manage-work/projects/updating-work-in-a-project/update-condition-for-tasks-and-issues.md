---
product-area: projects
navigation-topic: update-work-in-a-project
title: タスクおよびイシューの条件の更新
description: タスクまたはイシューの状況は、進行状況を示すために配置されたフラグです。これは、作業項目の現在の開発段階を示す作業項目のステータスとは異なります。
author: Alina
feature: Work Management
exl-id: 5d970af6-5996-4781-9b97-de02063dc32c
source-git-commit: ac5e56a2881d589c9a737d5e7115d82ee5c11ea6
workflow-type: tm+mt
source-wordcount: '1095'
ht-degree: 67%

---

# タスクおよびイシューの条件の更新

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべての顧客に対してプレビュー環境でのみ使用できるか、または迅速リリースを有効にした顧客の実稼動環境でのみ使用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

<span class="preview"> 現在のリリースについて詳しくは、[2024 年第 3 四半期リリースの概要 ](/help/quicksilver/product-announcements/product-releases/24-q3-release-activity/24-q3-release-overview.md) を参照してください。</span>

タスクまたはイシューの状況は、進行状況を示すために配置されたフラグです。これは、作業項目の現在の開発段階を示す作業項目のステータスとは異なります。

タスクまたはイシューの状況は、自動または手動で設定できます。

この記事で参照する条件値は、デフォルトでWorkfrontで使用できます。 [ カスタム条件の作成または編集 ](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md) で説明されているように、Adobe Workfront管理者が環境のカスタム条件を作成できます。

## アクセス要件 {#access-requirements}

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td>

新しいライセンスの場合：
<ul><li><p>タスクの標準</p></li>
   <li><p>イシューの場合は Contributor 以上</p></li></ul>


現在のライセンスの場合：
<ul><li><p>タスクの場合はワーク以上</p></li>
   <li><p>イシューの場合はリクエスト以上</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトに対する表示以上のアクセス権</p> <p>タスクおよびイシューに対する編集アクセス権 </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>状況を表示するための、タスクおよびイシューに対する表示以上の権限</p>
   <p>状況を更新するための、タスクおよびイシューに対する管理権限</p>
  </td> 
  </tr> 
 </tbody> 
</table>

*ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## 前提条件

手動で条件を更新するには、タスクまたは問題に割り当てられている必要があります。

## タスクおよびイシューの状況を見つける

状況は、タスクまたはイシューに関連付けられたフラグとして表示されます。また、ラベルの代わりにレポートに表示できる数値に関連付けることもできます。状況と数値の関連付けについて詳しくは、[カスタム状況の作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)を参照してください。

タスクとイシューの条件は、Workfrontの次の領域で見つけることができます。

* <span class="preview">Workfront管理者またはグループ管理者がレイアウトテンプレートに追加した後の詳細ページ。 詳しくは、[ レイアウトテンプレートを使用した詳細ビューのカスタマイズ ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md) を参照してください。</span>

* <span class="preview">Workfront管理者またはグループ管理者がレイアウトテンプレートに追加した後のタスクまたはイシューのヘッダー。 詳しくは、[ レイアウトテンプレートを使用したオブジェクトヘッダーのカスタマイズ ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md) を参照してください。</span>

* Workfront管理者またはグループ管理者がレイアウトテンプレートに概要パネルを追加した後。 詳しくは [ レイアウトテンプレートを使用したホームと概要のカスタマイズ ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md) を参照してください。

* ビューまたはグループ化で「状況」フィールドを表示する場合は、レポートおよびリスト。

  >[!NOTE]
  >
  >ジャーナルエントリレポートの「フィールド名」フィールドに「状況」という単語が表示される場合は、項目の状況が更新されたことを示します。ジャーナルエントリレポートで「状況」フィールドが追跡されると、新旧の数値には、名前ではなく状況に関連付けられた数値が表示されます。タスクまたはイシューに対して状況がもともと定義されていない状態で、後でその状況を更新した場合、更新を取り込むジャーナルエントリには、「状況」フィールドの「古い数値」が -2,147,483,648 と表示されます。

## ステータスを更新して状況を自動的に更新

タスクまたはイシューが割り当てられたときに「**作業をする**」、「タスクを開始」または「イシューの取り組みを開始」をクリックするか、そのステータスを更新すると、タスクまたはイシューの状況は、**順調**&#x200B;に関連付けられているデフォルトの状況に自動的に変更されます。

カスタム状況をデフォルトの状況として使用することについて詳しくは、[カスタム状況をタスクとイシューのデフォルトとして設定](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-tasks-issues.md)および[カスタム状況をプロジェクトのデフォルトとして設定](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/set-custom-condition-default-projects.md)の記事を参照してください。

タスクのステータスの変更について詳しくは、[タスクのステータスを更新](../../../manage-work/projects/updating-work-in-a-project/update-task-status.md)を参照してください。

イシューのステータスの変更について詳しくは、[イシューのステータスを更新](../../../manage-work/projects/updating-work-in-a-project/update-issue-status.md)を参照してください。

「作業をする」ボタンを「タスクを開始」または「イシューの取り組みを開始」ボタンに設定する方法について詳しくは、[「作業をする」ボタンを「開始」ボタンに置き換え](../../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md)を参照してください。

## 状況を手動で更新

状況を設定するには、タスクまたはイシューに割り当てられているか、タスクまたはイシューに対する管理権限を持っている必要があります。

ビューに「条件」フィールドを表示するときに、タスクまたはイシューのレポートまたはリストで、タスクまたはイシューの条件を手動で更新できます。

>[!NOTE]
>
>システム管理者またはグループ管理者に依頼して、概要パネルに条件フィールドを追加してもらい、Workfrontの様々な領域で更新しやすくすることができます。
>
>詳しくは、次の記事を参照してください。
>
>* [ 概要 ](/help/quicksilver/workfront-basics/the-new-workfront-experience/summary-overview.md)
>* [ レイアウトテンプレートを使用してホームと概要をカスタマイズする ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)。


<!--old Condition update - in the commenting stream: 
Updating the Condition of a task or issue differs depending on whether you are assigned to it or not:

* If you are using the legacy commenting experience, you can update the Condition in the Updates tab or in a list of tasks or issues if you are assigned to them. This is not supported in the new commenting experience. For information, see [New commenting experience](/help/quicksilver/product-announcements/betas/new-commenting-experience-beta/unified-commenting-experience.md). 
* You can update the Condition in a list of tasks or issues if you are not assigned to them, only if you have Manage permissions to them. In this case, you cannot update the Condition in the Update tab of the task or issue. -->

タスクまたは問題の条件を手動で更新するには、次のいずれかを行います。

<div class="preview">

1. タスクまたは問題ヘッダーでタスクまたは問題の条件を更新するには：

   1. （条件付き）Workfrontまたはグループ管理者がレイアウトテンプレートのタスクまたはイシューヘッダーに「条件」フィールドを追加した場合は、ヘッダーの **条件** フィールドをクリックして、次のオプションから選択します。
      * 順調
      * やや心配
      * 深刻な障害

      ![](assets/condition-in-task-header.png)
   1. 「Enter」をクリックして、条件を保存します。

1. 「タスクまたは問題の詳細」セクションでタスクまたは問題の条件を更新するには：

   1. （条件付き）Workfrontまたはグループ管理者が、レイアウトテンプレートのタスクまたは問題の「詳細」セクションに「条件」フィールドを追加した場合は、左側のパネルで **「詳細**」をクリックし、**タスク条件** または **問題条件** をクリックして、次のオプションから選択します。
      * 順調
      * やや心配
      * 深刻な障害
1. 「**変更を保存**」をクリックします。タスクまたは問題の条件が更新されます。

</div>

レポートまたはリスト内のタスクまたは問題の条件を更新するには：

1. 管理権限のあるタスクまたはイシューのリストに移動します。「**条件**」フィールドがリストのビューに表示されていることを確認します。

1. 既存の条件をダブルクリックし、ドロップダウンメニューから新しい値を選択して、イシューまたはタスクの&#x200B;**条件**&#x200B;をインラインで更新します。

   ![](assets/condition-drop-down-values-in-task-list.png)

   >[!NOTE]
   >
   >状況は環境に合わせてカスタマイズできるので、お使いの環境で状況の選択肢が 4 つ以上ある場合もあります。状況の名前は、上記の名前とは異なる場合があります。Workfront での状況のカスタマイズについては、[カスタム状況の作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)を参照してください。


1. キーボードの **Enter** キーを押すか、「条件」フィールドの外側をクリックして、新しいタスクまたはイシューの条件を保存します。

<!--   
<li><p>(NOTE: drafted because I can't do this anymore)</p><p>If you have Manage permissions to the task or issue but are not assigned to it, perhaps as a project manager, add the <strong>Condition</strong> column to any view you use in a task or issue list, then set the <strong>Condition</strong> in inline edit and press Enter.</p><p><img src="assets/change-condition-in-list-view-350x142.png" style="width: 350;height: 142;"></p><p>For information about adding a column to a view, see <a href="../../../reports-and-dashboards/reports/reporting-elements/views-overview.md">Views overview in Adobe Workfront</a>.</p></li>   
     -->


