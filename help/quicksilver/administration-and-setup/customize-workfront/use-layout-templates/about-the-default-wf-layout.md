---
title: デフォルトのAdobe Workfront レイアウトについて
user-type: administrator
content-type: reference;overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: デフォルトのレイアウトでは、Adobe Workfront 管理者がレイアウトテンプレートを使用して変更を行う前に、メインメニュー、左側のパネル、表示、グループ化およびフィルターが配置されています。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: a68bca5e-1cec-432d-bb38-14b426a9c051
source-git-commit: 58a6b489ca5f1683a5c40c63bb4528b1f49e9324
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 43%

---

# デフォルトの Adobe Workfront レイアウトについて

デフォルトのレイアウトは、Adobe Workfront管理者がレイアウトテンプレートを使用して変更を加える前の、メインメニュー![&#x200B; メインメニューアイコン &#x200B;](assets/main-menu-icon-left-nav.png)、左パネル、ビュー、グループ化、フィルターの配置です。

Workfront 管理者がユーザーにレイアウトテンプレートを割り当ててユーザーのデフォルトレイアウトを変更する方法について詳しくは、[レイアウトテンプレートにユーザーを割り当て](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)を参照してください。

>[!NOTE]
>
>ユーザーは、ユーザープロファイルの環境設定を編集することで、自分のレイアウトを変更できます。詳しくは、[個人設定を行う](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md)の[環境設定](../../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md#preferences)の節を参照してください。

## 各ライセンスタイプのデフォルトのメインメニュー項目

各ユーザーのデフォルトのレイアウトは、ライセンスの種類によって異なります。 割り当てられているライセンスの種類によっては、メインメニューまたは特定の左パネル項目に特定の領域が表示されない場合があります。

組織が割り当てるライセンスには、次の2種類があります。

* 現在のライセンス
* レガシーライセンス

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

### 現在のライセンスタイプのデフォルトのメインメニュー

次の表は、デフォルトのメインメニュー項目と、現在のライセンスタイプごとに表示される左パネル項目を示しています。

<table class="tg"><thead>
  <tr>
    <th class="tg-fymr">領域</th>
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
    <td class="tg-0pky">ホーム <br>優先度</td>
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
    <td class="tg-0pky">自分のレポート <br>共有<br>すべてのレポート</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky">✔</td>
    <td class="tg-0pky"></td>
    <td class="tg-0pky">✔（左側のパネルの「自分と共有」とすべてのレポート）</td>
    <td class="tg-0pky"></td>
  </tr>
  <tr>
    <td class="tg-0pky">ダッシュボード</td>
    <td class="tg-0pky">マイダッシュボード <br>共有ダッシュボード <br>すべてのダッシュボード <br> キャンバスダッシュボード*</td>
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
    <td class="tg-0pky">プランナー<br> ワークロードバランサー<br>稼働率<br> リソースプール</td>
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
    <td class="tg-0pky">送信済み<br> ドラフト</td>
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
    <td class="tg-0pky">ホーム <br>優先度</td>
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
    <td class="tg-0pky">✔（機能が限定的）</td>
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

* この領域を表示するには、Canvas Dashboards betaに登録する必要があります。 詳しくは、[Canvas ダッシュボードのベータ情報](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md)を参照してください。

### 従来のライセンスタイプのデフォルトのメインメニュー

次の表は、デフォルトのメインメニュー項目と、レガシーライセンスの種類ごとに表示される左パネル項目を示しています。

<table class="tg"><thead>
  <tr>
    <th class="tg-0lax"><span style="font-weight:bold">領域</span></th>
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
    <td class="tg-0lax">ホーム <br>優先度</td>
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
    <td class="tg-0lax">自分のレポート <br>共有<br>すべてのレポート</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔</td>
    <td class="tg-0lax">✔（左側のパネルで自分とすべてのレポートと共有）</td>
    <td class="tg-0lax"></td>
    <td class="tg-0lax">✔（左側のパネルで自分とすべてのレポートと共有）</td>
    <td class="tg-0lax"></td>
  </tr>
  <tr>
    <td class="tg-0lax">ダッシュボード</td>
    <td class="tg-0lax">マイダッシュボード <br>共有ダッシュボード <br>すべてのダッシュボード <br> キャンバスダッシュボード*</td>
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
    <td class="tg-0lax">プランナー<br> ワークロードバランサー<br>稼働率<br> リソースプール</td>
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
    <td class="tg-0lax">送信済み<br> ドラフト</td>
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
    <td class="tg-0lax">ホーム <br>優先度</td>
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
    <td class="tg-0lax">✔（機能が限定的）</td>
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

* この領域を表示するには、Canvas Dashboards betaに登録する必要があります。 詳しくは、[Canvas ダッシュボードのベータ情報](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md)を参照してください。


