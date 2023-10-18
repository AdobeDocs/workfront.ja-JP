---
title: タイムライン表示を管理
description: AdobeMaestro でレコードタイプのページにアクセスする際に、タイムラインビューにレコードを表示できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: f348af7f-5bb9-4d88-9bcb-3bef7e8892dd
source-git-commit: b02c81873d84946f8db54bcf9a1a464de38781de
workflow-type: tm+mt
source-wordcount: '1093'
ht-degree: 1%

---

# タイムライン表示を管理

<!--
title: Manage the timeline view in Adobe Maestro
description: You can display records in a timeline view, when accessing the record type page in Adobe Maestro. 
hidefromtoc: yes
hide: yes
author: Alina
feature: Work Management
role: User
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

>[!IMPORTANT]
>
>この記事の情報は、Adobe・マエストロに関して、Adobeからの新しいオファーです。
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

AdobeMaestro でレコードタイプのページにアクセスする際に、タイムラインビューにレコードを表示できます。

Maestro ビューについて詳しくは、 [レコードビューをAdobeMaestro で管理](../views/manage-record-views.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col>
 <tbody>
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

## タイムライン表示の管理 {#manage-a-timeline-view}

<!--insert screen shot of timeline view-->

タイムラインビューを作成すると、選択したレコードタイプのすべてのレコードが時系列で表示されます。

次の点に注意してください。

* タイムラインビューを作成できるのは、レコードタイプに関連付けられた日付フィールドが少なくとも 2 つある場合のみです。 1 つ以上の日付フィールドがレコードの種類に関連付けられている場合は、[ タイムライン表示 ] オプションは淡色表示になります。
* 次のシナリオでは、日付がレコードに関連付けられている場合に、一部のレコードがタイムラインビューに表示されないことがあります。

   * 開始日と終了日に値がない場合
   * 開始日または終了日に値がない場合
   * 開始日が終了日より後の場合

<!--these are NOT available now because there won't be a table for the timeline view for the near future, per Andy: 
* The records displayed in the timeline view also display in a view-only table to the left of the timeline. 
* Each row in the table and each bar on the timeline represent the same record. 
* Each column in the table is a record field. The columns of this table are preconfigured and cannot be customized. 
* Only a limited number of fields (or columns) display in the timeline view table. 
* You cannot do the following in a timeline view:
     * Add rows or records
     * Add columns or fields
     * Edit record information
-->

タイムラインビューを作成する場合、デフォルトでは、選択したレコードタイプのすべてのレコードがタイムラインにバーとして表示されます。

タイムラインビューを管理するには：

1. タイムラインを表示するレコードタイプページに移動します。
1. 記事の説明に従って、タイムラインビューを作成します。 [レコードビューの管理](../views/manage-record-views.md).

   ![](assets/timeline-view-example.png)

   選択したレコードの種類に関連付けられたレコードは、時系列にバーとして表示されます。

1. タイムラインに移動するには、次のいずれかの操作を行います。

   * 左右のアイコンをクリックするか、水平スクロールを使用してタイムライン内を前後に移動します。
   * クリック **今日** をクリックして、今日の日付をタイムラインの中心に配置します。
   * 時間枠ドロップダウンメニューから次のいずれかのオプションを選択して、時間間隔を更新します。

      * 年
      * 四半期
      * 月
1. クリック **標準に切り替え** 別々の行にレコードを表示するビュー <!--check to see if they updated the name of the setting here-->

   または

   クリック **コンパクト表示に切り替え** 日付が同じ行で交差しないレコードを表示します。 <!--check to see if they updated the name of the setting here-->

   デフォルトでは、レコードはコンパクトビューに表示されます。

1. 以下のサブセクションで説明するように、次のビュー要素を更新します。
   * [フィルター](#add-filters)
   * [グループ化](#add-grouping)
     <!--* [Sort](#add-sort) not sure if this is present in timeline views?!; also check the anchor and make sure it's correct-->
   * [設定](#edit-the-timeline-view-settings)

### フィルターを追加

フィルターを使用すると、画面に表示される情報の量を減らすことができます。

タイムライン表示でフィルターを操作する際は、次の点に注意してください。

<!-- this list is almost identical to the one for the table view - update both-->

* タイムライン表示用に作成したフィルタは、同じレコードタイプに適用された場合、テーブル表示のフィルタとは独立して機能します。

* フィルターは、選択したビューに固有です。 同じレコードタイプの 2 つのタイムラインビューに、異なるフィルターを適用することができます。 同じタイムライン表示を見ている 2 人のユーザーには、現在適用されているのと同じフィルターが表示されます。

* 作成してタイムラインビューに適用したフィルターに名前を付けることはできません。

* フィルターを削除すると、自分と同じレコードタイプにアクセスするすべてのユーザーからフィルターが削除され、使用したのと同じビューが使用されます。

タイムラインビューでのフィルターの追加方法は、テーブルビューでのフィルターの追加方法と同じです。

詳しくは、この記事の「フィルターの追加」の節を参照してください [テーブル表示の管理](../views/manage-the-table-view.md).

### グループ化を追加

<!-- if groupings are identical between the table and the timeline, consider replacing this section with this: 

Adding groupings in the timeline view is identical to adding filters in the table view. 

For more information, see the "Add filters" section in the article [Manage the table view](../views/manage-the-table-view.md). -->


グループ化をビューに適用する際に、類似の情報でレコードをグループ化できます。

タイムライン表示でグループ化を操作する際は、次の点に注意してください。

* テーブルビューとタイムラインビューの両方でグループを適用できます。 テーブルビューのグループは、同じレコードタイプのタイムラインビューのグループとは独立しています。
* マエストロビューでは、3 つのレベルのグループ化を適用できます。 レコードは、選択したグループ化の順にグループ化されます。
* API を使用する場合、最大 4 レベルのグループ化を適用できます。

グループを追加する手順は、次のとおりです。

1. 記事の説明に従って、タイムラインビューを作成します。 [レコードビューの管理](../views/manage-record-views.md).
1. クリック **グループ化**.

   ![](assets/grouping-ui-timeline-view.png)

1. 推奨フィールドの 1 つをクリックするか、 **別のフィールドを選択** 別のフィールドを検索し、リストに表示されたらクリックします。

   >[!TIP]
   >
   >リンクされたフィールドは選択できません。

   グループ化はタイムラインに自動的に適用され、レコードはグループ化ボックス内に表示されます。 グループ化の項目数がグループ化行に表示されます。

   <!-- add a step that you can rearrange the groupings here, when this will be possible-->

1. （オプション）上記の手順を繰り返して、最大 3 つのグループを追加します。

   適用したグループの数は、ツールバーの右上隅にあるグループ化アイコンの左側に表示されます。

   ![](assets/grouping-applied-in-timeline-view.png)

1. （オプション） **x** グループ化を削除するためのグループ化の右側のアイコン

   または

   クリック **すべてクリア** をクリックして、すべてのグループを削除します。

1. の外側をクリック **次の項目でレコードをグループ化** ボックスを使用して閉じます。

<!-- 

### Add sort

this is not possible right now; if this is the same functionality as the table view, document it there and link from here. 

-->

### タイムライン表示設定の編集 {#edit-the-timeline-view-settings}

タイムライン表示の設定を更新して、ビューのタイムラインセクションに表示する情報を指定します。

1. 記事の説明に従って、タイムラインビューを作成します。 [レコードビューの管理](../views/manage-record-views.md).
1. クリック **設定**.
1. クリック **日時** 左のパネルで、 **開始日** および **終了日** をクリックしてタイムラインに表示します。 デフォルトの開始日と終了日を選択するか、使用可能な任意の日付フィールドを選択できます。 レコードの開始日を表すバーは、[ 開始日 ] に指定した日付に開始し、[ 終了日 ] に対応する日付に終了します。

   >[!NOTE]
   >
   >    開始日または終了日の値がないレコード、または開始日が終了日より後のレコードは、タイムラインビューに表示されません。


1. クリック **レコードの詳細** をクリックして、レコードバーに表示するフィールドを指定します。

   「名前」フィールドはデフォルトで選択されています。

1. クリック **フィールドを追加** を使用して、レコードバーに最大 4 つのフィールドを追加できます。
1. 内側をクリック **検索フィールド** 」ボックスをクリックし、追加するフィールドをクリックします。

   >[!TIP]
   >
   >   * フィールドをレコードバーに追加する前に、フィールドを作成する必要があります。
   > 
   >   * 1 つ以上のフィールドを選択する必要があります。 **名前** はデフォルトで選択されています。

   タイムライン上のバーの外観のプレビューが右側に表示されます。

   ![](assets/record-details-panel-timeline-settings-with-preview.png)

1. 「**保存**」をクリックします。

   レコードは、選択した仕様と共にタイムライン表示に表示されます。
