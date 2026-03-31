---
product-area: projects
navigation-topic: use-the-home-area
title: マイリクエストウィジェットの使用
description: マイリクエストウィジェットでリクエストを送信できます。 また、フィルターと列を使用してウィジェットをカスタマイズすることもできます。
author: Alina, Courtney
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
source-git-commit: a9cc76139c0f542e4b27e8e3591a40bf626342f4
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 15%

---

# マイリクエストウィジェットの使用

>[!IMPORTANT]
>
>この記事では、新しいMy Requests ウィジェットについて説明します。 新しいウィジェットを表示するには、新しいリクエスト用エクスペリエンスを有効にする必要があります。
>リクエスト領域で新しいリクエストエクスペリエンスを有効にできます。

My Requests ウィジェットには、送信したリクエストが表示されます。 リクエストをフィルタリングしたり、特定のリクエストを検索したり、列の順序や表示を調整したりできます。 マイリクエストウィジェットから新しいリクエストを作成することもできます。

>[!NOTE]
>
>* マイリクエストウィジェットが読み込まれると、最大50件のリクエストが表示されます。 さらにリクエストを表示するには、リストを下にスクロールします。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>任意のWorkfrontまたはWorkflow パッケージ</p>
   <p>Workfront計画リクエストと作成されたオブジェクトにアクセスするためのWorkfront計画パッケージ</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス</strong></td> 
   <td> <p>コントリビューター以上</p>
   <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <!--
   <tr> 
   <td role="rowheader"><strong>Additional products</strong></td> 
   <td> You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>会話でタグ付けされたオブジェクトや承認を解決する必要があるオブジェクト（プロジェクト、タスク、イシュー、ドキュメント）への表示以上のアクセス権</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>会話でタグ付けされたまたは承認の解決が必要なプロジェクト、タスク、イシュー、ドキュメントに対する [!UICONTROL View] 権限またはそれ以上の権限</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## リクエストの作成

マイリクエストウィジェットから直接リクエストを作成できます。

