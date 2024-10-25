---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「フィルター：承認ステータスの項目のみを表示」
description: 特定のステータスの項目（現在「承認待ち」にある項目）のみを表示できます。これは、承認ステータスを持つ他のオブジェクトに対しても同じように機能します。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: a19668ac2238448010b5a177120f936ef7ba5bba
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 74%

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

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> 
    <p>新規：</p>
   <ul><li><p>フィルターを変更するコントリビューター </p></li>
   <li><p>レポートを変更する場合は Standard</p></li> </ul>

<p>現在：</p>
   <ul><li><p>フィルターを変更する場合は「要求」 </p></li>
   <li><p>レポートを変更するためのプラン</p></li> </ul></td> 
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

*詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## 承認ステータスの項目のみを表示

1. プロジェクトのリストに移動します。
1. **フィルター** ドロップダウンメニューから「**新しいフィルター**」を選択します。
1. **プロジェクト：ステータス** でフィルタリングすることを選択し、フィルタリングに使用するステータスをリストから選択します。

   例えば、プロジェクトレポートで、ステータスが&#x200B;**計画 - 承認待ち**&#x200B;のプロジェクトのみを表示する場合は、**ステータスと計画が等しい**&#x200B;を追加します。
1. **テキストモード** をクリックします。
1. ステータスの 3 文字のキーに **:A** を追加して、`status` の行を変更します。
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. **適用**/**新規保存** をクリックします。

   このリストには、計画 - 承認待ちのステータスのプロジェクトのみが表示されます。
