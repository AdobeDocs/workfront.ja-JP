---
product-area: resource-management
navigation-topic: the-workload-balancer
title: リンクによるワークロードバランサーの共有
description: リソースエリアを利用できない他のユーザーとワークロードバランサーを共有できます。ワークロードバランサーの使用方法については、ワークロードバランサーの操作を参照してください。
author: Lisa
feature: Resource Management
exl-id: e2d6b1f8-bdc9-4a34-bdc3-b56f7aa2e7a5
source-git-commit: 2c4fe48ef969741ba792e37c28adba86ffdcba9a
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 100%

---

# リンクによるワークロードバランサーの共有

リソースエリアを利用できない他のユーザーとワークロードバランサーを共有できます。ワークロードバランサーの使用方法の詳細については、[ワークロードバランサーの操作](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意のプラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン、リソース領域でワークロードバランサーを使用する場合</p>
   <p>ワーク、チームまたはプロジェクトのワークロードバランサーを使用する場合</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>次の項目に対する表示以上のアクセス権：</p> 
    <ul> 
     <li> <p>リソース管理</p> </li> 
     <li> <p>プロジェクト</p> </li> 
     <li> <p>タスク</p> </li> 
     <li> <p>イシュー</p> </li> 
    </ul> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、「<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>」を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクト、タスク、イシューに対する表示またはそれ以上の権限 </p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 共有リンクからワークロードバランサーを表示するときにワークロードバランサーに含まれる情報

ワークロードバランサーへのリンクを他のユーザーと共有すると、共有リンクには次の情報が含まれます。

* ワークロードバランサーの割り当てられた作業エリア。
* プロジェクト、タスク、ユーザー情報。これには、ユーザー割り当て情報が含まれます。
* 選択したフィルターに従って情報が表示されます。

  >[!IMPORTANT]
  >
  >リンクを共有した後にフィルターを削除すると、リンクからワークロードバランサーを表示しているユーザーにフィルターが削除されたという警告が表示されます。割り当てられた作業エリア内のすべてのユーザーが表示されます。これは、ワークロードバランサーのデフォルトのビューです。

* 以前に選択した週の数。

共有リンクからワークロードバランサーを表示しているユーザーは、自分自身を更新するために次のオプションを使用できます。

* 以下のタイムラインを選択します。

   * 今日
   * 戻るアイコンと進むアイコン
   * カレンダーの選択

* 日、週、月のアイコン
* 設定アイコン
* 割り当てを表示アイコン

  これらのオプションの使用方法の詳細については、[ワークロードバランサーの操作](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)を参照してください。

* 役割割り当てを表示アイコン

  プロジェクトのワークロードバランサーでのみ使用できます。

共有リンクを受信したユーザーは、このリンクからワークロードバランサーで次の操作を実行できません。

* 作業アイテムをユーザーに割り当てる
* ユーザー割り当ての管理
* 新しいフィルターを作成するか、最初に適用したフィルターを更新します

## 共有リンクからワークロードバランサーの情報を表示するために必要なアクセス

共有リンクからワークロードバランサーの情報を表示するには、次のアクセス権が必要です。

* 有効な Adobe Workfront ライセンスがあり、Workfront にログインしている必要があります。
* 少なくとも、アクセス レベルでリソース管理へのアクセス権を表示します。リソース管理へのアクセス権の付与については、[リソース管理へのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)を参照してください。
* ワークロードバランサーに表示されるプロジェクト、タスク、イシュー、およびユーザーに対する権限を表示します。

## リンクから他のユーザーとワークロードバランサーを共有

1. ワークロードバランサーへ移動

   ワークロードバランサーへのアクセスの詳細については、[ワークロードバランサーの操作](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md)を参照してください。

1. （オプション）次のいずれか 1 つ以上の操作を行います。

   * 期間の選択を更新します。
   * **日、週**、または&#x200B;**月**&#x200B;をクリックして、日次、週次、または月次の情報を表示します。

     ![](assets/month-icon-on-toolbar-selected-wb-350x226.png)

   * 「未割り当ての作業エリア」および「割り当て済みの作業領域」にフィルターを適用します。

     ワークロードバランサーでの情報のフィルタリングの詳細については、[ワークロードバランサーでの情報のフィルタリング](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md)を参照してください。

1. **リンクアイコン** ![](assets/wb-shearable-link-icon-small.png) をクリックします。

   これにより、リンクがクリップボードに追加されます。

1. リンクを他のユーザーと共有するには、次のいずれかの操作を行います。

   * メール、チャットメッセージ、またはその他のアプリケーションに貼り付けて、他のユーザーと共有します。
   * 外部ページとしてカスタムセクションに追加し、そのカスタムセクションを「ユーザープロファイル」または「レイアウトテンプレート」に追加して、そのレイアウトテンプレートをユーザー、チーム、職務、またはグループと共有します。

     外部ページの作成について詳しくは、[外部 web ページをダッシュボードに埋め込む](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)を参照してください。レイアウトテンプレートにカスタムセクションを追加する方法については、[レイアウトテンプレートを使用して左側のパネルをカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)を参照してください。

     >[!IMPORTANT]
     >
     >ワークロードバランサーをオブジェクトのカスタムセクションに追加すると、ワークロードバランサー内の情報はオブジェクトによってフィルターされません。ワークロードバランサーには、最初に適用されたフィルターによってフィルター処理された情報が表示されます。
