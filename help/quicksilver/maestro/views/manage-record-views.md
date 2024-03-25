---
title: レコードビューの管理
description: Adobe Workfront Planning を使用する際に、テーブル、タイムライン、またはカレンダー表示にレコードを表示できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 6%

---

# レコードビューの管理

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

Adobe Workfrontの計画領域でレコード・タイプを選択した後、次のビューにそのタイプのすべてのレコードを表示できます。

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
<p>組織は、Adobe Workfront Planning クローズ済みベータプログラムに登録されている必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
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
   <td> <p>Workfront Planning には、アクセスレベルの制御はありません</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ビューに対する権限の管理</p>  
</td>
  </tr>

<tr>
   <td role="rowheader">レイアウトテンプレート</td>
   <td> <p>システム管理者は、レイアウトテンプレートに計画領域を追加する必要があります。 詳しくは、 <a href="../access/access-overview.md">アクセスの概要</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

## レコードビューを使用する際の考慮事項

* Workfront計画のビューは、レコードのタイプに固有です。 同じビューを 2 つの異なるレコードタイプに適用することはできません。
* 作成したビューは、自分とそのビューを共有しているユーザーにのみ表示されます。
* ビューを変更または削除すると、そのビューに対する権限を持つすべてのユーザーに対して、ビューが変更および削除されます。
* 次の要素は、各レコードビューに固有です。

   * フィルター
   * グループ化
   * 並べ替え

  <!-- some of these are not available in all of the views - edit above-->

  たとえば、テーブルビューでフィルタを作成する場合、フィルタ結果は選択したビューにのみ表示され、レコードタイプに関連付けられているすべてのビューには表示されません。

  >[!NOTE]
  >
  > Adobe Workfront Planning は現在ベータ状態なので、一部のビュー要素が一部のビューで使用できない場合があります。

この記事では、レコードビューに関する次の情報について説明します。

* [ビューの作成と編集](#create-or-edit-record-views)
* [ビューの削除](#delete-views)
* [ビューの複製](#duplicate-views)
* [ビューの共有](#share-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->

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
| レコードのフィルタリング | ✓ | ✓ | ✓ |
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

1. クリック **+表示** をクリックして新しいビューを追加します。
1. 次のタイプのビューから選択します。

   * テーブル
   * タイムライン
   * カレンダー

   選択したビューで新しいタブが作成されます。

   画面の幅に応じて、 **その他** メニュー ![](assets/more-menu.png).


>[!TIP]
>
>レコードタイプを作成すると、テーブルビューもデフォルトで作成されます。
>
>タイムラインまたはカレンダービューを作成するには、ビューを作成するレコードの種類に少なくとも 2 つの日付フィールドが必要です。 それ以外の場合は、「タイムライン」および「カレンダー」オプションが淡色表示になります。
>

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

   ビューが新しいタブとして表示されます。 ビューは、自分が作成または共有された時点から時系列で表示されます。
1. （オプション） **その他** メニュー ![](assets/more-caret-down-icon-views.png) 選択したレコードタイプのすべてのビューを表示するには、最後のビューの横にあります。

   追加のビューは、 **その他** メニューを表示します。 の隣の数 **その他** メニューには、追加のビュー数が表示されます。
1. （オプション）ビューの作成後に名前を変更するには、ビューのドロップダウンメニューをクリックし、 **その他** メニュー ![](assets/more-menu.png) > **名前を変更** ビュー名を更新するには

   または

   ビュー名をダブルクリックし、新しい名前を入力します。  <!--ensure there is not another saving step here?!-->

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

1. 「表示」タブでビューの名前の 1 つにマウスポインターを置き、「 **その他** ![](assets/more-menu.png) ビュー名の左側に移動し、 **削除**.
最初に、 **その他** をクリックして、削除するビューを見つけます。

1. クリック **削除** をクリックして確定します。 <!--ensure there is not another saving step here?!-->

   このビューは、レコード領域にアクセスできるすべてのユーザーに対して削除され、復元できません。

## ビューを共有

ビューの共有について詳しくは、 [ビューの共有](/help/quicksilver/maestro/access/share-views.md).

<!--## Add a view as a favorite - this is not possible yet-->

<!--not possible yet - August 30, 2023: -->

## ビューの複製

複数のバージョンのビューを保持し、バージョン間で若干の変更を加える場合は、ビューを複製できます。

ビューを複製すると、既存のビューの同じコピーが作成されます。

元のビューの共有権限は、複製されたビューに転送されません。

{{step1-to-maestro}}

最後にアクセスしたワークスペースは、デフォルトで開きます。

ワークスペースの作成について詳しくは、 [ワークスペースの作成](../architecture/create-workspaces.md).

1. レコードタイプのカードをクリックします。 レコードタイプの作成について詳しくは、 [レコードタイプの作成](../architecture/create-record-types.md).

   デフォルトでは、選択したタイプのすべてのレコードがテーブルビューに表示されます。

1. 複製する表示のタブにマウスポインターを置いて、 **その他** メニュー ![](assets/more-menu.png) ビュー名の右に移動し、 **複製**.

   ![](assets/view-more-menu-with-duplicate-option.png)


   ビューが複製され、新しいビューの名前は次のパターンに従います。 `Original view's name (Copy)`. 新しいビュータブは、すべてのビュータブの最後に表示されます。

