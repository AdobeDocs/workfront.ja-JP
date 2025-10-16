---
title: デフォルトのAdobe Workfrontのレイアウトについて
user-type: administrator
content-type: reference;overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: デフォルトのレイアウトでは、Adobe Workfront 管理者がレイアウトテンプレートを使用して変更を行う前に、メインメニュー、左側のパネル、表示、グループ化およびフィルターが配置されています。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: a68bca5e-1cec-432d-bb38-14b426a9c051
source-git-commit: 76e32fa6b87583d2b8c296045da731afdb6d1f9a
workflow-type: tm+mt
source-wordcount: '614'
ht-degree: 42%

---

# デフォルトの Adobe Workfront レイアウトについて

デフォルトのレイアウトは、Adobe Workfront管理者がレイアウトテンプレートを使用して変更を行う前に、メインメニュー ![ メインメニューアイコン ](assets/main-menu-icon.png) またはメインメニュー ![ メインメニューアイコン ](assets/main-menu-icon-left-nav.png) （使用可能な場合）の左側のパネル、ビュー、グループ化、フィルターが配置されます。

Workfront 管理者がユーザーにレイアウトテンプレートを割り当ててユーザーのデフォルトレイアウトを変更する方法について詳しくは、[レイアウトテンプレートにユーザーを割り当て](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)を参照してください。

