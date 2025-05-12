---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: システム全体のフィルター、ビュー、グループ化の作成、編集、共有
description: デフォルトのフィルター、ビューおよびグループ化を作成すると、組織内のユーザーが使用できるようなります。
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: ad6d983524e19e60e0c884faed2990d9fa6549d7
workflow-type: tm+mt
source-wordcount: '742'
ht-degree: 62%

---

# システム全体のフィルター、ビュー、グループ化の作成、編集、共有

<!-- Audited: 5/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

フィルター、ビュー、グループ化を作成し、組織内のシステム全体でユーザーが使用できるようにします。

この記事で説明するようにシステム全体のフィルター、ビュー、およびグループ化を作成すると、それらを共有するユーザーは、リストを表示する際にそれらを活用できます。 ユーザーは、作成したフィルター、ビュー、グループに基づいて独自に作成できますが、直接変更することはできません。

システム全体で作成するフィルター、ビュー、グループ化は、Adobe Workfrontがシステム内で自動的に作成するデフォルトのフィルター、ビュー、グループ化とは異なることに注意してください。 これらのデフォルトのフィルター、ビュー、グループ化は、編集または削除できません。

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
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## フィルター、ビュー、グループの作成

{{step-1-to-setup}}


1. 「**[!UICONTROL インターフェース]**」をクリックし、「**[!UICONTROL フィルター]**」、「**[!UICONTROL ビュー]**」または「**[!UICONTROL グループ化]**」のいずれかをクリックします。

1. フィルター、ビューまたはグループ化を作成する場合は、「**[!UICONTROL フィルターを追加]**」、「**[!UICONTROL ビューを追加]**」または「**[!UICONTROL グループ化を追加]**」をクリックして、新しいフィルター、ビューまたはグループ化を関連付けるオブジェクトタイプを選択します。

   または

   既存のフィルター、ビューまたはグループ化を編集する場合は、そのフィルターを選択し、**[!UICONTROL 編集]**&#x200B;アイコン![編集アイコン](assets/edit-icon.png)をクリックします。

1. フィルター、ビューまたはグループ化を設定します。

   使用可能なオプションについて詳しくは、次の記事の 1 つを参照してください。

   * [フィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [[!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md) のビューの概要
   * [[!UICONTROL Adobe Workfront] のグループ化の概要](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. 左下隅付近にある「**[!UICONTROL 保存]**」をクリックします。

システム内のユーザーがフィルター、ビューまたはグループ化を使用できるようにします。他のユーザーとのフィルター、ビューまたはグループ化の共有について詳しくは、この記事の[フィルター、ビューまたはグループをユーザーに使用可能にする](#make-filters-views-or-groupings-available-to-users)を参照してください。


## レイアウトテンプレートから使用できるフィルター、ビューまたはグループ化を表示または非表示にする

レイアウトテンプレートから、フィルター、ビューまたはグループ化の表示と非表示を選択できます。表示されるフィルターは、システム全体のすべてのユーザーが使用できます。 レイアウトテンプレートを使用すると、特定のユーザーまたはグループに対して表示するフィルターを非表示にできます。

>[!NOTE]
>
>ユーザーがアクティブに使用しているフィルター、ビューまたはグループ化を管理者が無効にした場合、ユーザーは新しいフィルター、ビューまたはグループ化を選択するまでアクセスできます。新しいテンプレートを選択すると、非表示のテンプレートに戻すことはできません。

レイアウトテンプレートから使用できるフィルター、ビューまたはグループ化を表示または非表示にするには、次の手順に従います。

{{step-1-to-setup}}

1. 「**[!UICONTROL インターフェース]**」をクリックし、「**[!UICONTROL フィルター]**」、「**[!UICONTROL ビュー]**」または「**[!UICONTROL グループ化]**」のいずれかをクリックします。

1. （条件付き）ユーザーが使用できるフィルター、ビューまたはグループ化を選択し、「**[!UICONTROL システム全体で有効にする]**」をクリックします。

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >ほとんどのユーザーが使用できるフィルター、表示、グループ化を保持し、他のユーザーには非表示にする場合は、レイアウトテンプレートを使用できます。 詳しくは、[レイアウトテンプレートを使用したフィルター、ビューおよびグループ化のカスタマイズ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)を参照してください。

1. （条件付き）ユーザーに非表示にするフィルター、ビュー、またはグループ化を選択して、「**[!UICONTROL システム全体で無効にする]**」をクリックします。 フィルター、ビュー、グループ化が、システム全体でレイアウトテンプレートおよびユーザーに表示されなくなりました。


## フィルター、ビューまたはグループ化をすべてのユーザーに使用可能にする {#make-filters-views-or-groupings-available-to-users}

これらの手順では、[!UICONTROL 設定]の[!UICONTROL インターフェース]エリアにある[!UICONTROL 共有]ダイアログからフィルター、ビューおよびグループ化を使用できるようにする方法について説明します。この設定は、レイアウトテンプレートを含む、システム全体のオン／オフスイッチのように機能します。

{{step-1-to-setup}}

1. 「**[!UICONTROL インターフェース]**」をクリックし、「**[!UICONTROL フィルター]**」、「**[!UICONTROL ビュー]**」または「**[!UICONTROL グループ化]**」のいずれかをクリックします。

1. ユーザーが使用できるようにするフィルター、ビューまたはグループ化を選択し、**[!UICONTROL 共有]** アイコン ![ 共有アイコン ](assets/share-icon.png) をクリックします。
1. フィルター、ビューまたはグループ化を共有する特定のユーザー、チーム、役割、グループまたは会社の名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。

   共有について詳しくは、[オブジェクトに対する共有権限の概要](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

1. 「**[!UICONTROL 保存]**」をクリックします。指定したユーザーは、関連付けたオブジェクト タイプを表示するときに、フィルタ、表示、またはグループ化を表示できるようになりました。

## フィルター、ビュー、グループ化の削除

{{step-1-to-setup}}

1. 「**[!UICONTROL インターフェース]**」をクリックし、「**[!UICONTROL フィルター]**」、「**[!UICONTROL ビュー]**」または「**[!UICONTROL グループ化]**」のいずれかをクリックします。

1. リスト内の 1 つ以上の項目を選択し、**[!UICONTROL 削除]**&#x200B;アイコン ![削除アイコン](assets/delete.png) をクリックします。

1. 表示される **削除** ダイアログボックスで、「はい、削除 **をクリックし** す。
