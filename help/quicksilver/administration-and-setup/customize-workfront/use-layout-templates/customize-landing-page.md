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
TQID: https://experienceleague.adobe.com/mZG3AgBJta1RtzQAIrXv-3jfkxS67SY-l-jhgeLZFVM
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: ce22a157-dd2c-405f-b740-c2f204bb4c1aid: d3382524-5489-431b-bde9-271ab257bc37id: e147ce9d-7675-49bd-8a32-44f27d865560id: fceb5125-bb41-419a-b0db-31958cb42f6c
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 395
ht-degree: 68%

---

# レイアウトテンプレートを使用してランディングページをカスタマイズ

Adobe Workfront 管理者は、レイアウトテンプレートを使用して、ユーザーが Workfront にログインしたときに表示するエリアを指定できます。

ユーザーは次のいずれかを開くことができます。

* 指定されたWorkfrontエリア
* カスタムダッシュボード：

レイアウトテンプレートの作成について詳しくは、[レイアウトテンプレートを作成および管理](../use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

グループのレイアウトテンプレートについて詳しくは、[グループのレイアウトテンプレートの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

レイアウトテンプレートを設定した後、変更を他のユーザーに表示するために、ユーザーに割り当てる必要があります。 レイアウトテンプレートのユーザーへの割り当てについて詳しくは、[ユーザーをレイアウトテンプレートに割り当てる](../use-layout-templates/assign-users-to-layout-template.md)を参照してください。

>[!NOTE]
>
>リクエストがランディングページとして設定されている場合、レイアウトテンプレートに割り当てられたコントリビューターまたはリクエスターユーザーは、代わりにホームページをランディングページとして表示します。 コントリビューターユーザーまたはリクエスターユーザーを対象としたレイアウトテンプレートのリクエスト以外のランディングページを選択することをお勧めします。

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
   >シナリオ、目標、およびプランニング領域を表示するには、追加のライセンスが必要です。
   >
   >* Workfront Goals について詳しくは、[Adobe Workfront Goals の概要](../../../workfront-goals/goal-management/wf-goals-overview.md)を参照してください。
   >
   >* Workfront のシナリオプランナーについて詳しくは、[シナリオプランナーの概要](../../../scenario-planner/scenario-planner-overview.md)を参照してください。
   >
   >* Workfront計画について詳しくは、[Adobe Workfront計画の基本を学ぶ](/help/quicksilver/planning/general/planning-overview.md)を参照してください。

1. レイアウトテンプレートのカスタマイズを続行します。 「**適用**」はいつでもクリックして、進行状況を保存できます。

   または

   カスタマイズが完了したら、**保存して閉じる**&#x200B;をクリックします。
