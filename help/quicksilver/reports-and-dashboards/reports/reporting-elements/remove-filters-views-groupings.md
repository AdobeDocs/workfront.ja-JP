---
product-area: reporting
navigation-topic: reporting-elements
title: フィルター、ビュー、グループを削除
description: リストやレポートを作成した場合、または共有されている場合は、リストやレポートからフィルター、ビュー、またはグループ化を削除できます。デフォルトのフィルター、ビュー、グループ化は削除できません。
author: Nolan
feature: Reports and Dashboards
exl-id: 422d262e-e19d-4070-85f1-77ecb7430342
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 93%

---

# フィルター、ビュー、グループを削除

<!-- Audited: 11/2024 -->

リストやレポートを作成した場合、または共有されている場合は、リストやレポートからフィルター、ビュー、またはグループ化を削除できます。デフォルトのフィルター、ビュー、グループ化は削除できません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン*</strong></td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン*</strong></td> 
   <td> 
      <p>新規：</p>
         <ul>
         <li><p>投稿者以上</p></li>
         </ul>
      <p>現在：</p>
         <ul>
         <li><p>リクエスト以上</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td><p>フィルター、ビュー、グループ化に対する表示またはそれ以上のアクセス権</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td><p>削除するフィルター、ビュー、またはグループ化に対する共有アクセス限を持つ表示権限</p>
   </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## 標準ビルダーを使用してフィルターを削除する

標準ビルダーインターフェイスを使用して、自分と共有していたフィルターをプロジェクト、タスク、またはイシューのリストから削除できます。標準ビルダーインターフェイスは、他のオブジェクトに対しても、ビューやグループ化に対しても使用できません。

標準ビルダーインターフェイスを使用して、プロジェクト、タスク、またはイシューのリストから所有しているフィルターを削除することもできます。

システムのデフォルトのフィルターは、削除できません。

### 標準ビルダーを使用したフィルターの削除に関する考慮事項

標準ビルダーを使用してフィルターを削除する場合、次のシナリオが存在します。

* フィルターを自分と共有し、自分で削除した場合は、そのフィルターは自分に対してのみ削除されます。最初にフィルターを作成したユーザーと、それを共有している他のユーザーは、引き続きフィルターにアクセスできます。
* フィルターを所有していて、削除した場合、そのフィルターは Workfront システムから削除されます。以前にフィルターを共有していたユーザーは、フィルターを使用できなくなります。
* Workfront 管理者はフィルターを削除でき、所有者を含むすべてのユーザーに対してフィルターが完全に削除されます。

### 標準ビルダーを使用してフィルターを削除する

1. プロジェクト、タスク、イシュー、ポートフォリオ、プログラム、ユーザー、テンプレート、またはグループのリストに移動します。
1. **フィルター**&#x200B;アイコン ![フィルターアイコン](assets/filter-nwepng.png) をクリックします。
1. **自分と共有**&#x200B;の下のフィルターにポインタを合わせて、**その他**&#x200B;メニュー ![その他アイコン](assets/more-icon-spectrum.png) をクリックして、「**削除**」をクリックします。
1. 確認メッセージで「**削除**」を選択すると、フィルターが完全に削除されます。

### 標準ビルダーを使用してフィルターを削除する

1. プロジェクト、タスク、イシュー、ポートフォリオ、プログラム、ユーザー、テンプレート、またはグループのリストに移動します。
1. **フィルター** アイコン ![フィルターアイコン](assets/filter-nwepng.png) をクリックします。
1. 削除権限があるフィルターの上にポインターを合わせて、**その他**&#x200B;メニュー ![その他のアイコン](assets/more-icon-spectrum.png) をクリックして、「**削除**」をクリックします。

   ![フィルターを削除](assets/new-filters-more-menu-options-with-delete.png)

1. （オプション）確認メッセージで「**キャンセル**」をクリックすると、削除されずにフィルターのリストに戻ります。
1. 確認メッセージで「**削除**」をクリックすると、削除されます。

   このフィルターは、自分のほか、権限を持つすべてのユーザーに対して削除されます。

## レガシービルダーを使用してフィルター、ビュー、またはグループ化を削除する

レガシービルダーインターフェイスを使用して、すべてのオブジェクトのリストのフィルター、表示、またはグループ化を削除できます。

### レガシービルダーを使用してフィルター、ビュー、およびグループ化を削除する際の考慮事項

レポート要素を削除する方法は、最初に作成したか、自分と共有したかによって異なります。

フィルター、ビュー、またはグループ化を削除する場合、次のシナリオが存在します。

* **要素を作成して削除すると**、要素は Workfront システムから削除されます。以前に共有していたユーザーは利用できなくなります。
* **他のユーザーと共有していた要素を削除すると**、要素は自分に対してのみ削除されます。最初にそれを作成したユーザーと、共有している他のユーザーは、引き続きアクセスできます。

### レガシービルダーを使用してフィルター、ビュー、またはグループ化を削除する

1. オブジェクトのリストまたはレポートに移動します。
1. （条件付き）リストから、「**フィルター**」、「**表示**」または「**グループ化** アイコンをクリックし、削除するフィルター、表示またはグループ化にカーソルを合わせて **詳細** アイコン ![ 詳細アイコン ](assets/more-icon.png) をクリックし、**削除** をクリックします。 フィルター、ビュー、またはグループ化が削除されます。
1. （条件付き）レポートから、「**グループ化**」、「**フィルター**」、または「**ビュー**」ドロップダウンメニューをクリックして、「**グループ化の削除**」、「**フィルターの削除**」、または「**ビューの削除**」を選択します。

   「**マイグループ化**」、「**マイフィルター**」、または「**マイビュー**」ダイアログボックスが表示されます。

   削除する権限を持つすべてのレポート要素を削除できます。その他のレポート要素は淡色表示になります。

1. 削除するレポート要素の横にある「**x**」アイコンをクリックします。
1. （条件付き）作成して後で他のユーザーと共有したフィルター、ビュー、またはグループ化を削除することを選択した場合は、「**はい、削除します**」をクリックします。これにより、Workfront システムからフィルター、ビュー、またはグループ化が削除されます。

   >[!TIP]
   >
   >他のユーザーと共有せずに作成したフィルター、ビュー、またはグループ化を削除すると、確認を求めることなくシステムから削除されます。

1. 「**完了**」をクリックします。

