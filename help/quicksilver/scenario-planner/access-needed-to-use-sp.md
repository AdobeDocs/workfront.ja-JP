---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Scenario Planner を使用するために必要なアクセス権
description: シナリオプランナーには、Adobe Workfront ライセンスとは別のライセンスと追加のアクセス権が必要です。
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: f0f6c2bee98c6cebf8ea9e18bf34262f3c1d6e3a
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 79%

---

# [!DNL Scenario Planner] の使用に必要なアクセス権

[!DNL Scenario Planner] には、追加のライセンスが必要です。[!DNL Workfront Scenario Planner] について詳しくは、[ [!DNL Scenario Planner]  の概要](../scenario-planner/scenario-planner-overview.md)を参照してください。

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

正しいアクセス権や権限がないと、[!DNL  Adobe Workfront] の[!UICONTROL シナリオ]エリアの表示や、組織のプランとイニシアチブの管理ができない場合があります。プランとイニシアチブの管理には、プランとイニシアチブの作成、編集、削除も含まれます。

>[!IMPORTANT]
>
>[!UICONTROL シナリオ]へのアクセス時は、自分が作成したプランの表示と管理のみが可能です。自分が作成したプランの表示や管理を他のユーザーに許可する場合は、次の手順を実行する必要があります。
>
>* プランへのリンクを他のユーザーに送信
>* プランを他のユーザーと共有
>
>  プランの共有について詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md) でのプランの共有を参照してください。
>
>ユーザーが非アクティブ化されると、そのユーザーのプランの所有者が存在しなくなり、それまでにリンクによって共有されていない限りアクセスできなくなります。

## [!DNL Adobe Workfront Scenario Planner] の表示や使用に必要なアクセス権

[!DNL Workfront Scenario Planner] にアクセスするには、次の条件がすべて満たされていることを確認する必要があります。

