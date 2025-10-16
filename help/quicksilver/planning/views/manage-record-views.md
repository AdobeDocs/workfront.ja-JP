---
title: レコード表示の管理
description: Adobe Workfront Planning を使用する場合、レコードをテーブル、タイムラインまたはカレンダ・ビューで表示できます。 この記事では、ビューを作成して既存のビューを編集する方法について説明します。
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 77342724-0182-4134-903b-4428d54cdceb
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '1144'
ht-degree: 40%

---


# レコードビューの管理

<!--

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

-->

{{planning-important-intro}}

Adobe Workfront Planning でレコードタイプを選択すると、そのタイプのすべてのレコードを次のビューに表示できます。

* テーブル

  詳しくは、[テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)を参照してください。

* タイムライン

  詳しくは、[タイムラインビューの管理](/help/quicksilver/planning/views/manage-the-timeline-view.md)を参照してください。

* カレンダー

  詳しくは、[タイムラインビューの管理](/help/quicksilver/planning/views/manage-the-calendar-view.md)を参照してください。

この記事では、レコードビューに関する次の情報について説明します。

* [ビューの作成と編集](#create-or-edit-record-views)
* [ ビューでリアルタイムプレゼンス指標を有効にする ](#enable-the-real-time-presence-indicator-in-a-view)
  <!--* [Add a view as a favorite](#add-a-view-as-a-favorite) - not possible yet-->

Workfrontの計画レコードのビューの管理について詳しくは、次の記事も参照してください。

* [レコードビューを削除](/help/quicksilver/planning/views/delete-record-views.md)
* [レコードビューを複製](/help/quicksilver/planning/views/duplicate-record-views.md)
* [ビューの共有](/help/quicksilver/planning/access/share-views.md)


## アクセス要件

+++ 展開して、この記事の機能のアクセス要件を表示します。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>任意のWorkfrontと任意の Planning パッケージ</p>
<p>任意のワークフローおよび任意の計画パッケージ</p>
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p> ビューを作成および削除するための標準</p>
   <p>ビュー要素を更新する投稿者以上</p>
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ビューに対する権限を管理</p>  
   <p>ビュー設定を一時的に変更したり、複製したりするためのビューへのアクセス許可を表示します</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> ライト ライセンスまたはコントリビュータ ライセンスを持つユーザには、Planning を含むレイアウト テンプレートを割り当てる必要があります。
   <p>標準ユーザーとシステム管理者は、デフォルトで Planning 領域を有効にします。</p></div></li></ul>
</td>
  </tr> 
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++


<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard to create and delete views</p>
   <p>Contributor or higher to update view elements</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Manage permissions to a view</p>  
   <p>View permissions to a view to temporarily change the view settings or to duplicate it</p> </td> 
  </tr> 
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> Users with a Light or Contributor license must be assigned a layout template that includes Planning.
   <p>Standard users and System Administrators have the Planning areas enabled by default.</p></div></li></ul>
</td>
  </tr>
</tbody> 
</table>-->

## レコードビューを使用する際の考慮事項

* Workfront Planning のビューは、レコードタイプに固有です。同じビューを 2 つの異なるレコードタイプに適用することはできません。
* 作成したビューは、自分と、そのビューを共有しているユーザーにのみ表示されます。
* ビューを変更または削除すると、そのビューに対する権限を持つすべてのユーザーに対して、ビューが変更および削除されます。
* 各ユーザーは、最大 100 のビューを作成できます。 1 つのレコードタイプに対して 100 を超えるビューを表示できますが、1 人のユーザーが作成できるビューは 100 のみです。
* 一部のビュー要素は、同じレコードの複数のビューに適用できますが、各レコードビューに固有です。

   * フィルター
   * グループ化（テーブルビューとタイムラインビューの場合）
   * バーの外観（タイムラインビューとカレンダービューの場合）

  例えば、テーブルビューでフィルターを作成した場合、フィルター結果は、選択したビュー（テーブルビュー）にのみ表示され、レコードタイプに関連付けられたすべてのビューには表示されません。

  >[!TIP]
  >
  >一部のビュー要素は、すべてのビューで使用できるわけではありません。


## レコードビューの類似点と相違点

テーブルビュー、タイムラインビューおよびカレンダービューの類似点と相違点を次の表に示します。

<!--some of these are NOT available right now; if you make this public, comment out the ones not there-->

| 機能 | テーブルビュー | タイムラインビュー | カレンダービュー |
|-----------------------------------------------------------------------|------------|---------------|--------------|
| 一覧または表でレコードを表示します | ✓ |              | |
| すべてのフィールドをテーブル内の列として表示します（デフォルト） | ✓ |              |    |
| フィールド（または列）の表示／非表示を切り替える | ✓ |               |    |
| 各レコードのフィールド値を編集 | ✓ |               |             |
| ビューにレコードを新しい行として追加 | ✓ |               |        |
| ビューにフィールドを新しい列として追加 | ✓ |               |         |
| 外部リストから行をコピーしてテーブルに貼り付ける | ✓ |               |          |
| タイムラインでレコードを表示 |            | ✓ |             |
| レコードのフィルタリング | ✓ | ✓ | ✓ |
| カレンダーにレコードを表示 |           |              | ✓ |
| レコードをグループ化 | ✓ | ✓ |
| レコードの並べ替え | ✓ |              |
| カラーコードのレコード | ✓ | ✓ | ✓ |
| カラーコードのグループ化 |           | ✓ |
| 特定のレコードを検索 | ✓ | ✓ |
| 他のユーザーとのビューの共有 | ✓ | ✓ | ✓ |
| ビューからレコードのページを開く | ✓ | ✓ |    |
| レコードを年および四半期別に表示 |           | ✓ |    |
| 月別にレコードを表示 |           | ✓ | ✓ |
| レコードを週別に表示 |           |               | ✓ |
| ビューからの情報のエクスポート | ✓ |               |    |
| 全画面表示で表示 | ✓ | ✓ | ✓ |
| ビューでのレコードの作成 | ✓ | ✓ | ✓ |

## ビューを作成または編集 {#create-or-edit-views}

{{step1-to-planning}}


1. ワークスペースのカードをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。

   デフォルトでは、選択したタイプのすべてのレコードがテーブルビューに表示されます。

1. 現在のビュー名の横にあるドロップダウンアイコン ![ ドロップダウンアイコン ](assets/drop-down-icon.png) ドロップダウンアイコン）をクリックし、「**+新規ビュー**」をクリックします。

1. 次のタイプのビューから選択します。

   * テーブル
   * タイムライン
   * カレンダー

1. 表示タイプを選択し、「**作成**」をクリックします。 ドロップダウンメニューに新しいビューが追加されます。

   >[!TIP]
   >
   >レコードタイプを作成すると、テーブルビューもデフォルトで作成されます。
   >
   >タイムライン表示またはカレンダー表示を作成するには、ビューを作成するレコードタイプに少なくとも 2 つの日付フィールドが必要です。
   >
   >それ以外の場合は、「タイムライン」および「カレンダー」オプションは淡色表示になります。
   >  

   ![ ビューボックスを作成 ](assets/create-view-box.png)

1. （オプション）既存のビューを編集するには、現在のビュー名の右側にあるドロップダウンメニューをクリックし、「**検索**」フィールドにビュー名を入力して、キーボードの Enter キーを押します。
1. （オプション）表示ドロップダウンメニューから、希望する順序でビューをドラッグ&amp;ドロップします。

   ![ レコードタイプリストからの表示タイプドロップダウン ](assets/view-types-drop-down-from-record-type-list.png)

1. （条件付き）タイムラインビューまたはカレンダービューを作成する際は、「**次へ**」をクリックします。

   デフォルトでは、ビューに次のいずれかの名前が付けられます。

   * `Table < number >`
   * `Timeline < number >`
   * `Calendar < number >`

   この数字は自動的に 1 ずつ増えて生成されます。

1. （条件付き）タイムラインビューまたはカレンダービューに表示されるレコードの場合は、「**開始日**」と「**終了日**」を選択します。

   >[!NOTE]
   >
   >    レコードの日付フィールドから選択することも、接続されたレコードまたはオブジェクトタイプから日付フィールドを参照することもできます。
   >
   >レコードタイプを接続するときに参照フィールドを選択する場合は、日付フィールド（MAXまたは MIN）にアグリゲータを使用する必要があります。 アグリゲータを追加するだけで、タイムラインおよびカレンダービューの開始日および終了日として接続の日付を使用できます。
   >
   >詳しくは、[レコードタイプの接続](/help/quicksilver/planning/architecture/connect-record-types.md)を参照してください。

1. 「**作成**」をクリックします。

   ビューは新しいタブとして表示されます。ビューは、作成時または共有時からの時間順で表示されます。
1. （オプション）選択したレコードタイプのすべてのビューを表示するには、最後のビューの横にある **その他** メニュー ![ その他のキャレットダウンアイコンビュー ](assets/more-caret-down-icon-views.png) をクリックします。

   最後のビュータブの後の&#x200B;**その他**&#x200B;メニューに、追加のビューが表示されます。**その他**&#x200B;メニューの横の数字は、追加のビューの数を示します。
1. （オプション）作成後にビューの名前を変更するには、ビューのドロップダウンメニューをクリックし、**詳細** メニュー ![ 詳細メニュー ](assets/more-menu.png)>**名前を変更** をクリックしてビュー名を更新します

   または

   ビュー名をダブルクリックし、新しい名前を入力していきます。<!--ensure there is not another saving step here?!-->

1. （オプション） **フルスクリーン** アイコン ![ フルスクリーンアイコンを開く ](assets/open-full-screen-icon.png) をクリックしてフルスクリーンで任意の表示を開き、**フルスクリーンを終了** アイコン ![ フルスクリーンアイコンを終了 ](assets/exit-full-screen-icon.png) またはキーボードの Esc キーをクリックしてフルスクリーンを終了します。

1. （オプション）特定のタイプのビューを管理するには、次の記事を参照してください。

   * [テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)
   * [タイムラインビューの管理](/help/quicksilver/planning/views/manage-the-timeline-view.md)
   * [カレンダービューの管理](/help/quicksilver/planning/views/manage-the-calendar-view.md)

## ビューでリアルタイムプレゼンスインジケーターを有効にする

ビュー内のリアルタイムプレゼンスインジケーターに従うと、他のユーザーが同時にレコードを編集しているかどうかを確認できます。

デフォルトでは、すべてのレコードビューの右上隅に表示される、レコード情報を同時に編集している他のユーザーのアバターです。

テーブルビューを表示すると、レコードの表示中に別のユーザーが編集しているフィールドを表示することもできます。

詳しくは、[テーブルビューの管理](/help/quicksilver/planning/views/manage-the-table-view.md)を参照してください。



<!--## Add a view as a favorite - this is not possible yet-->
