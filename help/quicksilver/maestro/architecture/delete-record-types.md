---
title: レコードタイプの削除
description: 関係がなくなったレコードタイプは削除できます。 レコードタイプを削除すると、レコード、フィールド、ビューなど、レコードタイプに関連付けられているすべての情報も削除されます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: f4fb9d5c22ec6216a05e31cbcf80f1cf9add125f
workflow-type: tm+mt
source-wordcount: '386'
ht-degree: 36%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:
---
title: Delete record types
description: You can delete record types when they are no longer relevant. 
author: Alina
feature: Work Management
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->

# レコードタイプの削除

{{maestro-important-intro}}

関係がなくなったレコードタイプは削除できます。

ただし、レコードタイプを削除すると、そのレコードタイプに関連付けられているすべての情報も削除されます。 詳しくは、 [レコードタイプを削除する際の考慮事項](#considerations-when-deleting-record-types) この記事のセクションです。

レコードタイプについて詳しくは、を参照してください [レコードタイプの概要](../architecture/overview-of-record-types-and-taxonomies.md).

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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
 <td role="rowheader"><p>Adobe Workfront の契約</p></td>
   <td>
<p>Adobe Workfront Planning ベータ版プログラムに登録されている必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
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
   <td role="rowheader"><p>アクセスレベル設定</p></td>
   <td> <p>Adobe Workfront Planning には、アクセス レベルの制御はありません</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する権限を管理</a> </p>  
   <p>システム管理者は、自身が作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。
</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront管理者またはグループ管理者が、レイアウトテンプレートにプランニング エリアを追加する必要があります。 詳しくは、<a href="../access/access-overview.md">アクセス権の概要</a>を参照してください。 </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## レコードタイプを削除する際の考慮事項

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* 管理権限を持つワークスペースからは、レコードタイプのみを削除できます。
* レコードタイプを削除すると、それに関連付けられた次の情報が削除されます。

   * そのタイプのすべてのレコード。
   * レコードタイプに関連付けられているすべてのフィールド。
   * レコードタイプのすべての表示（フィルター、グループ化、並べ替え条件を含む）。
* そのレコードタイプは、ワークスペースにアクセスするすべてのユーザーから削除されます。
* 削除したレコードタイプやその情報は復元できません。
* 別のレコードタイプで削除するフィールドと、レコードタイプに関連付けられたレコードを、削除する前に再作成することをお勧めします。

## レコードタイプの削除

{{step1-to-maestro}}

最後にアクセスしたワークスペースが、デフォルトで開きます。

1. （オプション）既存のワークスペース名の右側にある下向き矢印を展開し、レコードタイプを削除するワークスペースを選択します。

   ワークスペースが開き、レコードタイプが表示されます。
1. 削除するレコードタイプのカードをクリックします。

   レコードタイプのページが開きます。
1. 「」をクリックします **詳細** メニュー ![](assets/more-menu.png) レコードタイプ名の右側にある「」をクリックします。 **削除**. <!--add screen shot when they finalize the UI-->
1. タイプ **削除** 確認ボックスで、 **完全に削除**.

   選択したレコードタイプは、フィールド、関連レコード、ビューと共に削除されます。
