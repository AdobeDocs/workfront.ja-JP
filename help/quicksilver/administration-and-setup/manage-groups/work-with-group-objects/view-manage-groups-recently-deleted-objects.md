---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: 最近削除されたグループの項目の表示と管理
description: グループエリアで管理しているグループを表示している場合、最近削除された作業アイテム、ドキュメント、テンプレートを表示、フィルター、復元、および書き出すことができます。
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: d5fbc71b-3b22-48d1-a056-f2c4b32c220c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '443'
ht-degree: 100%

---

# 最近削除されたグループの項目の表示と管理

グループエリアで管理しているグループを表示している場合は、最近削除されたプロジェクト、タスク、イシュー、ドキュメント、およびテンプレートを、次の方法で表示して操作できます。

* 最近削除された項目の一覧を表示、フィルター、およびグループ化
* 最近削除した選択項目を復元
* 最近削除した項目のリストを書き出す

グループの上にグループがある場合は、その管理者がグループに対してこれらの操作を実行することもできます。Workfront 管理者（すべてのグループ）も同様です。

削除された項目について詳しくは、[削除された項目を管理](../../../administration-and-setup/manage-workfront/manage-deleted-items/manage-deleted-items.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront プラン*</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> <p>グループのグループ管理者または Workfront 管理者である必要があります。詳しくは、<a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">グループ管理者</a>および<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーへの完全な管理アクセス権の付与</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>削除した項目は、グループまたはそのサブグループのいずれかに関連付ける必要があります。 </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプランまたはライセンスの種類を確認する必要がある場合は、Workfront 管理者にお問い合わせください。

## 最近削除されたグループの項目の表示と管理

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックして、**設定** ![](assets/gear-icon-settings.png) をクリックします。

1. 左側のパネルで、「**グループ** ![](assets/groups-icon.png)」をクリックします。

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

1. 次のいずれかの操作を行います。

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
      <td> <p>リストの上の右上隅にある<strong>フィルター</strong>を使用して、指定した条件に基づいて表示する内容を定義します。<strong>表示</strong>を使用して、列として表示するフィールドを定義します。<strong>グループ化</strong>を使用して、項目をカテゴリにグループ化します。</p> </td> 
     </tr> 
    </tbody> 
   </table>
