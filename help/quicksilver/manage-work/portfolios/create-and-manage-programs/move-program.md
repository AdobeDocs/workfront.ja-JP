---
product-area: programs
navigation-topic: create and manage programs
title: 既存のプログラムのPortfolioへの追加
description: 既存のプログラムをポートフォリオに追加できます。 プログラムは 2 つの異なるポートフォリオに存在できないため、既存のプログラムを追加すると、そのプログラムは 1 つのポートフォリオから別のポートフォリオへと永続的に移動されます。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 73dbe277-12d2-4041-8a02-91ccf5f8b465
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 9a35246858141a3b69ec85be3372c7a8d9497d6e
workflow-type: tm+mt
source-wordcount: '382'
ht-degree: 34%

---

# ポートフォリオに既存プログラムの追加

<!--Audited: 05/2026-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>
-->

既存のプログラムをポートフォリオに追加できます。 プログラムは 2 つの異なるポートフォリオに存在できないため、既存のプログラムを追加すると、そのプログラムは 1 つのポートフォリオから別のポートフォリオへと永続的に移動されます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> <p>[!UICONTROL Standard]</p><p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>[!UICONTROL Edit] [!UICONTROL Portfolios]および[!UICONTROL プログラム ]へのアクセス </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ポートフォリオおよびプログラムに対する [!UICONTROL Manage] 権限</p> </td> 
  </tr> 
 </tbody> 
</table>

* 詳しくは、[Workfront ドキュメント ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>New: [!UICONTROL Standard] </p><p>Or </p><p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Portfolios and Programs </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio and the program</p> </td> 
  </tr> 
 </tbody> 
</table>
-->

## ポートフォリオに既存プログラムの追加

>[!NOTE]
>
>ドキュメントに従来のWorkfrontとAdobe クラウドストレージの両方を使用する場合、次のシナリオが存在します。
>
>
>* Adobe クラウドストレージプログラムを従来のWorkfront ストレージポートフォリオに追加し、ポートフォリオにドキュメントが添付されていない場合、ポートフォリオはAdobe クラウドストレージに変換されます。
>* Adobe クラウドストレージプログラムを従来のWorkfront ストレージポートフォリオに追加し、ポートフォリオにドキュメントが添付されている場合、ポートフォリオドキュメントストレージはWorkfront ストレージに残ります。 ただし、従来のWorkfront ストレージアイコン ![従来のWorkfront ストレージアイコン ](assets/legacy-storage-project-icon.png)はポートフォリオから削除されます。
>* 従来のWorkfront ストレージプログラムをAdobe クラウドストレージポートフォリオに追加することはできません。
>
>詳しくは、[ プロジェクトおよび関連オブジェクトのドキュメント管理の概要](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md)を参照してください。
>
>すべてのWorkfront インスタンスに両方の種類のドキュメントストレージがあるわけではありません。

既存のプログラムを別のポートフォリオに追加するには：

1. ポートフォリオに移動し、左側のパネルで「**[!UICONTROL プログラム]**」をクリックします。
1. 「**[!UICONTROL 新規プログラム]**」をクリックします。
1. 「**[!UICONTROL 既存のプログラム]**」をクリックします。

   「**プログラムを追加**」ボックスが開きます。<!--check screen shot - I logged changes for this casing-->

   ![ プログラムボックスを追加](assets/add-programs-box.png)

   >[!IMPORTANT]
   >
   >既存のプログラムを追加すると、そのプログラムに関連するすべてのプロジェクトがポートフォリオに追加されます。 このようにプロジェクトを不用意に移動しないように注意してください。

1. 「**[!UICONTROL このポートフォリオにプログラムを追加]**」フィールドに、プログラムの名前を入力し、リストに表示されたら選択します。<!--see the name of this field, I suggested changes here-->

   複数のプログラムを追加できます。

1. （オプション）プログラムをポートフォリオに追加しない場合は、プログラム名の横にある&#x200B;**削除** アイコン ![削除アイコン ](assets/delete-icon.png)をクリックします。

1. 「**[!UICONTROL プログラムを追加]**」をクリックします。

   プログラムは、選択したポートフォリオの&#x200B;**[!UICONTROL プログラム]** タブに表示されます。

