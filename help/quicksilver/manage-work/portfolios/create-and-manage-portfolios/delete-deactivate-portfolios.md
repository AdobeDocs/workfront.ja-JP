---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: ポートフォリオの削除と非アクティブ化
description: ポートフォリオとは、Adobe Workfront のプロジェクトやプログラムを集めたものです。ポートフォリオがシステムに無関係な場合は、ポートフォリオを削除または非アクティブ化できます。
author: Alina
feature: Work Management, Strategic Planning
exl-id: f88669d2-e8e9-4905-a771-1427b1fd32b2
source-git-commit: 00e693fc8b35a59f6ed212bc30da7f85cc78c845
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 66%

---

# ポートフォリオを削除および非アクティブ化する

<!--Audited: 08/2025-->

ポートフォリオとは、[!DNL Adobe Workfront] のプロジェクトやプログラムを集めたものです。ポートフォリオがシステムに無関係な場合は、ポートフォリオを削除または非アクティブ化できます。

今後のプロジェクトと関連付ける必要がなくなったポートフォリオは、削除するよりも、非アクティブ化して、現在ポートフォリオとそのプログラムに関連付けられているプロジェクトの履歴情報を保持することをお勧めします。

## アクセス要件

+++ 展開してアクセス要件を表示します。展開して、この記事の機能のアクセス要件を表示します。 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] package</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトおよびポートフォリオへのアクセスの [!UICONTROL Edit]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ポートフォリオに対する [!UICONTROL Manage] 権限 </p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Projects and Portfolios</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions on the portfolio </p> </td> 
  </tr> 
 </tbody> 
</table>

For more detail about the information in this table, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
-->

## ポートフォリオの削除と非アクティブ化の概要

ポートフォリオを削除するか非アクティブ化するかを決める際は、次の点を考慮してください。

* ポートフォリオを削除すると、そのポートフォリオに関連付けられているプログラムが削除されます。

  >[!IMPORTANT]
  >
  >ポートフォリオを削除するために、プログラムに対する権限を持つ必要はありません。

* ポートフォリオを削除しても、ポートフォリオに関連付けられているプロジェクトは削除されません。
* 削除したポートフォリオを元に戻すことはできません。
* ポートフォリオを非アクティブ化すると、プロジェクトの作成時に、ポートフォリオとそのプログラムの名前をプロジェクトに割り当てることができなくなります。
* 既にプロジェクトに添付されているポートフォリオを非アクティブ化しても、プロジェクトから削除されません。 プロジェクトから非アクティブ化されたポートフォリオを削除した場合、そのポートフォリオをプロジェクトに再アタッチする前に再アクティブ化する必要があります。

## ポートフォリオの削除

{{step1-to-portfolios}}

1. 次のいずれかの操作を行います。

   * リストでポートフォリオを選択し、**[!UICONTROL 削除]** アイコン ![ 削除アイコン ](assets/delete.png) をクリックします。
   * ポートフォリオをクリックして開き、ポートフォリオ名の右側にある **その他** メニュー ![ その他のメニュー ](assets/more-icon.png) をクリックしてから、**Portfolioを削除** をクリックします。
1. **[!UICONTROL はい、削除します]** をクリックして確認します。

   ポートフォリオは削除され、復元できません。

## ポートフォリオの非アクティブ化

ポートフォリオを非アクティブ化しても、そのポートフォリオには引き続き[!UICONTROL ポートフォリオ]エリアからアクセスできます。ただし、ユーザーがポートフォリオをプロジェクトに追加しようとする際に、ポートフォリオのリストに表示されなくなります。

>[!NOTE]
>
>[!DNL Workfront] 管理者またはグループ管理者によるレイアウトテンプレートの設定によっては、[!UICONTROL ポートフォリオ]エリアが[!UICONTROL メインメニュー]に表示されない場合があります。詳細情報については、[レイアウトテンプレートを使用したメインメニューのカスタマイズ](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)を参照してください。

{{step1-click-main-menu}}

1. 「**[!UICONTROL ポートフォリオ]**」をクリックします。
1. ポートフォリオの名前をクリックします。
1. ポートフォリオ名の右側にある **その他** メニュー ![ その他メニュー ](assets/more-icon.png) をクリックし、**[!UICONTROL Portfolioのアクティベートを解除]** をクリックします。
ポートフォリオは直ちに非アクティブ化されます。
1. （オプション）ポートフォリオ名の右側にある **その他** メニュー ![ その他 ](assets/more-icon.png) メニューをクリックしてから、**[!UICONTROL Portfolioをアクティブ化]** をクリックして再アクティブ化します。


