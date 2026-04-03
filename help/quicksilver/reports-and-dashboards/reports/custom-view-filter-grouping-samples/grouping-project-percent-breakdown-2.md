---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: グループ化：プロジェクトのパーセント分類2
description: このカスタムのプロジェクトのグループ化では、プロジェクトを完了率の値の範囲でグループ化して表示できます。分類は10% ポイントの増分のパーセント完全な価値を示す：0-10%、11-20%、21-30%等
author: Courtney
feature: Reports and Dashboards
exl-id: 7845fd66-8304-4154-8630-e72482cd753f
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 72%

---

# グループ化：プロジェクトのパーセントでの分類 2

<!--Audited: 10/2024-->

このカスタムのプロジェクトのグループ化では、プロジェクトを完了率の値の範囲でグループ化して表示できます。分類は10% ポイントの増分のパーセント完全な価値を示す：0-10%、11-20%、21-30%等

次のグループ化では、プロジェクトを完了率の値で整理して、次のいずれかのグループに分けています。

* 0%
* 1～10％
* 11 - 20%
* 21 - 30%
* 31 - 40%
* 41 - 50%
* 51 - 60%
* 61 - 70%
* 71 - 80%
* 81 - 90%
* 91 - 99%
* 100%

![percent_complete_breakdown_for_projects_in_10__increments.png](assets/percent-complete-breakdown-350x94.png)

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>コントリビューターまたはフィルターを変更するリクエスト </p>
   <p>レポートを修正する標準または計画</p>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルターを変更する場合は、フィルター、ビュー、グループ化への編集アクセス権</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## プロジェクトのパーセントでの分類によるグループ化

このグループ化を適用するには、次の操作を行います。

1. プロジェクトのリストに移動します。
1. **グループ化**&#x200B;ドロップダウンメニューで「**新規グループ化**」を選択します。

1. 「**テキストモードに切り替える**」をクリックします。
1. ボックス内のテキストを削除して、使用可能なスペースに次のコードをペーストします。

   ```
   group.0.linkedname=direct
   group.0.name=Percent Breakdown
   group.0.notime=false
   group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}<=11,"1-10 %",IF({percentComplete}<=21,"11-20 %",IF({percentComplete}<=31,"21-30 %",IF({percentComplete}<41,"31-40 %",IF({percentComplete}<51,"41-50 %",IF({percentComplete}<61,"51-60 %",IF({percentComplete}<71,"61-70 %",IF({percentComplete}<81,"71-80 %",IF({percentComplete}<91,"81-90 %",IF({percentComplete}<100,"91-99 %","100 %")))))))))))
   textmode=true
   ```

1. 「**完了**」 > 「**グループ化を保存**」をクリックします。
1. （オプション）グループ化の名前を更新し、**グループ化を保存**&#x200B;をクリックします。
