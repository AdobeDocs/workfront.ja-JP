---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: タイムシートの手動生成
description: タイムシートプロファイルに加えた変更を現在のタイムシートに反映させるようにするには、まず既存のタイムシートを削除してから、新しいタイムシートを手動で生成する必要があります。 この記事で説明するように、タイムシートエリアまたは設定の診断エリアから、手動でタイムシートを生成できます。
author: Lisa
feature: Timesheets
exl-id: 316c270a-c64e-4d83-a035-4128abe33f87
TQID: https://experienceleague.adobe.com/0hU3VlHM8l5TXee6K3lJaV9-W3ZKujDYf9-f1NXH-Nc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 437
ht-degree: 73%

---

# タイムシートの手動生成

タイムシートプロファイルに加えた変更を現在のタイムシートに反映させるようにするには、まず既存のタイムシートを削除してから、新しいタイムシートを手動で生成する必要があります。 この記事で説明するように、タイムシートエリアまたは設定の診断エリアから、手動でタイムシートを生成できます。

タイムシートの削除手順については、[Adobe Workfrontのタイムシートを削除](../../timesheets/create-and-manage-timesheets/delete-timesheets.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto">
 <col> 
 <col>
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td>
   <p>標準</p>
   <p>プラン</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td><p>Workfront管理者である必要があります。または、グループのタイムシート プロファイルを作業する場合は、グループ管理者（またはWorkfront管理者）である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 手動で生成したタイムシートに関する考慮事項

タイムシートを手動で生成する場合、以下の手順を実行します。

* これらは、ユーザーに関連付けられたタイムシートプロファイルに従って生成されます。 タイムシートプロファイルが関連付けられていないユーザーは、タイムシートを受け取りません。
* 現在のタイムシートとその後のタイムシートのみが生成されます。 Workfront は、同じ期間に 2 つのタイムシートを生成しません。 現在のタイムシートが既にある場合、手動プロセスを使用してタイムシートを生成する際に、別のタイムシートは生成されません。

## タイムシートと時間領域からタイムシートを手動で生成する

「設定」の「タイムシートと時間」領域から、システムレベルまたはグループレベルのタイムシートを手動で生成できます。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックして、**設定** ![](assets/gear-icon-settings.png) をクリックします。

1. システム全体で使用中のタイムシートを生成する場合は、「**タイムシートと時間**」をクリックします。

   または

   特定のグループが使用するタイムシートを生成する場合は、「**グループ**」をクリックし、グループの名前をクリックします。

1. 「**定期タイムシート**」をクリックします。
1. 詳細アイコン ![詳細アイコン &#x200B;](assets/more-icon.png)をクリックし、**タイムシートを生成**&#x200B;します。

1. タイムシート プロファイルリストの上部で、システムレベルのタイムシート プロファイルの&#x200B;**More** アイコン ![More アイコン &#x200B;](assets/more-icon.png)、またはグループ タイムシート プロファイルの&#x200B;**More**&#x200B;をクリックし、**Generate timesheets**&#x200B;をクリックします。

   新しいタイムシートは、タイムシートプロファイルに関連付けられたユーザーに対して、最大 2 期間作成されます。

## 診断エリアからシステムレベルのタイムシートを手動で生成する

設定の診断エリアから、システムレベルのタイムシートを手動で生成できます。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、**設定** ![](assets/gear-icon-settings.png) をクリックします。

1. **システム**&#x200B;を展開し、「**診断**」をクリックします。

1. 「**診断を実行**」をクリックします。
1. 「**タイムシートの生成**」をクリックします。
