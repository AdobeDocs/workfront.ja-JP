---
product-area: templates
navigation-topic: templates-navigation-topic
title: プロジェクトテンプレートの作成
description: テンプレートエリアからテンプレートを作成および削除できます。新しいテンプレートを作成するときは、すべてのタスクと、将来のプロジェクト設定についての情報を入力できます。この情報は、テンプレートから作成するプロジェクトに転送されます。
author: Alina
feature: Work Management
exl-id: 5094ba3f-3cb0-4301-aa7d-88c64d112b78
source-git-commit: 46133f435c665dd82d134f18d0b5de4e70bab7d7
workflow-type: tm+mt
source-wordcount: '654'
ht-degree: 58%

---

# プロジェクトテンプレートの作成

<!-- Audited: 10/2025 -->

テンプレートエリアからテンプレートを作成および削除できます。新しいテンプレートを作成するときは、すべてのタスクと、将来のプロジェクト設定についての情報を入力できます。この情報は、テンプレートから作成するプロジェクトに転送されます。

>[!NOTE]
>
>テンプレートとそのタスクには実際の日付はありませんが、タスクが開始される可能性がある日（将来のプロジェクトが開始される可能性がある日）と、タスクを完了する必要がある可能性の日を示します。テンプレートを使用して将来のプロジェクトを作成する場合、プロジェクトは実際の日付を受け取ります。詳しくは、[プロジェクトの作成](../create-projects/create-project.md)を参照してください。


次の方法で新しいテンプレートを作成できます。

* 最初から（この記事で説明）。
* 既存のプロジェクトから、プロジェクトをテンプレートとして保存。

  既存のプロジェクトからテンプレートを作成する方法について詳しくは、[プロジェクトをテンプレートとして保存](../../../manage-work/projects/manage-projects/save-project-as-template.md)を参照してください。

* 別のテンプレートからコピー。

  既存のテンプレートのコピーについて詳しくは、[プロジェクトテンプレートをコピー](../../../manage-work/projects/create-and-manage-templates/copy-template.md)を参照してください。

* ブループリントを読み込む。ブループリントを読み込むには、Workfront の管理者である必要があります。詳しくは、[ブループリントの設定](../../../administration-and-setup/blueprints/configure-template-package.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準 </p><p>プラン</p> <p>ブループリントからテンプレートを読み込むには、システム管理者である必要があります</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>テンプレートへの編集アクセス</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>デフォルトでは、作成したテンプレートに対する管理権限があります。</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>New: Standard </p><p>Or </p><p>Current: Plan </p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">You must be a system administrator to import templates from Blueprints</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>You have Manage permissions to the templates you create, by default</p>  </td> 
  </tr> 
 </tbody> 
</table>-->

## テンプレートの作成

{{step1-to-templates}}

1. 「**新規テンプレート**」をクリックします。

   テンプレートは名称未設定です。

   ![新規テンプレート](assets/create-template-nwe-2022-350x102.png)

1. テンプレートヘッダーで新しいテンプレートの名前を指定し、**Enter** キーを押します。
1. 左側のパネルで「**テンプレートタスク**」セクションをクリックします。
1. 「**テンプレートタスクの追加を開始**」をクリックして、タスクをインラインで追加します

   または

   「**新規テンプレートタスク**」をクリックして、「**新規テンプレートタスク**」ボックスでテンプレートへのタスクの追加を開始します。

   ![&#x200B; 新規テンプレート タスク ボックス &#x200B;](assets/new-template-task-box.png)

   <!--<span class="preview">The Create Template Task opens in the new experience.</span>-->

   <!--
   1. <span class="preview">(Conditional) Using the new experience, update information in the following areas in the **Create Template Task** box:</span>
   <div class="preview">
   * Template Task Name
   * Overview
   * Assignments
   * Finance
   * Custom Forms
   * Documents
   * Settings 
   </div>
   1. Click **Save**
   Or (*******remove the 1. from the step below and continue with those steps here*********)
   1. (Optional) Click **Switch back to old experience** at the bottom of the **Create Template Task** box.
   The **New Template Task** opens. (************add screen shot***********)-->

1. 「**新規テンプレートタスク**」ボックスの次の領域の情報を更新します。

   * 概要
   * 財務
   * 設定
   * 割り当て
   * カスタムフォーム
   * ドキュメントの添付

     テンプレートタスクの情報の更新は、プロジェクトのタスクの編集に似ています。 詳しくは、[&#x200B; タスクの編集 &#x200B;](/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md) を参照してください。<!--should this be relinked at preview/ prod release to say it's the same as Edit template tasks??-->

   >[!NOTE]
   >
   >繰り返しタスクをテンプレートに追加することはできません。

1. 次のいずれかをクリックします。

   * **テンプレートタスクを保存**：現在のテンプレートタスクを保存し、「新規テンプレートタスク」ボックスを閉じます。
   * **テンプレート タスクを保存して別のタスクを開始**：現在のテンプレート タスクを保存し、別のタスクを追加するために別の新しいテンプレート タスク ボックスを開きます。
   * **キャンセル**：テンプレートタスクを保存せずにボックスを閉じます。
1. （オプション）テンプレートタスクを追加した後、タスクリストの右上隅にある「テンプレートタスク」セクションで **ガントチャート** アイコンをクリックすると、テンプレートのタスクリストが視覚的に表示されます。

   >[!TIP]
   >
   >このガントチャートから直接タスクを編集することはできません。

1. 新しいテンプレートに情報を追加するには、ヘッダーのテンプレート名の左側にある **その他** メニュー ![&#x200B; その他アイコン &#x200B;](assets/more-icon.png) をクリックしてから、「**編集** をクリックします。

   テンプレートの編集について詳しくは、[プロジェクトテンプレートの編集](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)を参照してください。

   >[!NOTE]
   >
   >   プロジェクトテンプレートとグループの関連付け（またはグループの欠如）は、プロジェクト、タスク、イシューの環境設定によってテンプレートの特定の設定が決定される方法に影響します。
   >
   >詳しくは、「グループのプロジェクトテンプレートの作成と変更 [&#x200B; の記事の「環境設定がテンプレートとテンプレートタスクに適用される方法 &#x200B;](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-templates.md) を参照してください。

1. 「**保存**」をクリックします。
1. （オプション）次の項目をテンプレートに追加します

   * ドキュメント
   * リスク
   * 承認プロセス
   * 請求レート
   * 費用
   * キューの詳細
   * トピックグループとキューのトピック

1. （オプション）テンプレートのタスクに次の項目を追加します。

   * ドキュメント
   * 費用
   * 承認

   詳しくは、「プロジェクトテンプレートの編集 [&#x200B; の「テンプレートにさらに項目を追加する」の節を参照し &#x200B;](../../../manage-work/projects/create-and-manage-templates/edit-templates.md) ください。




