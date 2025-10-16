---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: グループ化：プロジェクト スポンサー（時間）
description: この時間のグループ化では、時間が記録されるプロジェクトスポンサー別に時間数を整理します。時間グループ化の標準 Report Builder インターフェイスでは、プロジェクトスポンサーフィールドへのマッピングは提供されません。このフィールドにアクセスするには、テキストモードインターフェイスを使用する必要があります。
author: Nolan
feature: Reports and Dashboards
exl-id: 6b35b0ef-18b7-4121-ae39-d7957d76c04b
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '234'
ht-degree: 76%

---

# グループ化：数時間のプロジェクトスポンサー

<!--Audited: 10/2024-->

この時間のグループ化では、時間が記録されるプロジェクトスポンサー別に時間数を整理します。時間グループ化の標準 Report Builder インターフェイスでは、プロジェクトスポンサーフィールドへのマッピングは提供されません。このフィールドにアクセスするには、テキストモードインターフェイスを使用する必要があります。

![hour_report_grouped_by_sponsor.png](assets/hour-report-grouped-by-sponsor-350x39.png)

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

## プロジェクトスポンサー別に時間数をグループ化

このグループ化を適用するには、次の操作を行います。

1. 時間のリストに移動します。
1. **グループ化**&#x200B;ドロップダウンメニューで「**新規グループ化**」を選択します。

1. 「**テキスト モードに切り替える**」をクリックします。
1. 表示される領域のテキストを削除し、以下のコードに置き換えます。

```
   group.0.linkedname=project:sponsor:name
   group.0.name=
   group.0.valuefield=project:sponsor:name
   group.0.valueformat=HTML
   textmode=true
```

1. 「**完了**」をクリックします。
1. グループ化名を更新し、「**グループ化を保存**」をクリックします。
