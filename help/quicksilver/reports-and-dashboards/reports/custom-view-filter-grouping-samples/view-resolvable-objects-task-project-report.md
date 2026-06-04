---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: ビュー：タスクまたはプロジェクトレポート内の解決可能オブジェクト
description: すべての解決可能オブジェクトのリストを、プロジェクト、タスクビューまたはレポートに表示できます。
author: Courtney
feature: Reports and Dashboards
exl-id: 2b0d8e7c-9211-44e5-9d92-c87a2fe4336d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/jDQ1JmHcOEmRwmBMc6FXaqfxmmR-HCRB5mzsx8eJ4Lk
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 260
ht-degree: 68%

---

# ビュー：タスクまたはプロジェクトレポート内の解決可能なオブジェクト

<!--Audited: 11/2024-->

すべての解決可能オブジェクトのリストを、プロジェクト、タスクビューまたはレポートに表示できます。

解決可能オブジェクトについて詳しくは、[解決オブジェクトと解決可能オブジェクトの概要](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md)を参照してください。

![list_of_resolvables_in_report.png](assets/list-of-resolvables-in-report-350x54.png)

このビューの適用方法は、タスクとプロジェクトで同じです。

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
   <p>ビューを変更するコントリビューターまたはリクエスト </p>
   <p>レポートを修正する標準または計画</p>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルター、表示、グループ化へのアクセス権を編集して、表示を変更できるようにします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。


+++

## タスクまたはプロジェクトレポートでの解決可能オブジェクトの表示

1. イシューから変換されたタスクまたはプロジェクトのリストに移動します。
1. **表示**&#x200B;ドロップダウンメニューで、「**新規ビュー**」をクリックします。

1. **列プレビュー**&#x200B;領域で、**列を追加**&#x200B;をクリックします。

1. 新しい列のヘッダーをクリックし、**テキストモードに切り替え**/**テキストモードを編集**&#x200B;をクリックします。
1. 「**テキストモードを編集**」ボックスにあるテキストを削除し、次のコードに置き換えます。

   ```
   displayname=Resolvables
   listdelimiter=<br>
   listmethod=nested(resolvables).lists
   textmode=true
   type=iterate
   valuefield=name
   valueformat=HTML
   ```

1. **完了** / **ビューを保存**&#x200B;をクリックします。\
   新しい列に、すべての解決可能オブジェクトのリストが表示されます。 リスト内のオブジェクトの名前は、オブジェクトに直接リンクできません。
