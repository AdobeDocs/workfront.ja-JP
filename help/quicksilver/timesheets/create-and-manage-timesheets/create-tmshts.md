---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: 1回限りのタイムシートの作成
description: 定期的でないタイムシートが必要な場合は、1 回限りのタイムシートを手動で作成できます。 タイムシートの終了日に達し、より多くのタイムシートが必要になった場合は、新しいタイムシートを作成する必要があります。
author: Lisa
feature: Timesheets
exl-id: b293dd50-a9b8-448b-afc1-8c7c7c79183b
TQID: https://experienceleague.adobe.com/6ngmKzkpxxHYM7L9Z16JsJKcEW7CdFjJcdp6B6hgTtc
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
source-wordcount: '1048'
ht-degree: 79%
---
# 単一のタイムシートの作成

<!--Audited: 6/2025-->

定期的でないタイムシートが必要な場合は、1 回限りのタイムシートを手動で作成できます。 タイムシートの終了日に達し、より多くのタイムシートが必要になった場合は、新しいタイムシートを作成する必要があります。

ユーザーからの追加の介入なしに（推奨）、定期的なタイムシートを生成するタイムシートプロファイルの作成について詳しくは、[タイムシートプロファイルの作成、編集、割り当て](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)を参照してください。

タイムシート プロファイルに関連付けられているシステム内のすべてのユーザーのタイムシートを手動で生成する方法については、[手動でタイムシートを生成する](/help/quicksilver/timesheets/create-and-manage-timesheets/manually-generate-timesheets.md)を参照してください。

>[!NOTE]
>
>* 1 回限りのタイムシートは、グループに対して作成できません。
>* 1 回限りのタイムシートを作成する場合、タイムシートに含める特定の一般的な時間タイプを選択することはできません。 システムで有効化されたすべての一般的な時間タイプは、手動で作成されたタイムシートに表示されます。
>
>タイムシートに表示する特定の一般的な時間タイプのみを選択する場合は、タイムシートプロファイルを使用します。 タイムシートプロファイルについて詳しくは、[タイムシートプロファイルの作成、編集、割り当て](../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md)を参照してください。

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

## 単一のタイムシートの作成

{{step1-to-timesheets}}

表示するアクセス権のあるタイムシートはすべて、デフォルトで表示されます。

![ タイムシート リスト ](assets/list-of-all-timesheets.png)

1. （オプション）次のいずれかの操作を行って、タイムシートリストのフィルターを更新します。

   * ページの右上隅にある「**自分のタイムシートの承認**」を選択して、承認したタイムシートのみを表示します。

     または

     「**マイタイムシート**」を選択して、自分のタイムシートのみを表示する。

     これは、**マイタイムシート承認**&#x200B;または&#x200B;**マイタイムシート** フィルターをタイムシートのリストに適用します。

   * **フィルター** アイコン ![ フィルターアイコン ](assets/filter-nwepng.png)をクリックして、フィルターを適用するか、新しいフィルターを作成します。 フィルターの作成または更新について詳しくは、[Adobe Workfront でのフィルターの作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)を参照してください。

   >[!NOTE]
   >
   >Workfront 管理者またはグループ管理者が、設定エリアのリスト制御またはレイアウトテンプレートから、「マイタイムシート承認」と「マイタイムシート」のフィルターを削除した場合、「マイタイムシート承認」と「マイタイムシート」のオプションは、タイムシート一覧の先頭にもフィルター一覧にも表示されません。 詳しくは、[レイアウトテンプレートを使用したフィルター、ビューおよびグループ化のカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)を参照してください。

1. （オプション） **検索** アイコン ![検索アイコン ](assets/search-icon.png)をクリックしてキーワードを入力し、特定のタイムシートを検索します。 例えば、所有者名のタイムシート期間を検索できます。

1. （オプション）「**ビュー** ![ ビューのアイコン ](assets/view-icon.png)」または「**グループ化** ![ グループ化のアイコン ](assets/grouping.png)」アイコンをクリックして、ビューまたはグループ化を適用するか、新しいビューを作成します。

   フィルター、ビューまたはグループ化の作成については、次の記事を参照してください。

   * [Adobe Workfront でフィルターを作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-filters.md)
   * [Adobe Workfront でビューを作成または編集](../../reports-and-dashboards/reports/reporting-elements/create-edit-views.md)
   * [Adobe Workfront でのグループ化の作成](../../reports-and-dashboards/reports/reporting-elements/create-groupings.md)

