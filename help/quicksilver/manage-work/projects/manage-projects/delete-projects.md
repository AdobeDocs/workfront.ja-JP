---
title: プロジェクトの削除
product-area: projects
navigation-topic: manage-projects
description: プロジェクトとそのデータが不要になった場合は、プロジェクトを削除できます。プロジェクトを削除する代わりに、プロジェクトを編集して、ステータスを「完了」または「停止」に変更することをお勧めします。これにより、プロジェクトに関連する現在のタスクがユーザーのタスクリストからすべて削除されますが、プロジェクトに関連するすべてのデータは保存されます。
author: Alina
feature: Work Management
exl-id: a0e80c4d-29a8-4bf8-aa19-0c2d493236c6
recommendations: noDisplay, noCatalog
source-git-commit: ba5089fd02ca099d25ce0d3c2c2c039c2c6e2fe2
workflow-type: tm+mt
source-wordcount: '1067'
ht-degree: 79%

---

# プロジェクトの削除

<!--Audited: 07/2024-->

プロジェクトとそのデータが不要になった場合は、プロジェクトを削除できます。

プロジェクトを削除する代わりに、プロジェクトを編集して、ステータスを「完了」または「停止」に変更することをお勧めします。これにより、プロジェクトに関連する現在のタスクがユーザーのタスクリストからすべて削除されますが、プロジェクトに関連するすべてのデータは保存されます。

プロジェクトは、プロジェクトリストまたはプロジェクトレベルで削除できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront パッケージ</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront プラン</p> </td> 
   <td> <p>標準</p>
   <p>プラン</p> 
   </td> 
  </tr> 
    <td>アクセスレベル設定</td> 
   <td> <p>プロジェクトの作成とプロジェクトの削除が可能な編集アクセス権</p> </td> 
  </tr> 
    <td> <p>オブジェクト権限</p> </td> 
   <td> <p>プロジェクト、タスク、イシューに対する編集アクセス権（プロジェクト、タスク、イシューの削除が可能）</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>Adobe Workfront plan</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td> <p>Adobe Workfront license*</p> </td> 
   <td> <p>New license: Standard </p>
   <p>Current license: Plan </p> 
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level configuration</td> 
   <td> <p>Edit access to Projects with ability to Create and Delete projects</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>Edit access to Projects, Tasks, Issues with ability to Delete projects, tasks, and issues</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## プロジェクトを削除するプロセスについて

