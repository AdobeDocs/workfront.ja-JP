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
TQID: https://experienceleague.adobe.com/bgBICul4K2MFbMipuKZxp6i2vncdpV7RpFYtUyTFY7w
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aadid: e14a7f57-c82c-4874-a495-5d036cbbdc3d
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 814
ht-degree: 46%

---

# システム全体のフィルター、ビュー、グループ化を作成、編集、共有します

<!-- Audited: 5/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

フィルター、ビュー、グループ化を作成し、組織内のシステム全体でユーザーが使用できるようにすることができます。

この記事で説明したように、システム全体のフィルター、ビュー、グループ化を作成する場合、それらを共有するユーザーは、リストを表示するときに利用できます。 ユーザーは、作成したフィルター、ビュー、グループ化に基づいて独自のフィルター、ビュー、グループ化を作成できますが、直接変更することはできません。

作成するシステム全体のフィルター、ビュー、グループ化は、Adobe Workfrontが自動的に作成するデフォルトのフィルターと異なります。 これらのデフォルトのフィルター、ビュー、グループ化は、編集または削除できません。

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

## フィルター、ビューまたはグループ化の作成

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

システム内のユーザーがフィルター、ビューまたはグループ化を使用できるようにします。 他のユーザーとのフィルター、ビューまたはグループ化の共有について詳しくは、この記事の[フィルター、ビューまたはグループをユーザーに使用可能にする](#make-filters-views-or-groupings-available-to-users)を参照してください。


## フィルター、ビューまたはグループ化をすべてのユーザーに使用可能にする {#make-filters-views-or-groupings-available-to-users}

システム内のフィルター、ビュー、またはグループ化の表示と非表示を選択できます。 表示フィルターは、システム全体のすべてのユーザーで使用できます。 この設定は、レイアウトテンプレートを含む、システム全体のオン／オフスイッチのように機能します。

特定のユーザーのフィルター、ビュー、グループ化を非表示にする場合は、システム全体で無効にするのではなく、レイアウトテンプレートを使用することをお勧めします。

>[!NOTE]
>
>* ユーザーがアクティブに使用しているフィルター、ビューまたはグループ化を管理者が無効にした場合、ユーザーは新しいフィルター、ビューまたはグループ化を選択するまでアクセスできます。 新しい属性を選択すると、非表示の属性に戻すことができなくなります。
>* すべてのフィルター、ビュー、グループ化がレイアウトテンプレートまたはシステム全体で無効になっている場合は、システムに何かを表示する必要があるため、デフォルトのオプションが表示されます。

フィルター、ビューまたはグループ化を表示または非表示にするには：

{{step-1-to-setup}}

1. 「**[!UICONTROL インターフェース]**」をクリックし、「**[!UICONTROL フィルター]**」、「**[!UICONTROL ビュー]**」または「**[!UICONTROL グループ化]**」のいずれかをクリックします。

1. （条件付き）ユーザーが使用できるフィルター、ビューまたはグループ化を選択し、「**[!UICONTROL システム全体で有効にする]**」をクリックします。

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >ほとんどのユーザーがフィルター、表示、またはグループ化を利用できるようにしたまま、他のユーザーからは非表示にする場合は、レイアウトテンプレートを使用できます。 詳しくは、[レイアウトテンプレートを使用したフィルター、ビューおよびグループ化のカスタマイズ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)を参照してください。

1. （条件付き）ユーザーから非表示にするフィルター、表示、またはグループ化を選択し、**[!UICONTROL システム全体で無効にする]**&#x200B;をクリックします。 フィルター、ビュー、またはグループ化が、レイアウトテンプレートとシステム全体のユーザーの両方から非表示になりました。


## 特定のユーザーとカスタムフィルター、ビュー、グループ化を共有する

次の手順では、[!UICONTROL  セットアップ ]の[!UICONTROL  インターフェイス ]領域の共有ダイアログを使用して、特定のユーザーとカスタムフィルター、ビュー、グループ化を共有する方法について説明します。 自分または他のユーザーが作成したフィルター、ビュー、グループ化へのビューまたは管理アクセス権を付与できます。 システムのデフォルトをユーザーと共有することはできません。


{{step-1-to-setup}}

1. 「**[!UICONTROL インターフェース]**」をクリックし、「**[!UICONTROL フィルター]**」、「**[!UICONTROL ビュー]**」または「**[!UICONTROL グループ化]**」のいずれかをクリックします。

1. 共有するフィルター、表示、またはグループ化を選択し、**[!UICONTROL 共有]** アイコン ![共有アイコン ](assets/share-icon.png)をクリックします。
1. フィルター、ビューまたはグループ化を共有する特定のユーザー、チーム、役割、グループまたは会社の名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。

   共有について詳しくは、[オブジェクトに対する共有権限の概要](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md)を参照してください。

1. ユーザー、チーム、役割、グループ、または会社の名前の横にある&#x200B;**表示**&#x200B;または&#x200B;**管理**&#x200B;を選択します。 権限を微調整するには、スライダーアイコンをクリックして権限を調整します。

   ![権限を微調整](assets/fine-tune-permissions.png)

1. 「**[!UICONTROL 保存]**」をクリックします。 指定したユーザーは、関連付けたオブジェクトタイプを表示するときに、フィルター、表示、またはグループ化を操作できるようになりました。


## フィルター、ビュー、グループ化の削除

{{step-1-to-setup}}

1. 「**[!UICONTROL インターフェース]**」をクリックし、「**[!UICONTROL フィルター]**」、「**[!UICONTROL ビュー]**」または「**[!UICONTROL グループ化]**」のいずれかをクリックします。

1. リスト内の 1 つ以上の項目を選択し、**[!UICONTROL 削除]**&#x200B;アイコン ![削除アイコン](assets/delete.png) をクリックします。

1. 表示される&#x200B;**削除** ダイアログボックスで、**はい、削除**&#x200B;をクリックします。
