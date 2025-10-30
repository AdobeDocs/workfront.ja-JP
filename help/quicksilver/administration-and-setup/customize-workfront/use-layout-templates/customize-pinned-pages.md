---
title: レイアウトテンプレートを使用したピン留めページのカスタマイズ
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: レイアウトテンプレートでは、Adobe Workfront の上部に、ユーザーに常に利用できるようにしておきたいページをピン留めすることができます。これらは、メインメニューまたはダッシュボードからアクセスできるページです。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 55cc75c5-8b8c-48e7-b114-b41fe3d545d8
source-git-commit: a561620e218cafc0af861d2b157b8dc7c83dd7ed
workflow-type: tm+mt
source-wordcount: '572'
ht-degree: 58%

---

# レイアウトテンプレートを使用した固定されたページのカスタマイズ

{{preview-fast-release-general}}

レイアウトテンプレートでは、Adobe Workfront の上部に、ユーザーに常に利用できるようにしておきたいページをピン留めすることができます。これらのページは、メインメニュー ![&#x200B; メインメニューアイコン &#x200B;](assets/main-menu-icon.png) またはメインメニュー ![&#x200B; メインメニューアイコン &#x200B;](assets/main-menu-icon-left-nav.png) （使用可能な場合）からアクセスするページ、ダッシュボードのいずれかです。

ユーザーが独自に追加したピン留めは、レイアウト テンプレートに追加したピン留めの右側に表示されます。

ページのピン留めの詳細については、[ページを固定してワークスペースをカスタマイズ](../../../workfront-basics/the-new-workfront-experience/pin-pages.md)を参照してください。

レイアウトテンプレートについて詳しくは、[レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

グループのレイアウトテンプレートについて詳しくは、[グループのレイアウトテンプレートの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

レイアウトテンプレートを設定した後、変更を他のユーザーに表示するために、ユーザーに割り当てる必要があります。レイアウトテンプレートのユーザーへの割り当てについて詳しくは、[ユーザーのレイアウトテンプレートへの割り当て](../use-layout-templates/assign-users-to-layout-template.md)を参照してください。

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
   <td><p>標準</p>
       <p>プラン</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>これらの手順をシステムレベルで実行するには、システム管理者のアクセスレベルが必要です。</p>
        <p>グループに対して実行するには、そのグループの管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## レイアウトテンプレートを使用してページをピン留め

1. [レイアウトテンプレートを作成および管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)で説明されるように、レイアウトテンプレート上での作業を開始します。
1. **上部ナビゲーションエリア**&#x200B;の下で、「**新しいピン留めを追加**」をクリックします。

1. 表示されるドロップダウンメニューで、以下のいずれかを行います。

   * 次の領域から選択します。

      * カレンダー
      * ダッシュボード
      * ドキュメント
      * Goals
      * ホーム
      * マイ更新
      * ポートフォリオ
      * プログラム
      * プロジェクト
      * レポート
      * リクエスト
      * リソース
      * シナリオ
      * チーム
      * テンプレート
      * タイムシート
      * ユーザー
      * ブループリント
      * プラン

     >[!IMPORTANT]
     >
     >目標、シナリオおよび計画領域を表示するには、追加のライセンスが必要です。
     >
     >* Workfront Goals について詳しくは、[Adobe Workfront Goals の概要](../../../workfront-goals/goal-management/wf-goals-overview.md)を参照してください。
     >
     >* Workfront のシナリオプランナーについて詳しくは、[シナリオプランナーの概要](../../../scenario-planner/scenario-planner-overview.md)を参照してください。
     >
     >* Workfront計画について詳しくは、[Adobe Workfront計画の概要 &#x200B;](/help/quicksilver/planning/general/planning-overview.md) を参照してください。

   * 「**ダッシュボードを追加**」をクリックします
      * &#x200B;<!--**Quick link name**-->**カスタム名** フィールドにわかりやすい名前を入力します
      * 「**ダッシュボードを追加**」フィールドでダッシュボードを選択し <!-- dropdown for existing or canvas dashboard, called "Choose a dashboard" now --> す
      * 「**追加**」をクリックします。

1. 前の手順を繰り返して、他のページをピン留めします。

1. （オプション）ピンを移動するには、ピンにポインタを合わせて、ピン名の横にある「詳細」メニューアイコン ![&#x200B; その他のアイコン &#x200B;](assets/more-icon.png) その他のアイコン）をクリックします。次に、**左に移動** または **右に移動** をクリックして、選択した方向にピンを移動するか、**前に移動** をクリックして、ピンを一番左の位置に移動します。

1. （オプション）ピン留めの名前を変更するには、ピンにポインタを合わせて、ピン名の横にある「詳細」メニューアイコン ![&#x200B; 詳細アイコン &#x200B;](assets/more-icon.png) をクリックし、「**ピン留めの名前を変更**」をクリックします。 新しい名前を入力し、「**保存**」をクリックします。

1. （オプション）ピン留めを削除するには、ピンにポインタを合わせ、ピン名の横にある「詳細」メニューアイコン ![&#x200B; 詳細アイコン &#x200B;](assets/more-icon.png) をクリックしてから、「**ピン留めを削除** をクリックします。

1. <span class="preview"> プレビュー環境の場合：レイアウトテンプレートのカスタマイズを続行します。 「**適用**」をクリックすると、いつでも進捗を保存できます。</span>

   <span class="preview">または</span>

   <span class="preview"> カスタマイズが終了したら、「**保存して閉じる** をクリックします。</span>

1. 実稼動環境の場合：レイアウトテンプレートのカスタマイズを続行します。

   または

   カスタマイズが終了したら、「**保存**」をクリックします。

   >[!TIP]
   >
   >いつでも「**保存**」をクリックして進行状況を保存して、後でテンプレートの変更を続行できます。
