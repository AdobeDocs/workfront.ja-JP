---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: フィルター：承認ステータスの項目のみを表示
description: 特定のステータスの項目（現在「承認待ち」にある項目）のみを表示できます。これは、承認ステータスを持つ他のオブジェクトに対しても同じように機能します。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '265'
ht-degree: 72%

---

# フィルター：承認ステータスの項目のみを表示

<!--Audited: 10/2024-->

特定のステータスの項目（現在「承認待ち」にある項目）のみを表示できます。これは、承認ステータスを持つ他のオブジェクトに対しても同じように機能します。

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
   <p>フィルターの変更者または変更依頼 </p>
   <p>レポートを変更するための標準またはプラン</p>
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
1. **フィルター** ドロップダウンメニューから「**新しいフィルター**」を選択します。
1. **プロジェクト：ステータス** でフィルタリングすることを選択し、フィルタリングに使用するステータスをリストから選択します。

   例えば、プロジェクトレポートで、ステータスが&#x200B;**計画 - 承認待ち**&#x200B;のプロジェクトのみを表示する場合は、**ステータスと計画が等しい**&#x200B;を追加します。
1. **テキストモード** をクリックします。
1. ステータスの 3 文字のキーに `status` を追加して、**:A** の行を変更します。
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. **適用**/**新規保存** をクリックします。

   このリストには、計画 - 承認待ちのステータスのプロジェクトのみが表示されます。
