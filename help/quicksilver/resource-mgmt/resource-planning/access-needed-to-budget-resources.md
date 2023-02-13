---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Adobe Workfrontの予算リソースに必要なアクセス
description: 特定のアクセスレベル設定と、作業項目、ユーザー、ジョブの役割、およびチームに対する権限を持つ場合に、表示するプロジェクトのリソース計画に関する情報を表示および管理できます。
author: Alina
feature: Resource Management
exl-id: d2bfc411-188a-4f8b-8180-0e984f01b5ab
source-git-commit: d3172a681ef6ac8b7bde44c680ad7febc3f26121
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Adobe Workfrontの予算リソースに必要なアクセス

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><b>(LINKED TO PRODUCT</b>: This is also linked to the product, in two different tooltips in the RP:</p>
<p>- the tooltip for the View-only mode of the Budgeted Hours boxes. You gave this link to Vazgen and the team for the tooltip and documented this in this sheet:https://docs.google.com/spreadsheets/d/1zKjNVw_TyfQ474jbY7JorSWTkptMNb5RFCck2IficYs/edit#gid=0</p>
<p>- Also in the tooltip from this issue: https://hub.workfront.com/issue/view?ID=5ca708d00024a39e58b5dbeaceb00939)</p>
<p>This might need to be moved to Resource Management overview and title needs to be changed to "Acces needed to manage resources" when the res manager prerequisite will drop for resource scheduling and the field goes away.</p>
<p>This should be linked from Planning in the Resource Planner - in the Budgeting Resources in the RP area)</p>
</div>
-->

Resource Planning を含むAdobe Workfrontライセンスを購入した場合は、表示する権限を持つプロジェクトのリソース予算情報を表示できます。 予算計画情報は、「生産資源プランナ」で表示できます。

Workfrontの予算ツールを使用するための前提条件について詳しくは、 [リソース計画の概要](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

リソースを予算化するには、リソースプールを管理し、リソース計画ツールのコスト情報を参照してください。また、次のアクセス権を持っている必要があります。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> 
    <ul> 
     <li> <p>次の項目を含むアクセスレベルで、リソース管理へのアクセスを編集します。</p> 
      <ul> 
       <li> <p>プロジェクトの優先度と予算時間を編集するためのアクセス権。 </p> </li> 
       <li> <p>リソースプールを管理する必要がある場合は、リソースプールを管理するためのアクセス権。</p> </li> 
      </ul> <p>リソース管理のアクセスレベルについては、「 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">リソース管理へのアクセス権の付与</a>.</p> </li> 
     <li> <p>プロジェクトおよびユーザーへのアクセスを編集します。 </p> </li> 
     <li> <p> コスト別に情報を表示または管理する必要がある場合は、アクセス・レベルで財務データへのアクセスを編集します。</p> <p>金融データのアクセスレベルの詳細については、「 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">財務データへのアクセス権の付与</a>.</p> </li> 
    </ul>

<p><b>メモ</b> </p>

<p> まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>財務の管理権限を含む、プロジェクトの権限を管理します。</p> <p>プロジェクト権限の詳細については、「 <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfrontでプロジェクトを共有する</a>.</p> <p>プロジェクトに対する財務上の権限の詳細については、「 <a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md"><a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">オブジェクトに対する財務権限の共有</a></a>.</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md">オブジェクトへのアクセスのリクエスト </a>.</p>

<p><b>メモ</b>

[ 役割 ] ビューでリソースを予算設定する際に、その役割の下に表示される少なくとも 1 つのプロジェクトに対する [ 管理 ] 権限より少ない場合は、その役割の予算時間、工数、コストは使用できません。 管理権限を持つプロジェクトのみを予算に追加できます。</p> </td>
</tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。
