---
product-area: requests
navigation-topic: create-requests
title: リクエストエリアでのビューの作成と管理
description: 新しいリクエストエクスペリエンスを使用している場合は、リクエスト領域のビューを作成して保存できます。
author: Alina
feature: Work Management
exl-id: ed066075-6411-4350-8b39-f21dc4fa96c9
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 31aff197d6af521df2258f3f99fea6fb5785b9e3
workflow-type: tm+mt
source-wordcount: '683'
ht-degree: 10%

---


# リクエストエリアでのビューの作成と管理

<!--

<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

Adobe Workfrontで新しいリクエストエクスペリエンスを使用している場合は、リクエスト領域のビューを作成して保存できます。 これらのビューには、フィルター、列の配置、グループ化が含まれます。

>[!IMPORTANT]
>
>* この機能は、リクエスト領域の新しいリクエストエクスペリエンスでのみ使用できます。
>* ビュー設定は、ホームのマイリクエストウィジェットでも使用できます。 ただし、リクエスト領域のビューは、マイリクエストウィジェットのビューとは異なります。
>* リクエスト領域およびマイワークウィジェットのリクエストリストでは、Workfrontの拡張リストが使用されます。 詳しくは、[拡張リストの使用](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意のWorkfrontまたはWorkflow パッケージ</p>
   <p>任意のWorkfront プランニングライセンス。リクエストリストでWorkfront プランニングリクエストを表示できます</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>コントリビューター以上</p>
   <p>リクエスト以上</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>イシューへのアクセス権を編集</p>  <p>レイアウトテンプレートにビューを追加するには、Workfront管理者である必要があります</td> 
  </tr> 
  <!--
  <tr> 
   <td role="rowheader"> Product</td> 
   <td> <ul><li>Adobe Workfront</li><li>You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## リクエストのシステムビュー

>[!WARNING]
>
>この節で説明するシステムビューはまだ利用できません。 これらは、2026年4月16日より後の日付で利用できるようになります。

自分で作成できるビューに加えて、Workfrontでは、「リクエスト」エリアと「マイリクエスト」ウィジェットに対して、次のシステムビューをホームで提供しています。

* **すべてのリクエスト**：表示する権限を持つ、キューまたはワークスペースで自分または他の人が送信したすべてのリクエスト。 これは、マイリクエストウィジェットでは使用できません。
* **マイリクエスト**：ステータスに関係なく、送信したリクエスト。
* **自分が開いたリクエスト**：送信したリクエストが開いています。
* **自分のドラフト**：まだ送信されていないクエストのドラフト。
* **要求を開く**：自分または他の人がキュー内またはワークスペースに送信した要求のうち、表示する権限を持つものが開いています。 これは、マイリクエストウィジェットでは使用できません。

システムビューは編集できません。 要素を変更してから、ビューをコピーし、コピーを編集または共有できます。

## リクエストのビューの作成

新しいリクエストエクスペリエンスを使用すると、Workfrontのリクエスト領域にビューを作成できます。 リクエストエクスペリエンスを有効にして新しいリクエストエクスペリエンスを作成したら、ホームでマイリクエストウィジェットのビューを作成することもできます。

1. **リクエスト**&#x200B;のリストにアクセスするには：

   {{step1-to-requests}}

   1. 「**新しいエクスペリエンスを使用**」設定がオンになっていることを確認します。

1. ホームの&#x200B;**マイリクエスト** ウィジェットにアクセスするには：

   {{step1-to-home}}

   1. **マイリクエスト** ウィジェットを追加するか、に移動します。

1. リクエストのリストで、**ビュー** ドロップダウンメニュー![&#x200B; ビューのドロップダウン &#x200B;](assets/view-icon-requests.png)をクリックし、**新しいビュー**&#x200B;をクリックします。

   <!-- 
   
   replace the screen shot with release
   ![New view](assets/create-new-view.png)

   -->

1. 新しいビューの名前を入力し、**作成**&#x200B;をクリックします。
1. 引き続き[&#x200B; リクエストのビューを編集](#edit-a-view-for-requests)します。

## リクエストのビューの編集

既存のビューを編集できます。そのビューには、リクエスト エリアで作成したばかりのビューや、ホームのマイリクエストウィジェットがあります。

ビューを編集すると、ビューの次の要素を変更できます。

* 名前
* フィルター
* 列
* グループ化
* セルを書式設定
* 行の高さ

詳しくは、[拡張リストの使用](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)を参照してください。

<!-- 
hide these details - all the information is in "Use enhanced lists" - we need one point of messaging for this feature: 

1. To access a list of requests in the Requests are: 
   
   {{step1-to-requests}}

1. Ensure the **Use new experience** setting is turned on.
1. In the **Requests** list, locate the view that you want to edit from the **Views** dropdown menu ![Views dropdown](assets/view-icon-requests.png).

1. Click the **Views** dropdown ![Views dropdown](assets/view-icon-requests.png) and click the three-dot menu next to the view, select **Rename**, then type in the new name for the view.
1. Press Enter to save the new name. 
1. Click the **Views** dropdown ![Views dropdown](assets/view-icon-requests.png) and select the view you want to edit.
1. To add a field as a column, click the **Add column** icon ![Add column](assets/add-column.png) in the upper-right corner of the list. 

   The **Column manager** opens.
1. Click the plus icon next to the field that you want to add as a column to the view, then click **Save**.

   Fields associated with the objects in the list are available to add as columns. <!-keeping this general, and not referring to custom fields because there are some native fields that are supported and there will be more in the future->

   >[!TIP]
   >
   >Fields you add to the columns must exist before they are available in the **Column manager**.

1. (Optional) Click **Columns** to open the **Fields visibility and order** box. 
1. Turn on the setting for each field  you want to show in the list, turn it off to hide it, or drag and drop the fields in a different order.

1. (Optional) Click **Filters** and start adding conditions for what requests you want to view. 

    You can filter by the following request fields:  

    * **Workspace**: The workspace the request form is associated with.
    * **Object type**: The record type the request form is associated with.
    * **Entry date**: The date when the request was submitted.
    * **Request form**: The name of the request form used to submit the request.
    * **Status**: The status of the request.
    * **Entered by**: The name of the user who added the request. If the request was added by someone outside of Workfront, the **Entered by** field shows `N/A`.

    You can also filter by any fields that have been added to the view for any object visible in the view.

    You can have multiple filters joined by either **And** or **Or**.
    The request list is filtered automatically, as you add the filter conditions. 
-->

<!--
1. <Span class="preview">(Optional) Click **Group** and select the column that you want to group by.</span>

-->

>[!IMPORTANT]
>
> * ビューの変更は自動的に保存されます。
> * ビューに変更を加えた後にビューの新しいコピーを共有した場合にのみ、ビューを使用するユーザーにはビューの変更が表示されます。
> * ユーザーを値として持つ任意のフィールドで、**Me （ログインユーザー）** フィルターワイルドカードを使用します。

## レイアウトテンプレートへのリクエストビューの追加

Workfront管理者は、リクエスト領域のレイアウトテンプレートに新しいビューを追加できます。

手順については、[&#x200B; レイアウトテンプレートを使用したフィルター、ビュー、グループ化のカスタマイズ &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)を参照してください。

## ビューを共有

作成したビューは、他のユーザー、チーム、グループ、または会社と共有できます。

ビューを共有すると、他のユーザーは、ビュー用に編集した更新されたビュー要素を共有する前に表示できます。

ビューを更新した場合、同じビューのコピーを作成し、コピーを共有する前に変更内容を保持しない限り、変更内容は他のユーザーには表示されません。

詳しくは、[拡張リストの使用](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md)を参照してください。

<!--
Let's just redirect to Use enhanced lists so we avoid duplicating information. 

1. To access a list of requests in the Requests are: 
   
   {{step1-to-requests}}

1. Ensure the **Use new experience** setting is turned on.
1. In the **Requests** list, locate the view that you want to share.
1. Hover over the view that you want to share, then click on the three-dot menu to the right of the view name, then click  **Share**.
1. In the **Share** box, enter the people, teams, roles, groups, or companies that you want to share the view with, then select them from the list when they appear.
1. Click **Save**.

   The view is shared with the entities you indicate. 
-->