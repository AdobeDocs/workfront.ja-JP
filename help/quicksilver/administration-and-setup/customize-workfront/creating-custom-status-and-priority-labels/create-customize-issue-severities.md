---
title: イシューの重要度の作成またはカスタマイズ
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: ユーザーは重要度を使用して、イシューの重要度を定義できます。 Adobe Workfront の 5 つのデフォルトの重要度のいずれかをカスタマイズしたり、ユーザーに対して新しい重要度を作成したりできます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
TQID: https://experienceleague.adobe.com/jwRUKjxTd--9vcxXsfkbiPmrC1SsR-V8rjOdcXFfKCg
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 631
ht-degree: 66%

---

# イシューの重大度を作成またはカスタマイズ

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

ユーザーは重要度を使用して、イシューの重要度を定義できます。 Adobe Workfront の 5 つのデフォルトの重要度のいずれかをカスタマイズしたり、ユーザーに対して新しい重要度を作成したりできます。

>[!NOTE]
>
>タスクとプロジェクトには重要度はありません。

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

  重要度のカラーは、結果をイシューの重要度でグループ化すると、グラフレポートにも表示されます。 グラフレポートについて詳しくは、[レポートへのグラフの追加](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)を参照してください。

* デフォルトに設定する重要度

  デフォルトの重要度について詳しくは、[イシューの重要度の作成または編集](#create-or-edit-an-issue-severity)を参照してください。

* 説明
* Workfront で重要度が非表示になっているかどうか

  重大度を非表示にする方法の詳細については、この記事の「[問題の重大度を作成または編集する](#create-or-edit-an-issue-severity)」を参照してください。

* 重要度の削除

  削除する場合、置き換える重要度を選択する必要があります。

## イシューの重要度の作成または編集 {#create-or-edit-an-issue-severity}

Workfront の管理者は、ユーザー要件に合わせてイシューの重要度を作成および編集できます。

{{step-1-to-setup}}

1. 左側のパネルで、**プロジェクト環境設定**／**重要度**&#x200B;をクリックします。

1. 新しい重要度を作成する場合は、テーブルの下部にある&#x200B;**新しい行**&#x200B;をクリックします。
1. 新しい重要度で次のオプションを設定するか、既存の重要度を編集します。

   * **重大度の名前**：重大度の名前を入力します。
   * **重要度**：重大度に対して、Workfrontによって最初に割り当てられた重大度レベルを増減します。

     各重要度の重要性番号は一意である必要があります。 大きい数字は、重要度が高いレベルに対応します。

     重要度を保存した後は、この数字を編集できません。

   * **カラー**：重要度のカラーを選択します。

     重要度のカラーは、結果をイシューの重要度でグループ化すると、グラフレポートで表示されます。 グラフレポートについて詳しくは、[レポートへのグラフの追加](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md)を参照してください。

   * **既定の重要度**：新しく作成されたすべての問題にWorkfrontを自動的に適用する重要度を選択します。

     **Cosmetic**&#x200B;は、Workfrontの問題の既定の重大度です。

     非表示の重要度をデフォルトにすることはできません。

     デフォルトの重大度は、アイコン ![ デフォルトの重大度アイコン ](assets/default-icon.png)で示されます。 新しいデフォルトを選択するには、次のいずれかの操作を行います。

      * 重大度の名前の横にあるチェックボックスを選択し、画面の下部にあるアクションバーで「**デフォルトにする**」を選択します。
      * 重要度の名前にカーソルを合わせて、表示される&#x200B;**詳細** メニューをクリックします。 次に、「**デフォルトにする**」を選択します。

        新しいデフォルトの重要度には、アイコンのラベルが付けられます。

   * **説明**：重大度の説明を入力して、その機能を説明します。
   * **選択肢を非表示**: **はい**&#x200B;を選択して、不要になった重大度を非表示にします。

     非表示にした重要度は、Workfront のどこにも表示されず、ユーザーはイシューの重要度として選択できません。

     >[!IMPORTANT]
     >
     >使用しなくなった重大度を削除する代わりに、それらを非表示にすることをお勧めします。 これにより、その重要度の完了済みのオブジェクトに関する履歴データをすべて保持することができ、その重大度が将来使用されることを妨ぐこともできます。

1. （オプション）重要度の一覧表示順を変更するには、希望する順序に重要度をドラッグ＆ドロップします。

   これにより、イシューの表示順が変更されます。 **重要性**&#x200B;番号は変更されません。

1. 「**保存**」をクリックします。

イシューを扱う際に重要度を使用する方法について詳しくは、[イシューの重要度の更新](../../../manage-work/issues/issue-information/update-issue-severity.md)を参照してください。
