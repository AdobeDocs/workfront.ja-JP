---
title: レコードビューの管理
description: AdobeMaestro を使用する際に、テーブルまたはタイムラインビューにレコードを表示できます。
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '731'
ht-degree: 1%

---


# レコードビューの管理

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

[Adobeマエストロ ] でレコードの種類を選択した後、次のビューにその種類のすべてのレコードを表示できます。

* テーブル

  詳しくは、 [テーブル表示の管理](../views/manage-the-table-view.md).
* タイムライン

  詳しくは、 [タイムライン表示を管理](../views/manage-the-timeline-view.md).

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
   <p> Adobe産物</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront協定</p></td>
   <td>
<p>組織は、Maestro クローズ済みベータプログラムのAdobeに登録する必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfrontプラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfrontライセンス</p></td>
   <td>
   <p>任意</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">アクセスレベル</td>
   <td> <p>任意</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">レイアウトテンプレート</td>
   <td> <p>システム管理者は、レイアウトテンプレートに Maestro 領域を追加する必要があります。 詳しくは、 <a href="../access/grant-access.md">AdobeMaestro へのアクセスを許可</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## Maestro ビューを使用する際の考慮事項

* マエストロのビューは、レコードのタイプに固有です。 同じビューを 2 つの異なるレコードタイプに適用することはできません。
* 作成したビューは、Maestro 領域にアクセスするすべてのユーザに表示されます。 <!-- edit this when we have permissions and the views will be shared only to be visible by others-->
  <!-- this is not yet possible: * You can share views with others if you want them to also apply them to the same record types.-->
* オペレーショナルレコードタイプのビューの作成は、分類レコードタイプのビューの作成と同じです。
* ビューを修正または削除すると、Maestro 領域にアクセスできるすべてのユーザに対して、ビューが変更および削除されます。
* 次の要素は、Maestro の各ビューに固有です。

   * フィルター
   * グループ化
   * 並べ替え

  <!-- some of these are not available in all of the views - edit above-->

  例えば、テーブルビューでフィルタを作成する場合、フィルタ結果は選択したビューにのみ表示され、「ビュー」(View) ドロップダウンメニューにリストされるすべてのビューからは表示されません。

  >[!NOTE]
  >
  > Maestro は現在ベータ状態なので、一部のビュー要素は両方のビューで使用できない場合があります。


この記事では、Maestro ビューに関する次の情報について説明します。

