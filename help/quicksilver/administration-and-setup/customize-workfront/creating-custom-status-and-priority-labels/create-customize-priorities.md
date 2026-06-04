---
title: 優先順位の作成とカスタマイズ
description: Workfront の設定エリアで、プロジェクト、タスクおよびイシューの優先度を制御できます。 優先度は、Adobe Workfront のプロジェクト、タスクまたはイシューの重要性を指定します。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
TQID: https://experienceleague.adobe.com/hnZPQ8LCzcfU9SyyK3-qoWlkYoXyk5Bxcx0-yprX1pw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 725
ht-degree: 47%

---

# 優先度の作成とカスタマイズ

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Workfront の設定エリアで、プロジェクト、タスクおよびイシューの優先度を制御できます。 優先度は、Adobe Workfront のプロジェクト、タスクまたはイシューの重要性を指定します。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td><p>標準</p>
       <p>プラン</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>システム管理者</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 既存の優先度のカスタマイズ

Workfront 管理者は、Workfront で提供されるデフォルトの優先度に対して、次の変更を行うことができます。

* 優先度の名前を変更する。
* 優先度を並べ替える。

  優先順位を並べ替える方法について詳しくは、[&#x200B; プロジェクト、タスク、または問題の優先度を作成](#create-a-priority-for-a-project-task-or-issue)を参照してください。

* デフォルトの優先度を変更する。

  デフォルトの優先度を変更する機能について詳しくは、[&#x200B; プロジェクト、タスク、またはイシューの優先度の作成](#create-a-priority-for-a-project-task-or-issue)を参照してください。

* 優先度の説明を編集する。
* 各優先度に色を設定する。

  優先度の色は、結果を&#x200B;**優先度**&#x200B;でグループ化する際にグラフレポートで使用されます。

  グラフレポートについて詳しくは、[レポートへのグラフの追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)を参照してください。

* 優先度を削除する。

  既存の優先度を削除する場合は、置き換える優先度を選択する必要があります。

* 優先度を非表示にする。

  優先度を非表示にする機能について詳しくは、[&#x200B; プロジェクト、タスク、または問題の優先度を作成](#create-a-priority-for-a-project-task-or-issue)を参照してください。

  >[!NOTE]
  >
  >各オブジェクトに対して、Workfront アカウントに少なくとも 1 つの優先度が必要です。

各オブジェクトタイプ（プロジェクト、タスク、イシュー）にデフォルトで提供される優先度は同じです。

* なし
* 低
* 標準
* 高
* 緊急

## プロジェクト、タスク、または問題の優先度を作成する {#create-a-priority-for-a-project-task-or-issue}

Workfront で提供されるデフォルトの優先度に加えて、組織のニーズを反映する独自の優先度を追加できます。

{{step-1-to-setup}}

1. 左側のパネルで、**プロジェクト環境設定**／**優先度**&#x200B;をクリックします。

1. 優先度を作成するオブジェクトタイプのタブをクリックします（**プロジェクト**、**タスク**&#x200B;または&#x200B;**イシュー**）。
1. テーブルの下部にある&#x200B;**新しい行**&#x200B;をクリックします。
1. 優先度に対して次のオプションを設定します。

   * **優先度の名前**：優先度の名前を入力します。
   * **重要度**：新しい優先度を追加すると、デフォルトで番号が割り当てられます。 必要に応じて、この数値を編集します。

     各優先度の重要度の番号は一意である必要があります。 優先度の数は、プロジェクト、タスクまたは問題の重要性を反映します。最も高い数は、最も高い優先度に対応します。

     優先度を保存した後にこの番号を編集することはできません。

   * **カラー**：優先度のカラーを選択します。

     優先度の色は、グラフレポートとアジャイルチーム設定で使用されます。 グラフレポートについて詳しくは、[レポートへのグラフの追加](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)を参照してください。 アジャイルチーム設定について詳しくは、[&#x200B; アジャイルチームの作成](/help/quicksilver/agile/get-started-with-agile-in-workfront/create-an-agile-team.md)を参照してください。

   * **デフォルトの優先度**：新しく作成されたすべてのプロジェクト、タスク、またはイシューにWorkfrontを自動的に適用する優先度を選択します。

     **標準**&#x200B;は、Workfront のすべてのオブジェクトのデフォルトの優先度です。

     非表示の優先度をデフォルトにすることはできません。

     デフォルトの優先度は、アイコン ![&#x200B; デフォルトの優先度アイコン &#x200B;](assets/default-icon.png)で示されます。 新しいデフォルトを選択するには、次のいずれかの操作を行います。

      * 優先順位名の横にあるチェックボックスを選択し、画面下部のアクションバーで「**デフォルトにする**」を選択します。
      * 優先順位名にカーソルを合わせ、表示される&#x200B;**詳細** メニューをクリックします。 次に、「**デフォルトにする**」を選択します。

        新しいデフォルトの優先度には、アイコンのラベルが付けられます。

   * **説明**：優先度の説明を入力して、その機能を説明します。
   * **選択肢を非表示**: **はい**&#x200B;を選択すると、不要になった優先度を非表示にできます。

     隠れた優先度はWorkfrontのどこにも表示されないため、ユーザーはプロジェクト、タスク、問題に応じて優先度を選択できません。

     >[!IMPORTANT]
     >
     >使用しない優先度を削除する代わりに、これらの優先度を非表示にすることをお勧めします。 これにより、既に完了したオブジェクトに関するすべての履歴データを優先して保持し、今後は優先度を使用しないようにします。

1. （オプション）目的の順序で優先順位をドラッグ&amp;ドロップして、優先順位のリスト順序を変更します。

   これにより、プロジェクト、タスク、イシューに対して表示される順序が変更されます。 **重要性**&#x200B;番号は変更されません。

1. 「**保存**」をクリックします。

プロジェクト、タスク、イシューに優先度を適用する手順については、以下の記事を参照してください。

* [プロジェクトの優先度の理解と更新](../../../manage-work/projects/planning-a-project/project-priority.md)
* [タスクの優先度の更新](../../../manage-work/tasks/task-information/task-priority.md)
* [イシューの優先度の更新](../../../manage-work/issues/issue-information/update-issue-priority.md)
