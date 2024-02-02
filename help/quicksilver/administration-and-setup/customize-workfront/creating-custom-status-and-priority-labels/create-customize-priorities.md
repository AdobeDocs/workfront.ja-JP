---
title: 優先度の作成とカスタマイズ
description: Workfront の設定エリアで、プロジェクト、タスクおよびイシューの優先度を制御できます。優先度は、Adobe Workfront のプロジェクト、タスクまたはイシューの重要性を指定します。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: ht
source-wordcount: '735'
ht-degree: 100%

---

# 優先度の作成とカスタマイズ

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Workfront の設定エリアで、プロジェクト、タスクおよびイシューの優先度を制御できます。優先度は、Adobe Workfront のプロジェクト、タスクまたはイシューの重要性を指定します。

## アクセス要件

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
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 既存の優先度のカスタマイズ

Workfront 管理者は、Workfront で提供されるデフォルトの優先度に対して、次の変更を行うことができます。

* 優先度の名前を変更する。
* 優先度を並べ替える。

  優先度の並べ替え方法について詳しくは、[プロジェクトタスクまたはイシューの優先度の作成](#create-a-priority-for-a-project-task-or-issue)を参照してください。

* デフォルトの優先度を変更する。

  デフォルトの優先度を変更する機能について詳しくは、[プロジェクトタスクまたはイシューの優先度の作成](#create-a-priority-for-a-project-task-or-issue)を参照してください。

* 優先度の説明を編集する。
* 各優先度に色を設定する。

  優先度の色は、結果を&#x200B;**優先度**&#x200B;でグループ化する際にグラフレポートで使用されます。

  グラフレポートについて詳しくは、[レポートへのグラフの追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)を参照してください。

* 優先度を削除する。

  既存の優先度を削除する場合は、置き換える優先度を選択する必要があります。

* 優先度を非表示にする。

  優先度を非表示にする機能について詳しくは、[プロジェクトタスクまたはイシューの優先度の作成](#create-a-priority-for-a-project-task-or-issue)を参照してください。

  >[!NOTE]
  >
  >各オブジェクトに対して、Workfront アカウントに少なくとも 1 つの優先度が必要です。

各オブジェクトタイプ（プロジェクト、タスク、イシュー）にデフォルトで提供される優先度は同じです。

* なし
* 低
* 標準
* 高
* 緊急

## プロジェクトタスクまたはイシューの優先度の作成 {#create-a-priority-for-a-project-task-or-issue}

Workfront で提供されるデフォルトの優先度に加えて、組織のニーズを反映する独自の優先度を追加できます。

1. Adobe Workfront の右上隅で、**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、**設定** ![](assets/gear-icon-settings.png) の順にクリックします。

1. 左側のパネルで、**プロジェクト環境設定**／**優先度**&#x200B;をクリックします。

1. 優先度を作成するオブジェクトタイプのタブをクリックします（**プロジェクト**、**タスク**&#x200B;または&#x200B;**イシュー**）。
1. 「**新しい優先度を追加します**」をクリックします。
1. 新しい優先度に対して次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">優先度名</td> 
      <td>優先度の名前を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">重要度</td> 
      <td> <p>新しい優先度を追加する場合、デフォルトで数値が割り当てられます。必要に応じて、この数値を編集します。</p> <p>優先度の<strong>重要度</strong>の数値は、選択したオブジェクトに対して一意である必要があります。<br>優先度の数値は、プロジェクト、タスクまたはイシューの重要度を反映します。高い数値は、優先度の高さを示します。</p> <p><b>メモ</b>：優先度を保存した後は、重要度の数値を編集できません。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">色</td> 
      <td> <p>優先度の色を選択します。</p> <p>優先度の色は、グラフレポートとアジャイルチーム設定で使用されます。グラフレポートについて詳しくは、<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">レポートへのグラフの追加</a>を参照してください。</p> <p>アジャイルチームの設定について詳しくは、次を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">既定の優先度</td> 
      <td> <p>ラジオボタンを選択して、これをデフォルトの優先度にするかどうかを決定します。</p> <p>優先度が<strong>デフォルトの優先度</strong>の場合、Workfront のすべてのプロジェクト、タスクまたはイシューに対して自動的に選択されます。<strong>標準</strong>は、Workfront のすべてのオブジェクトのデフォルトの優先度です。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td>関数を説明する優先度の説明を追加します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">非表示</td> 
      <td> <p>優先度を非表示にする場合は、このボックスを選択します。</p><p>「<b>非表示</b>」オプションを選択した場合、優先度は Workfront のどこにも表示されず、ユーザーは自分のプロジェクト、タスクおよびイシューに対して優先度を選択できません。</p> 
      <p><b>重要</b>：今後使用しない優先度を削除するのではなく、非表示にすることをお勧めします。これらを非表示にすることで、この優先度で完了したオブジェクトの履歴データをすべて保持すると同時に、今後ユーザーがこの優先度を選択することを防ぎます。 </p>
      <p>必要に応じて、優先度のリスト順序を変更するには、目的の順序で優先度をドラッグ＆ドロップします。これにより、プロジェクト、タスクおよびイシューで表示される順序が変更されます。これによって、<b>重要度</b>の数値は変わりません。 </p></td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックします。

プロジェクト、タスク、イシューに優先度を適用する手順については、以下の記事を参照してください。

* [プロジェクトの優先度の理解と更新](../../../manage-work/projects/planning-a-project/project-priority.md)
* [タスクの優先度の更新](../../../manage-work/tasks/task-information/task-priority.md)
* [イシューの優先度の更新](../../../manage-work/issues/issue-information/update-issue-priority.md)