* [ビューの作成と編集](#create-or-edit-record-views)
* [ビューの削除](#delete-views)
  <!--* [Duplicate a view](#duplicate-views)-->
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->
  <!--* [Share a view](#share-views) - not possible yet-->

## テーブルビューとタイムラインビューの類似点と相違点

次の表は、Maestro のテーブルビューとタイムラインビューの類似点と相違点を示しています。

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| 機能 | テーブル表示 | タイムライン表示 |
|-----------------------------------------------------------------------|------------|---------------|
| リストまたはテーブルにレコードを表示 | ✓ |              |
| すべてのフィールドをテーブル内の列として表示（デフォルト） | ✓ |              |
| フィールド（または列）の表示/非表示を切り替える | ✓ |               |
| 各レコードのフィールド値を編集 | ✓ |               |
| レコードを新しい行としてビューに追加 | ✓ |               |
| ビューでフィールドを新しい列として追加 | ✓ |               |
| 外部リストから行をコピーしてテーブルに貼り付ける | ✓ |               |
| タイムラインでのレコードの表示 |            | ✓ |
| レコードのフィルタリング | ✓ | ✓ |
| レコードをグループ化 |           | ✓ |
| レコードの並べ替え | ✓ |              |

<!--| Sort groupings                                                        | ✓          | ✓             |-->

<!--| Display a limited number of fields as columns, by default                      | ✓          |               |-->

<!--| Color-code records                     |           | ✓              |-->
<!--| Color-code groupings                     |           | ✓              |-->

## ビューの作成または編集 {#create-or-edit-views}

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-workfront.png) 右上隅に <!--or the **Main Menu** icon ![](assets/main-menu-shell.png) in the upper-left corner, if available-->を選択し、次に **マエストロ** ![](assets/maestro-icon.png).
最後にアクセスしたワークスペースは、デフォルトで開きます。 ワークスペースの作成について詳しくは、 [ワークスペースの作成](../architecture-and-fields/create-workspaces.md).
1. レコードタイプのカードをクリックします。 レコードタイプの作成について詳しくは、 [レコードタイプの作成](../architecture-and-fields/create-record-types.md).

   デフォルトでは、選択したタイプのすべてのレコードがテーブルビューに表示されます。

1. 次をクリック： **表示** ドロップダウンメニューで、既存の **テーブル表示** ![](assets/table-view-icon.png) または、 **ビューを作成/テーブル** テーブルビューを作成するには

   または

   既存の **タイムライン表示** ![](assets/timeline-view-icon.png) 表示またはクリック **ビューを作成/タイムライン** をクリックして、タイムラインビューを作成します。

   ![](assets/view-types-drop-down-from-record-type-list.png)

   >[!NOTE]
   >
   >    タイムラインビューを作成するには、ビューを作成するレコードタイプに少なくとも 2 つの日付フィールドが必要です。 それ以外の場合は、「タイムライン」オプションは淡色表示になります。

1. （オプション）ビューの名前を更新し、「 **作成** をクリックして保存します。

   既定では、Maestro はビューに&quot;Table &lt; number >&quot;または&quot;Timeline &lt; number >&quot;と名前を付けます。 数値は、自動的に生成される増分です。

1. （オプション）ビューの作成後に名前を変更するには、ビューのドロップダウンメニューをクリックし、 **その他** メニュー ![](assets/more-menu.png) > **名前を変更** をクリックして、ビュー名を更新します。 <!--ensure there is not another saving step here?!-->
1. （オプション）ビューを管理するには、詳しくは次の記事を参照してください。

   * [テーブル表示の管理](../views/manage-the-table-view.md)
   * [タイムライン表示を管理](../views/manage-the-timeline-view.md)


<!--# Add a view as a favorite - this is not possible yet-->

<!-- ## Share views - not possible yet-->

## ビューを削除

1. 次から： **メインメニュー** ![](assets/main-menu-workfront.png) 画面の右上隅に <!--or the **Main Menu** ![](assets/main-menu-shell.png) in the upper-left corner of the screen, if available,--> click **マエストロ** ![](assets/maestro-icon.png).

   最後にアクセスしたワークスペースは、デフォルトで開きます。 ワークスペースの作成について詳しくは、 [ワークスペースの作成](../architecture-and-fields/create-workspaces.md).
1. レコードタイプのカードをクリックします。

   レコードタイプの作成について詳しくは、 [レコードタイプの作成](../architecture-and-fields/create-record-types.md).

   デフォルトでは、選択したタイプのすべてのレコードがテーブルビューに表示されます。

1. 「表示」ドロップダウンメニューをクリックし、リスト内のビューの 1 つにマウスポインターを置いて、 **その他** メニュー ![](assets/more-menu.png) > **削除**.
1. クリック **削除** をクリックして確定します。 <!--ensure there is not another saving step here?!-->

   ビューは、Maestro 領域にアクセスできるすべてのユーザに対して削除され、復元できません。

<!--not possible yet - August 30, 2023: 

## Duplicate views

If you want to keep multiple versions of a view and make slight changes between the version, you can duplicate a view. Duplicating a view creates identical copies of an existing view. 

1. From the **Main Menu**, click **Maestro**. 
    The workspace you last accessed opens by default. For information about creating workspaces, see [Create workspaces](../architecture-and-fields/create-workspaces.md).
1. Click a record type. For information about creating a record type, see [Create record types](../architecture-and-fields/create-record-types.md). 

    By default, all the records of the type selected display in the table view. 

1. Click the view drop-down menu, then click the **More** menu ![](assets/more-menu.png) to the right of the view name > **Duplicate**. (**********ensure there is not another saving step here?! also, add how this view is named; the button to duplicate was there but not the functionality yet************)
    
    The view is duplicated and visible to all users who can access the Maestro area. 

-->