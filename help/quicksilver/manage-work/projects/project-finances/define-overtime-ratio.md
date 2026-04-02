---
content-type: overview
product-area: projects
navigation-topic: financials
title: 残業率の定義
description: タスクの残業率を定義して、タスク割り当ての予定収益計算を調整できます。
author: Lisa
feature: Work Management
source-git-commit: bf8dcc9dfa9697c8d212072bb511c57aa01e7529
workflow-type: tm+mt
source-wordcount: '348'
ht-degree: 15%

---

# 残業率の定義

{{highlighted-preview-article-level}}

残業率がタスクに追加されると、その残業率はタスクのすべての割り当てに適用されます。 そのタスクのすべての予定時間が乗算され、予定収益の計算に影響します。

同じタスク内の割り当てに対して、残業率を変更することはできません。 異なる時間外乗数が必要な場合は、親タスクの下に別々のサブタスクを作成する必要があります。

>[!NOTE]
>
>残業率が残業以外のタスクに追加されることを防ぐ検証はありません。

## 予定収益の超過時間の計算

システムはまず、標準の請求レート階層を使用して請求レートを決定します。 詳しくは、[収益とコスト階層の概要](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)を参照してください。

残業率がタスクに存在する場合、計算は次のようになります。
予定収益= Billing Rate × Overtime Ratio × Planned Hours

残業率が空白の場合、計算は次のようになります。
予定収益=請求率×予定時間数

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td>ワークフロー Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td>標準</td> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>タスク、プロジェクト、財務データへのアクセス権の編集</td> 
  </tr> 
  <tr> 
   <td>オブジェクト権限</td> 
   <td><p>請求率の編集を含むタスクへの権限を管理します</p>
     <p>プロジェクトに対する参加以上の権限</p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

タスクの収益タイプは、ユーザーと役割の時間単位である必要があります。 詳しくは、[収益とコスト階層の概要](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md)を参照してください。

レイアウトテンプレートで&#x200B;**残業率** フィールドを有効にする必要があります。

1. レイアウトテンプレートで、**ユーザーに表示される内容をカスタマイズ**&#x200B;の下にある下向き矢印をクリックし、**タスク**&#x200B;をクリックします。
1. **詳細** セクションで、**財務** エリアの&#x200B;**残業率** フィールドを選択します。

   詳しくは、[&#x200B; レイアウトテンプレートを使用した詳細ビューのカスタマイズ &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)を参照してください。

## タスクの残業率の定義

1. 編集するタスクに移動します。

   詳細については、「[&#x200B; タスクの詳細のセクション &#x200B;](/help/quicksilver/manage-work/tasks/manage-tasks/task-finances-in-details.md)でタスクの財務を管理する」を参照してください。

1. 左パネルでの「**タスクの詳細**」をクリックします。
1. **Finance**&#x200B;領域で、**残業率** フィールドに残業乗数を入力します。
1. 「**変更を保存**」をクリックします。

