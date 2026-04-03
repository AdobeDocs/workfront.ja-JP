---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: グループ化：グループ化の結果をテキストモードで折りたたむか、拡張するかを示します
description: グループ化：テキストモードでグループ化の結果を折りたたむか展開するかを指定します
author: Courtney
feature: Reports and Dashboards
exl-id: 2880e06f-34f3-47b1-9462-5a15a20d6fee
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '329'
ht-degree: 84%

---

# グループ化：テキストモードでグループ化の結果を折りたたむか展開するかを指定します

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this article: NWE only; not possible in classic) </p>
-->

標準の Report Builder を使用することにより、リストまたはレポートでグループ化の結果を折りたたんで表示するか展開して表示するかを指定できます。グループ化の結果は、デフォルトでは展開して表示されます。グループ化の作成について詳しくは、[Adobe Workfront でのグループ化の作成](../../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)を参照してください。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: the tips repeat in the Create groupings to organize results article, Understanding text mode, Edit groupings to organize reports, Create a Custom Report; create a snippet when convenient)</p>
-->

>[!TIP]
>
>* リストを表示するときにグループ化を手動で調整すると、ログアウトするまで Adobe Workfront に手動の設定が記憶されます。再度ログインすると、この設定に従ってリストが表示されます。
>* グループ化の結果は、グラフ要素からアクセスした後で常に展開表示されます。
>

グループ化を展開して表示するか、折りたたんで表示するかは、テキストモードを使用して指定することもできます。

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

## テキストモードを使用してグループ化の結果を折りたたむか展開するかを指定

1. オブジェクトのリストに移動します。
1. **グループ化**&#x200B;ドロップダウンメニューで、「**新規グループ化**」を選択します。

1. グループ化を追加し、**テキストモードに切り替え**&#x200B;をクリックします。

   または

   グループ化が既にテキストモードの場合は、折りたたんで表示するグループ化レベルに次のコードを追加します。

   `group.0.iscollapsed=true`

1. （オプション）グループ化を展開して表示する場合は、該当するグループ化レベルに次のコードを追加します。

   `group.0.iscollapsed=false`

1. 「**完了**」、「**グループ化の保存**」の順にクリックします。
1. （オプション）グループ化の名前を更新し、**グループ化を保存**&#x200B;をクリックします。
