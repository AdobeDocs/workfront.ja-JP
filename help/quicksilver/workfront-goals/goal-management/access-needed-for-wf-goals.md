---
content-type: reference
product-previous: workfront-goals
navigation-topic: goal-management
title: Workfront Goals を使用するための要件
description: Adobe Workfront Goals にアクセスするには、Adobe Workfront管理者が特定の条件を満たしていることを確認する必要があります。 この記事では、Workfront Goals にアクセスするためのアクセス権、権限、レイアウト要件について説明します。
author: Alina
feature: Workfront Goals
exl-id: 3c7c832b-3e00-4ced-8829-8b1c23fa3871
source-git-commit: dacfd8ef7475b197ac6ce5dd598c99df97037479
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 71%

---

# Workfront Goals の使用要件

<!--Audited P&P only: 04/2025-->

Adobe Workfront Goals にアクセスする前に、Adobe Workfront の管理者が、次の条件がすべて満たされていることを確認する必要があります。

* お客様の組織が過去にAdobe Workfront Goals パッケージを購入したことがある。 Adobe Workfront Goals は購入できなくなりました。

  詳しくは、この記事の [Workfront Goals 組織のアクセス権の取得 ](#obtain-workfront-goals-organization-access) を参照してください。

* 適切なタイプの Workfront ライセンスが割り当てられます。ライセンスタイプとアクセスレベルの割り当てについては、[ライセンスタイプとアクセスレベルの設定を更新](#update-license-types-and-access-level-settings)の節を参照してください。

  >[!NOTE]
  >
  >外部ライセンスタイプを所有のユーザーは、Workfront Goals にアクセスできません。

* ご自身のアクセスレベルで Goals にアクセスできます。詳しくは、[Adobe Workfront Goals へのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)を参照してください。

  >[!NOTE]
  >
  >デフォルトでは、ユーザーはアクセスレベルで目標へのアクセス権を取得できません。


* メインメニューの Goals エリアを含むレイアウトテンプレートが割り当てられます。

  >[!NOTE]
  >
  >システム管理者を含むすべてのユーザーには、メインメニューの目標エリアを含むレイアウトテンプレートを割り当てる必要があります。

  詳しくは、この記事の [Workfron Goals レイアウトテンプレートに追加](#add-workfront-goals-to-a-layout-template)の節を参照してください。

* 自分で作成していない目標を変更する必要がある場合は、目標の作成者が目標を自分と共有し、目標の管理権限を作成者から付与される必要があります。

  詳しくは、この記事の[他のユーザーと個人の目標を共有](#share-individual-goals-with-other-users)の節を参照してください。

## Workfront Goals への組織のアクセス権の取得 {#obtain-workfront-goals-organization-access}

Workfront Goals を含む最後のAdobe Workfront パッケージは、Adobe Workfront Ultimateでした。
新しいパッケージでは、Workfront Goals は購入できなくなりました。
Workfront Goals については、アカウント担当者にお問い合わせください。

<!--Old: >
Depending on which Workfront plan your company is currently on, the following scenarios exist: 

* **A new Workfront plan**: You must have an Ultimate Workfront plan. Workfront Goals are included only in this plan. 

* **A current Workfront plan**: Your organization must purchase an additional license, in addition to the Workfront license.

  After your organization purchases the additional license, Workfront enables Workfront Goals for your account. For information about purchasing a license for Workfront Goals contact your Workfront account manager.

For information about Workfront access requirements, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). -->

## ライセンスタイプとアクセスレベルの設定の更新  {#update-license-types-and-access-level-settings}

以前の購入からWorkfront Goals にアクセスできる会社がある場合、Workfront Goals にアクセスするにはWorkfront管理者から次の権限を付与される必要があります。

1. 次のいずれかのライセンス：

   * 投稿者以上
   * リクエスト以上

<!--Old: 
* **The new access level model**: Your Workfront administrator must grant you one of the following Workfront license types to access Workfront Goals: 

  * Contributor
  * Light
  * Standard

* **The current access level model**: Your Workfront administrator must grant you one of the following Workfront license types to access Workfront Goals:

  * Plan
  * Work 
  * Review
  * Request
-->

1. 次のアクセス レベル：

   * アクセスレベルで目標への表示以上のアクセス権を設定します。

   Goals へのアクセスについて詳しくは、[Adobe Workfront Goals へのアクセス権の付与](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)を参照してください。

Workfront 管理者は、システム内の Workfront Goals ライセンスの数を確認し、現在有効になっている数を把握できます。詳しくは、[システムで使用可能なライセンスの管理](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md)を参照してください。

>[!NOTE]
>
>Workfront では、購入した Workfront Goals ライセンス以上を割り当てることができます。ただし、Workfront Goals の契約で許可されている数を超えるライセンスを割り当てると、Workfront のアカウントマネージャーから連絡があり、契約上の数を超えたことが通知されます。

## Workfront Goals をレイアウトテンプレートに追加 {#add-workfront-goals-to-a-layout-template}

Workfront Goals にアクセスできるようにするため、Workfront 管理者またはグループ管理者が、メインメニューの Goals エリアを含むレイアウトテンプレートを割り当てる必要があります。

![ レイアウトテンプレート ](assets/layout-template-align-highlighted-350x220.png)

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
