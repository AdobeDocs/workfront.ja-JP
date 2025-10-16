---
content-type: overview
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Adobe Workfront Goals の目標にプロジェクトを追加
description: プロジェクトを目標に結び付けると、プロジェクトの実際の進捗に基づいて目標の進捗状況を示すことができます。プロジェクトは、目標の進捗状況インジケーターになります。
author: Alina
feature: Workfront Goals
exl-id: 683c9cd9-6c7b-4d50-b326-b4000c9863e8
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '865'
ht-degree: 85%

---

# Adobe Workfront Goals の目標にプロジェクトを追加

<!--Audited for P&P only: 10/2025-->

プロジェクトを目標に結び付けると、プロジェクトの実際の進捗に基づいて目標の進捗状況を示すことができます。プロジェクトは、目標の進捗状況インジケーターになります。

プロジェクトを目標に結び付けると、組織の戦略的計画（目標）を、従業員が毎日実行し完了している実際の作業（プロジェクト）に結び付けることができます。

>[!IMPORTANT]
>
>プロジェクトのビジネスケース領域で作成されたプロジェクトレベルの目標は、Workfront Goals で作成された戦略目標には関連していません。 ビジネスケースのプロジェクト目標について詳しくは、[ビジネスケース目標を作成](../../manage-work/projects/define-a-business-case/create-business-case-goals.md)を参照してください。


## アクセス要件

>[!NOTE]
>
>過去にこのパッケージを購入したことがある会社は、Adobe Workfront Goals を引き続き使用する場合があります。 詳細については、アカウント担当者にお問い合わせください。
>
>Adobe Workfront Goals は購入できなくなりました。

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr>
  <td> <p>Adobe Workfront パッケージ</p> </td> 
   <td> 
   <p>Adobe WorkfrontUltimate</p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront プラン</td>
 <td>
 <p>投稿者以上</p>
<p>リクエスト以上</p></td>
 </tr>
  <tr>
 <td role="rowheader">アクセスレベル設定</td>
 <td> <p>Goals への編集アクセス権</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">オブジェクト権限</td>
 <td>
  <div>
  <p>目標の表示には表示権限以上が必要</p>
  <p>目標に対する編集権限を管理</p>
  </div> </td>
 </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>システム管理者を含むすべてのユーザーには、メインメニューの目標エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p>  
</td>
  </tr>
</tbody>
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:
<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> 
   <p>For the new plan and license structure:
  <ul><li>An Ultimate plan </li></ul>
   </p>
<p>For the current plan and license structure: 
<ul><li> A Pro or higher </li>
  <li>An Adobe Workfront Goals license in addition to a Workfront license.</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront license*</td>
 <td>
 <p>New license: Contributor or higher</p>
 Or
 <p>Current license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
 </tr>
 <tr>
 <td role="rowheader">Product*</td>
 <td>
 <p> New product requirement, one of the following: </p>
<ul>
<li>A Select or Prime Adobe Workfront plan and an additional Adobe Workfront Goals license.</li>
<li>An Ultimate Workfront plan which includes Workfront Goals by default. </li></ul>
 <p>Or</p>
 <p>Current product requirement: A Workfront plan and an additional license for Adobe Workfront Goals. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
 </tr>
 <tr>
 <td role="rowheader">Access level</td>
 <td> <p>Edit access to Goals</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">Object permissions</td>
 <td>
  <div>
  <p>View or higher permissions to the goal to view it</p>
  <p>Manage permissions to the goal to edit it</p>
  <p>For information about sharing goals, see <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Share a goal in Workfront Goals</a>. </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>All users, including Workfront administrators,  must be assigned a layout template that includes the Goals area in the Main Menu. </p>  
</td>
  </tr>
</tbody>
</table>-->

## プロジェクトを目標に結び付ける際の考慮事項

* 次の条件を満たすプロジェクトを目標に追加できます。

   * 表示する権限が少なくとも必要です。

     >[!NOTE]
     >
     >プロジェクトを目標に関連付けた後に、プロジェクトを表示する権限を失った場合でも、目標のプロジェクト情報は表示できますが、プロジェクトにはアクセスできなくなります。

   * プロジェクトのステータスを「無効」にすることはできません。

