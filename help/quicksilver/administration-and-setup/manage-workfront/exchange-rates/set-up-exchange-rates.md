---
user-type: administrator
product-area: system-administration;setup
navigation-topic: exchange-rates
title: 為替レートの設定
description: 為替レートは、Workfront のすべての財務要素に影響を与えます。基本通貨は、システム全体のすべてのプロジェクトのデフォルト通貨です。
feature: System Setup and Administration
role: Admin
author: Lisa
exl-id: 149c08de-fd3a-465a-afd1-0b53012d30d8
source-git-commit: b16523bf6c37747702efe3b5ecfcc33801526af1
workflow-type: tm+mt
source-wordcount: '834'
ht-degree: 41%

---

# 為替レートの設定

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">*** DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

{{highlighted-preview}}

Adobe Workfront 管理者は、Workfront で為替レートを設定できます。これには次が含まれます。

* Workfront システムのデフォルト通貨の設定
* 現在の為替レートに一致するように Workfront の為替レートを更新
* 複数の通貨の為替レートの設定（これにより、ユーザーはプロジェクトごとにデフォルト通貨を選択できます）

為替レートは、Workfront のすべての財務要素に影響を与えます。基本通貨は、特定のプロジェクトまたはジョブロールに対して上書きされない限り、システム全体のすべてのプロジェクトおよびレポートのデフォルト通貨です。 現在の基本通貨またはデフォルト通貨は、リストにアイコン ![&#x200B; デフォルト通貨アイコン &#x200B;](assets/default-icon.png)が表示されます。 また、レポートやリストで表示する際に、基準通貨やプロジェクトの通貨とは異なるシステム内で使用可能な通貨で財務情報を表示するよう選択することもできます。詳しくは、[一意の為替レートを使用した財務データレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md)を参照してください。

プロジェクトおよびジョブロールに対するWorkfrontの基本通貨の上書きについて詳しくは、次の記事を参照してください。

* [プロジェクトの通貨を変更](../../../manage-work/projects/project-finances/change-project-currency.md)
* [担当業務の作成と管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)

為替レートを設定する方法は、特定のプロジェクトの為替レートをユーザーが変更できるかどうかに影響します。

>[!IMPORTANT]
>
>Workfront の為替レートは動的ではなく、設定する値は、為替レートの変更が発生した場合に更新する必要があります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>為替レートを設定するには：任意のWorkfrontまたはワークフローパッケージ</p>
       <p>為替レートに有効な日付を適用するには：ワークフローUltimate パッケージ</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td><p>標準</p>
       <p>プラン</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>システム管理者</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 為替レートの設定

{{step-1-to-setup}}

1. **プロジェクトの環境設定** > **為替レート**&#x200B;をクリックします。
1. 「**通貨を追加**」をクリックします。
1. 「**通貨を追加**」ボックスで、通貨の名前を入力し始め、ドロップダウンリストに表示されたらクリックします。
1. 「**為替レート**」フィールドに、システムで基本通貨として設定されている通貨と比較して、選択した通貨のレートを入力します。
1. 「**追加**」をクリックして、新しい通貨とその為替レートを追加します。
1. （オプション）基本（デフォルト）通貨を変更するには、次のいずれかの操作を行います。

   * 通貨名の横にあるチェックボックスを選択し、画面下部のアクションバーで「**デフォルトにする**」を選択します。
   * 通貨名にカーソルを合わせ、表示される&#x200B;**詳細** メニューをクリックします。 次に、「**デフォルトにする**」を選択します。

     新しいデフォルト通貨は、アイコン ![&#x200B; デフォルト通貨アイコン &#x200B;](assets/default-icon.png)で更新されます。

     >[!NOTE]
     >
     >デフォルトの通貨は、リストの並べ替え方法に関係なく、常にリストの最初に表示されます。

1. （オプション）通貨を削除するには、通貨名の横にあるチェックボックスを選択し、画面下部のアクションバーで「**削除**」を選択します。 デフォルト通貨は削除できません。

<div class="preview">

## 通貨の為替レートに有効な日付を設定する

通貨の為替レートの適用日は、レート値が特定の日付で終了し、別のレートが開始されるように設定されます。 正しい日付の為替レートは、財務計算に使用されます。

{{step-1-to-setup}}

1. **プロジェクトの環境設定** > **為替レート**&#x200B;をクリックします。
1. リストで通貨を選択し、アクションバーの「**日付を管理**」をクリックします。
1. **（通貨名）日付有効レート** ダイアログで、現在の為替レートの&#x200B;**終了日**&#x200B;を選択します。

   または

   新しい為替レートの&#x200B;**開始日**&#x200B;を選択します。

   最初の為替レートには開始日がなく、最後のレートには終了日がありません。 一部の日付は自動的に追加されます。例えば、最初のレートに終了日がなく、開始日が2025年12月1日の為替レートを追加した場合、ギャップが存在しないように、2025年11月30日の終了日が最初のレートに追加されます。

   ![有効な為替レート ダイアログの日付](assets/euro-date-effective-rates.png)

1. 新しい&#x200B;**為替レート**&#x200B;値を入力します。
1. （オプション）「**日付有効レートを追加**」をクリックして、この通貨の有効な日付を含む為替レートをさらに追加します。
1. 「**保存**」をクリックします。

</div>

## ユーザーがプロジェクトのデフォルト通貨を変更できるようにする

ユーザーは、次の条件を満たした場合に、プロジェクトのデフォルト通貨を変更できます。

* ユーザーは、Exchange Ratesへの管理アクセス権を持つStandardまたはPlan ライセンスを持っています。

  詳しくは、[特定のエリアに対する管理者アクセス権をユーザーに付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)を参照してください。

* Workfront システムで複数の通貨が有効になっています。

ユーザーが特定のプロジェクトでデフォルトの通貨を変更する方法について詳しくは、[プロジェクトの通貨の変更](../../../manage-work/projects/project-finances/change-project-currency.md)を参照してください。

## 担当業務のデフォルトの通貨をユーザーが変更できるようにする

次の条件を満たす場合、ユーザーは担当業務の通貨を変更できます。

* ユーザーには、ジョブロールへの管理アクセス権を持つ標準またはプランのライセンスがあります。

  詳しくは、[特定のエリアに対する管理者アクセス権をユーザーに付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md)を参照してください。

* Workfront システムで複数の通貨が有効になっています。

特定の担当業務でユーザーがデフォルトの通貨を変更する方法について詳しくは、[担当業務の作成と管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)を参照してください。



