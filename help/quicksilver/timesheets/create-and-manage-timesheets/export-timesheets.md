---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: タイムシートのリストを書き出し
description: 管理職またはタイムシート承認者は、担当する従業員のタイムシートに関する情報をすばやく表示するために、タイムシートのリストをダウンロードする必要がある場合があります。 これを行うには、タイムシートのリストを書き出します。
author: Lisa
feature: Timesheets
exl-id: cb5b1c6c-7800-48f4-ae2c-c4007a161a6c
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/-bihpKoVoPCwTpAj-SK-RPPFpaCubsyLAfnfSmpTnyI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
    internal-label: Approvals
  - id: ce22a157-dd2c-405f-b740-c2f204bb4c1a
    internal-label: Timesheets
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 64bb9e6dba8976ba413ec9b58e926da931bba1c5
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 63%
---
# タイムシートのリストを書き出し

<!--Audited: 8/2024-->

管理職またはタイムシート承認者は、担当する従業員のタイムシートに関する情報をすばやく表示するために、タイムシートのリストをダウンロードする必要がある場合があります。 これを行うには、タイムシートのリストを書き出します。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td> <p>明るいまたはそれ以上 </p>
   <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>タスクとイシューへのアクセス権を表示または高くする</p> </td> 
  </tr> 
  <tr> 
   <td>オブジェクト権限</td> 
   <td> <p>タスクとイシューに対する表示またはそれ以上の権限</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## タイムシートのリストを書き出し

{{step1-to-timesheets}}

表示するアクセス権のあるタイムシートはすべて、デフォルトで表示されます。

![&#x200B; タイムシート リスト &#x200B;](assets/list-of-all-timesheets.png)

1. （オプション）次のいずれかの操作を行って、タイムシートリストのフィルターを更新します。

   * ページの右上隅にある「**自分のタイムシートの承認**」を選択して、承認したタイムシートのみを表示します。

     または

     「**マイタイムシート**」を選択して、自分のタイムシートのみを表示する。

     これは、**マイタイムシート承認**&#x200B;または&#x200B;**マイタイムシート** フィルターをタイムシートのリストに適用します。

   * **フィルター** アイコン ![&#x200B; フィルターアイコン &#x200B;](assets/filter-nwepng.png)をクリックして、フィルターを適用するか、新しいフィルターを作成します。 フィルターの作成または更新について詳しくは、[Adobe Workfront でのフィルターの作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)を参照してください。

   >[!NOTE]
   >
   >Workfrontの管理者またはグループ管理者が設定エリアのリストコントロールまたはレイアウトテンプレートからこれらのフィルターを削除した場合、タイムシートリストの上部またはフィルターのリストに「マイタイムシートの承認」オプションと「マイタイムシート」オプションが表示されません。 詳しくは、[レイアウトテンプレートを使用したフィルター、ビューおよびグループ化のカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)を参照してください。

1. （オプション）「**ビュー** ![&#x200B; ビューのアイコン &#x200B;](assets/view-icon.png)」または「**グループ化** ![&#x200B; グループ化のアイコン &#x200B;](assets/grouping.png)」アイコンをクリックして、ビューまたはグループ化を適用するか、新しいビューを作成します。

   フィルター、ビューまたはグループ化の作成については、次の記事を参照してください。

   * [Adobe Workfront でフィルターを作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Adobe Workfront でビューを作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Adobe Workfront でのグループ化の作成](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. 書き出すタイムシートを選択し、**書き出し** ![書き出しアイコン &#x200B;](assets/export-38x15.png) アイコンをクリックします。

   ![書き出しアイコン &#x200B;](assets/export-timesheets.png)をクリックします

1. タイムシートの一覧を書き出すファイルの種類を次のオプションから選択します。

   * PDF 横
   * PDF 縦
   * PDF のその他のサイズ
   * Excel
   * Excel（xlsx）
   * タブ区切り

   タイムシートのリストは、選択した形式でコンピューターにダウンロードされ、次のタイムシート情報が含まれます。

   * 日付範囲
   * 所有者名
   * 合計時間数
   * 超過作業時間
   * 承認者名
   * ステータス
