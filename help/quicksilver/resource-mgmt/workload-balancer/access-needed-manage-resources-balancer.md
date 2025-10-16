---
product-area: resource-management
navigation-topic: the-workload-balancer
title: ワークロードバランサーでリソースを管理するために必要なアクセス
description: 適切なアクセス権または権限がなければ、ワークロードバランサーで作業の割り当てを表示または管理できない場合があります。
author: Lisa
feature: Resource Management
exl-id: b3da9a62-481e-4503-8f27-136d6513262e
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '374'
ht-degree: 67%

---

# ワークロードバランサーでリソースを管理するために必要なアクセス

{{preview-fast-release-general}}

適切なアクセス権または権限がなければ、ワークロードバランサーで作業の割り当てを表示または管理できない場合があります。

ワークロードバランサーでワークロードを表示または管理したいユーザーを表示するアクセス権が必要です。これに加えて、作業が関連付けられているプロジェクトに対する正しいアクセスレベルと正しい権限が必要です。

<!--## Adobe Workfront package needed to use the Workload Balancer for different areas

The following table illustrates the connection between the Workfront plan your company has and where in the system you can use the Workload Balancer:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><p><b>Workfront Plan (Current)</b></p></td> 
   <td> <p><b>Areas where you can access the Workload Balancer</b></p> </td> 
  </tr> 
  <tr> 
   <td>Team or higher </td> 
   <td>Workload Balancer for a team or a project</td> 
  </tr> 
  <tr> 
   <td>Pro or higher</td> 
   <td>Workload Balancer for multiple projects, at the system level</td> 
  </tr> 
  <tr> 
   <td><p><b>Workfront Plan (New)</b></p></td> 
   <td> <p><b>Areas where you can access the Workload Balancer</b></p> </td> 
  </tr>
  <tr> 
   <td>Any </td> 
   <td>Access the Workload Balancer anywhere in Workfront</td> 
  </tr> 
 </tbody> 
</table>

For information about the Workfront plans, see [Our Plans](https://business.adobe.com/jp/products/workfront/pricing.html).

For information about where you can locate the Workload Balancer in Workfront, see [Locate the Workload Balancer](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).-->

## ワークロードバランサーの表示に必要なアクセス

ワークロードバランサーを表示するには、次のアクセス権が必要です。

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
       <p>リソース エリアでワークロードバランサーを表示するには、作業を計画し、チームまたはプロジェクトのワークロードバランサーを表示します</p></td>
  </tr>  
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>リソース管理への表示以上のアクセス</p> <p>リソース管理のアクセスレベルについて詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md">リソース管理へのアクセス権の付与</a>の記事を参照してください。</p></td> 
  </tr> 
  <tr> 
   <td>オブジェクト権限</td> 
   <td> <p>割り当てを表示するプロジェクトの表示権限が必要です。 </p> <p>プロジェクトの権限について詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md">Adobe Workfront でのプロジェクトの共有</a>の記事を参照してください。</p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

<span class="preview"> すべてのユーザーが、自分のプロファイルでワークロードバランサーを表示するアクセス権を持ちます。 これは、ライセンスやアクセスレベルによる制限ではありません。 ユーザープロファイルのワークロードバランサーは読み取り専用で、割り当てと割り当てを変更することはできません。</span>

## ワークロードバランサーで割り当てを管理するために必要なアクセス

ワークロードバランサーを管理するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody>
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td>
  </tr>
  <tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td><p>標準</p>
       <p>リソース エリアのワークロードバランサーで割り当てを管理するために計画を立てる。作業を立て、チームまたはプロジェクトのワークロードバランサーで割り当てを管理する</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td>
   <td> <p>リソース管理へのアクセスを編集</p>
     <p>リソース管理のアクセスレベルについて詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" >リソース管理へのアクセス権の付与</a>の記事を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td>オブジェクト権限</td> 
   <td> <p> 割り当てを行う権限を含む、割り当てを管理したいプロジェクトに対する参加以上の権限。 </p> <p>プロジェクトの権限について詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md">Adobe Workfront でのプロジェクトの共有</a>の記事を参照してください。</p></td>
  </tr> 
 </tbody>
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

<!--these notes were inside the table: for the Edit access to Res Management
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">View or higher access to Financial Data, if you want to view information by cost (NOTE: this is not possible yet!)</p>    
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Financial Data access level, see the article<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. (NOTE: this is not possible yet!)</p>
    -->
