---
title: レコードタイプを削除
description: 関連性がなくなった場合は、オペレーショナルレコードタイプまたは分類レコードタイプを削除できます。
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '371'
ht-degree: 1%

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

>[!IMPORTANT]
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

関連性がなくなった場合は、オペレーショナルレコードタイプまたは分類レコードタイプを削除できます。

レコード・タイプと分類の詳細は、 [レコード・タイプと分類の概要](../architecture-and-fields/overview-of-record-types-and-taxonomies.md).

別のレコードタイプで削除するレコードタイプまたは分類に関連付けられたフィールドとレコードを、削除する前に再度作成することをお勧めします。

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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

## レコードタイプを削除する際の考慮事項

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* 自分または組織内の任意のユーザーが作成した任意のレコードタイプまたは分類を削除できます。 <!--this will change with access levels and permissions-->
* レコードタイプを削除すると、そのタイプのフィールドやレコードを含め、レコードに関連するすべての情報が削除されます。
* 削除したレコードの種類やその情報は復元できません。

## レコードタイプを削除

分類レコードタイプの削除は、オペレーショナルレコードタイプの削除と同じです。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-workfront.png) Workfrontの右上隅に <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> 次に、「 **マエストロ** ![](assets/maestro-icon.png).

   最後にアクセスしたワークスペースは、デフォルトで開きます。

1. （オプション）既存のワークスペース名の右側にある下向き矢印を展開し、レコードタイプを削除するワークスペースを選択します。

   ワークスペースが開き、それに関連付けられたレコードタイプと分類が表示されます。
1. レコードタイプまたは削除する分類のカードをクリックします。

   レコードタイプのページが開きます。
1. 次をクリック： **その他** メニュー ![](assets/more-menu.png) をクリックし、 **削除**.
1. クリック **削除** をクリックして確定します。

   選択したレコードタイプまたは分類が、そのフィールドおよび関連するレコードと共に削除されます。