1. 所属する組織で、以下に説明するWorkfront プランのいずれかが必要です。

   新しいWorkfrontプランと現在の Workfront プランのどちらを使用するかに応じて、組織には次のいずれかが必要です。

   * 新しいプランの場合、組織には次のいずれかが必要です。

      * [!UICONTROL Ultimate][!DNL Workfront] プラン。 シナリオプランナーは Ultimate 計画に含まれています。

        または

      * [!UICONTROL Select] または [!UICONTROL Prime][!DNL Workfront] プランで、別途 [!DNL Scenario Planner] ライセンスを購入します。

   * 現在のWorkfront プランでは、組織に次の両方が必要です。

      * 組織では、[!DNL Workfront] の[!UICONTROL ビジネス]プランまたはそれ以上の [!DNL Workfront] プランを購入する必要があります。[!DNL Workfront] のプランについて詳しくは、[Workfront プラン](https://workfront.com/plans)を参照してください。

      * 組織では、[!DNL Workfront] ライセンスに加え、[!DNL Workfront Scenario Planner] ライセンスを購入する必要があります。[!DNL Workfront Scenario Planner] ライセンスについて詳しくは、[!DNL Workfront] アカウント担当者にお問い合わせください。

1. 以下に説明するWorkfront ライセンスが 1 つ必要です。

   新しいライセンスと現在のライセンスのどちらを使用するかに応じて、[!DNL Workfront] 管理者は次のいずれかのタイプのライセンスを割り当てる必要があります。

   * 新しいライセンスの場合：
      * [!UICONTROL 標準]
      * [!UICONTROL ライト]

   * 現在のライセンスについて：

      * [!UICONTROL 計画]
      * [!UICONTROL 作業]
      * [!UICONTROL 確認]

   >[!NOTE]
   > 
   >* 新しいライセンスを使用する際、[!UICONTROL  コントリビューター ] または [!UICONTROL  外部 ] ライセンスタイプを持つユーザーは、[!DNL Scenario Planner] にアクセスできません。
   >
   >* 現在のライセンスを使用する場合、リクエストまたは外部ライセンスタイプを持つユーザーは、シナリオプランナーにアクセスできません。

1. [!DNL Workfront] 管理者は、ユーザーのアクセスレベルで [!DNL Scenario Planner] に対する[!UICONTROL 表示]または[!UICONTROL 編集]のアクセス権を付与する必要があります。

   [!DNL Workfront Scenario Planner] へのアクセス権の付与について詳しくは、[ [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md) へのアクセス権の付与を参照してください。

1. （オプションおよび推奨）プランやイニシアチブの財務情報を表示または更新するには、[!DNL Workfront] 管理者がユーザーのアクセスレベルで[!UICONTROL 財務データ]へのアクセス権も付与する必要があります。アクセスレベルでの財務データへのアクセス権の付与について詳しくは、[財務データへのアクセス権の付与](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)を参照してください。

1. （オプション）自分が作成していないプランにアクセスする必要がある場合、プラン作成者は、プランにアクセスするための正しい権限を付与する必要があります。 作成していないプランやイニシアチブへのアクセスに必要な権限について詳しくは、[プランやイニシアチブへのアクセスに必要な権限](#permissions-needed-to-access-plans-and-initiatives)の節を参照してください。

<!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

## プランやイニシアチブの表示に必要なアクセス権

会社が [!DNL Workfront Scenario Planner] の正しいライセンスを取得するのに加えて、[!DNL Workfront] 管理者は、ユーザーに次のアクセス権と設定を割り当てて、ユーザーが [!DNL Workfront Scenario Planner] およびこのエリアの情報を表示できるようにする必要があります。

* 少なくとも [!DNL Scenario Planner] への[!UICONTROL 表示]アクセス権があるアクセスレベル。

  [!DNL Scenario Planner] へのアクセスレベルについて詳しくは、[ [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md) へのアクセス権の付与を参照してください。

* プランやイニシアチブに関する財務情報も表示する必要がある場合は、少なくとも[!UICONTROL 財務データ]への[!UICONTROL 表示]アクセス権があるアクセスレベル。財務情報の例としては、予算、コスト、または担当業務の料率があります。

  [!UICONTROL 財務データ]のアクセスレベルについて詳しくは、[財務データへのアクセス権の付与](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)を参照してください。

  >[!TIP]
  >
  >[!UICONTROL 要求者]および[!UICONTROL 外部]ユーザーは、[!DNL Scenario Planner] を表示するアクセス権を持っていません。

* プランに対する表示権限。作成していないプランやイニシアチブへのアクセスに必要な権限について詳しくは、[プランやイニシアチブへのアクセスに必要な権限](#permissions-needed-to-access-plans-and-initiatives)の節を参照してください。

## プランやイニシアチブの管理に必要なアクセス権

[!DNL Workfront] 管理者は、ユーザーが [!DNL Scenario Planner] でプランや情報を管理できるようにするには、次のアクセス権を付与する必要があります。

* アクセスレベルで [!DNL Scenario Planner] への編集アクセス権がある[!UICONTROL プラン]または[!UICONTROL ワーク]ライセンスタイプ。

  その他すべてのライセンスタイプには、プランを管理するためのアクセス権がありません。

  アクセスレベルからの [!DNL Scenario Planner] へのアクセス権の付与について詳しくは、[ [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md) へのアクセス権の付与を参照してください。

* プランに関する財務情報も更新する必要がある場合は、アクセスレベルで[!UICONTROL 財務データ]への[!UICONTROL 編集]アクセス権がある[!UICONTROL プラン]ライセンスタイプ。

  編集可能な財務情報の例としては、[!UICONTROL 予算]、[!UICONTROL 予定利益]、または[!UICONTROL 固定費]があります。

  >[!TIP]
  >
  >[!UICONTROL 財務データ]への[!UICONTROL 編集]アクセス権を持つのは、[!UICONTROL プラン]ライセンスの所有者のみです。

  [!UICONTROL 財務データ]のアクセスレベルについて詳しくは、[財務データへのアクセス権の付与](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)を参照してください。

* 自分が作成しなかった計画に対する権限を管理します。作成しなかった計画やイニシアチブへのアクセスに必要な権限について詳しくは、[計画およびイニシアチブへのアクセスに必要な権限](#permissions-needed-to-access-plans-and-initiatives)の節を参照してください。

## 計画およびイニシアチブへのアクセスに必要な権限

アクセスレベルは、[!DNL Workfront] を使用して、自分が作成しなかった計画やイニシアチブを目で見ることができます。[!DNL Scenario Planner] にアクセスするための適切なアクセスレベルを持っていることに加え、これらのプランの作成者でない場合、表示または管理する計画に対して適切な権限を持っている必要があります。

デフォルトでは、自分が作成した計画にのみアクセスできます。他のユーザーが作成した計画を表示するには、自分の計画を自分と共有する必要があります。計画の共有について詳しくは、[ [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md) での計画の共有を参照してください。

計画を共有せずに計画へのリンクを共有した場合は、計画に対する権限をリクエストできます。プランに対する権限のリクエストについては、[ 内の計画へのアクセスのリクエスト [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md)を参照してください。

