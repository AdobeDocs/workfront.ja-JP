---
title: レイアウトテンプレートを使用したピン留めページのカスタマイズ
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: レイアウトテンプレートでは、Adobe Workfront の上部に、ユーザーに常に利用できるようにしておきたいページをピン留めすることができます。これらは、メインメニューまたはダッシュボードからアクセスできるページです。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 55cc75c5-8b8c-48e7-b114-b41fe3d545d8
source-git-commit: 1768c0610eb459148ff3e51ed08c115053c7d8f7
workflow-type: tm+mt
source-wordcount: '516'
ht-degree: 91%

---

# レイアウトテンプレートを使用した固定されたページのカスタマイズ

レイアウトテンプレートでは、Adobe Workfront の上部に、ユーザーに常に利用できるようにしておきたいページをピン留めすることができます。これらは、メイン メニュー ![](assets/main-menu-icon.png) またはダッシュボードからアクセスできるページです。

ユーザーが独自に追加したピン留めは、レイアウト テンプレートに追加したピン留めの右側に表示されます。

ページのピン留めの詳細については、[ページを固定してワークスペースをカスタマイズ](../../../workfront-basics/the-new-workfront-experience/pin-pages.md)を参照してください。

レイアウトテンプレートについて詳しくは、[レイアウトテンプレートの作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

グループのレイアウトテンプレートについて詳しくは、[グループのレイアウトテンプレートの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

レイアウトテンプレートを設定した後、変更を他のユーザーに表示するために、ユーザーに割り当てる必要があります。レイアウトテンプレートのユーザーへの割り当てについて詳しくは、[ユーザーのレイアウトテンプレートへの割り当て](../use-layout-templates/assign-users-to-layout-template.md)を参照してください。

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
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>これらの手順をシステムレベルで実行するには、システム管理者のアクセスレベルが必要です。
グループに対して実行するには、そのグループの管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## レイアウトテンプレートを使用してページをピン留め

1. [レイアウトテンプレートを作成および管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)で説明されるように、レイアウトテンプレート上での作業を開始します。
1. **上部ナビゲーションエリア**&#x200B;の下で、「**新しいピン留めを追加**」をクリックします。

1. 表示されるドロップダウンメニューで、以下のいずれかを行います。

   * 次の領域から選択します。

      * 分析
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
   >シナリオ、目標および計画領域を表示するには、追加のライセンスが必要です。
   >
   >* Workfront Goals について詳しくは、[Adobe Workfront Goals の概要](../../../workfront-goals/goal-management/wf-goals-overview.md)を参照してください。
   >
   >* Workfront のシナリオプランナーについて詳しくは、[シナリオプランナーの概要](../../../scenario-planner/scenario-planner-overview.md)を参照してください。
   >
   >* Workfront計画について詳しくは、[Adobe Workfront計画の概要 ](/help/quicksilver/planning/general/planning-overview.md) を参照してください。

   * **ダッシュボードを追加**&#x200B;をクリックし、次に、説明的な&#x200B;**カスタムセクションのタイトル**&#x200B;を入力し、ダッシュボードを追加します。

1. 前の手順を繰り返して、他のページをピン留めします。

1. （オプション）ピン留めの名前を変更するには、ピン留めにポインタを合わせ、ピン留め名の横の矢印をクリックして、「**ピン留めの名前を変更**」を選択します。新しいピン留め名を入力し、「チェックマーク」アイコンをクリックするか、Enter を押します。

   チェックマークをクリックした後、または Enter を押した後、小さなポップアップウィンドウが数秒間表示され、保存する前にピン留め名の変更を元に戻すことができます。

1. 引き続きレイアウトテンプレートをカスタマイズします。

   または

   カスタマイズが終了したら、「**保存**」をクリックします。

   >[!TIP]
   >
   >いつでも「**保存**」をクリックして進行状況を保存して、後でテンプレートの変更を続行できます。
