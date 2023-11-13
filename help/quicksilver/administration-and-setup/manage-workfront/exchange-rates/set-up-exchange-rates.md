---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: 為替レートの設定
description: Adobe Workfrontの管理者は、Workfrontで為替レートを設定できます。
feature: System Setup and Administration
role: Admin
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: b0cf0a5ec6b932267c8714b966638d8da93331b8
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 3%

---

# 為替レートの設定

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Adobe Workfrontの管理者は、Workfrontで為替レートを設定できます。 これには以下が含まれます。

* Workfrontシステムのデフォルト通貨の設定
* 現在の為替レートに一致するようにWorkfrontの為替レートを更新しています
* 複数の通貨の為替レートの設定（これにより、ユーザーは個々のプロジェクトのデフォルト通貨を選択できます）

為替レートは、Workfrontのすべての金融要素に影響を与えます。 「基準通貨」は、特定のプロジェクトまたはジョブの役割に対して上書きされない限り、システム全体のすべてのプロジェクトのデフォルト通貨です。 また、レポートやリストで表示する際に、システム内で使用可能な通貨で財務情報を表示する場合に、基本通貨やプロジェクトの通貨とは異なる通貨で表示するよう選択することもできます。 詳しくは、 [一意の為替レートを使用した財務データレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

プロジェクトおよびジョブの役割用のWorkfrontでのベース通貨の上書きについて詳しくは、次の記事を参照してください。

* [プロジェクトの通貨を変更](../../../manage-work/projects/project-finances/change-project-currency.md)
* [担当業務の作成と管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

為替レートを設定する方法は、特定のプロジェクトの為替レートをユーザーが変更できるかどうかに影響します。

>[!IMPORTANT]
>
>Workfrontの為替レートは動的ではありません。設定する値は、為替レートの変更が発生した場合に更新する必要があります。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront管理者である。</p> <p><b>注意</b>：まだアクセス権がない場合は、Workfront管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 為替レートの設定

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **プロジェクト環境設定** > **為替レート。**

1. クリック **通貨を追加します。**
1. 通貨の名前を入力し始め、ドロップダウンリストに表示されたらクリックします。

1. 指定したフィールドで、システムで基準通貨として設定される通貨に関連して、選択した通貨のレートを指定します。
1. （オプション）通貨をWorkfrontの基本（デフォルト）通貨として設定します。

   これは、システム全体ですべてのプロジェクトとレポートのデフォルトとして使用される通貨です。

1. クリック **保存** をクリックして変更を保存します。

## ユーザーがプロジェクトのデフォルトの通貨を変更できるようにする

ユーザーは、次の条件を満たした場合に、プロジェクトのデフォルトの通貨を変更できます。

* ユーザーは、為替レートに対する管理者アクセス権を持つプランライセンスを持っています。

  詳しくは、 [特定の領域に対する管理者アクセス権をユーザーに付与する](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Workfrontシステムで複数の通貨が有効になっています。

ユーザーが特定のプロジェクトでデフォルトの通貨を変更する方法について詳しくは、 [プロジェクトの通貨を変更](../../../manage-work/projects/project-finances/change-project-currency.md).

## ジョブの役割の既定の通貨をユーザーが変更できるようにします

次の条件を満たす場合、ユーザーはジョブの役割の通貨を変更できます。

* ユーザーは、ジョブロールに対する管理者アクセス権を持つプランライセンスを持っています。

  詳しくは、 [特定の領域に対する管理者アクセス権をユーザーに付与する](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Workfrontシステムで複数の通貨が有効になっています。

特定のジョブの役割でユーザーがデフォルトの通貨を変更する方法について詳しくは、 [ジョブの役割の作成と管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).
