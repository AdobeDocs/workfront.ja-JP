---
content-type: overview
product-previous: workfront-goals
product-area: projects
navigation-topic: results-and-activities
title: Adobe Workfront目標の目標へのプロジェクトの追加
description: プロジェクトを目標に接続して、プロジェクトの実際の進捗状況に基づいて目標の進捗状況を示すことができます。 プロジェクトは目標の進捗状況インジケーターになります。
author: Alina
feature: Workfront Goals
exl-id: 683c9cd9-6c7b-4d50-b326-b4000c9863e8
source-git-commit: dc3461803e23f61877c31efa2c52fffdc7bd79bf
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 1%

---

# Adobe Workfront目標の目標へのプロジェクトの追加

<!--
THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE
-->

プロジェクトを目標に接続して、プロジェクトの実際の進捗状況に基づいて目標の進捗状況を示すことができます。 プロジェクトは目標の進捗状況インジケーターになります。

プロジェクトを目標に結び付けることで、組織の戦略的計画（目標）を、従業員が毎日実行し、完了している実際の作業（プロジェクト）に結び付けることができます。

>[!IMPORTANT]
>
>プロジェクトのビジネスケース領域で作成されたプロジェクトレベルの目標は、Workfront目標で作成された戦略目標とは関連していません。 ビジネス事例のプロジェクト目標については、 [ビジネスケース目標の作成](../../manage-work/projects/define-a-business-case/create-business-case-goals.md).


## アクセス要件

<!--drafted for P&P release: replace the table below with this: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
  <tr>
   <td role="rowheader">Adobe Workfront plan*</td>
   <td>
   <p>Current plan: Select or higher</p>
   Or
   <p>Legacy plan: Pro or higher</p>
   
   </td>
  </tr>
  <tr>
   <td role="rowheader">Adobe Workfront license*</td>
   <td>
   <p>Current license: Contributor or higher</p>
   Or
   <p>Legacy license: Request or higher</p> <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Product</td>
   <td>
   <p> Current product requirement: If you have the Select or Prime Adobe Workfront plan, you must also buy an additional Adobe Workfront Goals license.  Workfront Goals are included in the Ultimate Workfront Plan.</p>
   Or
   <p>Legacy product requirement: You must purchase an additional license for the Adobe Workfront Goals to access functionality described in this article. </p> <p>For information, see <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Requirements to use Workfront Goals</a>. </p> </td>
  </tr>
  <tr>
   <td role="rowheader">Access level*</td>
   <td> <p>Edit access to Goals</p> <p><b>NOTE</b><p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see:</p>
     <ul>
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a> </p> </li>
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Grant access to Adobe Workfront Goals</a></span> </p> </li>
     </ul> </p> </td>
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
 </tbody>
</table>

-->
以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>リクエスト以上</p> <p>詳しくは、 <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfrontライセンスの概要</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td> <p>この記事で説明する機能にアクセスするには、 Adobe Workfront Goals の追加ライセンスを購入する必要があります。 </p> <p>詳しくは、 <a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Workfront目標の使用要件</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>目標へのアクセスを編集</p> <p><b>メモ</b>

<p>まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、以下を参照してください。</p> 
     <ul> 
      <li> <p><a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a> </p> </li> 
      <li> <p><span href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md"><a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md" class="MCXref xref">Adobe Workfront目標へのアクセス権の付与</a></span> </p> </li> 
     </ul> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> 
    <div> 
     <p>目標に対する権限の管理</p> 
     <p>目標の共有について詳しくは、 <a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront目標での目標の共有</a>. </p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。

Workfront Goals へのアクセスについて詳しくは、 [Workfront目標の使用要件](../goal-management/access-needed-for-wf-goals.md).

## プロジェクトを目標に接続する際の考慮事項

* 以下の条件を満たすプロジェクトを目標に追加できます。

   * 表示する権限が少なくとも必要です。

      >[!NOTE]
      >
      >プロジェクトを目標に関連付けた後に、プロジェクトを表示する権限を失った場合でも、目標に関するプロジェクト情報は表示されますが、プロジェクトにアクセスできなくなります。

   * プロジェクトのステータスを「デッド」にすることはできません。

