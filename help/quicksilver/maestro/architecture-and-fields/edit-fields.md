---
title: フィールドを編集
description: Adobeマエストロでは、既に作成済みのフィールドのフィールド設定を編集できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: 4cdebe4890b775a097469e7d7035a38397b71094
workflow-type: tm+mt
source-wordcount: '454'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# フィールドを編集

>[!IMPORTANT]
>
>この記事の情報は、Adobe・マエストロに関して、Adobeからの新しいオファーです。
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

作成済みのフィールドのフィールド設定を編集できます。

AdobeMaestro フィールドの作成については、 [フィールドの作成](../architecture-and-fields/create-fields.md).

この記事では、Maestro フィールドの設定を編集する方法について説明します。 Maestro レコードのフィールド値の編集について詳しくは、 [レコードを編集](../records/edit-records.md).

## フィールド情報の編集に関する考慮事項

* 自分が作成したフィールドや、他のユーザーが作成したフィールドを編集できます。 <!--this will change with access levels/ permissions-->
* レコードタイプテーブルのフィールドを編集できます。
* フィールドを保存した後は、フィールドタイプを編集できません。
* 添付先のレコードに既に負の値が格納されている場合は、[ 数値 ]、[ 割合 ]、または [ 通貨 ] フィールドに対して、以前に選択した [ 負の値を許可する ] 設定の選択を解除することはできません。
<!--this is not true yet; one piece of it is true and I added it as the bullet above: 
* You cannot edit the options, or the special format of the following fields, after they are saved:

    * Allow negative numbers option from a Number, Percentage, or Currency field. 
    * The Options of a Single-select or a Multi-select field.
-->

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

## フィールドを編集

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-workfront.png) Workfrontの右上隅、または **メインメニュー** アイコン ![](assets/main-menu-shell.png)  左上隅にある場合は、「 **マエストロ** ![](assets/maestro-icon.png).

   最後にアクセスしたワークスペースは、デフォルトで開きます。

1. （オプション）既存のワークスペース名の右側にある下向き矢印を展開し、レコードタイプを削除するワークスペースを選択します。

   ワークスペースが開き、それに関連付けられたレコードタイプと分類が表示されます。
1. フィールドを編集するレコードタイプまたは分類のカードをクリックします。

   レコードタイプのページが開きます。
1. （条件付き） **テーブル表示** から **表示** レコードタイプページの右上隅にあるドロップダウンメニュー。
1. 編集するフィールドの列見出しの上にマウスポインターを置き、フィールド名の後の下向き矢印をクリックします。

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. クリック **フィールドを編集**&#x200B;をクリックし、フィールドに関する情報を更新して、 **保存**.

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >フィールドを保存した後は、フィールドタイプを更新できません。


1. （条件付き）リンクされたレコードフィールドの場合、 **参照フィールドの編集** リンクされたレコードタイプに対して、任意のフィールドを追加または削除します。

   詳しくは、 [レコードタイプを接続](../architecture-and-fields/connect-record-types.md).
