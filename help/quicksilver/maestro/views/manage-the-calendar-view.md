---
title: カレンダー表示を管理
description: レコードとそのフィールドをカレンダービューに表示できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: ff52e43fc5ed5a7939b9e28b2bda195e94e81724
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 8%

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

Maestro ビューとその管理方法については、 [レコードビューの管理](../views/manage-record-views.md).

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
<p>組織は、Maestro クローズ済みベータプログラムのAdobeに登録する必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
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
   <td> <p>Maestro のアクセスレベルコントロールはありません </p>  
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


## カレンダービューの管理 {#manage-a-calendar-view}

<!--insert screen shot of calendar view-->

次の点に注意してください。

* カレンダービューを作成できるのは、レコードの種類に関連付けられた日付フィールドが少なくとも 2 つある場合のみです。 レコードの種類に関連付けられている日付フィールドが 1 つ以上ある場合は、[ カレンダー表示 ] オプションは淡色表示になります。
* 次のシナリオに従います。

   * 開始日と終了日に値が設定されていない場合、レコードはカレンダーに表示されません
   * 開始日または終了日に値がない場合、レコードは 1 日イベントとして表示されます
   * 開始日が終了日より後の場合、レコードはカレンダーに表示されません。

カレンダー・ビューを管理する手順は、次のとおりです。

1. カレンダーを表示するレコードの種類のページに移動します。
1. 記事の説明に従って、カレンダービューを作成します。 [レコードビューの管理](../views/manage-record-views.md).

   ![](assets/calendar-view-example.png)

   選択したレコードの種類に関連付けられたレコードは、カレンダーのバーとして表示されます。

1. カレンダー内を移動するには、次のいずれかの操作を行います。

   * 左右のアイコンをクリックするか、横スクロールを使用して、カレンダー内を前後に移動します。
   * クリック **今日** カレンダーを今日の日付の中央に配置します。
   * 時間枠ドロップダウンメニューから次のいずれかのオプションを選択して、時間間隔を更新します。

      * 月