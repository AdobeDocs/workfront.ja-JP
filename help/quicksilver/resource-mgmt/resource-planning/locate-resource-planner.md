---
product-area: resource-management
navigation-topic: resource-planning
title: リソースプランナーを配置
description: リソースプランナーを使用して、プロジェクトへのリソースの配分を管理できます。リソースプランナーへは、プロジェクトの「ビジネスケース」エリアから、同時に複数のプロジェクトに対して、または 1 つのプロジェクトに対してアクセスすることができます。
author: Lisa
feature: Resource Management
exl-id: 0de749df-5af9-4124-8539-06b82dca2ec4
source-git-commit: a5317e3126939d4c648977635af2dbc6add02780
workflow-type: tm+mt
source-wordcount: '500'
ht-degree: 90%

---

# リソースプランナーを配置

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(This came off this article: draft that content in the article when this comes live: /Content/Resource Mgmt/Resource Planning/get-started-resource-planner.html)</p>
-->

リソースプランナーを使用して、プロジェクトへのリソースの配分を管理できます。リソースプランナーへは、プロジェクトの「ビジネスケース」エリアから、同時に複数のプロジェクトに対して、または 1 つのプロジェクトに対してアクセスすることができます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：任意</p>
       <p>または</p>
       <p>現在：Pro 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：Light 以上；</br>
          メインメニューでリソースプランナーを検索するための標準</p>
       <p>または</p>
       <p>現在：レビューまたはそれ以上；</br>
       メインメニューでリソースプランナーを探す</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>リソース管理に対する表示以上のアクセス権</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトおよびユーザーに対する表示権限 </p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

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

{{step1-to-resourcing}}

「計画担当者」が、デフォルトで表示されます。リソースプランナーでのリソースの予算計上について詳しくは、[プロジェクトビューと役割ビューを使用したリソースプランナーでのリソースの予算計上](../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md)の記事を参照してください。

![](assets/qs-resource-management-area-with-planner-as-default-350x152.png)

1. 左側のパネルで **リソースプール** をクリックします。
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