* 1 つの目標に複数のプロジェクトを関連付けることができます。
* 同じプロジェクトを複数の目標に関連付けることができます。
* プロジェクトが関連付けられている目標から、プロジェクトの進行状況を手動で更新することはできません。 代わりに、Workfront はプロジェクトの完了率を計算し、Workfront Goals はこの完了率を使用して目標の進捗を計算します。これにより、プロジェクト率が更新された後に、目標がリアルタイムで更新されます。
* プロジェクトの期間は、目標の期間外になる場合があります。 プロジェクトが目標の期限より長く続く場合でも、目標を終了して完了したと見なすことはできますが、目標完了率は 100％にはなりません。 プロジェクトの完了率が目標に対して更新されなくなりました。

<!--this is no longer visible in the new redesigned interface for goals: logged a bug for this: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/63ceb049000080d30022aab9a359f6f1/updates - but confirmed that this will not be brought back at least for now - Jan 2023. 

There is an indication on the goal list that the project no longer updates progress for the goal.

  ![Goal closed](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* 目標に関連付けられたプロジェクトを削除すると、そのプロジェクトも目標から削除されます。

  >[!CAUTION]
  >
  >プロジェクトを削除する前に目標がアクティブでも、目標に他の進捗状況インジケーターがない場合、目標は非アクティブになります。


## 目標にプロジェクトを追加

1. **メインメニュー**![&#x200B; メインメニューアイコン &#x200B;](assets/main-menu-icon.png) （シェルの下書き：または左上隅の **メインメニュー**![&#x200B; メインメニューの行 &#x200B;](assets/three-line-main-menu-icon.png) をクリックします（利用可能な場合））、**目標** の順にクリックします。
1. 目標リストで目標の名前をクリックし、目標ページを開きます。
1. 左側のパネルの「**進捗状況インジケーター**」をクリックします。
1. **新しい進捗状況インジケーター**&#x200B;ドロップダウンメニューから、「**既存のプロジェクトを追加**」をクリックします。

   「目標にプロジェクトを追加」ボックスが表示されます。
1. （オプション）リストの右上隅にあるそれぞれのアイコンをクリックして、「**ビュー**」、「**フィルター**」、「**グループ化**」を更新し、プロジェクトリストの表示方法を変更します。
1. （任意） **検索** アイコン ![&#x200B; 検索アイコン &#x200B;](assets/search-icon.png) をクリックし、プロジェクトの名前の入力を開始すると、リスト内をすばやく見つけることができます。
1. 目標に追加するプロジェクトを選択し、「**追加**」をクリックします。

   選択したプロジェクトが目標に追加され、**プロジェクト**&#x200B;グループの下の目標ページの「進捗状況インジケーター」セクションに表示されます。

   目標をアクティベートした後、プロジェクトの進捗状況が更新されると、目標の進捗状況が自動的に更新されます。 目標のアクティブ化については、[Adobe Workfront Goals で目標をアクティベート](../goal-management/activate-goals.md)を参照してください。

## 目標のプロジェクト情報を見つける

<p>
次のプロジェクト情報は、目標のページの「進捗状況インジケーター」セクションの目標レベルに表示されます。

</p>

<table>
  <tr>
   <td>プロジェクト名
   </td>
   <td>プロジェクト名の変更は、関連付けされたプロジェクトにも反映されます。
   </td>
  </tr>
  <tr>
   <td>プロジェクト所有者
   </td>
   <td>プロジェクト所有者の変更は、関連付けされたプロジェクトにも反映されます。
   </td>
  </tr>
    <tr>
   <td>実際の進捗状況
   </td>
   <td> <p>プロジェクトの完了率。 目標からプロジェクトの完了率を手動で更新することはできません。 Workfront は、タスクの完了率に基づいて自動的に計算します。 </p>
   </td>
  </tr>
  <tr>
   <td>進捗状況
   </td>
   <td>棒グラフで表される、プロジェクトの完了率。 プロジェクトの完了率を変更すると、目標がクローズされない限り、目標の進捗状況が自動更新されます。
   </td>
  </tr>

</table>

## プロジェクトの目標情報を見つける

次の目標情報は、プロジェクトリストまたはレポートに表示されます。

| 目標情報 | 説明 |
|---|---|
| Goals | プロジェクトが関連付けられているすべての目標のリスト。 |
| 目標階層 | 目標が属する階層。このフィールドには、目標と目標の親のみが表示されます。子の目標は表示されません。 |
| リンクされた目標の数 | 1 つのプロジェクトにリンクされた目標の数。 |
