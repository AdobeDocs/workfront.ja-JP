---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: フィルター：承認ステータスの項目のみを表示
description: 特定のステータスの項目（現在「承認待ち」にある項目）のみを表示できます。 これは、承認ステータスを持つ他のオブジェクトに対しても同じように機能します。
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/nvD3qBAK0Y-k9P0Vzp9aY1GiHp2L5qVLCdkT32s698c
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 265
ht-degree: 76%

---

# フィルター：承認ステータスの項目のみを表示

<!--Audited: 10/2024-->

特定のステータスの項目（現在「承認待ち」にある項目）のみを表示できます。 これは、承認ステータスを持つ他のオブジェクトに対しても同じように機能します。

次のオブジェクトを承認ステータスに配置できます。

* タスク
* イシュー
* プロジェクト

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

## 承認ステータスの項目のみを表示

1. プロジェクトのリストに移動します。
1. **フィルター** ドロップダウンメニューから、**新しいフィルター**&#x200B;を選択します。
1. 「**プロジェクト：ステータス**」でフィルタリングを選択し、リストからフィルタリングするステータスを選択します。

   例えば、プロジェクトレポートで、ステータスが&#x200B;**計画 - 承認待ち**&#x200B;のプロジェクトのみを表示する場合は、**ステータスと計画が等しい**&#x200B;を追加します。
1. **テキストモード**&#x200B;をクリックします。
1. `status`行を変更するには、ステータスの3文字のキーに&#x200B;**:A**&#x200B;を追加します。
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. **適用** / **新規として保存**&#x200B;をクリックします。

   このリストには、計画 - 承認待ちのステータスのプロジェクトのみが表示されます。
