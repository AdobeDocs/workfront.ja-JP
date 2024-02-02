---
product-area: resource-management
navigation-topic: resource-planning
title: リソースプランナーを配置
description: 「（次の記事を元としています。これが公開されたら、記事内のコンテンツのドラフトを作成してください：/Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html）」
author: Alina
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: ht
source-wordcount: '512'
ht-degree: 100%

---

# リソースプランナーを配置

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

リソースプランナーを使用して、プロジェクトへのリソースの配分を管理できます。リソースプランナーへは、プロジェクトの「ビジネスケース」エリアから、同時に複数のプロジェクトに対して、または 1 つのプロジェクトに対してアクセスすることができます。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>Pro 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>レビュー以上<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (this seems to be the case in NWE only, not classic. Waiting on Vazgen's response for this)
      </MadCap:conditionalText>
     --></p> <p>グローバルエリアにリソースプランナーを配置するには、プラン以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>リソース管理に対する表示以上のアクセス権</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトおよびユーザーに対する表示権限 </p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 前提条件

リソースプランナーにアクセスし、使用するためのすべての前提条件が満たされていることを確認してから、使用を開始してください。これにより、リソースの予算計上を開始する前に、リソースプランナーに正しい情報が表示されることを確認できます。

リソースプランナーの前提条件について詳しくは、[リソース計画の概要](../../resource-mgmt/resource-planning/get-started-resource-planning.md)を参照してください。

## リソースプランナーを配置

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(this was moved from the get-started-resource-planner article)</p>
-->

複数のプロジェクトに対してリソースを予算計上するか、1 つのプロジェクトに対してのみ予算を計上するかに応じて、リソースプランナーを Workfront の 2 つのエリアに配置することができます。

* [複数のプロジェクトに対してリソースプランナーを使用](#use-the-resource-planner-for-multiple-projects)
* [1 つのプロジェクトに対してリソースプランナーを使用](#use-the-resource-planner-for-one-project)

### 複数のプロジェクトに対してリソースプランナーを使用 {#use-the-resource-planner-for-multiple-projects}

複数のプロジェクトに対してリソースプランナーを使用する場合、リソースの配分数は、複数のプロジェクトにわたる数値を表します。

「リソース」エリアの「計画担当者」セクションにアクセスするには：

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックします。

1. 「**リソース**」をクリックします。「計画担当者」が、デフォルトで表示されます。リソースプランナーでのリソースの予算計上について詳しくは、[プロジェクトビューと役割ビューを使用したリソースプランナーでのリソースの予算計上](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)の記事を参照してください。

   ![](assets/qs-resource-management-area-with-planner-as-default-350x152.png)

1. 左パネルにポインタを合わせて、「**リソースプール**」をクリックします。\
   リソースプールの作成について詳しくは、[リソースプールを作成](../../resource-mgmt/resource-planning/resource-pools/create-resource-pools.md)を参照してください。

### 1 つのプロジェクトに対してリソースプランナーを使用 {#use-the-resource-planner-for-one-project}

1 つのプロジェクトに対してリソースプランナーを使用する場合、リソースの配分数は、選択したプロジェクトの数値を表します。

1. リソースを予算計上するプロジェクトに移動します。
1. 左パネルの「**ビジネスケース**」をクリックします。
1. ビジネスケースの「**リソース予算計上**」セクションまでスクロールします。
1. 「**リソース予算計上の編集**」をクリックしてリソースプールをプロジェクトに追加し、リソースの予算計上を開始します。

   >[!TIP]
   >
   >ビジネスケースの「リソース予算計上」エリアにリソースプールを追加できるのは、プロジェクトにリソースプールが関連付けられていない場合のみです。プロジェクトに既にリソースプールが存在する場合、プール内のユーザーとその担当業務が、「リソース予算計上」エリアにデフォルトで表示されます。

   ![](assets/resource-budgeting-area-on-project-350x70.png)

   1 つのプロジェクトのリソースの予算計上について詳しくは、[ビジネスケースのリソース予算計上](../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)を参照してください。
