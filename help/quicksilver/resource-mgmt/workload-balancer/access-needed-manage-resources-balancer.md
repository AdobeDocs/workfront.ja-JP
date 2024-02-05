---
product-area: resource-management
navigation-topic: the-workload-balancer
title: ワークロードバランサーでリソースを管理するために必要なアクセス
description: 正しいアクセス権または権限がないと、ワークロードバランサーで作業割り当てを表示または管理できない場合があります。
author: Lisa
feature: Resource Management
exl-id: b3da9a62-481e-4503-8f27-136d6513262e
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 96%

---

# ワークロードバランサーでリソースを管理するために必要なアクセス

正しいアクセス権または権限がないと、ワークロードバランサーで作業割り当てを表示または管理できない場合があります。

ワークロードバランサーでワークロードを表示または管理したいユーザーを表示するアクセス権が必要です。これに加えて、作業が関連付けられているプロジェクトに対する正しいアクセスレベルと正しい権限が必要です。

## Adobe Workfront のプランでは、異なるエリアでワークロードバランサーを使用する必要があります。

次の表に、会社が保有する Workfront プランと、システム内でワークロードバランサーを使用できる場所との関係を説明します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p><b>Workfront プラン</b></p></td> 
   <td> <p><b>ワークロードバランサーにアクセスできるエリア</b></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">チームまたはそれ以上 </td> 
   <td>チームまたはプロジェクト用のワークロードバランサー</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pro 以上</td> 
   <td>複数のプロジェクト用のワークロードバランサー（システムレベル）</td> 
  </tr> 
 </tbody> 
</table>

Workfront のプランについて詳しくは、[アドビの計画](https://www.workfront.com/plans)を参照してください。

Workfront のワークロードバランサーの場所について詳しくは、[ワークロードバランサーの検索](../../resource-mgmt/workload-balancer/locate-workload-balancer.md)を参照してください。

## ワークロードバランサーの表示に必要なアクセス

ワークロードバランサーを表示するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>リソースエリアにワークロードバランサーを表示するプラン</p>
   <p>チームまたはプロジェクトのワークロードバランサーを表示するワーク</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>リソース管理に対する表示以上のアクセス権</p> <p>リソース管理のアクセスレベルについて詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">リソース管理へのアクセス権の付与</a>の記事を参照してください。</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>割り当てを表示したいプロジェクトに対する表示権限があります。 </p> <p>プロジェクト権限の詳細については、<a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfront でのプロジェクトの共有</a>を参照してください。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;自分のプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## ワークロードバランサーで割り当てを管理するために必要なアクセス

ワークロードバランサーを管理するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン：リソースエリアのワークロードバランサーで割り当てを管理する</p>
   <p>ワーク：チームまたはプロジェクトのワークロードバランサーで割り当てを管理する</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>リソース管理へのアクセスを編集</p> 
     <p>リソース管理のアクセスレベルについて詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">リソース管理へのアクセス権の付与</a>の記事を参照してください。</p>
     <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p> 割り当てを行う権限を含む、割り当てを管理したいプロジェクトに対する参加以上の権限。 </p> <p>プロジェクトの権限について詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfront でのプロジェクトの共有</a>の記事を参照してください。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。

<!--these notes were inside the table: for the Edit access to Res Management
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">View or higher access to Financial Data, if you want to view information by cost (NOTE: this is not possible yet!)</p>    
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Financial Data access level, see the article<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. (NOTE: this is not possible yet!)</p>
    -->