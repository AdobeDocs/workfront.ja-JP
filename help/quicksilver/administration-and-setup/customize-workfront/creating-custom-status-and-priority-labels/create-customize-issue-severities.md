---
title: イシューの重大度を作成またはカスタマイズ
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: ユーザーは重要度を使用して、イシューの重要度を定義できます。Adobe Workfront の 5 つのデフォルトの重要度のいずれかをカスタマイズしたり、ユーザーに対して新しい重要度を作成したりできます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '592'
ht-degree: 100%

---

# イシューの重大度を作成またはカスタマイズ

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

ユーザーは重要度を使用して、イシューの重要度を定義できます。Adobe Workfront の 5 つのデフォルトの重要度のいずれかをカスタマイズしたり、ユーザーに対して新しい重要度を作成したりできます。

>[!NOTE]
>
>タスクとプロジェクトには重要度はありません。

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

## 組み込みのイシュー重要度

Workfront のイシューには 5 つの重要度が組み込まれています。

* 一時回避
* 混乱を招く
* 対処策のあるバグ
* 対処策のないバグ
* 致命的なエラー

<p>これらの重要度に対して、以下を編集できます。</p>

* 名前
* 色

  重要度のカラーは、結果をイシューの重要度でグループ化すると、グラフレポートにも表示されます。グラフレポートについて詳しくは、[レポートへのグラフの追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)を参照してください。

* デフォルトに設定する重要度

  デフォルトの重要度について詳しくは、[イシューの重要度の作成または編集](#create-or-edit-an-issue-severity)を参照してください。
* 説明
* Workfront で重要度が非表示になっているかどうか

  重要度の非表示について詳しくは、[イシューの重要度の作成または編集](#create-or-edit-an-issue-severity")を参照してください。

* 重要度の削除

  削除する場合、置き換える重要度を選択する必要があります。

## イシューの重要度の作成または編集 {#create-or-edit-an-issue-severity}

Workfront の管理者は、ユーザー要件に合わせてイシューの重要度を作成および編集できます。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、**設定** ![](assets/gear-icon-settings.png) の順にクリックします。

1. 左側のパネルで、**プロジェクト環境設定**／**重要度**&#x200B;をクリックします。

1. 新しい重要度を作成する場合は、「**新しい重要度を追加**」をクリックします。
1. 新しい重要度で次のオプションを設定するか、既存の重要度を編集します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">重要度名</td> 
      <td>重要度の名前を入力</td> 
     </tr> 
     <tr> 
      <td role="rowheader">重要性</td> 
      <td>Workfront が最初に割り当てた重要度の深刻さのレベルを増減させます。
      <p>各重要度の重要性番号は一意である必要があります。大きい数字は、重要度が高いレベルに対応します。</p> <p>重要度を保存した後は、この数字を編集できません。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">色</td> 
      <td> <p>重要度のカラーを選択します。</p> 
      <p>重要度のカラーは、結果をイシューの重要度でグループ化すると、グラフレポートで表示されます。グラフレポートについて詳しくは、<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">レポートへのグラフの追加</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">デフォルトの重要度</td> 
      <td>新しく作成されたすべてのイシューに対して、Workfront が自動的に選択する重要度を選択します。</p>
      <p>Workfront のイシューのデフォルトの重要度は、一時回避です。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td>重要度の意味を表す説明を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">非表示</td> 
      <td> 使わなくなった重要度を非表示にします。 
      <p>非表示にした重要度は、Workfront のどこにも表示されず、ユーザーはイシューの重要度として選択できません。</p> 
      <p><b>重要</b>：今後使用しない重要度は、削除せずに、非表示にすることをお勧めします。これにより、その重要度の完了済みのオブジェクトに関する履歴データをすべて保持することができ、その重大度が将来使用されることを妨ぐこともできます。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）重要度の一覧表示順を変更するには、希望する順序に重要度をドラッグ＆ドロップします。

   これにより、イシューの表示順が変更されます。**重要性**&#x200B;番号は変更されません。

1. 「**保存**」をクリックします。

イシューを扱う際に重要度を使用する方法について詳しくは、[イシューの重要度の更新](../../../manage-work/issues/issue-information/update-issue-severity.md)を参照してください。
