---
title: レコードタイプを削除
description: 関連性がなくなった場合は、オペレーショナルレコードタイプまたは分類レコードタイプを削除できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 4016ba2c1b94ba84037612bdc9c1136267513fd5
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav:
---
title: Delete record types
description: You can delete operational record types or taxonomy record types when they are no longer relevant. 
author: Alina
feature: Work Management
topic: Architecture
role: User
hidefromtoc: yes
hide: yes
---
-->

# レコードタイプを削除

{{maestro-important-intro}}

関連性がなくなった場合は、オペレーショナルレコードタイプまたは分類レコードタイプを削除できます。

レコード・タイプと分類の詳細は、 [レコード・タイプと分類の概要](../architecture/overview-of-record-types-and-taxonomies.md).

別のレコードタイプで削除するレコードタイプまたは分類に関連付けられたフィールドとレコードを、削除する前に再度作成することをお勧めします。

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
   <p> Adobe Workfront</p> <p>Maestro のレコードタイプをExperience Manager Assetsに接続するには、Adobe Experience Manager Assetsライセンスが必要です。組織のWorkfrontインスタンスをAdobeビジネスプラットフォームまたはAdobe Admin Consoleにオンボーディングする必要があります。</p> </td>
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
   <td role="rowheader"><p>アクセスレベル設定</p></td>
   <td> <p>Maestro のアクセスレベルコントロールはありません</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する権限の管理</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています
</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfrontまたはグループ管理者は、レイアウトテンプレートに Maestro 領域を追加する必要があります。 詳しくは、 <a href="../access/access-overview.md">アクセスの概要</a>. </p>  
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

## レコードタイプを削除する際の考慮事項

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* 管理権限を持つワークスペースから、レコード・タイプまたは分類のみを削除できます。
* レコードタイプを削除すると、そのタイプのフィールドやレコードを含め、レコードに関連するすべての情報が削除されます。 レコードタイプは、ワークスペースにアクセスするすべてのユーザーから削除されます。
* 削除したレコードの種類やその情報は復元できません。

## レコードタイプを削除

分類レコードタイプの削除は、オペレーショナルレコードタイプの削除と同じです。

{{step1-to-maestro}}

最後にアクセスしたワークスペースは、デフォルトで開きます。

1. （オプション）既存のワークスペース名の右側にある下向き矢印を展開し、レコードタイプを削除するワークスペースを選択します。

   ワークスペースが開き、それに関連付けられたレコードタイプと分類が表示されます。
1. レコードタイプまたは削除する分類のカードをクリックします。

   レコードタイプのページが開きます。
1. 次をクリック： **その他** メニュー ![](assets/more-menu.png) をクリックし、 **削除**.
1. クリック **削除** をクリックして確定します。

   選択したレコードタイプまたは分類が、そのフィールドおよび関連するレコードと共に削除されます。
