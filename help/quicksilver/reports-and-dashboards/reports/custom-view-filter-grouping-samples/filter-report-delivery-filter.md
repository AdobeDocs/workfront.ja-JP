---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Filter: Display Reports Scheduled for Delivery'
description: このレポートフィルターには、Adobe Workfront で自動的に配信されるようにスケジュールされたすべてのレポートが表示されます。 標準ビューを使用することが最適です。
author: Lisa and Courtney
feature: Reports and Dashboards
exl-id: 7b937384-80c9-4bc7-94be-5573cf86b35b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/OVEZ55Gkq3Q4uLGsQYetKMQNcbgRJgFOw1-kmfmPVzI
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 179
ht-degree: 88%

---

# フィルター：配信予定のレポートを表示

<!--Audited: 10/2024-->

このレポートフィルターには、Adobe Workfront で自動的に配信されるようにスケジュールされたすべてのレポートが表示されます。 標準ビューを使用することが最適です。

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

## レポート配信フィルター

このフィルターを適用するには、次の手順に従います。

1. レポートのリストに移動します。

1. **フィルター**&#x200B;ドロップダウンメニューから、「**新規フィルター**」を選択します。

1. 「**テキストモードに切り替え**」をクリックします。

1. **レポートのフィルタールールを設定**&#x200B;エリアに次のコードを追加します。

   ```
    scheduledReportsOM:ID_Mod=notblank
   ```

1. 「**フィルターを保存**」をクリックします。
