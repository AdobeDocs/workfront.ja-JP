---
title: フィールドを削除
description: Adobeマエストロでは、不要になったカスタムフィールドを削除できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 908a3136b2537310305f282b7a76d8f09cae3836
workflow-type: tm+mt
source-wordcount: '370'
ht-degree: 1%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# フィールドを削除

>[!IMPORTANT]
>
>この記事の情報は、Adobe・マエストロに関して、Adobeからの新しいオファーです。
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

Adobeマエストロでは、レコードに関する情報を格納するカスタムフィールドを作成できます。

Maestro でのカスタムフィールドの作成について詳しくは、 [フィールドの作成](../architecture-and-fields/create-fields.md).

関連性がなくなったマエストロフィールドは削除できます。

## マエストロフィールドの削除に関する考慮事項：

* 自分が作成したフィールドや他のユーザーが作成したフィールドを削除できます。 <!--this will change with access levels/ permissions-->
* レコードタイプテーブル内のフィールドのみを削除できます。
* フィールドに格納されている情報はすべて削除され、復元できません。
* リンクされたレコードフィールドを削除すると、リンク元のレコードの種類から、リンクされたすべての参照フィールドも削除されます。 リンク先のレコードタイプのリンクされたレコードフィールドは削除されません。

  詳しくは、 [レコードタイプを接続](../architecture-and-fields/connect-record-types.md).
  <!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

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

## フィールドを削除

<!--When they release the sharing of fields between other records, revise this section.  -->

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-workfront.png) Workfrontの右上隅に <!--or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> 次に、「 **マエストロ** ![](assets/maestro-icon.png).

   これにより、Maestro で最後にアクセスしたワークスペースが開きます。
1. フィールドを削除するレコードタイプのカードをクリックします。
1. （条件付き） **テーブル表示** から **表示** レコードタイプページの右上隅にあるドロップダウンメニュー。
1. 列ヘッダーで削除するフィールドを見つけ、列ヘッダーの上にマウスポインターを置き、フィールド名の後の下向き矢印をクリックします。

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. クリック **削除**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. クリック **削除** をクリックして確定します。

   フィールドが削除され、復元できず、レコードと関連付けられなくなります。
