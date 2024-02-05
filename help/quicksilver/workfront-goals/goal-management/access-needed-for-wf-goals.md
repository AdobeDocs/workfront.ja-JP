---
content-type: reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Workfront Goals の使用要件
description: Adobe Workfront Goals にアクセスする前に、Adobe Workfront の管理者が、特定の条件が満たされていることを確認する必要があります。
author: Alina
feature: Workfront Goals
exl-id: 3c7c832b-3e00-4ced-8829-8b1c23fa3871
source-git-commit: 86f9a88518c8a03643061b3328719d2da4016f2b
workflow-type: tm+mt
source-wordcount: '616'
ht-degree: 96%

---

# Workfront Goals の使用要件

Adobe Workfront Goals にアクセスする前に、Adobe Workfront の管理者が、次の条件がすべて満たされていることを確認する必要があります。

<!--drafted for P&P - replace the first bullet with this one when licensing changes: 
* Your company must purchase the correct Adobe Worfront plan or Adobe Workfront Goal license. For information, see the section [Obtain Workfront Goals organization access](#obtain-workfront-goals-organization-access)in this article.-->

* 組織は、Workfront Goals の正規のライセンスを購入する必要があります。詳しくは、この記事の [Workfront Goals への組織のアクセス権の取得](#obtain-workfront-goals-organization-access)の節を参照してください。

* 適切なタイプの Workfront ライセンスが割り当てられます。ライセンスタイプとアクセスレベルの割り当てについては、[ライセンスタイプとアクセスレベルの設定を更新](#update-license-types-and-access-level-settings)の節を参照してください。

>[!NOTE]
>
>外部ライセンスタイプを所有のユーザーは、Workfront Goals にアクセスできません。

* ご自身のアクセスレベルで Goals にアクセスできます。詳しくは、[Adobe Workfront Goals へのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)を参照してください。

* メインメニューの Goals エリアを含むレイアウトテンプレートが割り当てられます。

  >[!NOTE]
  >
  >Workfront管理者を含むすべてのユーザーに、メインメニューの目標領域を含むレイアウトテンプレートを割り当てる必要があります。

  詳しくは、この記事の [Workfron Goals レイアウトテンプレートに追加](#add-workfront-goals-to-a-layout-template)の節を参照してください。

* 自分で作成していない目標を変更する必要がある場合は、目標の作成者が目標を自分と共有し、目標の管理権限を作成者から付与される必要があります。

  詳しくは、この記事の[他のユーザーと個人の目標を共有](#share-individual-goals-with-other-users)の節を参照してください。

## Workfront Goals への組織のアクセス権の取得 {#obtain-workfront-goals-organization-access}

<!--drafted for P&P release: 

If your company has a current Workfront plan, you must have one of the following:

* An Ultimate Workfront plan. Workfront Goals are included in this plan. 
* A Select or higher Workfront plan and a separate Workfront Goals license. -->

<!-- drafted for P&P - add this to the sentence below at release: 

If your company has a legacy Workfront plan, -->

ユーザーが Workfront Goals にアクセスできるようにするには、Workfront ライセンスに加えて、追加のライセンスを購入する必要があります。組織が追加のライセンスを購入すると、Workfront をお使いのアカウントで Workfront Goals が有効になります。Workfront Goals のライセンスの購入について詳しくは、Workfront のアカウントマネージャーにお問い合わせください。

## ライセンスタイプとアクセスレベルの設定の更新  {#update-license-types-and-access-level-settings}

<!--drafted for P&P release: 
If your company has the current access level model, your Workfront administrator must grant you one of the following Workfront license types to access Workfront Goals: 

* Contributor
* Light
* Standard-->

<!--drafted for P&P release: add this to the first sentence: 
If your company has the legacy access level model, -->

Workfront Goals にアクセスするためには、次のいずれかの Workfront ライセンスタイプを、Workfront の管理者が付与する必要があります。

* プラン
* ワーク
* レビュー
* リクエスト

Workfront 管理者がこれらのライセンスタイプの 1 つを付与したら、Goals に対するアクセスレベルでのアクセス権も付与する必要があります。Goals へのアクセスについて詳しくは、[Adobe Workfront Goals へのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)を参照してください。

Workfront 管理者は、システム内の Workfront Goals ライセンスの数を確認し、現在有効になっている数を把握できます。詳しくは、[システムで使用可能なライセンスの管理](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md)を参照してください。

>[!NOTE]
>
>Workfront では、購入した Workfront Goals ライセンス以上を割り当てることができます。ただし、Workfront Goals の契約で許可されている数を超えるライセンスを割り当てると、Workfront のアカウントマネージャーから連絡があり、契約上の数を超えたことが通知されます。

## Workfront Goals をレイアウトテンプレートに追加 {#add-workfront-goals-to-a-layout-template}

Workfront Goals にアクセスできるようにするため、Workfront 管理者またはグループ管理者が、メインメニューの Goals エリアを含むレイアウトテンプレートを割り当てる必要があります。

![](assets/layout-template-align-highlighted-350x220.png)

Workfront 管理者またはグループ管理者は、Workfront Goals に簡単にアクセスできるようにするために、レイアウトテンプレートに以下のものを追加することもできます。

* 固定タブ
* Goals エリアをランディングページにする

レイアウトテンプレートの更新について詳しくは、次の記事を参照してください。

* [レイアウトテンプレートの作成と管理](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)
* [レイアウトテンプレートを使用したメインメニューのカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
* [レイアウトテンプレートを使用した固定ページのカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
* [レイアウトテンプレートを使用したランディングページのカスタマイズ](../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
* [レイアウトテンプレートにユーザーを割り当て](../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

## 他のユーザーとの個人の目標の共有 {#share-individual-goals-with-other-users}

デフォルトでは、アクセスレベルで Goals への表示アクセス権を持つすべてのユーザーが、Workfront ですべての目標を表示できます。

Goals への編集アクセス権を持つユーザーは誰でも目標を作成でき、自分が作成した目標の管理アクセス権を自動的に取得します。他のユーザーの目標を編集する必要がある場合は、それらの目標の管理権限を持つユーザーが、他のユーザーが作成しなかった目標を共有する必要があります。

ユーザーとの目標の共有と管理権限の付与について詳しくは、[Workfront Goals での目標の共有](../../workfront-goals/workfront-goals-settings/share-a-goal.md)を参照してください。
