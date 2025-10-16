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
source-git-commit: 20ebcb74c79aea67ea7cb1ba083dfea623fe7c16
workflow-type: tm+mt
source-wordcount: '363'
ht-degree: 57%

---

# カスタム四半期を有効にする

<!--Audited: 11/2024-->

レポートの目的で、組織の四半期がカレンダーの日付（営業日や買い物日など）以外の特定の条件に基づいている場合は、カスタム四半期を作成できます。

会社が購入した商品に応じて、Workfrontの設定領域で次の四半期数を設定できます。

* [!DNL Workfront] のみを購入したお客様は、[!DNL Adobe Workfront] システムに最大 8 つのカスタム四半期を設定できます。
* [!DNL Workfront] と [!DNL Workfront Planning] を購入したお客様は、[!DNL Workfront] システムに最大 100 四半期を設定できます。この設定は [!DNL Planning] でも利用できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] package</td> 
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

1. **[!UICONTROL プロジェクト環境設定]**／**[!UICONTROL プロジェクト]をクリックします。**

1. 「**[!UICONTROL タイムライン]**」セクションで、「**[!UICONTROL カスタム四半期を有効にする]**」を選択します。

1. 「2021 年度第 1 四半期」などのカスタム四半期の名前を入力します。
1. カスタム四半期の開始日と終了日を選択します。

   ![&#x200B; カスタム四半期 &#x200B;](assets/custom-quarters-nwe.png)

1. （オプション）「**[!UICONTROL カスタム四半期を追加]**」をクリックして、システムにカスタム四半期を追加します。

   >[!IMPORTANT]
   >
   > [!DNL Workfront Planning] を購入した場合、四半期の間にギャップや重複があると、カスタム四半期を保存できません。
   >![&#x200B; 重複警告のあるカスタム四半期 &#x200B;](assets/custom-quarters-with-overlap-warning.png)
   >四半期の間のギャップと重複は、[!DNL Workfront] 顧客にのみ許可されています。

1. （オプションおよび条件付き）会社が [!DNL Workfront] のみを購入した場合、[!DNL Workfront Planning] を付けずに、会計四半期を参照するレポート要素を作成します。


   **例：**&#x200B;[!UICONTROL プロジェクト]リストのフィルターを作成し、カスタム四半期を参照するプロジェクトの予定完了日を含めます。

   ![&#x200B; カスタム四半期を使用したプロジェクトフィルター &#x200B;](assets/example-of-project-filter-with-custom-quarters.png)

   「今四半期」、「次四半期」、「前四半期」の参照は、カスタム四半期の新しい参照に置き換えられます。

   レポート要素について詳しくは、[レポート要素：フィルター、ビュー、およびグループ化](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)を参照してください。

   フィルターの作成について詳しくは、[フィルターを作成または編集 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)を参照してください。
1. （オプションおよび条件付き） [!DNL Workfront Planning] へのアクセス権を持っている場合は、レコードタイプのページに移動して、タイムライン表示を開きます。 ビューには、新しいカスタム四半期が表示されます。
詳しくは、[タイムラインビューの管理](/help/quicksilver/planning/views/manage-the-timeline-view.md)を参照してください。