手順については、「[作業項目とプロジェクトをホーム エリア &#x200B;](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md/#create-a-request)から作成する」の「[&#x200B; リクエストを作成](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md)」の節を参照してください。

## リクエストをコピーする

マイリクエストウィジェットでリクエストをコピーして編集し、新しいリクエストとして送信できます。

手順については、[要求のコピーと送信](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md)を参照してください。

## マイリクエストウィジェットのリクエストリストの情報を管理する

<!--
The My Requests widget features a customizable filter that allows you to control which requests appear in the widget. You can configure this filter for different fields and values, and can stack conditions using AND and OR operators.

To configure the filter in the My Requests widget:
-->

1. 左上隅の&#x200B;**[!UICONTROL メインメニュー]** ![&#x200B; メインメニューアイコン &#x200B;](assets/lines-main-menu.png)をクリックし、**[!UICONTROL ホーム]**&#x200B;をクリックします。
1. （条件付き）ホーム画面に&#x200B;**マイリクエスト** ウィジェットを追加するには。 **カスタマイズ**&#x200B;をクリックして&#x200B;**マイリクエスト**&#x200B;を見つけ、それをクリックして&#x200B;**ホーム**&#x200B;に追加します。
1. （オプション）情報がリクエストリストに表示される方法を管理するには、リストの次のビュー要素を更新します。

   * 表示
   * フィルター
   * 列

   <!--
   <div class="preview">
      * Group
   * Format cells
   * Row height
      </div>
   -->

   リクエストリストでの情報の管理について詳しくは、[拡張リストの使用](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)を参照してください。


<!-- Removed all these sections because this is common to ALL the Glists/ enhanced lists. So, we will update that article with all the specific steps: 
1. Select the field that you want to filter by. Available options are:

   * Workspace
   * Object type
   * Entry date
   * Request form
   * Status
   * Entered by
   * Custom fields from the request or from the created object   

1. In the next field, select the operator that you want to use for this filter condition. Available operators depend on the chosen field.
1. (Conditional) If a field appears to the right of the operator, select the value that you want to filter by.
1. (Optional) To add another filter condition, click **Add condition** and repeat steps 4-6.
1. (Optional and conditional) If you have multiple conditions, switch the And or Or value by clicking **And** or **Or** to the left of the condition.


The filter is saved automatically.

-->

>[!TIP]
>
>組織がAdobe Workfrontに加えてWorkfront Planningを購入した場合、マイリクエストウィジェットにはWorkfrontとWorkfront Planningの両方のリクエストが含まれます。
> 
>* Workfront リクエストのみをフィルタリングするには、フィルターを&#x200B;**Object type** > **Has any of** > **Issues**&#x200B;に設定します。
>* Workfront Planning リクエストのみをフィルタリングするには、フィルターを&#x200B;**Object type** > **Has none of** > **Issues**&#x200B;に設定します。

<!--

## Adjust or add columns

You can choose which of the available columns appear on the My Requests widget, and set their order.

Available columns include:

* Subject
* Created object
* Object type
* Status
* Request form
* Entry date
* Entered by

To adjust the columns on the My Requests widget:

1. Click the **[!UICONTROL Main Menu]** ![Main Menu icon](assets/main-menu-icon.png) in the upper-right corner, then click **[!UICONTROL Home]**.
1. (Conditional) To add the **My Requests** widget to your home screen. Click **Customize**, and find **My Requests**, then click it to add it to **Home**. 
1. In the **My Requests** widget, click **Columns**.
1. (Optional) To reorder columns, click the drag handle ![drag handle](assets/drag-handle.png) of the column you want to move and drag it to the desired locations. The column at the top of the list appears in the My Requests widget as the first column.
1. (Optional) Use the toggle to hide or show the column in the requests list.
1. To add a custom field as a column, click the **Add column** icon ![Add column](assets/add-column.png) in the upper-right corner of the list, and click the plus icon next to the custom field that you want to add as a column to the widget.

   Custom fields on forms attached to the object in the list are available to add as columns.

Column preferences are saved automatically.

-->

<!--

## Create a view

You can create views in the My Requests widget to change the way the information displays in the request list. 

Consider the following when working with views in the My Requests widget:

* A view in the My Requests widget contains the columns and filters applied to the view.
* You can create views and share them with others. The filters and columns you select for the view before you share it are included in the views you share. 
* The following is a system view which you cannot edit, share, or delete: 

   * Widget Unified Requests Default View
* Creating and editing a view in the My Requests widget is similar to enhanced lists. For information, see [Use enhanced lists](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md). 

-->

## 検索リクエスト

マイリクエストウィジェットで特定のリクエストを検索するには：

1. 右上隅の&#x200B;**[!UICONTROL メインメニュー]** ![&#x200B; メインメニューアイコン &#x200B;](assets/main-menu-icon.png)をクリックし、**[!UICONTROL ホーム]**&#x200B;をクリックします。
1. （条件付き）ホーム画面に&#x200B;**マイリクエスト** ウィジェットを追加するには。 **カスタマイズ**&#x200B;をクリックして&#x200B;**マイリクエスト**&#x200B;を見つけ、それをクリックして&#x200B;**ホーム**&#x200B;に追加します。
1. マイリクエストウィジェットの右上付近にある検索バーで、検索する語句を入力します。

   用語を含むリクエストはオレンジ色で強調表示されます。

1. （オプション）強調表示されたリクエストにジャンプするには、検索バーの上向き矢印または下向き矢印をクリックします。

## リクエストによって作成されたオブジェクトに移動

リクエストで作成されたオブジェクトは、マイリクエストウィジェットで見つけることができます。

>[!NOTE]
>
>作成されたオブジェクトへのリンクは、新しいリクエストのエクスペリエンスでは、リクエスト自体がオブジェクトを作成した場合にのみ、Planning リクエストでのみ使用できます。 Workfront リクエストがプロジェクトまたは他のオブジェクトに変換された場合、変換後のオブジェクトへのリンクは、新しいリクエストエクスペリエンスのリクエストリストで使用できません。

1. 右上隅の&#x200B;**[!UICONTROL メインメニュー]** ![&#x200B; メインメニューアイコン &#x200B;](assets/main-menu-icon.png)をクリックし、**[!UICONTROL ホーム]**&#x200B;をクリックします。
1. （条件付き）ホーム画面に&#x200B;**マイリクエスト** ウィジェットを追加するには。 **カスタマイズ**&#x200B;をクリックして&#x200B;**マイリクエスト**&#x200B;を見つけ、それをクリックして&#x200B;**ホーム**&#x200B;に追加します。
1. オブジェクトを作成したリクエストを探します。
1. そのリクエストの&#x200B;**作成済みオブジェクト**&#x200B;列のオブジェクト名をクリックします。

   オブジェクトのページが開きます。

