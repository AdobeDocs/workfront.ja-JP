---
product-area: resource-management
keywords: 作業，チーム，スタッフ，リソース
navigation-topic: the-workload-balancer
title: ワークロード・バランサの検索
description: ワークロード・バランサを使用して、作業用のリソースをスケジュールしたり、その可用性と現在の割り当てをレビューしたりできます。
author: Alina
feature: Resource Management
exl-id: 88029c9d-b588-4d33-801a-04f49b12a6e8
source-git-commit: 59c3a57e334d1660e3e59da480a90060b1ba81b7
workflow-type: tm+mt
source-wordcount: '764'
ht-degree: 0%

---

# ワークロード・バランサの検索


ワークロード・バランサを使用して、作業用のリソースをスケジュールしたり、その可用性と現在の割り当てをレビューしたりできます。

ワークロード・バランサには、次の方法でアクセスできます。

* Adobe Workfrontで事前に定義されたいくつかの領域から
* カスタムセクションに追加する

この記事では、ワークロードバランサーにアクセスできる領域について説明します。

>[!NOTE]
>
>ワークロードバランサーにアクセスする方法に関係なく、ナビゲーションし、リソースを管理する方法は同じです。
>
>ワークロードバランサーの詳細と、リソースの管理およびスケジュール設定に使用する方法については、次の記事を参照してください。
>
>* [ワークロードバランサーの概要](../../resource-mgmt/workload-balancer/overview-workload-balancer.md)
>* [ワークロード・バランサのナビゲート](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)
>* [ワークロードバランサーでの作業割り当ての概要](../../resource-mgmt/workload-balancer/assign-work-in-workload-balancer.md)
>* [ワークロードバランサーでのユーザー割り当ての管理](../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md)
>

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>リソース領域でワークロードバランサーを使用する場合の計画</p>
   <p>チームまたはプロジェクトのワークロードバランサーを使用する場合の作業</p>
 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>次の項目へのアクセス権を表示または高くします。</p> 
    <ul> 
     <li> <p>リソース管理</p> </li> 
     <li> <p>プロジェクト</p> </li> 
     <li> <p>タスク</p> </li> 
     <li> <p>イシュー</p> </li> 
    </ul> <p><b> メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>プロジェクト、タスクおよび問題に対する権限以上の表示 </p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。

## 事前定義済みの領域でワークロード・バランサにアクセス

次の節では、Workfront内のワークロードバランサーにアクセスする場所を示します。

### リソース領域の複数のプロジェクト用のワークロードバランサーへのアクセス

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png)を選択し、次に **リソース**.
1. クリック **ワークロードバランサー** をクリックします。

   ![](assets/nwe-balancer-global.png)

   ワークロード・バランサには、デフォルトで、リソース領域の情報別に次の情報が表示されます。

   * **未割り当ての作業**：未割り当ての作業項目はありません。
   * **割り当てられた作業**：システム内のすべてのアクティブユーザー。

     「割り当てられた作業」領域にユーザーを表示する場合は、フィルターを使用することをお勧めします。 詳しくは、 [ワークロードバランサーの情報のフィルタリング](../workload-balancer/filter-information-workload-balancer.md).

### チームのワークロードバランサーへのアクセス

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png)、「チーム」をクリックします。
ホームチームのページが表示されます。

   チームのワークロードバランサーがデフォルトで表示されます。

   ![](assets/nwe-balancer-team-350x172.png)

   チームのワークロード・バランサには、デフォルトで次の情報が表示されます。

   * **未割り当ての作業**：チームに割り当てられ、ユーザーに割り当てられていない項目。
   * **割り当てられた作業**：チームのすべてのメンバー（すべての割り当てを含む）

     >[!TIP]
     >
     >チームメンバーは、チームに割り当てられた作業に割り当てられたり、他のチームやロールに割り当てられた作業に割り当てられたりします。



### プロジェクトのワークロードバランサーへのアクセス

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png)を選択し、次に **プロジェクト**.
1. プロジェクトの名前をクリックして、プロジェクトページを開きます。
1. クリック **ワークロードバランサー** をクリックします。 クリックする必要がある場合があります **表示を増やす**&#x200B;を、 **ワークロードバランサー**.

   プロジェクトのワークロードバランサーが表示されます。

   ![](assets/nwe-balancer-project-350x152.png)

   プロジェクトのワークロード・バランサには、デフォルトで次の情報が表示されます。

   * **未割り当ての作業**：ジョブの役割またはチームに割り当てられ、ユーザーに割り当てられていないプロジェクトの項目。
   * **割り当てられた作業**：プロジェクト上の項目に割り当てられたユーザー。

     >[!TIP]
     >
     >「すべてのユーザーを表示」オプションを有効にすると、プロジェクト上のユーザーのみではなく、システム内のすべてのユーザーを（割り当てられた作業領域で）表示できます。 詳しくは、 [ワークロード・バランサのナビゲート](../workload-balancer/navigate-the-workload-balancer.md).


## ワークロードバランサーのカスタムセクションへの追加

ワークロードバランサーを任意のカスタムセクションに追加できます。

既にワークロードバランサーに適用しているカスタマイズのほとんどは、カスタムセクションに追加する際に保持されます。

1. 次のいずれかの領域に移動して、ワークロードバランサーにアクセスします。

   * リソース領域
   * チーム
   * プロジェクト

1. 共有可能なリンクを取得し、クリップボードにコピーします。詳しくは、 [リンクとのワークロードバランサーの共有](../../resource-mgmt/workload-balancer/share-link-for-workload-balancer.md).
1. 外部ページを含むダッシュボードの作成 ( [外部 Web ページをダッシュボードに埋め込む](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md). 手順 2 で取得した共有可能なリンクを、外部ページに使用します。

   <!--
      (NOTE: ensure this stays correct)
      -->

1. カスタムセクションを作成します。詳しくは、 [カスタムタブまたはセクションの作成](../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/create-custom-tabs.md) をクリックして、ダッシュボードをカスタムタブに配置します。

   カスタム・セクションからワークロード・バランサにアクセスする場合、手順 1 に示す元の領域の 1 つから直接アクセスする場合と同じように表示できます。

   <!--
      (NOTE: ensure this stays correct)
     -->

1. （オプション）レイアウトテンプレートのカスタムタブを共有します。詳しくは、  [レイアウトテンプレートを使用して左のパネルをカスタマイズする](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md) .


<!--
For a team:

* From the Workload Balancer section of a team.

  You can adjust allocations and review or assign work from multiple projects to individual team members.

For a project:

  You can do the following when you use the Workload Balancer within a project:

   * Assign work on the project to users already assigned other work on the project.
   * Assign work to any user that might not be on the project.

   * View additional work that users are assigned to on other projects.
   * Adjust user allocations to work items.-->