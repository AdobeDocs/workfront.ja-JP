---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: 為替レートの設定
description: Adobe Workfront 管理者は、Workfront で為替レートを設定できます。
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '533'
ht-degree: 97%

---

# 為替レートの設定

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Adobe Workfront 管理者は、Workfront で為替レートを設定できます。これには次が含まれます。

* Workfront システムのデフォルト通貨の設定
* 現在の為替レートに一致するように Workfront の為替レートを更新
* 複数の通貨の為替レートの設定（これにより、ユーザーはプロジェクトごとにデフォルト通貨を選択できます）

為替レートは、Workfront のすべての財務要素に影響を与えます。「基準通貨」は、特定のプロジェクトまたは担当業務が上書きされない限り、システム全体のすべてのプロジェクトのデフォルト通貨です。また、レポートやリストで表示する際に、基準通貨やプロジェクトの通貨とは異なるシステム内で使用可能な通貨で財務情報を表示するよう選択することもできます。詳しくは、[一意の為替レートを使用した財務データレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md)を参照してください。

プロジェクトおよび担当業務用の Workfront での基準通貨の上書きについて詳しくは、次の記事を参照してください。

* [プロジェクトの通貨を変更](../../../manage-work/projects/project-finances/change-project-currency.md)
* [担当業務の作成と管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

為替レートを設定する方法は、特定のプロジェクトの為替レートをユーザーが変更できるかどうかに影響します。

>[!IMPORTANT]
>
>Workfront の為替レートは動的ではなく、設定する値は、為替レートの変更が発生した場合に更新する必要があります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：プラン</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 為替レートの設定

{{step-1-to-setup}}

1. **プロジェクト環境設定**／**為替レート**&#x200B;をクリックします。

1. 「**通貨を追加する**」をクリックします。
1. 通貨の名前を入力し始め、ドロップダウンリストに表示されたらクリックします。

1. 表示されたフィールドで、システムで基準通貨として設定される通貨に関連して、選択した通貨のレートを指定します。
1. （オプション）通貨を Workfront の基準（デフォルト）通貨として設定します。

   これは、システム全体ですべてのプロジェクトおよびレポートのデフォルトとして使用される通貨です。

1. 「**保存**」をクリックして変更を保存します。

## ユーザーがプロジェクトのデフォルト通貨を変更できるようにする

ユーザーは、次の条件を満たした場合に、プロジェクトのデフォルト通貨を変更できます。

* ユーザーは、為替レートに対する管理者アクセス権を持つプランライセンスを持っています。

  詳しくは、[特定のエリアに対する管理者アクセス権をユーザーに付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)を参照してください。

* Workfront システムで複数の通貨が有効になっています。

ユーザーが特定のプロジェクトでデフォルトの通貨を変更する方法について詳しくは、[プロジェクトの通貨の変更](../../../manage-work/projects/project-finances/change-project-currency.md)を参照してください。

## 担当業務のデフォルトの通貨をユーザーが変更できるようにする

次の条件を満たす場合、ユーザーは担当業務の通貨を変更できます。

* ユーザーは、担当業務に対する管理者アクセス権を持つプランライセンスを持っています。

  詳しくは、[特定のエリアに対する管理者アクセス権をユーザーに付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)を参照してください。

* Workfront システムで複数の通貨が有効になっています。

特定の担当業務でユーザーがデフォルトの通貨を変更する方法について詳しくは、[担当業務の作成と管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)を参照してください。
