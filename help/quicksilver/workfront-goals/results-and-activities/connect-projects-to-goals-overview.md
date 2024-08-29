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
source-git-commit: d7dd5ab4e3041a100b13c5bf169747f58db0ea39
workflow-type: tm+mt
source-wordcount: '923'
ht-degree: 92%

---

# Adobe Workfront Goals の目標にプロジェクトを追加

<!--
THIS MIGHT NEED TO BE RENAMED BECAUSE THERE WILL BE OTHER OBJECTS CONNECTED TO GOALS IN THE FUTURE
-->

プロジェクトを目標に結び付けると、プロジェクトの実際の進捗に基づいて目標の進捗状況を示すことができます。プロジェクトは、目標の進捗状況インジケーターになります。

プロジェクトを目標に結び付けると、組織の戦略的計画（目標）を、従業員が毎日実行し完了している実際の作業（プロジェクト）に結び付けることができます。

>[!IMPORTANT]
>
>プロジェクトのビジネスケース領域で作成されたプロジェクトレベルの目標は、Workfront Goals で作成された戦略目標には関連していません。 ビジネスケースのプロジェクト目標について詳しくは、[ビジネスケース目標を作成](../../manage-work/projects/define-a-business-case/create-business-case-goals.md)を参照してください。


## アクセス要件

以下が必要です。

<table style="table-layout:auto">
<col>
</col>
<col>
</col>
<tbody>
 <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> 
   <p>新しいプランとライセンス構造の場合：
  <ul><li>究極の計画 </li></ul>
   </p>
<p>現在のプランおよびライセンス構造の場合： 
<ul><li> プロまたはそれ以上 </li>
  <li>Workfront ライセンスに加えて、Adobe Workfront Goals ライセンス。</li></ul></p>
   </td> 
  </tr>
 <tr>
 <td role="rowheader">Adobe Workfront プラン*</td>
 <td>
 <p>新規ライセンス：コントリビューター以上</p>
 または
 <p>現在のライセンス：リクエスト以上</p> <p>詳しくは、<a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront ライセンスの概要</a>を参照してください。</p> </td>
 </tr>
 <tr>
 <td role="rowheader">製品*</td>
 <td>
 <p> 新製品の要件は、次のいずれかです。 </p>
<ul>
<li>Select または Prime Adobe Workfront プランと、追加のAdobe Workfront Goals ライセンス。</li>
<li>Workfront Goals をデフォルトで含む究極のWorkfront プラン。 </li></ul>
 <p>または</p>
 <p>現在の必要な製品：Workfront プランとAdobe Workfront Goals の追加ライセンス。 </p> <p>詳しくは、<a href="../../workfront-goals/goal-management/access-needed-for-wf-goals.md" class="MCXref xref">Workfront Goals の使用要件</a>を参照してください。 </p> </td>
 </tr>
 <tr>
 <td role="rowheader">アクセスレベル</td>
 <td> <p>Goals への編集アクセス権</p> </td>
 </tr>
 <tr data-mc-conditions="">
 <td role="rowheader">オブジェクト権限</td>
 <td>
  <div>
  <p>目標の表示には表示権限以上が必要</p>
  <p>目標に対する編集権限を管理</p>
  <p>目標の共有について詳しくは、<a href="../../workfront-goals/workfront-goals-settings/share-a-goal.md" class="MCXref xref">Workfront Goals での目標の共有</a>を参照してください。 </p>
  </div> </td>
 </tr>
 <tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront 管理者を含むすべてのユーザーには、メインメニューに「目標」エリアが含まれるレイアウトテンプレートを割り当てる必要があります。 </p>  
</td>
  </tr>
</tbody>
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

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

  ![](assets/goal-closed-project-active-warning-goal-list-350x94.png)
-->

* 目標に関連付けられたプロジェクトを削除すると、そのプロジェクトも目標から削除されます。

  >[!CAUTION]
  >
  >プロジェクトを削除する前に目標がアクティブでも、目標に他の進捗状況インジケーターがない場合、目標は非アクティブになります。


## 目標にプロジェクトを追加

1. **メインメニュー** ![](assets/main-menu-icon.png)（これをシェル用に下書き：または（使用可能な場合）左上隅にある&#x200B;**メインメニュー** ![](assets/three-line-main-menu-icon.png)）をクリックし、「**目標**」をクリックします。
1. 目標リストで目標の名前をクリックし、目標ページを開きます。
1. 左側のパネルの「**進捗状況インジケーター**」をクリックします。
1. **新しい進捗状況インジケーター**&#x200B;ドロップダウンメニューから、「**既存のプロジェクトを追加**」をクリックします。

   「目標にプロジェクトを追加」ボックスが表示されます。
1. （オプション）リストの右上隅にあるそれぞれのアイコンをクリックして、「**ビュー**」、「**フィルター**」、「**グループ化**」を更新し、プロジェクトリストの表示方法を変更します。
1. （オプション）**検索**&#x200B;アイコン ![](assets/search-icon.png) をクリックし、プロジェクトの名前を入力し始めると、リスト内でプロジェクトがすぐに見つかります。
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
