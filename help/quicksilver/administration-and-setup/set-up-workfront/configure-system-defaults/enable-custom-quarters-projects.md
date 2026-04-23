---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: カスタム四半期を有効にする
description: レポートの目的で、組織の四半期がカレンダーの日付（営業日や買い物日など）以外の特定の条件に基づいている場合は、カスタム四半期を作成できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0f643d36-6235-4fd3-b6d3-54fbd03c9b33
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 453dbf1c7598858e99d963f7a3806355a8cc80a9
workflow-type: tm+mt
source-wordcount: '364'
ht-degree: 57%

---

# カスタム四半期の有効化

<!--Audited: 03/2026-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

レポートの目的で、組織の四半期がカレンダーの日付（営業日や買い物日など）以外の特定の条件に基づいている場合は、カスタム四半期を作成できます。

会社が購入した商品に応じて、Workfrontの設定領域で次の数の四半期を設定できます。

* [!DNL Workfront]のみを購入したお客様は、[!DNL Adobe Workfront] システムに対して最大8つのカスタム四半期を設定できます。
* [!DNL Workfront]および[!DNL Workfront Planning]を購入したお客様は、ご使用の[!DNL Workfront] システムに対して最大100 クォーターを設定できます。このクォーターは[!DNL Planning]でも利用できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## [!DNL Workfront] システムのカスタム四半期を設定する

{{step-1-to-setup}}

1. **[!UICONTROL カスタム四半期]**&#x200B;をクリックします。

1. 「**[!UICONTROL カスタム四半期を有効にする]**」を選択します。

1. 「2021 年度第 1 四半期」などのカスタム四半期の名前を入力します。
1. カスタム四半期の開始日と終了日を選択します。

   ![ カスタム四半期](assets/custom-quarters-nwe.png)

1. （オプション）「**[!UICONTROL カスタム四半期を追加]**」をクリックして、システムにカスタム四半期を追加します。

   >[!IMPORTANT]
   >
   > 会社が[!DNL Workfront Planning]を購入した場合、四半期の間にギャップまたは重複がある場合は、カスタム四半期を保存できません。
   >![重複警告を含むカスタム四半期](assets/custom-quarters-with-overlap-warning.png)
   >四半期間のギャップと重複は、[!DNL Workfront]人のお客様に対してのみ許可されます。

1. （オプションおよび条件付き）会社が[!DNL Workfront]なしで[!DNL Workfront Planning]のみを購入した場合は、会計四半期を参照するレポート要素を作成します。

   **例：**[!UICONTROL プロジェクト]リストのフィルターを作成し、カスタム四半期を参照するプロジェクトの予定完了日を含めます。

   ![ カスタム四半期を含むプロジェクトフィルター](assets/example-of-project-filter-with-custom-quarters.png)

   「今四半期」、「次四半期」、「前四半期」の参照は、カスタム四半期の新しい参照に置き換えられます。

   レポート要素について詳しくは、[レポート要素：フィルター、ビュー、およびグループ化](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)を参照してください。

   フィルターの作成について詳しくは、[フィルターを作成または編集 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)を参照してください。
1. （オプションおよび条件付き）会社がWorkfront Planningを購入し、[!DNL Workfront Planning]にアクセスできる場合は、レコードタイプページに移動してタイムラインビューを開きます。 ビューには、新しいカスタム四半期が表示されます。
詳しくは、[タイムラインビューの管理](/help/quicksilver/planning/views/manage-the-timeline-view.md)を参照してください。
