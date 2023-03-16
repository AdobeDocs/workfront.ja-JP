---
product-area: resource-management
navigation-topic: the-workload-balancer
title: リンクとのワークロードバランサーの共有
description: リソース領域を利用できない他のユーザーと、ワークロードバランサーを共有できます。 ワークロード・バランサの使用の詳細は、「ワークロード・バランサのナビゲート」を参照してください。
author: Alina
feature: Resource Management
exl-id: e2d6b1f8-bdc9-4a34-bdc3-b56f7aa2e7a5
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 0%

---

# リンクとのワークロードバランサーの共有

リソース領域を利用できない他のユーザーと、ワークロードバランサーを共有できます。 ワークロード・バランサの使用の詳細は、 [ワークロード・バランサのナビゲート](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意のプラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>リソース領域でワークロードバランサーを使用する場合の計画</p>
   <p>チームまたはプロジェクトのワークロードバランサーを使用する場合の作業</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>次の項目へのアクセス権を表示または高くします。</p> 
    <ul> 
     <li> <p>リソース管理</p> </li> 
     <li> <p>プロジェクト</p> </li> 
     <li> <p>タスク</p> </li> 
     <li> <p>問題</p> </li> 
    </ul> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクト、タスクおよび問題に対する権限を表示またはそれ以上に設定します </p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 共有リンクから表示する際にワークロード・バランサに含まれる情報

他のユーザーとワークロード・バランサへのリンクを共有する場合、共有リンクには次の情報が含まれます。

* ワークロードバランサーの割り当て済み作業領域。
* プロジェクト、タスク、ユーザー情報。 これには、ユーザー割り当て情報が含まれます。
* 選択したフィルターに応じて情報が表示されます。

   >[!IMPORTANT]
   >
   >リンクを共有した後にフィルタを削除すると、リンクからワークロード・バランサを表示しているユーザーに対して、フィルタが削除されたことを示す警告が表示されます。 割り当てられた作業領域のすべてのユーザーが表示されます。 これは、ワークロード・バランサのデフォルト・ビューです。

* 以前に選択した週数。

共有リンクからワークロード・バランサを表示しているユーザーは、次のオプションを使用して、自身を更新できます。

* 以下のタイムラインを選択します。

   * 今日
   * 前と前のアイコン
   * カレンダーの選択

* 日、週、月のアイコン
* 設定アイコン
* 割り当てを表示アイコン

   これらのオプションの使用について詳しくは、 [ワークロード・バランサのナビゲート](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

* 役割割り当てを表示アイコン

   これは、プロジェクトのワークロードバランサーに対してのみ使用できます。

共有リンクを受け取るユーザーは、このリンクからのワークロードバランサーで次の操作を実行できません。

* 作業項目をユーザーに割り当てる
* ユーザー割り当ての管理
* 新しいフィルターを作成するか、最初に適用したフィルターを更新します

## 共有リンクからワークロード・バランサの情報を表示するために必要なアクセス

共有リンクからワークロードバランサーの情報を表示するには、次のアクセス権が必要です。

* 有効なAdobe Workfrontライセンス。Workfrontにログインする必要があります。
* 少なくとも、アクセスレベルでリソース管理へのアクセスを表示します。 リソース管理へのアクセス権の付与については、 [リソース管理へのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).
* ワークロード・バランサに表示されるプロジェクト、タスク、問題、およびユーザーに対する権限を表示します。

## リンクから他のユーザーとワークロードバランサーを共有します

1. ワークロードバランサーに移動

   ワークロード・バランサへのアクセスの詳細は、 [ワークロード・バランサのナビゲート](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. （オプション）次の 1 つ以上の操作を行います。

   * 期間の選択を更新します。
   * クリック **日、週**&#x200B;または **月** ：日別、週別、月別の情報を表示します。

      ![](assets/month-icon-on-toolbar-selected-wb-350x226.png)

   * [ 未割り当て ] および [ 割り当て済み ] 作業領域にフィルタを適用します。

      ワークロード・バランサの情報のフィルタリングの詳細は、 [ワークロードバランサーの情報のフィルタリング](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

1. 次をクリック： **リンクアイコン** ![](assets/wb-shearable-link-icon-small.png).

   これにより、リンクがクリップボードに追加されます。

1. リンクを他のユーザーと共有するには、次のいずれかの操作を行います。

   * 電子メール、チャットメッセージ、または他のアプリケーションに貼り付け、他のユーザーと共有します。
   * 外部ページとしてカスタムセクションに追加したり、カスタムセクションをユーザーのプロファイルまたはレイアウトテンプレートに追加したりして、レイアウトテンプレートをユーザー、チーム、役割、グループと共有します。

      外部ページの作成について詳しくは、 [外部 Web ページをダッシュボードに埋め込む](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md). レイアウトテンプレートにカスタムセクションを追加する方法については、 [レイアウトテンプレートを使用して左のパネルをカスタマイズする](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

      >[!IMPORTANT]
      >
      >ワークロード・バランサをオブジェクトのカスタム・セクションに追加した場合、ワークロード・バランサの情報はオブジェクトによってフィルタリングされません。 ワークロード・バランサには、最初に適用したフィルタでフィルタされた情報が表示されます。
