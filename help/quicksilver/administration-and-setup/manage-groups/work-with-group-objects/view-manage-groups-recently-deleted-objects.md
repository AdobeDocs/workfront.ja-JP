---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: グループの最近削除された項目の表示と管理
description: '[ グループ ] 領域で管理するグループを表示している場合、最近削除した作業項目、ドキュメント、およびテンプレートを表示、フィルタ、復元、および書き出すことができます。'
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: d5fbc71b-3b22-48d1-a056-f2c4b32c220c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 1%

---

# グループの最近削除された項目の表示と管理

[ グループ ] 領域で管理するグループを表示している場合、最近削除したプロジェクト、タスク、問題、ドキュメント、およびテンプレートを次の方法で表示および操作できます。

* 最近削除された項目の一覧を表示、フィルタ、およびグループ化します
* 選択した最近削除した項目を復元します
* 最近削除した項目のリストを書き出す

グループの上にグループがある場合は、その管理者がグループに対してこれらの操作を実行することもできます。 Workfront管理者（すべてのグループ）も同様です。

削除された項目の詳細については、 [削除された項目を管理](../../../administration-and-setup/manage-workfront/manage-deleted-items/manage-deleted-items.md).

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront plan*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> <p>グループのグループ管理者またはWorkfront管理者である必要があります。 詳しくは、 <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a> および <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>削除した項目は、グループまたはそのサブグループに関連付ける必要があります。 </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランまたはライセンスの種類を確認する必要がある場合は、Workfront管理者にお問い合わせください。

## グループの最近削除された項目の表示と管理

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **グループ** ![](assets/groups-icon.png).

1. グループの名前をクリックします。
1. 左側のパネルで、 **最近削除された項目**.
1. グループの最近削除された項目を表示および管理する次のタブを開きます。

   * プロジェクト
   * タスク
   * 問題
   * ドキュメント
   * テンプレート

   各タブには、現在のグループまたはそのサブグループに属し、過去 30 日以内に削除された、対応するオブジェクトタイプの項目が一覧表示されます。

   >[!NOTE]
   >
   >誰かがプロジェクトを削除した場合、そのプロジェクトで個々のタスク、問題、ドキュメントがすべて削除されました。 「タスク」、「タスク」、「タスク」、「ドキュメント」または「テンプレート」タブに個別に表示されるわけではありません。 ただし、プロジェクトを復元すると、これらの子オブジェクトもすべてプロジェクトに復元されます。
   >
   >
   >タスク、イシュー、ドキュメント、またはテンプレートを個別に削除した場合は、該当するタブでそのタスクを表示および管理できます。

1. 次のいずれかの操作を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>オブジェクトの復元</p> </td> 
      <td> <p>最大 10 個のオブジェクトを選択し、 <strong>復元</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>「 」タブのオブジェクトのリスト全体を書き出し</p> </td> 
      <td> <p>クリック <strong>書き出し</strong>.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"> <p>リスト内の情報の表示を変更する</p> </td> 
      <td> <p>リストの上の右上隅で、 <strong>フィルター</strong> を使用して、指定した条件に基づいて表示する内容を定義します。 用途 <strong>表示</strong> を使用して、列として表示するフィールドを定義します。 用途 <strong>グループ化</strong> をクリックして、項目をカテゴリにグループ化します。</p> </td> 
     </tr> 
    </tbody> 
   </table>