* [プロジェクトの削除に関する制限](#limitations-for-deleting-projects)
* [プロジェクトの削除による影響](#the-impact-of-deleting-projects)

### プロジェクトの削除に関する制限  {#limitations-for-deleting-projects}

* 削除された項目は 30 日間ごみ箱に移動され、復元することができるのは Workfront 管理者のみとなります。

  オブジェクトの復元について詳しくは、[削除したアイテムの復元](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)の記事を参照してください。

* 時間が記録されたタスクやイシューがプロジェクトに含まれている場合、これらのタスクを含むプロジェクトをユーザーが削除できるようにするには、Workfront 管理者またはグループ管理者は、Workfront インスタンスでタスクとイシューの環境設定を行うことで、これらのタスクの削除を許可する必要があります。

  時間が記録されたタスク、イシュー、プロジェクトの削除を有効にする方法について詳しくは、[システム全体のタスクとイシューの環境設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md)を参照してください。

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Quicksilver,QuicksilverOrClassic.Draft mode">(NOTE: this bullet stays in NWE only forever)</p>
  -->

### プロジェクトの削除による影響 {#the-impact-of-deleting-projects}

* プロジェクトを削除すると、そのプロジェクトにリンクされている他のオブジェクトに影響を与えます。

  プロジェクトを削除すると、プロジェクトに添付されている次のオブジェクトも削除されます。

   * ドキュメント

     チェックアウトされた添付ドキュメントが含まれるプロジェクトは削除できません。ドキュメントのチェックアウトについて詳しくは、[ドキュメントのチェックアウト](../../../documents/managing-documents/check-out-documents.md)を参照してください。

   * タスク
   * サブタスク
   * イシュー
   * アップデート
   * 承認
   * 費用
   * リスク
   * ベースライン
   * ビジネスケースの情報
   * キューの詳細情報
   * 請求レート
   * 請求記録

     ステータスが「請求済み」になっている請求記録を含んだプロジェクトは削除できません。詳しくは、[請求記録を作成](../../projects/project-finances/create-billing-records.md)を参照してください。

* Workfront インスタンスのタイムシートおよび時間の環境設定で Workfront 管理者が指定したプロジェクトや、タスク、イシューの削除に関する環境設定に応じて、タスク、イシュー、またはプロジェクトに記録される時間は、タスクを削除する際に次のいずれかの方法で処理されます。

   * 時間は、タイムシートに一般的な時間として残されます。
   * 時間は削除され、今後プロジェクトが復元された場合に時間も復元されます。

  イシューに時間が記録されている場合の削除の環境設定について詳しくは、[タイムシートおよび時間の環境設定を指定](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)を参照してください。

* 削除したプロジェクトが Workfront シナリオプランナーのイニシアチブにリンクされている場合は、次の方法で処理されます。

   * イニシアチブは計画に残されますが、プロジェクトへのリンクは削除されます。
   * 削除したプロジェクトが計画の唯一の公開イニシアチブにリンクされている場合は、計画が公開されたことを示す指標も削除されます。
   * 削除したプロジェクトを復元すると、そのプロジェクトは復元されますが、イニシアチブへのリンクは復元されず、シナリオプランナーのエリアは「プロジェクト詳細」に表示されなくなります。

     シナリオプランナには、追加のライセンスが必要です。Workfront シナリオプランナについては、[シナリオプランナの概要](../../../scenario-planner/scenario-planner-overview.md)を参照してください。

     シナリオプランナーのイニシアチブにリンクされたプロジェクトについて詳しくは、[シナリオプランナーでイニシアチブを公開して、プロジェクトをアップデートまたは作成](../../../scenario-planner/publish-scenarios-update-projects.md)を参照してください

* プロジェクトが Workfront Goals の目標のためのアクティビティでもある場合、以下のようになります。

   * 目標からプロジェクトが削除されます。プロジェクトによって目標に示された進捗状況も削除されます。

   * 削除したプロジェクトを復元すると、そのプロジェクトも目標のアクティビティとして復元されます。

     追加のライセンスが必要です。Workfront Goals について詳しくは、[Adobe Workfront Goals の概要](../../../workfront-goals/goal-management/wf-goals-overview.md)を参照してください。

     プロジェクトを目標に関連付ける方法について詳しくは、[Adobe Workfront Goals の目標にプロジェクトを追加](../../../workfront-goals/results-and-activities/connect-projects-to-goals-overview.md)を参照してください。

## リスト内のプロジェクトを削除

プロジェクトのリストからプロジェクトを削除できます。

1. プロジェクトのリストまたはプロジェクトレポートに移動します。
1. 削除するプロジェクト（1 つまたは複数）を選択し、リストの上部にある **削除** アイコン ![ 削除アイコン ](assets/delete-icon.png) をクリックします。

1. クリック「**はい、削除します**」をクリックして削除を確定します。

   プロジェクトが削除され、30 日間ごみ箱に保存されます。この間に Workfront 管理者が、削除されたプロジェクトをごみ箱から復元することができます。

## プロジェクトレベルでプロジェクトを削除

1. 削除するプロジェクトに移動します。
1. プロジェクト名の右側にある **その他** アイコン ![ その他メニュー ](assets/qs-more-menu.png) をクリックし、**プロジェクトを削除** をクリックします。

   ![ 詳細メニューが展開されました ](assets/more-icon-expanded-delete-project-highlighted.png)

1. 「**はい、削除します**」をクリックします。

   プロジェクトが削除され、30 日間ごみ箱に保存されます。この間 Workfront 管理者が、削除されたプロジェクトをごみ箱から復元することができます。

## Workfront Planning レコードの接続されたレコード ページからプロジェクトを削除します

>[!NOTE]
>
>この節では、Adobe Workfrontの追加機能であるAdobe Workfront Planning について説明します。
>
>Adobe Workfront Planning にアクセスするための要件の一覧については、[Workfront Planning アクセスの概要 ](/help/quicksilver/planning/access/access-overview.md) を参照してください。
> 
>Adobe Workfront Planning の一般情報については、[Workfront Planning の基本を学ぶ ](/help/quicksilver/planning/general/planning-overview.md) を参照してください。

Workfront Planning の接続されたレコード ページからプロジェクトにアクセスして削除するには、次のものが必要です：

* Workfront プロジェクトに接続された計画レコードタイプ。 詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。
* 計画レコード。 詳しくは、[レコードの作成](/help/quicksilver/planning/records/create-records.md)を参照してください。
* 計画レコードに接続されているプロジェクトを表示する、接続されているレコード ページ。 詳しくは、[ 接続されたレコードページのレコードへの追加 ](/help/quicksilver/planning/records/add-a-connected-records-page-to-a-record.md) を参照してください。

接続されたレコードページからレコードを削除するには：

1. レコードに接続されたプロジェクトを表示する「接続されたレコード」ページで、プロジェクトの名前にポインタを合わせて **詳細** アイコン ![ 詳細アイコン ](assets/more-icon.png) をクリックします。

   または

   リストで 1 つまたは複数のプロジェクトを選択します。 プロジェクトリストの下部に青いバーが表示されます。

1. **削除** をクリックし、**削除** をクリックして確定します。

   プロジェクトが削除され、Workfrontのごみ箱に入れられます。

## 削除されたプロジェクトの復元

システム管理者またはグループ管理者は、[削除した項目を復元](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)の記事の説明に従って、削除後 30 日以内に削除されたプロジェクトを復元できます。
