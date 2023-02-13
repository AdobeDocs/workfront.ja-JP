---
product-area: resource-management
navigation-topic: resource-planning
title: リソース・プランナの検索
description: 「( この記事は以下のものから出てきました。この記事が公開されたときに記事の内容を下書きします。/Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)'
author: Alina
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '512'
ht-degree: 0%

---

# リソース・プランナの検索

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

リソース・プランナを使用して、プロジェクトへのリソースの割り当てを管理できます。 複数のプロジェクトのリソース・プランナに同時にアクセスするか、1 つのプロジェクトの場合は、プロジェクトの「ビジネス・ケース」領域からアクセスできます。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>レビュー以上<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> <p>グローバル・エリアにリソース・プランナを配置するには、計画を立てるか、それ以上を設定します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>リソース管理へのアクセス権以上の表示</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトおよびユーザーに対する権限を表示 </p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

リソースプランナーにアクセスし、使用するためのすべての前提条件が満たされていることを確認してから、使用を開始してください。 これにより、リソースの予算を作成する前に、リソース・プランナに正しい情報が表示されることを確認できます。

リソース・プランナの前提条件については、 [リソース計画の概要](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

## リソース・プランナの検索

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this was moved from the get-started-resource-planner article)</p>
-->

リソースプランナーは、複数のプロジェクトに対してリソースを予算するか、1 つのプロジェクトに対してのみ予算を割り当てるかに応じて、Workfrontの 2 つの領域に配置できます。

* [複数のプロジェクトに対してリソースプランナーを使用](#use-the-resource-planner-for-multiple-projects)
* [1 つのプロジェクトに対してリソースプランナーを使用](#use-the-resource-planner-for-one-project)

### 複数のプロジェクトに対してリソースプランナーを使用 {#use-the-resource-planner-for-multiple-projects}

複数のプロジェクトに対してリソース・プランナを使用する場合、リソースの割付数は、複数のプロジェクトにわたる数値を表します。

「生産資源」領域の「プランナ」セクションにアクセスする手順は、次のとおりです。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅にある

1. クリック **リソース**. プランナはデフォルトで表示されます。  リソース・プランナでの予算リソースの詳細は、この記事を参照してください。 [「プロジェクト」ビューと「ロール」ビューを使用する、リソースプランナーの予算リソース](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   ![](assets/qs-resource-management-area-with-planner-as-default-350x152.png)

1. 左のパネルにマウスポインターを置いて、 **リソースプール**.\
   リソースプールの作成の詳細については、 [資源プールの作成](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md).

### 1 つのプロジェクトに対してリソースプランナーを使用 {#use-the-resource-planner-for-one-project}

1 つのプロジェクトに対してリソースプランナーを使用する場合、リソースの割り当て数は、選択したプロジェクトの数を表します。

1. リソースを予算するプロジェクトに移動します。
1. クリック **ビジネス事例** をクリックします。
1. スクロールして **リソース予算設定** 」の項を参照してください。
1. クリック **リソース予算の編集** リソースプールをプロジェクトに追加し、リソースの予算を作成し始めます。

   >[!TIP]
   >
   >プロジェクトにリソースプールが関連付けられていない場合は、ビジネスケースの「リソース予算設定」領域にリソースプールのみ追加できます。 プロジェクトに既にリソースプールが存在する場合、プール内のユーザーとそのジョブの役割は、デフォルトで「リソース予算」領域に表示されます。

   ![](assets/resource-budgeting-area-on-project-350x70.png)

   1 つのプロジェクトの予算リソースの詳細については、「 [ビジネス事例の予算リソース](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).
