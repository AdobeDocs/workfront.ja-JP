---
title: レコードの共有
description: 他のユーザーとレコードを共有して、共同作業を強化できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 83ff53ac-f18e-4b71-bdb2-57e05d69ed29
source-git-commit: 4e3449e7c31d29e1a289a7866ba98f873e62922c
workflow-type: tm+mt
source-wordcount: '381'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->
<!--should this move to the Access folder when we have sharing for ALL the objects???-->

# レコードの共有

>[!IMPORTANT]
>
>この記事の情報は、Adobe Workfrontからの新しいオファーであるAdobe・マエストロを指します。
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。 Maestro 機能を使用するには、Workfrontのお客様である必要があります。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

他のユーザーと共同作業する場合は、他のユーザーとレコードを共有できます。

Maestro レコードは次の方法で共有できます。

* ページが開いている場合に、レコードの詳細ページのリンクをブラウザーからコピーします。

* レコードタイプのテーブルビューのレコードを表示する際に、レコードの詳細ページへのリンクをコピーします。

<!-- Update with this when we release permissions: 

* You can share all records in a workspace with other users by sharing the workspace. For more information, see [Grant access to Adobe Maestro](../access/grant-access.md).
-->

この記事では、レコードタイプのテーブルビューからレコードの詳細ページへのリンクをコピーする方法について説明します。

<!-- add information about permissions, like:
- in the table below, you must have at least View permissions to the record
- the user you're sharing with must have at least View permissions to the record to view it
- etc - others???-->

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
   <td> <p>システム管理者は、レイアウトテンプレートに Maestro 領域を追加する必要があります。 詳しくは、 <a href="../access/access-overview.md">アクセスの概要</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permissions - replace the table with - below
****AND - see more above, another bullet point to update when permissions are released****

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

## レコードタイプのテーブルビューからレコードリンクを共有する

{#step1-to-maestro}

最後にアクセスしたワークスペースが開きます。
1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。
1. （条件付き） **表示** テーブルの右上隅にあるドロップダウンメニューから、テーブルビューを選択します。 最後にアクセスしたときにタイムラインビューでレコードタイプを表示した場合を除き、これがデフォルトのビューになります。

   選択したレコードタイプに関連付けられているレコードが、テーブルビューに表示されます。
1. レコード行を右クリック

   または

   レコードの名前の上にマウスポインターを置いて、 **その他** メニュー ![](assets/more-menu.png)を選択し、次に **リンクをコピー**.

   ![](assets/contextual-menu-for-record-row.png)

   リンクがクリップボードにコピーされます。

1. 他のユーザーと共有するには、メールまたはチャットウィンドウにリンクを貼り付けます。 ユーザーがリンクを受け取ると、レコードの詳細ページが開きます。

   >[!TIP]
   >
   >[ 詳細 ] ページのレコードのフィールドは、そのレコードの [ テーブル ] ビューで使用できるフィールドと同じです。


   <!--add there when it will be available: if they have access to this record-->
