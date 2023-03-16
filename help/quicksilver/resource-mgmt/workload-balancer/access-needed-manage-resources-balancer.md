---
product-area: resource-management
navigation-topic: the-workload-balancer
title: ワークロードバランサーでリソースを管理するために必要なアクセス
description: 正しいアクセス権または権限がないと、ワークロードバランサーで作業割り当てを表示または管理できない場合があります。
author: Alina
feature: Resource Management
exl-id: b3da9a62-481e-4503-8f27-136d6513262e
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '535'
ht-degree: 0%

---

# ワークロードバランサーでリソースを管理するために必要なアクセス

正しいアクセス権または権限がないと、ワークロードバランサーで作業割り当てを表示または管理できない場合があります。

ワークロード・バランサで表示または管理するワークロードを持つユーザーを表示するアクセス権が必要です。 これに加えて、作業が関連付けられているプロジェクトに対する正しいアクセスレベルと正しい権限が必要です。

## Adobe Workfrontのプランでは、異なる領域でワークロードバランサーを使用する必要があります

次の表に、会社が保有するWorkfrontプランと、システム内でワークロードバランサーを使用できる場所との間の接続を示します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Workfront プラン</p></td> 
   <td> <p>ワークロードバランサーにアクセスできる領域</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">チーム以上 </td> 
   <td>チームまたはプロジェクト用のワークロードバランサー</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Pro 以上</td> 
   <td>複数のプロジェクト用のワークロードバランサー（システムレベル）</td> 
  </tr> 
 </tbody> 
</table>

Workfrontの計画について詳しくは、 [アドビの計画](https://www.workfront.com/plans).

Workfrontのワークロードバランサーの場所について詳しくは、 [ワークロード・バランサの検索](../../resource-mgmt/workload-balancer/locate-workload-balancer.md).

## ワークロードバランサーの表示に必要なアクセス

ワークロードバランサーを表示するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>リソースエリアにワークロードバランサーを表示する計画</p>
   <p>チームまたはプロジェクトのワークロードバランサーを表示する作業</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>リソース管理へのアクセス権を表示または高くします</p> <p>リソース管理のアクセスレベルについては、「 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">リソース管理へのアクセス権の付与</a>.</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>割り当てを表示するプロジェクトに対する表示権限があります。 </p> <p>プロジェクト権限の詳細については、「 <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfrontでプロジェクトを共有する</a>.</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## ワークロードバランサーで割り当てを管理するために必要なアクセス

ワークロードバランサーを管理するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>リソース領域のワークロードバランサーで割り当てを管理する計画</p>
   <p>チームまたはプロジェクトのワークロードバランサーで割り当てを管理する作業</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>リソース管理へのアクセスを編集</p> 
     <p>リソース管理のアクセスレベルについては、「 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">リソース管理へのアクセス権の付与</a>.</p>
     <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p> 割り当てを行う権限を含む、割り当てを管理するプロジェクトに対する権限を付与するか、それ以上に設定します。 </p> <p>プロジェクト権限の詳細については、「 <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Adobe Workfrontでプロジェクトを共有する</a>.</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

<!--these notes were inside the table: for the Edit access to Res Management
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">View or higher access to Financial Data, if you want to view information by cost (NOTE: this is not possible yet!)</p>    
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Financial Data access level, see the article<a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. (NOTE: this is not possible yet!)</p>
    -->