---
title: レコードビューの管理
description: Adobe Workfrontの計画機能を使用する際に、テーブル、タイムライン、またはカレンダー表示にレコードを表示できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: b795ceccb3f72eb64269062823199be9c8511860
workflow-type: tm+mt
source-wordcount: '857'
ht-degree: 7%

---

# レコードビューの管理

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

「Adobe Workfront計画機能」領域でレコード・タイプを選択した後、次のビューにそのタイプのすべてのレコードを表示できます。

* テーブル

  詳しくは、 [テーブル表示の管理](../views/manage-the-table-view.md).

* タイムライン

  詳しくは、 [タイムライン表示を管理](../views/manage-the-timeline-view.md).

* カレンダー

  詳しくは、 [カレンダー表示を管理](/help/quicksilver/maestro/views/manage-the-calendar-view.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 製品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront協定</p></td>
   <td>
<p>組織は、Adobe Workfront Planning 機能クローズ済みベータプログラムに登録されている必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront ライセンス</p></td>
   <td>
   <p>任意</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">アクセスレベルの設定</td>
   <td> <p>Workfront Planning 機能に対するアクセスレベルの制御はありません</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ビューに対する権限の管理</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">レイアウトテンプレート</td>
   <td> <p>システム管理者は、レイアウトテンプレートに Maestro 領域を追加する必要があります。 詳しくは、 <a href="../access/access-overview.md">アクセスの概要</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## レコードビューを使用する際の考慮事項

* 「Workfront計画機能」領域のビューは、レコードのタイプに固有です。 同じビューを 2 つの異なるレコードタイプに適用することはできません。
* 作成したビューは、自分とそのビューを共有しているユーザーにのみ表示されます。
* オペレーショナルレコードタイプのビューの作成は、分類レコードタイプのビューの作成と同じです。
* ビューを変更または削除すると、そのビューに対する権限を持つすべてのユーザーに対して、ビューが変更および削除されます。
* 次の要素は、各レコードビューに固有です。

   * フィルター
   * グループ化
   * 並べ替え

  <!-- some of these are not available in all of the views - edit above-->

  例えば、テーブルビューでフィルタを作成する場合、フィルタ結果は選択したビューにのみ表示され、「ビュー」(View) ドロップダウンメニューにリストされるすべてのビューからは表示されません。

  >[!NOTE]
  >
  > Adobe Workfrontの計画機能は現在ベータ状態なので、一部のビュー要素が一部のビューで使用できない場合があります。

この記事では、レコードビューに関する次の情報について説明します。

* [ビューの作成と編集](#create-or-edit-record-views)
* [ビューの削除](#delete-views)
  <!--* [Duplicate a view](#duplicate-views)-->
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->
* [ビューを共有](#share-a-view)

## レコードビュー間の類似点と相違点

次の表に、テーブル、タイムライン、およびカレンダービューの類似点と相違点を示します。

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| 機能 | テーブル表示 | タイムライン表示 | カレンダー表示 |
|-----------------------------------------------------------------------|------------|---------------|--------------|
| リストまたはテーブルにレコードを表示 | ✓ |              | |
| すべてのフィールドをテーブル内の列として表示（デフォルト） | ✓ |              |    |
| フィールド（または列）の表示/非表示を切り替える | ✓ |               |    |
| 各レコードのフィールド値を編集 | ✓ |               |             |
| レコードを新しい行としてビューに追加 | ✓ |               |        |
| ビューでフィールドを新しい列として追加 | ✓ |               |         |
| 外部リストから行をコピーしてテーブルに貼り付ける | ✓ |               |          |
| タイムラインでのレコードの表示 |            | ✓ |             |
| レコードのフィルタリング | ✓ | ✓ |           |
| カレンダーにレコードを表示する |           |              | ✓ |
| レコードをグループ化 | ✓ | ✓ |
| レコードの並べ替え | ✓ |              |
| カラーコードのレコード |           | ✓ | ✓ |
| カラーコードのグループ化 |           | ✓ |
| 特定のレコードの検索 | ✓ | ✓ |
| 表示を共有 | ✓ | ✓ | ✓ |
| レコードの詳細ページをビューから開きます。 | ✓ | ✓ |    |


## ビューの作成または編集 {#create-or-edit-views}

{{step1-to-maestro}}


最後にアクセスしたワークスペースは、デフォルトで開きます。 ワークスペースの作成について詳しくは、 [ワークスペースの作成](../architecture/create-workspaces.md).

1. レコードタイプのカードをクリックします。 レコードタイプの作成について詳しくは、 [レコードタイプの作成](../architecture/create-record-types.md).

   デフォルトでは、選択したタイプのすべてのレコードがテーブルビューに表示されます。

<!--
1. Click **+ View** to add a new view. 
1. Select from the following types of views: 

    * Table
    * Timeline
    * Calendar

    A new tab is created with the selected view. 

    Depending on the width of your screen, additional views might display in the **More** menu ![](assets/more-menu.png).   
-->

>[!TIP]
>
>レコードタイプを作成すると、テーブルビューもデフォルトで作成されます。
>
>タイムラインまたはカレンダービューを作成するには、ビューを作成するレコードの種類に少なくとも 2 つの日付フィールドが必要です。 それ以外の場合は、「タイムライン」および「カレンダー」オプションが淡色表示になります。
>

1. 次をクリック： **表示** ドロップダウンメニューで、既存の **テーブル表示** ![](assets/table-view-icon.png) または、 **ビューを作成/テーブル** テーブルビューを作成するには

   または

   既存の **タイムライン表示** ![](assets/timeline-view-icon.png) または、 **ビューを作成/タイムライン** をクリックして、タイムラインビューを作成します。

   または

   既存の **カレンダー表示** ![](assets/calendar-view-icon.png) または、 **ビューを作成/カレンダー** をクリックして、カレンダービューを作成します。

   ![](assets/view-types-drop-down-from-record-type-list.png)

   >[!NOTE]
   >
   >    タイムラインまたはカレンダービューを作成するには、ビューを作成するレコードの種類に少なくとも 2 つの日付フィールドが必要です。 それ以外の場合は、「タイムライン」または「カレンダー」オプションが淡色表示になります。

1. （条件付き）クリック **次へ**（タイムラインまたはカレンダービューを作成する場合）

   デフォルトでは、Workfrontは次のいずれかの名前をビューに付けます。

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   数値は、自動的に生成される増分です。

1. （条件付き） **開始** および **終了日** タイムラインまたはカレンダー表示に表示されるレコードの
1. 「**作成**」をクリックします。

   <!--add for view redesign: The view displays as a new tab. Views display in the chronological order from when they were created or shared with you. -->
<!--1. (Optional) Click the **More** menu ![](assets/more-caret-down-icon-views.png) next to the last view to view all views for the selected record type. 

    Additional views display under the **More** menu after the last view tab. The number next to the **More** menu shows the number of additional views. -->
1. （オプション）ビューの作成後に名前を変更するには、ビューのドロップダウンメニューをクリックし、 **その他** メニュー ![](assets/more-menu.png) > **名前を変更** をクリックして、ビュー名を更新します。 <!--ensure there is not another saving step here?!-->
   <!--1. (Optional) To rename a view after it is created, double-click the view name and start typing the new name, or click the **More** menu ![](assets/more-menu.png) to the right of the view name, then click **Rename**.-->
1. （オプション）特定のタイプの表示を管理するには、次の記事を参照してください。

   * [テーブル表示の管理](../views/manage-the-table-view.md)
   * [タイムライン表示を管理](../views/manage-the-timeline-view.md)
   * [カレンダー表示を管理](/help/quicksilver/maestro/views/manage-the-calendar-view.md)


## ビューを削除

{{step1-to-maestro}}

最後にアクセスしたワークスペースは、デフォルトで開きます。 ワークスペースの作成について詳しくは、 [ワークスペースの作成](../architecture/create-workspaces.md).

1. レコードタイプのカードをクリックします。

   レコードタイプの作成について詳しくは、 [レコードタイプの作成](../architecture/create-record-types.md).

   デフォルトでは、選択したタイプのすべてのレコードがテーブルビューに表示されます。

<!--1. Hover over one the of the view's names in the view tab, then click **More** ![](assets/more-menu.png) to the left of the view name, then click **Delete**. (********delete the instructions in the point below but keep the last step***********)
First, you might need to click **More** to the left of the last tab to find the view you want to delete. -->

1. 「表示」ドロップダウンメニューをクリックし、リスト内のビューの 1 つにマウスポインターを置いて、 **その他** メニュー ![](assets/more-menu.png) > **削除**.
1. クリック **削除** をクリックして確定します。 <!--ensure there is not another saving step here?!-->

   このビューは、レコード領域にアクセスできるすべてのユーザーに対して削除され、復元できません。

## ビューを共有

ビューの共有について詳しくは、 [ビューの共有](/help/quicksilver/maestro/access/share-views.md).

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: 

## Duplicate views

If you want to keep multiple versions of a view and make slight changes between the version, you can duplicate a view. Duplicating a view creates identical copies of an existing view. 

1. From the **Main Menu**, click **Maestro**. 
    The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture/create-workspaces.md).
1. Click a record type. For information about creating a record type, see [Create record types](../architecture/create-record-types.md). 

    By default, all the records of the type selected display in the table view. 

1. Click the view drop-down menu, then click the **More** menu ![](assets/more-menu.png) to the right of the view name > **Duplicate**. (**********ensure there is not another saving step here?! also, add how this view is named; the button to duplicate was there but not the functionality yet************)
    
    The view is duplicated and visible to all users who can access the Maestro area. 

-->
