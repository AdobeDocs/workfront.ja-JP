---
title: イシューの重要度の作成またはカスタマイズ
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: ユーザーは重要度を使用して、イシューの重要度を定義できます。Adobe Workfront の 5 つのデフォルトの重要度のいずれかをカスタマイズしたり、ユーザーに対して新しい重要度を作成したりできます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: 7cb1eed72b0f5ce4abd83013b7a2f224dbb2c229
workflow-type: tm+mt
source-wordcount: '665'
ht-degree: 64%

---

# イシューの重大度を作成またはカスタマイズ

{{highlighted-preview}}

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

ユーザーは重要度を使用して、イシューの重要度を定義できます。Adobe Workfront の 5 つのデフォルトの重要度のいずれかをカスタマイズしたり、ユーザーに対して新しい重要度を作成したりできます。

>[!NOTE]
>
>タスクとプロジェクトには重要度はありません。

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

## ビルトインのイシュー重要度

Workfront のイシューには、5 つのビルトインの重要度があります。

* 一時回避
* 混乱を招く
* 対処策のあるバグ
* 対処策のないバグ
* 致命的なエラー

これらの重要度に対して、以下を編集できます。

* 名前
* 色

  重要度のカラーは、結果をイシューの重要度でグループ化すると、グラフレポートにも表示されます。グラフレポートについて詳しくは、[レポートへのグラフの追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)を参照してください。

* デフォルトに設定する重要度

  デフォルトの重要度について詳しくは、[イシューの重要度の作成または編集](#create-or-edit-an-issue-severity)を参照してください。

* 説明
* Workfront で重要度が非表示になっているかどうか

  重要度の非表示について詳しくは、この記事の [&#x200B; 重要度の作成または編集 &#x200B;](#create-or-edit-an-issue-severity) を参照してください。

* 重要度の削除

  削除する場合、置き換える重要度を選択する必要があります。

## イシューの重要度の作成または編集 {#create-or-edit-an-issue-severity}

Workfront の管理者は、ユーザー要件に合わせてイシューの重要度を作成および編集できます。

{{step-1-to-setup}}

1. 左側のパネルで、**プロジェクト環境設定**／**重要度**&#x200B;をクリックします。

1. 新しい重要度を作成する場合は、テーブルの下部にある <span class="preview">**新しい行** または </span>**新しい重要度の追加** をクリックします。
1. 新しい重要度で次のオプションを設定するか、既存の重要度を編集します。

   * **重要度名**：重要度の名前を入力します。
   * **重要度**：最初にWorkfrontによって割り当てられた、重要度のレベルを増減します。

     各重要度の重要性番号は一意である必要があります。大きい数字は、重要度が高いレベルに対応します。

     重要度を保存した後は、この数字を編集できません。

   * **カラー**：重要度の色を選択します。

     重要度のカラーは、結果をイシューの重要度でグループ化すると、グラフレポートで表示されます。グラフレポートについて詳しくは、[レポートへのグラフの追加](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)を参照してください。

   * **デフォルトの重要度**：新しく作成したすべてのイシューにWorkfrontを自動的に適用する重要度を選択します。

     **一時回避** は、Workfrontのイシューのデフォルトの重要度です。

     非表示の重要度を既定値にすることはできません。

     <div class="preview">

     デフォルトの重要度は、アイコン ![&#x200B; デフォルトの重要度アイコン &#x200B;](assets/default-icon.png) で示されます。 新しいデフォルトを選択するには、次のいずれかの操作を行います。

      * 重要度名の横にあるチェックボックスをオンにし、画面の下部にあるアクションバーで「**デフォルトにする**」を選択します。
      * 重要度名にポインタを合わせて、表示される **詳細** メニューをクリックします。 次に、「**デフォルトにする** を選択します。

        新しいデフォルトの重要度には、アイコンのラベルが付いています。

     </div>

   * **説明**：重要度の説明を入力し、その機能を説明します。
   * <span class="preview">**選択肢を非表示**</span> または **非表示**: <span class="preview"> 選択 **はい**</span> またはチェックボックスをオンにして、不要になった重要度を非表示にします。

     非表示にした重要度は、Workfront のどこにも表示されず、ユーザーはイシューの重要度として選択できません。

     >[!IMPORTANT]
     >
     >使用しなくなった重要度を削除する代わりに、非表示にすることをお勧めします。 これにより、その重要度の完了済みのオブジェクトに関する履歴データをすべて保持することができ、その重大度が将来使用されることを妨ぐこともできます。

1. （オプション）重要度の一覧表示順を変更するには、希望する順序に重要度をドラッグ＆ドロップします。

   これにより、イシューの表示順が変更されます。**重要性**&#x200B;番号は変更されません。

1. 「**保存**」をクリックします。

イシューを扱う際に重要度を使用する方法について詳しくは、[イシューの重要度の更新](../../../manage-work/issues/issue-information/update-issue-severity.md)を参照してください。
