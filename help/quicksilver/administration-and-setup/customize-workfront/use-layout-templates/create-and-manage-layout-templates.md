---
title: レイアウトテンプレートの作成と管理
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: Workfrontの管理者またはグループ管理者は、レイアウトテンプレートを作成および変更して、Workfrontのレイアウト要素をユーザーに合わせてカスタマイズできます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# レイアウトテンプレートの作成と管理

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Workfrontの管理者またはグループ管理者は、レイアウトテンプレートを作成および変更して、Workfrontで次のレイアウト要素をユーザーに合わせてカスタマイズできます。

* メインメニュー
* 左側のナビゲーションパネル
* ホームエリア
* 担当者がリストやレポートで使用するビュー、フィルター、グループ化を示します。
* 画面上の用語

レイアウトテンプレートを作成または変更した後、個々のユーザー、チーム、グループまたはジョブの役割に割り当てることができます。

すべてのユーザーのデフォルトのWorkfrontレイアウトは、アクセスレベルとライセンスの種類に応じて異なります。 例えば、一部のユーザーは、メインメニューに一部の領域が表示されない場合があります。 詳しくは、 [デフォルトのAdobe Workfrontレイアウトについて](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>これらの手順をシステムレベルで実行するには、システム管理者のアクセスレベルが必要です。
グループに対して実行するには、そのグループの管理者である必要があります。</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## レイアウトテンプレートの作成と管理に関する考慮事項

* ユーザーは、独自のレイアウトの一部の領域をカスタマイズできます。 レイアウトテンプレートを変更すると、変更内容は、上書きやリセットを行わずに、カスタマイズした内容とマージされます。 これは、ユーザーを新しいレイアウトテンプレートに割り当てる場合にも当てはまります。
* 2019 年秋初めに移行されたので、Adobe Workfront Classic で作成した古いレイアウトテンプレートは、新しいAdobe Workfrontエクスペリエンスのインスタンスで自動的に使用できるようになりました。 その後、Adobe Workfront Classic で作成されたレイアウトテンプレートは、2020 年 4 月に移行されました。 新しいAdobe Workfrontエクスペリエンスでこれらのレイアウトテンプレートを更新して、新しい機能を活用し、その環境でより役に立つようにすることをお勧めします。
* 他のユーザを編集できるプランライセンスを持つグループ管理者とユーザは、プロファイルの編集時に管理できるユーザに対して、システムレベルおよびグループレベルのレイアウトテンプレートを追加できます。
* グループ管理者は、レイアウトテンプレートをジョブの役割やチームに割り当てることはできません。

レイアウトテンプレートについて詳しくは、 [レイアウトテンプレート](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

## レイアウトテンプレートの作成または変更

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **インターフェイス** > **レイアウトテンプレート**.

1. クリック **新規レイアウトテンプレート**.

   または

   変更するレイアウトテンプレートの名前をクリックします。

1. 新しいレイアウトテンプレートを作成する場合は、 **レイアウトテンプレート名** および（オプション） a **説明** それに対して

1. 次の記事の説明に従って、ユーザーインターフェイスの領域をカスタマイズします。

   * [レイアウトテンプレートを使用したメインメニューのカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [レイアウトテンプレートを使用して左のパネルをカスタマイズする](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [レイアウトテンプレートを使用して固定されたページをカスタマイズする](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [レイアウトテンプレートを使用して詳細ビューをカスタマイズする](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [レイアウトテンプレートを使用してホームと概要をカスタマイズする](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [レイアウトテンプレートを使用したランディングページのカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [レイアウトテンプレートを使用したフィルター、ビューおよびグループのカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [レイアウトテンプレートを使用したユーザインターフェイスの用語のカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. 次の記事で説明するように、引き続きレイアウトテンプレートをテストし、ユーザーが使用できるようにします。

   * [新しいレイアウトテンプレートのテスト](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [レイアウトテンプレートの管理アクセス権の付与](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [レイアウトテンプレートにユーザーを割り当てる](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

新しいレイアウトテンプレートをコピーして、コピーを変更することで、新しいレイアウトテンプレートを作成することもできます。 詳しくは、 [レイアウトテンプレートのコピー](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).
