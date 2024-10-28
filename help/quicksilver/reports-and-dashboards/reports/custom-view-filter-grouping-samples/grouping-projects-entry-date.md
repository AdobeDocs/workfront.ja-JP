---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「グループ化：エントリ日別プロジェクト」
description: このカスタムプロジェクトのグループ化では、エントリ日の値でグループ化されたプロジェクトを表示できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 511faad5-b5bd-4e2d-8daa-3fcde49a502c
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 68%

---

# グループ化：入力日別プロジェクト

このカスタムプロジェクトのグループ化では、エントリ日の値でグループ化されたプロジェクトを表示できます。

各グループ化では、次の範囲のエントリ日のプロジェクトが表示されます。

* 過去 30 日間
* 30 日～ 60 日前
* 60 日以上前

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

## プロジェクトをエントリ日別にグループ化

このグループ化を適用するには、次の操作を行います。

1. 既存のプロジェクトレポートに移動するか、新しいプロジェクトレポートを作成します。\
   レポートの作成について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。
1. **レポートアクション**/**編集** をクリックします。
1. 「**グループ化**」タブで「**グループ化を追加**」をクリックします。
1. 「**テキストモードに切り替える**」をクリックします。
1. **グループ化** 領域のテキストを削除します。
1. 次のコードでテキストを置き換えます。

   group.0.linkedname=direct
group.0.name=プロジェクトエントリ
group.0.valueexpression=IF （ABS （DATEDIFF （{entryDate},$$TODAY）） &lt;=30,&quot;過去 30 日間&quot;,IF （ABS （DATEDIFF （{entryDate},$$TODAY）） >30&amp;&amp;ABS （DATEDIFF （{entryDate},$$TODAY）） &lt;=60,&quot;30-60 日間&quot;,&quot;60 日以上&quot;））
group.0.valueformat=atDateAsMonthString
textmode=true

1. **完了**/**グループ化を保存** をクリックします。
1. （オプション）グループ化の名前を更新し、「**グループ化を保存**」をクリックします。