1. タイムシートのリストの上部にある「**新規タイムシート**」をクリックします。

   次の情報を入力します。

   | フィールド名 | 説明 |
   | --------- | ---------- |
   | 次のタイムシートを作成 : | 作成するタイムシートの対象となるユーザー、担当業務またはチームの名前を入力していき、リストに表示されたら名前をクリックします。 |
   | 開始日 | これは、タイムシートの開始日です。 |
   | 終了日 | これは、タイムシートの終了日です。 |
   | 承認者 | <p>承認者とは、タイムシートに関連付けられたユーザーのタイムシートを承認するユーザーです。 承認者として設定できるのは、タイムシートの管理権限を持つユーザーのみです。 タイムシート管理権限について詳しくは、[特定の領域に対する管理アクセス権をユーザーに付与](/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)を参照してください。</p> <p>タイムシート承認者の名前の入力を開始し、リストに表示されたら、その名前を選択します。</p> <p>1 つのタイムシートに複数の承認者を設定できます。 この場合、承認者のうちの 1 人がタイムシートを承認すると、タイムシートは&#x200B;**クローズ**&#x200B;とマークされ、残りのすべての承認者のタイムシート承認リストに表示されなくなります。</p> |
   | 時間を編集可能 | <p>承認者がタイムシートの時間を編集できるようにする場合は、このオプションを選択します。</p><p>このオプションは、設定／タイムシートと時間／環境設定エリアの「**タイムシートの編集を所有者と管理者に制限**」設定と連携して機能します。 詳しくは、[タイムシートと時間の環境設定の構成](/help/quicksilver/administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)を参照してください。</p><p>次のシナリオが存在します。</p><p>「**タイムシートの編集を所有者と管理者に制限**」オプションが有効な場合は、以下のようになります。</p><ul><li>承認者は、**時間を編集できます**&#x200B;が有効かどうかに関係なく、タイムシートのみを承認および却下できます。</li><li>タイムシート所有者のマネージャーは、自分のダイレクトレポートのタイムシートのみを表示できます。</li></ul><p>「**タイムシートの編集を所有者と管理者に制限**」オプションが無効である場合は、以下のようになります。</p><ul><li>**時間を編集できます**&#x200B;が有効になっている場合、承認者はタイムシートを送信、再オープン、または閉じることができ、時間を編集できます。</li><li>**時間を編集できます**&#x200B;が無効になっている場合、承認者はタイムシートを送信、再オープン、または閉じることができず、時間を編集できません。 承認者が行えるのは、タイムシートの承認または却下のみです。</li><li>タイムシート所有者のマネージャーは、ダイレクトレポートのタイムシートの提出、取り消し、リオープン、編集を行うことができます。</li></ul><p>**メモ**</br>&#x200B;承認のためにタイムシートを送信すると、時間を編集できなくなります。 提出されたタイムシートを編集可能な状態に戻すには、タイムシートを取り消すか、承認者にタイムシートを却下させます。 詳しくは、[承認を受けるためのタイムシートの送信](/help/quicksilver/timesheets/create-and-manage-timesheets/submit-timesheet-for-approval.md)と[タイムシートの承認](/help/quicksilver/timesheets/create-and-manage-timesheets/timesheet-approvals.md)を参照してください。 |
   | 超過作業時間 | タイムシートの「**残業**」ボックスを非表示にすることができます。 このオプションはデフォルトでは無効になっています。 |

1. 「**タイムシートを作成**」をクリックします。

## タスクとイシューがユーザーのタイムシートに表示される条件

タスクやイシューが次の条件のいずれかに一致する場合、ユーザーに割り当てられたタスクやイシューは、ユーザーのタイムシートに自動的に表示されます。

* ユーザーがタスクやイシューに費やした時間数を記録した
* タスクやイシューの予定日がタイムシートの日付範囲内に収まる
* タスクやイシューに実際の開始日がある（タスクやイシューのステータスは「処理中」）
* タスクやイシューがタイムシートにピン留めされている
* 予定完了日がタイムシートの日付範囲内に収まり、そのステータスが「処理中」になっている

**次以内の作業についてタイムシートを自動入力する**」環境設定（「タイムシートと時間」環境設定にある）が選択されていない場合、タイムシートには「処理中」のステータスを持つイシューとタスクが表示されます。 「タイムシートと時間」環境設定について詳しくは、[タイムシートと時間の環境設定](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/timesheet-and-hour-preferences.md)を参照してください。