>[!NOTE]
>
>ユーザーは、ユーザープロファイルの環境設定を編集することで、自分のレイアウトを変更できます。詳しくは、[個人設定を行う](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)の[環境設定](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md#preferences)の節を参照してください。

## 各ライセンスの種類の既定のメイン メニュー項目

各ユーザーのデフォルトのレイアウトは、ユーザーのライセンスタイプによって異なります。 割り当てられているライセンスの種類に応じて、メインメニューの特定の領域や左側のパネル項目が表示されないことがあります。

組織が割り当てるライセンスには、次の 2 種類があります。

* 新しいライセンス
* 現在のライセンス

<!--rename the above if we change Current to Legacy-->

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

### 現在のライセンスの種類に対する既定のメイン メニュー

次の表に、現在の各ライセンス タイプの既定のメイン メニュー項目と左パネル項目の表示内容を示します。

<table class="tg"><thead>
  <tr>
    <th class="tg-0lax"><span style="font-weight:bold">エリア</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">左側のパネル項目</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">システム管理者</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">プランナー</span></th>
    <th class="tg-0lax"><span style="font-weight:bold">作業者</span></th>
    <th class="tg-1wig">レビュアー</th>
    <th class="tg-1wig">依頼者</th>
    <th class="tg-1wig">外部ユーザー</th>
  </tr></thead>
<tbody>
  <tr>
    <td class="tg-0lax">ホーム</td>
    <td class="tg-0lax">ホーム <br> 優先度</td>
    <td class="tg-0lax">✔（デフォルトのランディングページ）</td>
    <td class="tg-0lax">✔（デフォルトのランディングページ）</td>
    <td class="tg-0lax">✔（デフォルトのランディングページ）</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">プロジェクト</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔ </td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">ポートフォリオ</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">プログラム</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">レポート</td>
    <td class="tg-0lax">自分の報告書 <br> 自分と共有 <br> すべての報告書</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔（左側のパネルの「自分と共有」および「すべてのレポート」）</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔（左側のパネルの「自分と共有」および「すべてのレポート」）</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">ダッシュボード</td>
    <td class="tg-0lax">マイダッシュボード <br> 共有ダッシュボード <br> すべてのダッシュボード <br> キャンバスダッシュボード*</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">カレンダー</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">リソース</td>
    <td class="tg-0lax">プランナー <br> ワークロードバランサー <br> 稼働率 <br> リソースプール</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔（左側のパネルのプランナーとリソースプール）</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">チーム</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">ユーザー</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">リクエスト</td>
    <td class="tg-0lax">Submitted<br>Drafts</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">タイムシート</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">ドキュメント</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">テンプレート</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">シナリオ</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">ボード</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">ブループリント</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔（インストール機能）</td>
    <td class="tg-0lax">✔（リクエスト機能のみ）</td>
    <td class="tg-0lax">✔（リクエスト機能のみ）</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">優先度</td>
    <td class="tg-0lax">ホーム <br> 優先度</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔<br></td>
  </tr>
  <tr>
    <td class="tg-0lax">設定</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔（機能が制限されています）</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">マイ更新</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔（デフォルトのランディングページ）</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax"></td>
  </tr>

</tbody></table>

*この領域を表示するには、キャンバスダッシュボードベータ版に登録している必要があります。 詳しくは、[ キャンバスダッシュボードのベータ版情報 ](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md) を参照してください。

### 新しいライセンスの種類の既定のメイン メニュー

次の表に、既定のメイン メニュー項目と、新しいライセンスの種類ごとに表示される左側のパネル項目を示します。

<table class="tg"><thead>
  <tr>
    <th class="tg-fymr">エリア</th>
    <th class="tg-fymr">左側のパネル項目</th>
    <th class="tg-fymr">システム管理者</th>
    <th class="tg-fymr">標準</th>
    <th class="tg-fymr">ライト</th>
    <th class="tg-fymr">コントリビューター</th>
    <th class="tg-fymr">外部ユーザー</th>
  </tr></thead>
<tbody>
  <tr>
    <td class="tg-0pky">ホーム</td>
    <td class="tg-0pky">ホーム <br> 優先度</td>
    <td class="tg-0pky">✔（デフォルトのランディングページ）</td>
    <td class="tg-0pky">✔（デフォルトのランディングページ）</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔（デフォルトのランディングページ）</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">プロジェクト</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔ </td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">ポートフォリオ</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">プログラム</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">レポート</td>
    <td class="tg-0pky">自分の報告書 <br> 自分と共有 <br> すべての報告書</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔（自分と共有され、左側のパネルのすべてのレポート）</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">ダッシュボード</td>
    <td class="tg-0pky">マイダッシュボード <br> 共有ダッシュボード <br> すべてのダッシュボード <br> キャンバスダッシュボード*</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">カレンダー</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">リソース</td>
    <td class="tg-0pky">プランナー <br> ワークロードバランサー <br> 稼働率 <br> リソースプール</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">チーム</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">ユーザー</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">リクエスト</td>
    <td class="tg-0pky">Submitted<br>Drafts</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">タイムシート</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">ドキュメント</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">テンプレート</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">シナリオ</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">ボード</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">ブループリント</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔（インストール機能）</td>
    <td class="tg-0pky">✔（リクエスト機能のみ）</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">優先度</td>
    <td class="tg-0pky">ホーム <br> 優先度</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔<br></td>
  </tr>
  <tr>
    <td class="tg-0pky">設定</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔（機能が制限されています）</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">マイ更新</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔（デフォルトのランディングページ）</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
  </tr>
</tbody></table>

*この領域を表示するには、キャンバスダッシュボードベータ版に登録している必要があります。 詳しくは、[ キャンバスダッシュボードのベータ版情報 ](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md) を参照してください。

<!--

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th>Area</th> 
   <th> Left panel items </th> 
   <th> System Administrator</th> 
   <th> Planner </th> 
   <th>Worker</th> 
   <th>Reviewer</th> 
   <th>Requestor</th> 
   <th>External User</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td rowspan="2"><strong>Projects</strong> </td> 
   <td><strong>Projects</strong> </td> 
   <td>✔ <br>(Default landing area)</td> 
   <td><span style="font-weight: 400;"> ✔</span> <br>(Default landing area)</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Portfolios</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td rowspan="3"><strong>Reporting</strong> </td> 
   <td><strong>Reports</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Dashboards</strong> </p> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Calendars</strong> </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td rowspan="5"><strong>People</strong> (renamed to <strong>Teams</strong> for users with a Work license)</td> 
   <td><strong>Teams</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>People</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Planning</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Scheduling</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td rowspan="3"><strong>Requests</strong> </td> 
   <td>New Request </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td><strong>Requests I've Submitted</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ <br>(Default landing area)</td> 
   <td>✔ <br>(Default landing area)</td> 
  </tr> 
  <tr> 
   <td><strong>All Requests</strong> </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
  </tr> 
  <tr> 
   <td rowspan="3"><strong>Timesheet</strong> </td> 
   <td><strong>My Timesheets</strong> </td> 
   <td>✔ </td> 
   <td> ✔</td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Timesheets I Approve</strong> </td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>All Timesheets</strong> </td> 
   <td>✔</td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Documents</strong> </td> 
   <td>&nbsp;</td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>✔ </td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
  <tr> 
   <td><strong>Setup</strong> </td> 
   <td>&nbsp;</td> 
   <td>✔ </td> 
   <td>Limited Functionality</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
   <td>&nbsp;</td> 
  </tr> 
 </tbody> 
</table>
-->
