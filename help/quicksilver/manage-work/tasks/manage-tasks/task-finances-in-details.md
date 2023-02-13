---
product-area: projects
navigation-topic: manage-tasks
title: '[ タスクの詳細 ] セクションでタスクの財務を管理します'
description: '[ タスクの詳細 ] セクションでタスクの財務を管理します'
author: Alina
feature: Work Management
exl-id: 54ae48e5-bc8c-4e90-8fa1-0015523df4e6
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 5%

---

# [ タスクの詳細 ] セクションでタスクの財務を管理します

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: some of the information (fields) in this article is also in the Edit tasks article; if you need to update one field, to it in both articles)</p>
-->

タスクの財務情報を表示または編集するには、「タスクの詳細」セクションの「概要」領域にアクセスします。 この領域で表示または編集できるフィールドは限られています。 タスクのすべての財務情報の編集の詳細については、を参照してください。 [タスクを編集](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>仕事以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトとタスクへのアクセスを編集</p> <p>財務データ以上へのアクセスを表示</p> <p>タスクに関する財務情報を編集するには、財務データへの編集アクセス権が必要です</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>「財務の表示」以上を含むタスクに対する権限を表示します</p> <p>タスクに関する財務情報を編集するには、[ 財務の編集 ] を含むタスクに対する管理権限が必要です</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## [ タスクの詳細 ] セクションでタスクの財務状況を編集します

1. タスクを表示するプロジェクトに移動します。

   >[!NOTE]
   >
   >タスクを検索するには、タスクを検索し、名前をクリックしてタスクにアクセスします。 Workfrontでのオブジェクトの検索について詳しくは、 [検索Adobe Workfront](../../../workfront-basics/navigate-workfront/search/search-workfront.md).

1. クリック **タスク** をクリックします。
1. 表示するタスクの名前をクリックします。
1. クリック **タスクの詳細**.
1. （オプション） **すべて折りたたむ** アイコンを使用して、タスクの詳細ページの右上に表示できます。

   ![](assets/collapse-all-icon-on-details-page.png)

   >[!NOTE]
   >
   >Workfront管理者またはグループ管理者がレイアウトテンプレートを設定する方法に応じて、「タスクの詳細」セクションのフィールドが再配置されたり表示されなかったりする場合があります。 詳しくは、 [レイアウトテンプレートを使用して詳細ビューをカスタマイズする](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).

1. クリック **金融** タスクの財務情報を展開して表示します。

   次をクリック： **編集** アイコン ![](assets/edit-icon.png) 「詳細」セクションの右上隅で、 **金融**.

1. フィールドをシングルクリックまたはクリックして、編集可能なフィールドを編集します。 **+追加** をクリックして、空のフィールドに情報を追加します。
1. 次の情報を **金融** 領域：

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">コストの種類</td> 
      <td> <p>タスクのコストタイプを指定します。 これにより、タスクの時間数に基づいて、タスクのコストを計算する方法が決まります。 </p> <p>次のオプションから選択します。 </p> 
       <ul> 
        <li> <p>コストなし</p> </li> 
        <li> <p>固定 (毎時) </p> </li> 
        <li> <p> ユーザー (毎時) </p> </li> 
        <li> <p> 役割 (毎時)</p> </li> 
       </ul> <p>コストの追跡について詳しくは、 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a> . Workfront管理者またはグループ管理者が、システムまたはグループ内のタスクのデフォルトのコストタイプ設定を選択します。 プロジェクトの既定値の設定については、 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクト環境設定の指定</a> .</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">収益タイプ</td> 
      <td> <p>タスクの収益タイプを指定します。 これにより、タスクの時間数に基づいて、タスクの売上高の計算方法が決まります。 </p> <p>次のオプションから選択します。 </p> 
       <ul> 
        <li> <p> 請求不可 </p> </li> 
        <li> <p>ユーザー (毎時) </p> </li> 
        <li> <p>役割 (毎時) </p> </li> 
        <li> <p>固定 (毎時) </p> </li> 
        <li> <p>ユーザー (毎時) (上限付き) </p> </li> 
        <li> <p>役割 (毎時) (上限付き) </p> </li> 
        <li> <p>ユーザー (毎時) + 固定 </p> </li> 
        <li> <p>役割 (毎時) + 固定 </p> </li> 
        <li> <p>固定収益 </p> </li> 
       </ul> <p>売上高の追跡について詳しくは、<a href="../../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">請求と売上高の概要</a> . </p> <p>Workfront管理者またはグループ管理者が、システムまたはグループのタスクのデフォルトの売上高の種類設定を選択します。 プロジェクトの既定値の設定については、 <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md" class="MCXref xref">システム全体のプロジェクト環境設定の指定</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">予定コスト</td> 
      <td> <p>これは、ユーザーまたはジョブの役割の予定時間、コストタイプ、時間単価に基づいてタスクのコストを表示する計算です。 コストの追跡について詳しくは、 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">実費</td> 
      <td> <p> これは、ユーザーまたはジョブの役割の実際の時間、コストタイプ、時間単価に基づいてタスクのコストを表示する計算です。 コストの追跡について詳しくは、 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">予定収益</td> 
      <td> <p>これは、タスクに関連する売上高を、予定時間、売上高タイプ、ユーザーまたはジョブの役割の時間単価に基づいて表示する計算です。 コストの追跡について詳しくは、 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">実際の売上高</td> 
      <td> <p>これは、実際の時間、売上高のタイプ、ユーザーまたはジョブの役割の時間単価に基づいて、タスクに関連付けられた売上高を表示する計算です。 コストの追跡について詳しくは、 <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">コストの追跡</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>CPI/SPI/CSI</strong> </td> 
      <td> <p>これらは、タスクの実行状況を特定の時間に示すタスクのパフォーマンス指標です。 その値は、プロジェクトのパフォーマンスインデックスメソッドに基づいて計算されます。<br>詳しくは、次の記事を参照してください。</p> 
       <ul> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-cpi.md" class="MCXref xref">コスト効果指数 (CPI) の計算</a> </p> </li> 
        <li> <p><a href="../../../manage-work/projects/project-finances/calculate-spi.md" class="MCXref xref">スケジュールパフォーマンスインデックスの計算 (SPI) </a> </p> </li> 
        <li> <p> <p><a href="../../../manage-work/projects/project-finances/calculate-csi.md" class="MCXref xref">CSI(Calculate Cost Schedule Performance Index)</a> </p> </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">完了時の推定 (EAC)</td> 
      <td> <p>これは、完了時のタスクの総コストを示す計算です。 完了時の見積もりについて詳しくは、 <a href="../../../manage-work/projects/project-finances/calculate-eac.md" class="MCXref xref">完了時の推定 (EAC) を計算</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （条件付き）「財務」セクションのフィールドを編集する場合、 **保存****変更**.
