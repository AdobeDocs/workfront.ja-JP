---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: タイムシート情報を編集する
description: タイムシートへの管理アクセス権を持つユーザーは、Adobe Workfrontで既存のタイムシートに関する情報を編集できます。 例えば、所有者、承認者、またはタイムシートの期間を編集できます。
author: Lisa
feature: Timesheets
exl-id: e6cffe81-ab45-4c34-aafe-2f947f9a67fd
TQID: https://experienceleague.adobe.com/--QshuygnTfcEJtt6-Tx-2QtNT-5p9TrTWaQTMBZNAg
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
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
    internal-label: Customer experience
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: a3c1ab8fc8012199d9863fc978cca7418fa0a2f5
workflow-type: tm+mt
source-wordcount: '739'
ht-degree: 69%
---
# タイムシート情報を編集する

タイムシートへの管理アクセス権を持つユーザーは、Adobe Workfrontで既存のタイムシートに関する情報を編集できます。 例えば、所有者、承認者、またはタイムシートの期間を編集できます。

1 つのタイムシートの情報を編集することも、複数のタイムシートを一括編集することもできます。

>[!IMPORTANT]
>
>ユーザーがタイムシートプロファイルに関連付けられ、タイムシートが自動的に生成される場合、既存のタイムシートに対して行った変更は、将来の日付に対して生成されるタイムシートには反映されません。 自動的に生成されるすべてのタイムシートには、タイムシートプロファイルで確立された設定が含まれます。 詳しくは、[タイムシートプロファイルを作成](../create-and-manage-timesheets/create-timesheet-profiles.md)を参照してください。

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
   <td><p>タイムシートへの管理アクセス</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## タイムシートを編集する

{{step1-to-timesheets}}

表示するアクセス権のあるタイムシートはすべて、デフォルトで表示されます。

![&#x200B; タイムシート リスト &#x200B;](assets/list-of-all-timesheets.png)

1. （オプション） **検索** アイコン ![検索アイコン &#x200B;](assets/search-icon.png)をクリックし、特定のタイムシートを検索するキーワードを入力します。 例えば、タイムシートの期間または所有者名を検索できます。

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

1. 1つまたは複数のタイムシートを選択し、タイムシート リストの上部にある&#x200B;**編集** アイコン ![編集アイコン &#x200B;](assets/edit-icon.png)をクリックします。
1. 次の情報を表示または入力します。

   | フィールド名 | 説明 |
   | --------- | ---------- |
   | 所有者 | <p>これは、タイムシートが作成されたユーザーの名前です。 このフィールドは編集できません。</p><p>複数のタイムシートを選択した場合、このフィールドは表示されません。</p> |
   | 開始日 | これは、タイムシートの開始日です。 |
   | 終了日 | これは、タイムシートの終了日です。 |
   | ステータス | <p>これがタイムシートのステータスです。 タイムシートのステータスについて、次のオプションがあります。</p><ul><li>**オープン**：タイムシートを開いて、時間エントリを編集できます。</li><li>**送信済み**：指定された承認者にタイムシートが承認用に送信されます。</li><li>**却下**：タイムシートは承認者によって承認されず、ユーザーが時間エントリを編集できるようになりました。</li><li>**クローズ**：タイムシートは、ユーザーがクローズしたか、承認者が承認したためクローズされました。 クローズされたタイムシートに時間を追加することはできません。</li></ul> |
   | 承認者 | <p>承認者とは、タイムシートに関連付けられたユーザーのタイムシートを承認するユーザーです。 承認者として設定できるのは、タイムシートの管理権限を持つユーザーのみです。 タイムシート管理権限について詳しくは、[特定の領域に対する管理アクセス権をユーザーに付与](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)を参照してください。</p> <p>タイムシート承認者の名前の入力を開始し、リストに表示されたら、その名前を選択します。</p> <p>1 つのタイムシートに複数の承認者を設定できます。 この場合、承認者のうちの 1 人がタイムシートを承認すると、タイムシートは&#x200B;**クローズ**&#x200B;とマークされ、残りのすべての承認者のタイムシート承認リストに表示されなくなります。</p> |
   | 時間を編集可能 | <p>承認者がタイムシートの時間を編集できるようにする場合は、このオプションを選択します。</p><p>複数のタイムシートを選択した場合は、このオプションは使用できません。</p> |
   | 超過作業時間 | <p>タイムシートの「超過作業時間」ボックスを非表示にすることができます。</p><p>このオプションはデフォルトでは無効になっています。</p> |

1. 「**保存**」をクリックします。
