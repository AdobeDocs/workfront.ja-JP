---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: デフォルトのフィルター、ビュー、グループ化を作成、編集、共有します。
description: デフォルトのフィルター、ビューおよびグループ化を作成すると、組織内のユーザーが使用できるようなります。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: caaba90f4cdd835e1a1fddf16bcefa30995cca0d
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 97%

---

# デフォルトのフィルター、ビュー、グループ化を作成、編集および共有

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

デフォルトのフィルター、ビューおよびグループ化を作成すると、組織内のユーザーが使用できるようなります。

この記事で説明するように、デフォルトのフィルター、ビューおよびグループ化を作成すると、共有相手のユーザーは、リストを表示する際にそれらを活用できます。ユーザーは、作成されたフィルター、ビューおよびグループに基づいて独自のフィルター、ビューおよびグループ化を作成できますが、他のユーザーに作成されたフィルター、ビューおよびグループ化を直接変更することはできません。

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

## デフォルトのフィルター、ビューまたはグループ化の作成

{{step-1-to-setup}}

1. フィルター、ビューまたはグループ化を作成または編集するかどうかに応じて、次のいずれかの操作を実行します。

   * **[!UICONTROL インターフェイス]**／**[!UICONTROL フィルター]**&#x200B;をクリックします。

   * **[!UICONTROL インターフェイス]／** **[!UICONTROL ビュー]**&#x200B;をクリックします。

   * **[!UICONTROL インターフェイス]**／**[!UICONTROL グループ化]**&#x200B;をクリックします。

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

レイアウトテンプレートから、フィルター、ビューまたはグループ化の表示と非表示を選択できます。表示されるフィルターは、システム全体のすべてのユーザーが使用できます。レイアウトテンプレートを使用すると、特定のユーザーまたはグループに対して表示するフィルターを非表示にできます。

>[!NOTE]
>
>ユーザーがアクティブに使用しているフィルター、ビューまたはグループ化を管理者が無効にした場合、ユーザーは新しいフィルター、ビューまたはグループ化を選択するまでアクセスできます。新しいフィルター、ビューまたはグループ化を選択した後は、非表示のフィルター、ビューまたはグループ化に戻せなくなります。

レイアウトテンプレートから使用できるフィルター、ビューまたはグループ化を表示または非表示にするには、次の手順に従います。

1. 「**[!UICONTROL インターフェース]**」をクリックし、「**[!UICONTROL フィルター]**」、「**[!UICONTROL ビュー]**」または「**[!UICONTROL グループ化]**」のいずれかをクリックします。

1. （条件付き）ユーザーが使用できるフィルター、ビューまたはグループ化を選択し、「**[!UICONTROL システム全体で有効にする]**」をクリックします。

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >フィルター、ビューまたはグループ化を、ほとんどのユーザーに対して使用可能にし、他のユーザーに対しては非表示にする場合は、レイアウトテンプレートを使用します。詳しくは、[レイアウトテンプレートを使用したフィルター、ビューおよびグループ化のカスタマイズ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)を参照してください。

1. （条件付き）ユーザーに対して非表示にするフィルター、ビューまたはグループ化を選択し、「**[!UICONTROL システム全体で無効にする]**」をクリックします。無効にすると、フィルター、ビューまたはグループ化がレイアウトテンプレートやシステム全体でユーザーに非表示になります。


## フィルター、ビューまたはグループ化をすべてのユーザーに使用可能にする {#make-filters-views-or-groupings-available-to-users}

これらの手順では、[!UICONTROL 設定]の[!UICONTROL インターフェース]エリアにある[!UICONTROL 共有]ダイアログからフィルター、ビューおよびグループ化を使用できるようにする方法について説明します。この設定は、レイアウトテンプレートを含む、システム全体のオン／オフスイッチのように機能します。

{{step-1-to-setup}}

1. 「**[!UICONTROL インターフェース]**」をクリックし、「**[!UICONTROL フィルター]**」、「**[!UICONTROL ビュー]**」または「**[!UICONTROL グループ化]**」のいずれかをクリックします。

1. ユーザーが使用できるフィルター、ビューまたはグループ化を選択し、**[!UICONTROL 共有]**&#x200B;アイコン![共有アイコン](assets/share-icon.png)をクリックして、[!UICONTROL フィルターアクセス]、[!UICONTROL ビューアクセス]または[!UICONTROL グループ化アクセス]のフォームを開きます。
1. （条件付き）システム内のすべてのユーザーがフィルター、ビュー、またはグループ化を利用できるようにするには、**[!UICONTROL ギア]**&#x200B;ドロップダウンメニュー ![](assets/gear-menu-for-sharing-items.png)、**[!UICONTROL システム全体でこれを表示する]**&#x200B;の順にクリックします。システム内のすべてのユーザーが、フィルター、ビューまたはグループ化を表示できるようになりました。

   または

   フィルター、ビューまたはグループ化を共有する特定のユーザー、チーム、役割、グループまたは会社の名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。

   共有について詳しくは、[オブジェクトに対する共有権限の概要](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

1. 「**[!UICONTROL 保存]**」をクリックします。

   指定したユーザーは、関連付けたオブジェクトタイプを表示する際に、既定のフィルター、ビュー、またはグループ化を表示できます。

## フィルター、ビュー、グループ化の削除

{{step-1-to-setup}}

1. 削除するフィルター、ビュー、グループ化のいずれを選択するかに応じて、次の操作を実行します。

   * **[!UICONTROL インターフェイス]**／**[!UICONTROL フィルター]**&#x200B;をクリックします。

   * **[!UICONTROL インターフェイス]**／**[!UICONTROL ビュー]**&#x200B;をクリックします。

   * **[!UICONTROL インターフェイス]**／**[!UICONTROL グループ化]**&#x200B;をクリックします。

1. リスト内の 1 つ以上の項目を選択し、**[!UICONTROL 削除]**&#x200B;アイコン ![削除アイコン](assets/delete.png) をクリックします。
1. フィルター、ビューまたはグループ化の設定について詳しくは、次のいずれかの記事を参照してください。

   * [フィルターの概要](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [ [!DNL Adobe Workfront] でのビューの概要](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [ [!DNL Adobe Workfront] でのグループ化の概要](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
