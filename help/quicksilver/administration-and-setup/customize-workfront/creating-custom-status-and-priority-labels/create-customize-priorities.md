---
title: 優先度の作成とカスタマイズ
description: Workfrontの「設定」領域で、プロジェクト、タスクおよび問題の優先度を制御できます。 優先度は、Adobe Workfrontのプロジェクト、タスクまたは問題を重視します。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 6e7952cf-f07a-412b-9f9a-623cdba46849
source-git-commit: e20934501c2117455ca7950834d868f78576dee7
workflow-type: tm+mt
source-wordcount: '735'
ht-degree: 2%

---

# 優先度の作成とカスタマイズ

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Workfrontの「設定」領域で、プロジェクト、タスクおよび問題の優先度を制御できます。 優先度は、Adobe Workfrontのプロジェクト、タスクまたは問題を重視します。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront管理者である。</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 既存の優先度のカスタマイズ

Workfront管理者は、Workfrontで提供されるデフォルトの優先度に対して、次の変更を行うことができます。

* 優先度の名前を変更します。
* 優先度を並べ替えます。

   優先度の並べ替え方法の詳細については、 [プロジェクトタスクまたはタスクの優先度を作成する](#create-a-priority-for-a-project-task-or-issue).

* デフォルトの優先度を変更します。

   デフォルトの優先度を変更する機能について詳しくは、 [プロジェクトタスクまたはタスクの優先度を作成する](#create-a-priority-for-a-project-task-or-issue).

* 優先度の説明を編集します。
* 優先度ごとに色を設定します。

   優先度の色は、結果をグループ化する際にグラフレポートで使用されます。 **優先度**.

   グラフレポートについて詳しくは、 [レポートへのグラフの追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* 優先度を削除します。

   既存の優先度を削除する場合は、置き換える優先度を選択する必要があります。

* 優先度を非表示にする。

   優先度を非表示にする機能について詳しくは、 [プロジェクトタスクまたはタスクの優先度を作成する](#create-a-priority-for-a-project-task-or-issue).

   >[!NOTE]
   >
   >各オブジェクトに対して、Workfrontアカウントに少なくとも 1 つの優先度が必要です。

各オブジェクトタイプ（プロジェクト、タスク、問題）にデフォルトで提供される優先度は同じです。

* なし
* 低
* 標準
* 高
* 緊急

## プロジェクトタスクまたはタスクの優先度を作成する {#create-a-priority-for-a-project-task-or-issue}

Workfrontで提供されるデフォルトの優先度に加えて、組織のニーズを反映する独自の優先度を追加できます。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **プロジェクト環境設定** > **優先度**.

1. 優先度を作成するオブジェクトタイプのタブをクリックします (**プロジェクト**, **タスク**&#x200B;または **問題**) をクリックします。
1. クリック **新しい優先度を追加**.
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
      <td> <p>新しい優先度を追加する場合、デフォルトでは数値が割り当てられます。 必要に応じて、この数値を編集します。</p> <p>この <strong>重要度</strong> 各優先度の数は、選択したオブジェクトに対して一意である必要があります。<br>優先度の数は、プロジェクト、タスクまたは問題の重要性を反映しています。最も高い数が、最も高い優先度に対応します。</p> <p><b>注意</b>:優先度を保存した後は、重要度番号を編集できません。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">色</td> 
      <td> <p>優先度の色を選択します。</p> <p>優先度の色は、グラフレポートとアジャイルチーム設定で使用されます。 グラフレポートについて詳しくは、 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">レポートへのグラフの追加</a>.</p> <p>アジャイルチームの設定の詳細については、のを参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">既定の優先度</td> 
      <td> <p>ラジオボタンを選択して、これをデフォルトの優先度にするかどうかを決定します。</p> <p>優先度が <strong>デフォルトの優先度</strong>の場合は、Workfrontのすべてのプロジェクト、タスクまたはイシューで自動的に選択されます。 <strong>標準</strong> は、Workfrontのすべてのオブジェクトのデフォルトの優先度です。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td>優先度の関数を説明する説明を追加します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">非表示</td> 
      <td> <p>優先度を非表示にする場合は、このボックスを選択します。</p><p>を選択し、 <b>を隠す</b> 「 」オプションを選択した場合、優先度はWorkfrontのどこにも表示されず、ユーザーは自分のプロジェクト、タスクおよびタスクに対して優先度を選択できません。</p> 
      <p><b>重要</b>:今後使用しない優先度を削除するのではなく、非表示にすることをお勧めします。 これらを隠すことで、この優先順位で完了したオブジェクトの履歴データをすべて保持し、将来、人々がこの優先順位を選択するのを防ぎます。 </p>
      <p>必要に応じて、優先度のリスト順序を変更するには、目的の順序で優先度をドラッグ&amp;ドロップします。 これにより、プロジェクト、タスクおよびタスクで表示される順序が変更されます。 これによって <b>重要度</b> 数値。 </p></td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックします。

プロジェクト、タスクおよび問題に優先度を適用する手順については、次の記事を参照してください。

* [プロジェクトの優先度の理解と更新](../../../manage-work/projects/planning-a-project/project-priority.md)
* [タスクの優先度を更新](../../../manage-work/tasks/task-information/task-priority.md)
* [問題の優先度を更新](../../../manage-work/issues/issue-information/update-issue-priority.md)
