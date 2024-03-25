---
title: カレンダー表示を管理
description: レコードとそのフィールドをカレンダービューに表示できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 45b5be81-703c-45d5-a08c-60cb8ec5b103
source-git-commit: a0f12a016ae8ac73136f05bf3255f9882e2ce6d4
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 6%

---

# カレンダー表示を管理

<!--
title: Manage the calendar view
description: You can display records in a calendar view.
hidefromtoc: yes
author: Alina
feature: Work Management
role: User
hide: yes
-->

<!--update the metadata with real information when making this available in TOC and in the left nav-->

{{maestro-important-intro}}

レコードタイプのページから、レコードとそのフィールドをカレンダービューに表示できます。

Adobe Workfront Planning 機能の表示と管理方法について詳しくは、 [レコードビューの管理](../views/manage-record-views.md).

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
<p>組織がAdobe Workfront Planning ベータプログラムに登録されている必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
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
   <td> <p>Adobe Workfront Planning には、アクセスレベルの制御はありません</p>  
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


## カレンダービューの管理 {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

次の点に注意してください。

* カレンダービューを作成できるのは、レコードの種類に関連付けられた日付フィールドが少なくとも 2 つある場合のみです。 レコードの種類に関連付けられている日付フィールドが 1 つ以上ある場合は、[ カレンダー表示 ] オプションは淡色表示になります。
* 次のシナリオが存在します。

   * 開始日と終了日の両方に値が設定されていない場合、レコードはカレンダーに表示されません
   * 開始日または終了日に値がない場合、レコードは 1 日イベントとして表示されます
   * 開始日が終了日より後の場合、レコードはカレンダーに表示されません。

カレンダー・ビューを管理する手順は、次のとおりです。

1. カレンダーを表示するレコードの種類のページに移動します。
1. 記事の説明に従って、カレンダービューを作成します。 [レコードビューの管理](../views/manage-record-views.md).

   ![](assets/calendar-view-example.png)

   選択したレコードの種類に関連付けられたレコードは、カレンダーのバーとして表示されます。 バーの色は、レコードアイコンの色と一致します。

1. カレンダー内を移動するには、次のいずれかの操作を行います。

   * 左右のアイコンをクリックするか、横スクロールを使用して、カレンダー内を前後に移動します。
   * クリック **今日** カレンダーを今日の日付の中央に配置します。
   * 時間枠ドロップダウンメニューから次のいずれかのオプションを選択して、時間間隔を更新します。

      * 月
1. 以下のサブセクションで説明するように、次のビュー要素を更新します。
   * [フィルター](#add-filters)
     <!--* [Grouping](#add-grouping)-->
     <!--* [Settings](#edit-the-calendar-view-settings)-->
     <!--* [Sort](#add-sort) not sure if this is present in calendar views?!; also check the anchor and make sure it's correct-->

### フィルターを追加

フィルターを使用すると、画面に表示される情報の量を減らすことができます。

カレンダービューでフィルターを使用する際は、次の点に注意してください。

<!-- this list is almost identical to the one for the table view - update both-->

* カレンダービューに対して作成したフィルタは、同じレコードタイプに適用される他のビューのフィルタとは独立して機能します。

* フィルターは、選択したビューに固有です。 同じレコードタイプの 2 つのカレンダービューに、異なるフィルタを適用することができます。

* 同じカレンダー表示を見ている 2 人のユーザーには、現在適用されているのと同じフィルターが表示されます。

* カレンダービューに対して作成したフィルターに名前を付けることはできません。

* フィルターを削除すると、自分と同じレコードタイプにアクセスし、自分と同じビューを表示する人から、自分が削除されます。

* カレンダービューでのフィルターの追加方法は、テーブルビューでのフィルターの追加方法と同じです。

  詳しくは、この記事の「フィルターの追加」の節を参照してください [テーブル表示の管理](/help/quicksilver/maestro/views/manage-the-table-view.md).

* 接続されたレコードフィールドまたは参照フィールドでフィルタリングできますが、複数のレコードにリンクできるフィールドに対してはフィルタリングできません。
