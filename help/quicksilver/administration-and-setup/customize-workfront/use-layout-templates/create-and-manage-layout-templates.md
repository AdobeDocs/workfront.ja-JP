---
title: レイアウトテンプレートの作成と管理
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: Workfront の管理者またはグループ管理者は、レイアウトテンプレートを作成および変更して、Workfront のレイアウト要素をユーザーに合わせてカスタマイズできます。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
source-git-commit: a79e4146ce6d076ef0e3707416a9c21d643b96e1
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 95%

---

# レイアウトテンプレートの作成と管理

<!--Audited: 12/2023-->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Adobe Workfront の管理者またはグループ管理者は、レイアウトテンプレートを作成および変更して、Workfront で次のレイアウト要素をユーザーに合わせてカスタマイズできます。

* メインメニュー
* 左側のナビゲーションパネル
* ホームエリア
* 担当者がリストやレポートで使用するビュー、フィルターおよびグループ化を示します。
* 画面上の用語
* プロジェクト、タスク、イシューのヘッダー

レイアウトテンプレートを作成または変更した後、個々のユーザー、チーム、グループまたは担当業務に割り当てることができます。

すべてのユーザーのデフォルトの Workfront レイアウトは、アクセスレベルとライセンスタイプに応じて異なります。例えば、一部のユーザーは、メインメニューに一部の領域が表示されない場合があります。詳しくは、[デフォルトの Adobe Workfront レイアウトについて](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td><p>新規：標準</p>
  <p> 現在：プラン</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>これらの手順をシステムレベルで実行するには、システム管理者のアクセスレベルが必要です。
グループに対して実行するには、そのグループの管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## レイアウトテンプレートの作成と管理に関する考慮事項

* ユーザーは、独自のレイアウトの一部の領域をカスタマイズできます。レイアウトテンプレートを変更すると、変更内容は、上書きやリセットを行わなくても、カスタマイズした内容と結合されます。このことは、ユーザーを新しいレイアウトテンプレートに割り当てる場合にも当てはまります。
* 他のユーザーを編集できるプランライセンスを持つグループ管理者とユーザーは、プロファイルの編集時に管理できるユーザーに対して、システムレベルおよびグループレベルのレイアウトテンプレートを追加できます。
* グループ管理者は、レイアウトテンプレートを担当業務やチームに割り当てることはできません。

レイアウトテンプレートについて詳しくは、[レイアウトテンプレート](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md)を参照してください。

<!--removed this from above, but keeping it for a bit, in case it will be needed - known issue around old templates still visible at time:
* Your older layout templates created in Adobe Workfront Classic have been automatically available in your instance of the new Adobe Workfront experience since they were migrated in early Fall 2019. Layout templates created in Adobe Workfront Classic after that time were migrated in April 2020. We recommend that you update these layout templates in the new Adobe Workfront experience to take advantage of new functionality and to make them even more useful in that environment.
-->

## レイアウトテンプレートを作成または変更

{{step-1-to-setup}}

1. 左側のパネルで、**インターフェイス**／**レイアウトテンプレート**&#x200B;をクリックします。

1. 「**新規レイアウトテンプレート**」をクリックします。

   または

   変更するレイアウトテンプレートの名前をクリックします。

1. 新しいレイアウトテンプレートを作成する場合は、**レイアウトテンプレート名**&#x200B;および（オプション）**説明**&#x200B;を入力します。

1. 次の記事の説明に従って、ユーザーインターフェイスの領域をカスタマイズします。

   * [レイアウトテンプレートを使用したメインメニューのカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [レイアウトテンプレートを使用して左のパネルをカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [レイアウトテンプレートを使用してピン留めされたページをカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [レイアウトテンプレートを使用して詳細ビューをカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [レイアウトテンプレートを使用してホームと概要をカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [レイアウトテンプレートを使用したランディングページのカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [レイアウトテンプレートを使用したフィルター、ビューおよびグループ化のカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [レイアウトテンプレートを使用したユーザーインターフェイスの用語のカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. 次の記事で説明するように、引き続きレイアウトテンプレートをテストし、ユーザーが使用できるようにします。

   * [ 新しいレイアウトテンプレートのテスト ](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [レイアウトテンプレートの管理アクセス権を付与](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [レイアウトテンプレートにユーザーを割り当て](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

>[!TIP]
>
>レイアウトテンプレートをコピーして、そのコピーを変更することで、新しいレイアウトテンプレートを作成することもできます。詳しくは、[レイアウトテンプレートをコピー](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md)を参照してください。