* 1 つの目標に複数のプロジェクトを関連付けることができます。
* 同じプロジェクトを複数の目標に関連付けることができます。
* プロジェクトが関連付けられている目標から、手動でプロジェクトの進行状況を更新することはできません。 代わりに、Workfrontはプロジェクトの完了率を計算し、Workfront目標はこの完了率を使用して目標の進捗を計算します。 これにより、プロジェクトの割合が更新された後に、目標がリアルタイムで更新されます。
* プロジェクトの期間は、目標の期間外にすることができます。 プロジェクトが目標の期限より長く続く場合でも、目標を終了して完了したと見なすことはできますが、目標達成率は 100%にはなりません。 プロジェクトの完了率が目標に対して更新されなくなりました。

<!--this is no longer visible in the new redesigned interface for goals: logged a bug for this: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/63ceb049000080d30022aab9a359f6f1/updates - but confirmed that this will not be brought back at least for now - Jan 2023. 

There is an indication on the goal list that the project no longer updates progress for the goal.

  ![](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* 目標に関連付けられたプロジェクトを削除すると、そのプロジェクトも目標から削除されます。

   >[!CAUTION]
   >
   >プロジェクトを削除する前に目標がアクティブで、目標に他の進捗状況インジケーターがない場合、目標は非アクティブになります。


## 目標へのプロジェクトの追加

1. 次をクリック： **メインメニュー** ![](assets/main-menu-icon.png) ( シェルの下書き：または **メインメニュー** ![](assets/three-line-main-menu-icon.png) （使用可能な場合）、左上隅に表示されます。 **目標**.
1. 「目標リスト」で目標の名前をクリックし、目標ページを開きます。
1. クリック **進行状況指標** をクリックします。
1. 次の **新しい進行状況インジケーター** ドロップダウンメニューで、 **既存のプロジェクトを追加**.

   「目標にプロジェクトを追加」ボックスが表示されます。
1. （オプション） **表示**, **フィルター**&#x200B;または **グループ化** リストの右上隅にある各アイコンをクリックして、プロジェクトのリストの表示方法を変更します。
1. （オプション） **検索** アイコン ![](assets/search-icon.png) リスト内のプロジェクトをすばやく見つけるには、プロジェクトの名前を入力します。
1. 目標に追加するプロジェクトを選択し、「 **追加**.

   選択したプロジェクトが目標に追加され、目標ページの「進行状況インジケーター」セクション (「 **プロジェクト** グループ化。

   目標をアクティブ化すると、プロジェクトの進捗状況が更新されると、目標の進捗状況が自動的に更新されます。 目標のアクティブ化について詳しくは、 [Adobe Workfront目標で目標を有効化](../goal-management/activate-goals.md).

## 目標に関するプロジェクト情報の検索

<p>
次のプロジェクト情報は、目標のページの「進行状況インジケーター」セクションの目標レベルに表示されます。

</p>

<table>
  <tr>
   <td>プロジェクト名
   </td>
   <td>プロジェクト名の変更は、接続されたプロジェクトにも反映されます。
   </td>
  </tr>
  <tr>
   <td>プロジェクト所有者
   </td>
   <td>プロジェクト所有者の変更は、接続されたプロジェクトにも反映されます。
   </td>
  </tr>
    <tr>
   <td>実際の進捗状況
   </td>
   <td> <p>プロジェクトの完了率。 目標からプロジェクトの完了率を手動で更新することはできません。 Workfrontは、タスクの完了率に基づいて自動的に計算します。 </p>
   </td>
  </tr>
  <tr>
   <td>進捗状況
   </td>
   <td>棒グラフで表される、プロジェクトの完了率です。 プロジェクトの完了率を変更すると、目標がクローズされない限り、目標の進捗状況が自動的に更新されます。
   </td>
  </tr>

</table>

## プロジェクトの目標情報の検索

次の目標情報は、プロジェクトリストまたはレポートに表示されます。

| 目標情報 | 説明 |
|---|---|
| 目標 | プロジェクトが関連付けられているすべての目標のリスト。 |
| 目標階層 | 目標が属する階層。 このフィールドには、目標と目標の親のみが表示されます。 子の目標は表示されません。 |
| リンクされた目標の数 | 1 つのプロジェクトにリンクされた目標の数。 |
