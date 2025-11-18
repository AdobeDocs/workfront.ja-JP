---
title: レイアウトテンプレートを使用したランディングページのカスタマイズ
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Workfront 管理者は、レイアウトテンプレートを使用して、Workfront へのログイン時にユーザーに表示するエリアを指定できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 57a1046a-434a-4453-a101-c5f0a16e079e
source-git-commit: 96028446d76f32daf512adf77d3b1c53021821ec
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 67%

---

# レイアウトテンプレートを使用してランディングページをカスタマイズ

{{preview-fast-release-general}}

Adobe Workfront 管理者は、レイアウトテンプレートを使用して、ユーザーが Workfront にログインしたときに表示するエリアを指定できます。

ユーザーは、次のいずれかを開くことができます。

* Workfront指定地域
* カスタムダッシュボード。

レイアウトテンプレートの作成について詳しくは、[レイアウトテンプレートを作成および管理](../use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

グループのレイアウトテンプレートについて詳しくは、[グループのレイアウトテンプレートを作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

レイアウトテンプレートを設定した後、変更を他のユーザーに表示するために、ユーザーに割り当てる必要があります。レイアウトテンプレートのユーザーへの割り当てについて詳しくは、[ユーザーをレイアウトテンプレートに割り当てる](../use-layout-templates/assign-users-to-layout-template.md)を参照してください。

>[!NOTE]
>
>リクエストがランディングページとして設定されている場合、レイアウトテンプレートに割り当てられた投稿者または依頼者ユーザーには、代わりにホームページがランディングページとして表示されます。 投稿者または依頼者ユーザー向けのレイアウトテンプレートの場合は、リクエスト以外のランディングページを選択することをお勧めします。

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
   <td><p>Standard</p>
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

## ランディングページのカスタマイズ

1. [レイアウトテンプレートを作成および管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)で説明されているように、レイアウトテンプレートの使用を開始します。
1. Adobe Analytics の **ナビゲーション領域上部**&#x200B;で、「**ランディングページを選択**」をクリックし、ユーザーがログインしたときに表示するエリアを選択します。

   次の領域から選択するか、カスタムダッシュボードを追加します。

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
   >* Workfront Planning については、[Adobe Workfront Planning の基本を学ぶ &#x200B;](/help/quicksilver/planning/general/planning-overview.md) を参照してください。

1. <span class="preview"> プレビュー環境の場合：レイアウトテンプレートのカスタマイズを続行します。 「**適用**」をクリックすると、いつでも進捗を保存できます。</span>

   <span class="preview">または</span>

   <span class="preview"> カスタマイズが終了したら、「**保存して閉じる** をクリックします。</span>

1. 実稼動環境の場合：レイアウトテンプレートのカスタマイズを続行します。

   または

   カスタマイズが終了したら、「**保存**」をクリックします。

   >[!TIP]
   >
   >いつでも「**保存**」をクリックして進行状況を保存して、後でテンプレートの変更を続行できます。
