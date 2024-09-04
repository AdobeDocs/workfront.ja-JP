---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Workfrontでのリソースの予算計上に必要なアクセス
description: 特定のアクセスレベル設定と、作業項目、ユーザー、担当業務、およびチームに対する権限を持っている場合に、表示アクセスを持つプロジェクトのリソース計画に関する情報を表示および管理できます。
author: Lisa
feature: Resource Management
exl-id: d2bfc411-188a-4f8b-8180-0e984f01b5ab
source-git-commit: a5317e3126939d4c648977635af2dbc6add02780
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 83%

---

# Workfrontでのリソースの予算計上に必要なアクセス

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><b>(LINKED TO PRODUCT</b>: This is also linked to the product, in two different tooltips in the RP:</p>
<p>- the tooltip for the View-only mode of the Budgeted Hours boxes. You gave this link to Vazgen and the team for the tooltip and documented this in this sheet:https://docs.google.com/spreadsheets/d/1zKjNVw_TyfQ474jbY7JorSWTkptMNb5RFCck2IficYs/edit#gid=0</p>
<p>- Also in the tooltip from this issue: https://hub.workfront.com/issue/view?ID=5ca708d00024a39e58b5dbeaceb00939)</p>
<p>This might need to be moved to Resource Management overview and title needs to be changed to "Acces needed to manage resources" when the res manager prerequisite will drop for resource scheduling and the field goes away.</p>
<p>This should be linked from Planning in the Resource Planner - in the Budgeting Resources in the RP area)</p>
</div>
-->

リソース計画を含む Adobe Workfront ライセンスを会社が購入している場合は、表示権限を持つプロジェクトのリソース予算計上情報を表示できます。予算計上情報は、リソースプランナーで表示できます。

Workfront の予算計上ツールを使用するための前提条件について詳しくは、[リソース計画の概要](../../resource-mgmt/resource-planning/get-started-resource-planning.md)を参照してください。

リソース計画ツールでリソースを予算計上し、リソースプールを管理し、コスト情報を確認するには、所属する会社とユーザー本人が次のアクセス権を持っている必要があります。

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
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：プラン</p></td>
  </tr>  
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> 
    <ul> 
     <li> <p>次を含むアクセスレベルでリソース管理へのアクセスを編集します。</p> 
      <ul> 
       <li> <p>プロジェクトの優先度と予算計上時間数を編集するためのアクセス権。 </p> </li> 
       <li> <p>リソース プールを管理する必要がある場合は、リソース プールを管理するためのアクセス権。</p> </li> 
      </ul> <p>リソース管理のアクセスレベルについて詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">リソース管理へのアクセス権の付与</a>の記事を参照してください。</p> </li> 
     <li> <p>プロジェクトおよびユーザーへのアクセスを編集します。 </p> </li> 
     <li> <p> コスト別に情報を表示または管理する必要がある場合は、アクセス レベルで財務データへのアクセスを編集します。</p> <p>財務データのアクセスレベルについて詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">財務データへのアクセス権の付与</a>の記事を参照してください。</p> </li> 
    </ul> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>財務の管理権限を含む、プロジェクトの権限を管理します。</p> <p>プロジェクトの権限について詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfront でのプロジェクトの共有</a>の記事を参照してください。</p> <p>プロジェクトに対する財務権限について詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md"><a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">オブジェクトに対する財務権限の共有</a></a>の記事を参照してください。</p>

<p><b>メモ</b>

役割ビューでリソースを予算計上する際に、その役割の下に表示される少なくとも 1 つのプロジェクトに対する権限が管理権限未満である場合、その役割の時間数、FTE、コストは予算計上できません。予算計上できるのは、管理権限を持つプロジェクトのみです。</p> </td>
</tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。
