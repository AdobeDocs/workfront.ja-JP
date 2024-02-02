---
product-area: resource-management
navigation-topic: resource-pools
title: リソースプールを作成する
description: リソースプールは、Adobe Workfront でリソースをより簡単に管理するのに役立つユーザーのコレクションです。リソースプールについて詳しくは、リソースプールの概要を参照してください。
author: Alina
feature: Resource Management
exl-id: 4991634c-e400-466e-bcee-3b461b6662d8
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '589'
ht-degree: 100%

---

# リソースプールを作成する

リソースプールは、Adobe Workfront でリソースをより簡単に管理するのに役立つユーザーのコレクションです。リソースプールについて詳しくは、[ リソースプールの概要](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md)を参照してください。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>Pro 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>リソースプールの管理へのアクセスを含む、リソース管理への編集アクセス権</p> <p>ユーザー、プロジェクトおよびテンプレートへの編集アクセス権</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>リソースプールを関連付けるプロジェクトおよびテンプレートの管理権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## リソースプールの作成 {#create-a-resource-pool}

1. リソースプールを編集するためのアクセス権を持つユーザーとしてログインします。\
   詳しくは、[リソースプールの作成](#create-a-resource-pool)を参照してください。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックします。

1. 「**リソース**」をクリックします。
1. 左側のパネルで「**リソースプール**」をクリックします。\
   ![resource_pools_tab.png](assets/resource-pools-tab-350x198.png)

1. 「**新しいリソースプール**」をクリックします。
1. 以下を指定します。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>名前</strong></td>
      <td>これは、リソースプールの名前です。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>説明</strong></td>
      <td>これは、このリソースプールに関する簡単な説明です。例えば、どのような目的でそれを使用するかを指定できます。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>プールのメンバー</strong></td>
      <td><p> ユーザーを個別にリソースプールに追加します。<br>または<br>リソースプールに多数のユーザーを一度に追加する場合。ユーザーまたはユーザーのコレクションに関連付けられた次のエンティティの 1 つを追加できます。
        <ul>
         <li><strong>チーム</strong>：チームのすべてのメンバーはリソースプールに追加されます。</li>
         <li><strong>グループ</strong>：グループのすべてのメンバーはリソースプールに追加されます。</li>
         <li><strong>役割</strong>：その役割に関連付けられているすべてのユーザーが、リソースプールに追加されます。</li>
         <li><strong>会社</strong>：会社のすべてのユーザーはリソースプールに追加されます。</li>
        </ul><p>ヒント：アクティブなユーザー、チーム、<span>役割、</span>または会社のみを追加できます。</p><p>メモ：ユーザーがグループ、チーム、会社のメンバーになった場合、またはグループ、チーム、会社、または担当業務がリソースプールに追加された後に担当業務に関連付けられた場合、新しいメンバーはリソースプールに自動的に追加されません。<br>追加するチーム、グループ、会社および担当業務に、ユーザーが属している場合、ユーザーは同時に、リソースプールに一度だけ追加されます。<br>リソースプールに追加した後に非アクティブ化されたユーザーは、ユーザーのリストでグレー表示になり、非アクティブ化とマークされます。</p></p></td>
     </tr>
    </tbody>
   </table>

1. （オプション）グループ、チーム、会社、または担当業務を通じて追加されたユーザーを削除するための&#x200B;**取り消し**&#x200B;リンクを使用します。

   >[!NOTE]
   >
   >リソースプール内のユーザー数に制限はありません。ただし、リソース管理が課題になる可能性があるので、リソースプールに多くのユーザーを追加しすぎないようにすることをお勧めします。ユーザーのリストには、リソースプール内の最初の 2,000 人のユーザーがアルファベット順で表示されます。

   ![Resource_pools_NEW___UNDO_button_for_teams_groups_etc.png](assets/resource-pools-new---undo-button-for-teams-groups-etc-350x113.png)

1. （オプション）ユーザー名の右にある「X」アイコンをクリックして、ユーザーを削除します。リソースプールからユーザーを削除する方法について詳しくは、[リソースプールからのユーザーの削除](../../../resource-mgmt/resource-planning/resource-pools/remove-users-from-resource-pool.md)を参照してください。
1. （オプション）「**検索**」オプションを使用して、リソースプール内のユーザーを検索します。
1. 「**作成**」をクリックします。
