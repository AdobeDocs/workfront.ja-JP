---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: シナリオ・プランナを使用するために必要なアクセス
description: シナリオプランナーには、Adobe Workfrontとは別のライセンスと追加のアクセス権が必要です。
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---

# を使用するために必要なアクセス [!DNL Scenario Planner]

この [!DNL Scenario Planner] には、追加のライセンスが必要です。 詳しくは、 [!DNL Workfront Scenario Planner]を参照してください。 [この [!DNL Scenario Planner] 概要](../scenario-planner/scenario-planner-overview.md).

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

正しいアクセス権や権限がないと、 [!UICONTROL シナリオ] ～の面積[!DNL  Adobe Workfront] 組織のプランやイニシアチブを管理することもできません。 プランとイニシアチブの管理には、プランとイニシアチブの作成、編集、削除が含まれます。

>[!IMPORTANT]
>
>アクセス時 [!UICONTROL シナリオ]を使用すると、自分が作成したプランの表示と管理のみが可能です。 作成したプランの表示や管理を他のユーザーに許可する場合は、次の手順を実行する必要があります。
>
>* プランへのリンクを他のユーザーに送信
>* プランを他のユーザーと共有
>
>  プランの共有について詳しくは、 [プランを [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).
>
>ユーザーが非アクティブ化されると、そのプランには所有者がなく、以前にリンクと共有されていない限りアクセスできなくなります。

## を表示して使用するために必要なアクセス [!DNL Adobe Workfront Scenario Planner]

次の条件がすべて満たされていることを確認してから、 [!DNL Workfront Scenario Planner]:

<!--drafted for P&P:

* Depending on whether you use the current or the legacy Workfront plans, your organization must have the following:

  * For the current plans:  

    * The [!UICONTROL Ultimate] [!DNL Workfront] plan.

      Or
  
    * The [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Workfront] plan, in addition to purchasing a separate [!DNL Scenario Planner] license.

  * For the legacy plans: (indent the bullets below, before the NOTE)

-->

* 組織では、 [!DNL Workfront] [!UICONTROL 法人] またはそれ以降 [!DNL Workfront] プラン 詳しくは、 [!DNL Workfront] プラン、詳しくは、 [Workfront Plans](http://workfront.com/plans).
* 組織では、 [!DNL Workfront Scenario Planner] ライセンス ( [!DNL Workfront] ライセンス。 お問い合わせ [!DNL Workfront] アカウント担当者にお問い合わせください [!DNL Workfront Scenario Planner] ライセンス。

<!--drafted for P&P: 

* Depending on whether you use the current or legacy licenses, your [!DNL Workfront] administrator must assign you a license of any of the following types: 

  * For the current licenses: 
    * [!UICONTROL Standard]
    * [!UICONTROL Light]

  * For the legacy licenses: (re-indent the licenses below and reword the sentence)

-->



* お使いの [!DNL Workfront] 管理者は、次のいずれかのライセンスを割り当てる必要があります [!DNL Workfront] タイプ：

   * [!UICONTROL 計画]
   * [!UICONTROL 作業]
   * [!UICONTROL 確認]

   >[!NOTE]
   >
   >を持つユーザー [!UICONTROL リクエスト] または [!UICONTROL 外部] ライセンスの種類が [!DNL Workfront Scenario Planner].

<!--drafted - replace the note above with this at P&P release: 
  * When using the current licenses, users with a [!UICONTROL Contributor] or [!UICONTROL External] license type cannot access the [!DNL Scenario Planner].
  * When using the legacy licenses, users with a Request or External license type cannot access the Scenario Planner. -->

* お使いの [!DNL Workfront] 管理者が [!UICONTROL 表示] または [!UICONTROL 編集] ～へのアクセス [!DNL Scenario Planner] を設定します。

   へのアクセス権の付与に関する情報 [!DNL Workfront Scenario Planner]を参照してください。 [へのアクセス権の付与 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* （オプションおよび推奨）プランやイニシアチブの財務情報を表示または更新するには、 [!DNL Workfront] 管理者は、ユーザーに対してもアクセス権を付与する必要があります [!UICONTROL 財務データ] を設定します。 アクセス・レベルでの財務データの付与の詳細は、 [財務データへのアクセス権の付与](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

   <!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

* 作成していないプランにアクセスする必要がある場合は、プラン作成者が、そのプランに対して正しいアクセス権を与える必要があります。 作成しなかったプランやイニシアチブへのアクセスに必要な権限については、 [プランとイニシアチブへのアクセスに必要な権限](#permissions-needed-to-access-plans-and-initiatives) 」の節を参照してください。

## プランとイニシアチブを表示するために必要なアクセス

お客様の会社に加えて、 [!DNL Workfront Scenario Planner]、 [!DNL Workfront] 管理者は、次のアクセス権と設定を割り当てて、 [!DNL Workfront Scenario Planner] この領域の情報は次のとおりです。

* 少なくとも [!UICONTROL 表示] ～へのアクセス [!DNL Scenario Planner].

   へのアクセスレベルについて [!DNL Scenario Planner]を参照してください。 [へのアクセス権の付与 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* 少なくとも [!UICONTROL 表示] ～へのアクセス [!UICONTROL 財務データ] プランとイニシアチブに関する財務情報も表示する必要がある場合。 財務情報の例としては、予算、コスト、または役割率があります。

   詳しくは、 [!UICONTROL 財務データ] アクセスレベル： [財務データへのアクセス権の付与](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

   >[!TIP]
   >
   >[!UICONTROL リクエスタ] および [!UICONTROL 外部] ユーザーは、 [!DNL Scenario Planner].

* プランに対する権限を表示します。 作成しなかったプランやイニシアチブへのアクセスに必要な権限については、 [プランとイニシアチブへのアクセスに必要な権限](#permissions-needed-to-access-plans-and-initiatives) 」の節を参照してください。

## プランとイニシアチブの管理に必要なアクセス

お使いの [!DNL Workfront] 管理者は、 [!DNL Scenario Planner]:

* A [!UICONTROL プラン] または [!UICONTROL 作業] に対する編集アクセス権を持つライセンスタイプ [!DNL Scenario Planner] を設定します。

   その他のライセンスの種類には、プランを管理するためのアクセス権がありません。

   へのアクセス許可の詳細 [!DNL Scenario Planner] アクセスレベルから、 [へのアクセス権の付与 [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* A [!UICONTROL プラン] ライセンスの種類 [!UICONTROL 編集] ～へのアクセス [!UICONTROL 財務データ] アクセスレベルで、プランに関する財務情報も更新する必要がある場合。

   編集可能な財務情報の例は次のとおりです。 [!UICONTROL 予算], [!UICONTROL 計画済み特典]、および [!UICONTROL 固定コスト].

   >[!TIP]
   >
   >のみ [!UICONTROL プラン] ライセンス所有者 [!UICONTROL 編集] ～へのアクセス [!UICONTROL 財務データ].

   詳しくは、 [!UICONTROL 財務データ] アクセスレベル： [財務データへのアクセス権の付与](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* 自分が作成しなかったプランに対する権限を管理します。 作成しなかったプランやイニシアチブへのアクセスに必要な権限については、 [プランとイニシアチブへのアクセスに必要な権限](#permissions-needed-to-access-plans-and-initiatives) 」の節を参照してください。

## プランとイニシアチブへのアクセスに必要な権限

アクセスレベルは、 [!DNL Workfront] を使用して、自分が作成しなかったプランやイニシアチブを目で見ることができます。 正しいアクセスレベルで [!DNL Scenario Planner]を使用する場合は、表示または管理するプランに対する正しい権限も持っている必要があります（これらのプランの作成者でない場合）。

デフォルトでは、自分が作成したプランにのみアクセスできます。 他のユーザーが作成したプランを表示するには、自分のプランを自分と共有する必要があります。 プランの共有について詳しくは、 [プランを [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

プランを共有せずにプランへのリンクを共有した場合は、プランに対する権限を要求できます。 プランに対する権限のリクエストについては、 [内のプランへのアクセスをリクエスト [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).

