---
title: レコードを削除
description: 自分または別のユーザーが作成したレコードを削除できます。 削除したレコードは復元できません。
hidefromtoc: true
hide: true
source-git-commit: f058c369bdb3b991910d3a820895de73ea4709f0
workflow-type: tm+mt
source-wordcount: '465'
ht-degree: 2%

---


<!--udpate the metadata with real information when making this available in TOC and in the left nav-->

# レコードを削除

>[!IMPORTANT]
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

Adobe・マエストロでは、不要になったレコードを削除できます。

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

## レコードの削除に関する考慮事項

* 自分または別のユーザーが作成したレコードを削除できます。
* 削除したレコードは復元できません。 <!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* 削除したレコードが他のレコードにリンクされている場合、リンクされたレコードは削除されませんが、削除したレコードの情報も削除されます。
* レコードは一括で削除できません。 <!--this will probably change-->
* タイムラインビューからレコードを削除することはできません。

## レコードを削除

次の領域からレコードを削除できます。

* [レコードの詳細ページから](#delete-a-record-from-the-records-details-page)
* [レコードタイプのテーブルビューから](#delete-a-record-from-the-record-type-table-view)

### レコードの詳細ページからレコードを削除する

1. 次をクリック： **メインメニュー** ![](assets/main-menu-workfront.png) を右上に配置するか、 **メインメニュー** ![](assets/main-menu-shell.png) 左上隅にある場合は、[ マエストロ ] をクリックします。

   最後にアクセスしたワークスペースが開きます。
1. レコードタイプをクリックします。

   レコードタイプのページが開きます。
1. 次のいずれかの操作を行います。

   * テーブルビューで、レコードの名前をクリックします。
   * テーブルビューで、レコード名の上にマウスポインターを置いて、 **その他** メニュー ![](assets/more-menu.png)を選択し、次に **表示**

     ![](assets/contextual-menu-for-record-row.png)
   * タイムラインビューで、レコードバーをクリックします。

   レコード **詳細** ページが開きます。

1. 次をクリック： **その他** メニュー ![](assets/more-menu.png) をクリックし、 **削除**&#x200B;を、 **削除** 再び確認します。

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
レコードは削除されているため、復元できません。

### レコードタイプのテーブルビューからレコードを削除する

1. 次をクリック： **メインメニュー** ![](assets/main-menu-workfront.png) を右上に配置するか、 **メインメニュー** ![](assets/main-menu-shell.png) 左上隅にある場合は、「 **マエストロ**.

   最後にアクセスしたワークスペースが開きます。
1. レコードタイプをクリックします。

   レコードタイプのページが開きます。
1. （条件付き） **表示** テーブルの右上隅にあるドロップダウンメニューから、テーブルビューを選択します。 最後にアクセスしたときにタイムラインビューでレコードタイプを表示した場合を除き、これがデフォルトのビューになります。

   選択したレコードタイプに関連付けられているレコードが、テーブルビューに表示されます。
1. レコード行を右クリックし、 **削除**.

   ![](assets/contextual-menu-for-record-row.png)

   レコードは削除されているため、復元できません。
