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
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '442'
ht-degree: 57%

---

# カスタム四半期を有効にする

<!--Audited: 11/2024-->

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。[!DNL Adobe Workfront Planning] を購入したすべての顧客が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

レポートの目的で、組織の四半期がカレンダーの日付（営業日や買い物日など）以外の特定の条件に基づいている場合は、カスタム四半期を作成できます。

<div class="preview">

会社が購入した商品に応じて、Workfrontの設定領域で次の四半期数を設定できます。

* [!DNL Workfront] のみを購入したお客様は、[!DNL Adobe Workfront] システムに最大 8 つのカスタム四半期を設定できます。
* [!DNL Workfront] と [!DNL Workfront Planning] を購入したお客様は、[!DNL Workfront] システムに最大 100 四半期を設定できます。この設定は [!DNL Planning] でも利用できます。

</div>

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td><p>新規：[!UICONTROL Standard]</p>
   または
   <p>現在：[!UICONTROL Plan]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## [!DNL Workfront] システムのカスタム四半期を設定する

{{step-1-to-setup}}

1. **[!UICONTROL プロジェクト環境設定]**／**[!UICONTROL プロジェクト]をクリックします。**

1. 「**[!UICONTROL タイムライン]**」セクションで、「**[!UICONTROL カスタム四半期を有効にする]**」を選択します。

1. 「2021 年度第 1 四半期」などのカスタム四半期の名前を入力します。
1. カスタム四半期の開始日と終了日を選択します。

   ![ カスタム四半期 ](assets/custom-quarters-nwe.png)

1. （オプション）「**[!UICONTROL カスタム四半期を追加]**」をクリックして、システムにカスタム四半期を追加します。

   >[!IMPORTANT]
   >
   > <span class="preview">[!DNL Workfront Planning] を購入した場合、四半期の間にギャップや重複があると、カスタム四半期を保存できません。</span>
   ><span class="preview">![ 重複警告のあるカスタム四半期 ](assets/custom-quarters-with-overlap-warning.png)</span>
   >四半期の間のギャップと重複は、[!DNL Workfront] 顧客にのみ許可されています。

1. （オプションおよび条件付き）会社が [!DNL Workfront] のみを購入した場合、[!DNL Workfront Planning] を付けずに、会計四半期を参照するレポート要素を作成します。


   **例：**&#x200B;[!UICONTROL プロジェクト]リストのフィルターを作成し、カスタム四半期を参照するプロジェクトの予定完了日を含めます。

   ![ カスタム四半期を使用したプロジェクトフィルター ](assets/example-of-project-filter-with-custom-quarters.png)

   「今四半期」、「次四半期」、「前四半期」の参照は、カスタム四半期の新しい参照に置き換えられます。

   レポート要素について詳しくは、[レポート要素：フィルター、ビュー、およびグループ化](../../../reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md)を参照してください。

   フィルターの作成について詳しくは、[フィルターを作成または編集 [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/create-filters.md)を参照してください。
1. <span class="preview"> （オプションおよび条件付き） [!DNL Workfront Planning] へのアクセス権を持っている場合は、レコードタイプのページに移動して、タイムライン表示を開きます。 ビューには、新しいカスタム四半期が表示されます。</span>
