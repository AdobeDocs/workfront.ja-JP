---
title: 優先度の作成とカスタマイズ
description: Workfront の設定エリアで、プロジェクト、タスクおよびイシューの優先度を制御できます。優先度は、Adobe Workfront のプロジェクト、タスクまたはイシューの重要性を指定します。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: 4a7362ae663b73ce48f049556145b4de3e6a6ac9
workflow-type: tm+mt
source-wordcount: '761'
ht-degree: 45%

---

# 優先度の作成とカスタマイズ

{{highlighted-preview}}

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Workfront の設定エリアで、プロジェクト、タスクおよびイシューの優先度を制御できます。優先度は、Adobe Workfront のプロジェクト、タスクまたはイシューの重要性を指定します。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
     <p>新規：標準</p>
     <p>または</p>
     <p>現在：プラン</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 既存の優先度のカスタマイズ

Workfront 管理者は、Workfront で提供されるデフォルトの優先度に対して、次の変更を行うことができます。

* 優先度の名前を変更する。
* 優先度を並べ替える。

  優先度の並べ替え方法の詳細については、「[ プロジェクト、タスク、イシューの優先度を作成する ](#create-a-priority-for-a-project-task-or-issue)」を参照してください。

* デフォルトの優先度を変更する。

  デフォルトの優先度を変更する機能の詳細については、[ プロジェクト、タスク、イシューの優先度を作成する ](#create-a-priority-for-a-project-task-or-issue) を参照してください。

* 優先度の説明を編集する。
* 各優先度に色を設定する。

  優先度の色は、結果を&#x200B;**優先度**&#x200B;でグループ化する際にグラフレポートで使用されます。

  グラフレポートについて詳しくは、[レポートへのグラフの追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)を参照してください。

* 優先度を削除する。

  既存の優先度を削除する場合は、置き換える優先度を選択する必要があります。

* 優先度を非表示にする。

  優先度を非表示にする機能の詳細については、[ プロジェクト、タスク、イシューの優先度を作成する ](#create-a-priority-for-a-project-task-or-issue) を参照してください。

  >[!NOTE]
  >
  >各オブジェクトに対して、Workfront アカウントに少なくとも 1 つの優先度が必要です。

各オブジェクトタイプ（プロジェクト、タスク、イシュー）にデフォルトで提供される優先度は同じです。

* なし
* 低
* 標準
* 高
* 緊急

## プロジェクト、タスク、イシューの優先度を作成する {#create-a-priority-for-a-project-task-or-issue}

Workfront で提供されるデフォルトの優先度に加えて、組織のニーズを反映する独自の優先度を追加できます。

{{step-1-to-setup}}

1. 左側のパネルで、**プロジェクト環境設定**／**優先度**&#x200B;をクリックします。

1. 優先度を作成するオブジェクトタイプのタブをクリックします（**プロジェクト**、**タスク**&#x200B;または&#x200B;**イシュー**）。
1. テーブルの下部にある <span class="preview">**新しい行** または </span>**新しい優先度の追加** をクリックします。
1. 優先度に関して次のオプションを設定します。

   * **優先度名**：優先度の名前を入力します。
   * **重要度**：新しい優先度を追加すると、デフォルトで数値が割り当てられます。 必要に応じて、この数値を編集します。

     各優先度の重要度番号は一意である必要があります。 優先度の数値は、プロジェクト、タスクまたはイシューの重要度を反映しています。最も高い数値は、最も高い優先度に対応します。

     優先度を保存した後で、この番号を編集することはできません。

   * **カラー**：優先度の色を選択します。

     優先度の色は、グラフレポートとアジャイルチーム設定で使用されます。グラフレポートについて詳しくは、[ レポートへのグラフの追加 ](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md) を参照してください。 アジャイルチームの設定について詳しくは、[ アジャイルチームの作成 ](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md) を参照してください。

   * **デフォルトの優先度**：新しく作成したすべてのプロジェクト、タスクまたはイシューにWorkfrontで自動適用する優先度を選択します。

     **標準**&#x200B;は、Workfront のすべてのオブジェクトのデフォルトの優先度です。

     非表示の優先度をデフォルトにすることはできません。

     <div class="preview">

     デフォルトの優先度は、アイコン ![ デフォルトの優先度アイコン ](assets/default-icon.png) で示されます。 新しいデフォルトを選択するには、次のいずれかの操作を行います。

      * 優先度名の横にあるチェックボックスをオンにし、画面の下部にあるアクションバーで「**デフォルトにする**」を選択します。
      * 優先度名の上にマウスポインターを置き、表示される **詳細** メニューをクリックします。 次に、「**デフォルトにする** を選択します。

        新しいデフォルトの優先度には、アイコンのラベルが付いています。

     </div>

   * **説明**：優先度の機能を説明する説明を入力します。
   * <span class="preview">**選択肢を非表示**</span> または **非表示**: <span class="preview"> 選択 **はい**</span> またはチェックボックスをオンにして、不要になった優先度を非表示にします。

     非表示の優先度は、Workfrontのどこにも表示されないので、ユーザーはプロジェクト、タスク、イシューに対して選択できません。

     >[!IMPORTANT]
     >
     >使用したくない優先度を削除するのではなく、非表示にすることをお勧めします。 これにより、既に完了したオブジェクトの履歴データをすべて優先度と共に保持し、ユーザーが将来その優先度を使用するのを防ぐことができます。

1. （オプション）優先度のリスト順序を変更するには、目的の順序でドラッグ&amp;ドロップします。

   これにより、プロジェクト、タスクまたは問題に対する表示の順序が変更されます。 **重要性**&#x200B;番号は変更されません。

1. 「**保存**」をクリックします。

プロジェクト、タスク、イシューに優先度を適用する手順については、以下の記事を参照してください。

* [プロジェクトの優先度の理解と更新](../../../manage-work/projects/planning-a-project/project-priority.md)
* [タスクの優先度の更新](../../../manage-work/tasks/task-information/task-priority.md)
* [イシューの優先度の更新](../../../manage-work/issues/issue-information/update-issue-priority.md)
