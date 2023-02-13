---
title: 問題の重要度を作成またはカスタマイズ
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: ユーザーは重大度を使用して、問題の重大度を定義できます。 Adobe Workfrontに存在する 5 つのデフォルトの重大度のいずれかをカスタマイズしたり、ユーザーに対して新しい重大度を作成したりできます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '592'
ht-degree: 4%

---

# 問題の重要度を作成またはカスタマイズ

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

ユーザーは重大度を使用して、問題の重大度を定義できます。 Adobe Workfrontに存在する 5 つのデフォルトの重大度のいずれかをカスタマイズしたり、ユーザーに対して新しい重大度を作成したりできます。

>[!NOTE]
>
>タスクとプロジェクトには重要性はありません。

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

## 組み込みの問題の重要度

Workfrontには 5 つの重大な問題が組み込まれています。

* 一時回避
* 混乱を招く
* 対処策のあるバグ
* 対処策のないバグ
* 致命的なエラー

<p>次の重要度に対して、以下を編集できます。</p>

* 名前
* 色

   重大度の色は、結果を問題の重大度でグループ化した場合、グラフレポートに保持されます。 グラフレポートについて詳しくは、 [レポートへのグラフの追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* デフォルトの重大度はどれですか。

   デフォルトの重大度の詳細については、 [問題の重大度の作成または編集](#create-or-edit-an-issue-severity) 」を参照してください。
* 説明
* 重大度がWorkfrontで非表示かどうか

   重大度の非表示の詳細については、 [問題の重大度の作成または編集](#create-or-edit-an-issue-severity")

* 重大度の削除

   この場合、置き換える重大度を選択する必要があります。

## 問題の重大度の作成または編集 {#create-or-edit-an-issue-severity}

Workfrontの管理者は、ユーザーのニーズに合わせてイシューの重要度を作成および編集できます。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **プロジェクト環境設定** > **重大度**.

1. 新しい重大度を作成する場合は、「 **新しい重大度を追加**.
1. 新しい重大度に対して次のオプションを設定するか、既存の重大度に対して編集します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">重要度名</td> 
      <td>重大度の名前を入力</td> 
     </tr> 
     <tr> 
      <td role="rowheader">重要度</td> 
      <td>深刻度のWorkfrontが最初に割り当てた重大度のレベルを増減させます。
      <p>各重大度の重要度の数は一意である必要があります。 最も大きい数は、最も重大度の高いレベルに対応します。</p> <p>重大度を保存した後は、この数を編集できません。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">色</td> 
      <td> <p>重大度の色を選択します。</p> 
      <p>重大度の色は、結果を問題の重大度でグループ化する際にグラフレポートで使用されます。 グラフレポートについて詳しくは、 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">レポートへのグラフの追加</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">既定の重要度</td> 
      <td>Workfrontが新しく作成したすべての問題を自動的に選択する重要度を選択します。</p>
      <p>Workfrontの問題のデフォルトの重大度は、「コスメティック」です。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">説明</td> 
      <td>機能を説明する重大度の説明を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">非表示</td> 
      <td> 不要になった重大度を非表示にします。 
      <p>非表示の重大度は、Workfrontのどこにも表示されないので、ユーザーは問題のために選択できません。</p> 
      <p><b>重要</b>:今後使用しなくなった重大度を削除する代わりに、それらを非表示にすることをお勧めします。 これにより、重大度の高い完了済みのオブジェクトに関する履歴データをすべて保持し、将来の重大度の使用を妨げます。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）重要度を目的の順序でドラッグ&amp;ドロップして、重要度の一覧表示順を変更します。

   これにより、問題の表示順が変更されます。 これによって **重要度** 数値。

1. 「**保存**」をクリックします。

問題を処理する際に重要度を使用する方法について詳しくは、 [問題の重大度を更新](../../../manage-work/issues/issue-information/update-issue-severity.md).
