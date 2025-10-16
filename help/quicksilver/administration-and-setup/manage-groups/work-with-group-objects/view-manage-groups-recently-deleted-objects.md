---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: グループの最近削除されたアイテムの表示と管理
description: グループエリアで管理しているグループを表示している場合、最近削除された作業アイテム、ドキュメント、テンプレートを表示、フィルター、復元、および書き出すことができます。
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: d5fbc71b-3b22-48d1-a056-f2c4b32c220c
source-git-commit: 7eaff1c74cd880bde062e6fdf169c73d6eeb7f75
workflow-type: tm+mt
source-wordcount: '414'
ht-degree: 88%

---

# 最近削除されたグループの項目の表示と管理

グループエリアで管理しているグループを表示している場合は、最近削除されたプロジェクト、タスク、イシュー、ドキュメント、およびテンプレートを、次の方法で表示して操作できます。

* 最近削除された項目の一覧を表示、フィルター、およびグループ化
* 最近削除した選択項目を復元
* 最近削除した項目のリストを書き出す

グループの上にグループがある場合は、その管理者がグループに対してこれらの操作を実行することもできます。Workfront 管理者（すべてのグループ）も同様です。

削除された項目について詳しくは、[削除された項目を管理](../../../administration-and-setup/manage-workfront/manage-deleted-items/manage-deleted-items.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td><p>標準</p>
       <p>プラン</p></td>
  </tr> 
  <tr>
   <td>アクセスレベル設定</td> 
   <td>グループのグループ管理者またはシステム管理者である必要があります。</td>
  </tr>
  <tr> 
   <td>オブジェクト権限</td>
   <td>削除した項目は、グループまたはそのサブグループのいずれかに関連付ける必要があります。</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 最近削除されたグループの項目の表示と管理

{{step-1-to-setup}}

1. 左側のパネルで、「**グループ**![&#x200B; グループ &#x200B;](assets/groups-icon.png)」をクリックします。

1. グループの名前をクリックします。
1. 左側のパネルで、**最近削除された項目**&#x200B;をクリックします。
1. グループの最近削除された項目を表示して管理する次のタブを開きます。

   * プロジェクト
   * タスク
   * イシュー
   * ドキュメント
   * テンプレート

   各タブには、現在のグループまたはそのサブグループに属し、過去 30 日以内に削除された、対応するオブジェクトタイプの項目が一覧表示されます。

   >[!NOTE]
   >
   >誰かがプロジェクトを削除すると、そのプロジェクトの個々のタスク、イシュー、ドキュメントもすべて削除されます。「タスク」、「イシュー」、「ドキュメント」または「テンプレート」タブに個別に表示されるわけではありません。ただし、プロジェクトを復元すると、これらの子オブジェクトもすべてプロジェクトに復元されます。
   >
   >
   >タスク、イシュー、ドキュメント、またはテンプレートを個別に削除した場合は、該当するタブでそのタスクを表示して管理できます。

1. 次のいずれかのアクションを実行します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>オブジェクトを復元</p> </td> 
      <td> <p>最大 10 個のオブジェクトを選択し、「<strong>復元</strong>」をクリックします。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>タブのオブジェクトのリスト全体を書き出し</p> </td> 
      <td> <p>「<strong>書き出し</strong>」をクリックします。</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"> <p>リスト内の情報の表示を変更</p> </td> 
      <td> <p>リストの上の右上隅にある<strong>フィルター</strong>を使用して、指定した条件に基づいて表示する内容を定義します。<strong>ビュー</strong>を使用して、列として表示するフィールドを定義します。<strong>グループ化</strong>を使用して、項目をカテゴリにグループ化します。</p> </td> 
     </tr> 
    </tbody> 
   </table>
