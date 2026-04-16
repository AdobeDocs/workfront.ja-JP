---
product-area: projects
navigation-topic: manage-tasks
title: タスク詳細セクションでのタスクの財務の管理
description: タスクの財務情報を表示または編集するには、「タスクの詳細」セクションの「概要」領域にアクセスします。 タスクの詳細セクションで表示または編集できるフィールドの数は限られています。
author: Alina
feature: Work Management
exl-id: 54ae48e5-bc8c-4e90-8fa1-0015523df4e6
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 39630b50384d710dadb1f48342113b74338a9104
workflow-type: tm+mt
source-wordcount: '987'
ht-degree: 68%

---

# タスクの詳細セクションでのタスクの財政の管理

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, to it in both articles)</p>
-->

タスクの財務情報を表示または編集するには、「タスクの詳細」セクションの「概要」領域にアクセスします。 この領域で表示または編集できるフィールドの数は限られています。

タスクのすべての財務情報の編集について詳しくは、[&#x200B; タスクの編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>ユーザーおよび役割の時間別収益タイプとコストタイプを使用し、残業率を追加するには：Workflow Ultimate</p>
      <p>その他のすべての設定を編集し、その他のすべての収益タイプとコストタイプを使用するには：任意のWorkfrontまたはワークフローパッケージ</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>標準</p> 
   <p>Work またはそれ以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトとタスクへのアクセス権を編集</p> <p>財務データ以降へのアクセスを表示</p> <p>タスクの財務情報を編集するには、財務データへの編集アクセス権が必要です</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>財務の表示権限以上を含むタスクの表示権限</p> <p>タスクに関する財務情報を編集するには、財務の編集を含むタスクに対する管理権限が必要です</p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--
Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects and Tasks</p> <p>View access to Financial Data or higher</p> <p>You must have Edit access to Financial Data to edit financial information on tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the task that include View Finance or higher</p> <p>You must have Manage permissions on the task that include Edit Finance to edit financial information on tasks</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## 「タスクの詳細」セクションでのタスクの財務の編集

1. タスクを表示するプロジェクトに移動します。

   >[!NOTE]
   >
   >タスクにアクセスするには、タスクを検索して名前をクリックします。Workfront でのオブジェクトの検索について詳しくは、[Adobe Workfront の検索](../../../workfront-basics/navigate-workfront/search/search-workfront.md)を参照してください。

1. 左パネルの「**タスク**」をクリックします。
1. 表示するタスクの名前をクリックします。
1. 「**タスクの詳細**」をクリックします。
1. （オプション）タスクの詳細ページの右上にある「**すべて折りたたむ**」アイコンをクリックします。

   ![詳細ページのすべてのアイコンを折りたたむ](assets/collapse-all-icon-on-details-page.png)

   >[!NOTE]
   >
   >Workfront 管理者またはグループ管理者がレイアウトテンプレートを設定する方法によっては、「タスクの詳細」セクションのフィールドが再配置されるか、表示されない場合があります。詳しくは、[レイアウトテンプレートを使用した詳細ビューのカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)を参照してください。

1. 「**財務**」をクリックして展開し、タスクの財務情報を表示します。

   詳細セクションの右上隅にある&#x200B;**編集** アイコン ![編集アイコン &#x200B;](assets/edit-icon.png)をクリックし、**財務**&#x200B;をクリックします。

1. 編集可能なフィールドをシングルクリックして編集するか、「**+ 追加**」をクリックして空のフィールドに情報を追加します。
1. **Finance**&#x200B;領域で次の情報を確認または編集します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">コストタイプ</td> 
      <td> <p>タスクのコストタイプを指定します。これにより、タスクの時間数に基づいて、タスクのコストの計算方法が決まります。 </p> <p>次のオプションから選択します。 </p> 
       <ul> 
        <li> <p>コストなし</p> </li> 
        <li> <p>固定 (毎時) </p> </li> 
        <li> <p> ユーザー (毎時) </p> </li> 
        <li> <p> 役割（毎時）</p> </li> 
        <li> <p>ユーザーと役割 (毎時)</p> </li> 
       </ul> <p>コストの追跡について詳しくは、<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a>を参照してください。システムまたはグループのタスクに対するデフォルトのコストタイプ設定は、Workfront 管理者またはグループ管理者が選択します。プロジェクトのデフォルトの設定については、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクトの環境設定の指定</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">収益タイプ</td> 
      <td> <p>タスクの収益タイプを指定します。これにより、タスクの時間数に基づいて、タスクの収益の計算方法が決まります。 </p> <p>次のオプションから選択します。 </p> 
       <ul> 
        <li> <p> 請求不可 </p> </li> 
        <li> <p>ユーザー (毎時) </p> </li> 
        <li> <p>役割（毎時） </p> </li> 
        <li> <p>ユーザーと役割 (毎時)</p> </li>
        <li> <p>固定 (毎時) </p> </li> 
        <li> <p>ユーザー (毎時) (キャップ付き) </p> </li> 
        <li> <p>役割（毎時）（キャップ付き） </p> </li>
        <li> <p>キャップ付きのユーザーと役割の時間単位</p> </li> 
        <li> <p>ユーザー（毎時）+ 固定 </p> </li> 
        <li> <p>役割（毎時）+ 固定 </p> </li> 
        <li> <p>ユーザーと役割 (毎時) + 固定</p> </li>
        <li> <p>固定収益 </p> </li> 
       </ul> <p>収益のトラッキングについて詳しくは、<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">請求と収益の概要</a>および<a href="/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md">収益とコスト階層の概要</a>を参照してください。 </p> <p>システムまたはグループのタスクに対する収益タイプのデフォルト設定は、Workfront 管理者またはグループ管理者が選択します。プロジェクトのデフォルトの設定については、<a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクトの環境設定の指定</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">予定コスト</td> 
      <td> <p>ユーザーまたは担当業務の時間単価、予定時間数、コストタイプに基づいて、タスクのコストが算出されます。コストの追跡について詳しくは、<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a>を参照してください。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">実際のコスト</td> 
      <td> <p> ユーザーまたは担当業務の時間単価、実際の時間数、コストタイプに基づいてタスクのコストが算出されます。コストの追跡について詳しくは、<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">予定収益</td> 
      <td> <p>ユーザーまたは担当業務の時間単価、予定時間数、収益タイプに基づいて、タスクに関連する収益が算出されます。コストの追跡について詳しくは、 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">実収益</td> 
      <td> <p>ユーザーまたは担当業務の時間単価、実際の時間、収益タイプに基づいて、タスクに関連付けられた収益が算されます。コストの追跡について詳しくは、 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a>を参照してください。</p> </td> 
     </tr> 
     <tr>
      <td>時間外労働率</td> 
      <td><p>タスクの残業乗数（1.5または2.0など）を入力します。デフォルトは1.0 （乗数なし）です。 詳しくは、<a href="/help/quicksilver/manage-work/projects/project-finances/define-overtime-ratio.md">残業率の定義</a>を参照してください。</p><p>「残業率」フィールドを表示するには、次の手順を実行します。</p>
       <ul>
       <li>タスクの収益タイプは、ユーザーと役割の時間単位である必要があります。 詳しくは、<a href="/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md">収益とコスト階層の概要</a>を参照してください。</li>
       <li>このフィールドは、レイアウトテンプレートで、タスクの詳細ビューの「財務」領域で有効にする必要があります。 詳しくは、<a href="/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md"> レイアウトテンプレートを使用した詳細ビューのカスタマイズ </a>を参照してください。</li>
       </ul>
      </td>
     </tr>
     <tr> 
      <td role="rowheader">CPI/SPI/CSI</td> 
      <td> <p>これらは、特定の時点でのタスクのパフォーマンスを示す指標です。プロジェクトのパフォーマンスインデックスメソッドに基づいて、値が計算されます。<br>詳しくは、次の記事を参照してください。</p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">コスト効率指数（CPI）の計算</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">スケジュール効率指数（SPI）の計算</a> </p> </li> 
        <li> <p> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">コストスケジュール効率指数（CSI）の計算</a> </p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">完成時総コスト見積り（EAC）</td> 
      <td> <p>これは、完成時のタスクの総コストを示す計算です。完成時の見積りについて詳しくは、<a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">完成時総コスト見積り（EAC）の計算</a>を参照してください。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （条件付き）財務セクションのフィールドを編集する場合は、**変更を保存**&#x200B;をクリックします。
