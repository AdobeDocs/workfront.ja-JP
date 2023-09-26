---
title: レコードタイプを編集
description: 保存後にレコードタイプを編集できます。 レコードタイプは、AdobeMaestro のオブジェクトタイプです。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 28602d66b43ec4c30a9f13cff43157b978439d99
workflow-type: tm+mt
source-wordcount: '417'
ht-degree: 1%

---


<!--update the metadata with real information when making this available in TOC and in the left nav
---
title: Edit record types
description: You can edit record types after they have been saved. Record types are the objec types of Adobe Maestro.
author: Alina
role: User
feature: Work Management 
topic: Architecture
hidefromtoc: yes
hide: yes
---

-->

# レコードタイプを編集

>[!IMPORTANT]
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

レコードタイプは、AdobeMaestro のオブジェクトタイプです。 自分または他のユーザーが作成したレコードタイプの外観を編集できます。 Maestro レコードタイプの作成について詳しくは、 [レコードタイプの作成](../architecture-and-fields/create-record-types.md).

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

## レコードタイプを編集

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-workfront.png) Workfrontの右上隅に <!---or the **Main menu** icon ![](assets/main-menu-shell.png)  in the upper-left corner, if available--> 次に、「 **マエストロ** ![](assets/maestro-icon.png).

   最後にアクセスしたワークスペースは、デフォルトで開きます。

1. （オプション）既存のワークスペース名の右側にある下向き矢印を展開し、レコードタイプを作成するワークスペースを選択します。
1. レコードタイプのカードの上にマウスポインターを置いて、 **その他** メニュー ![](assets/more-menu.png) レコードタイプカードの右上隅にあるをクリックし、 **外観を更新**.

   ![](assets/update-appearance-link-from-more-menu-on-record-type-card.png)

1. [ レコードの種類の更新 ] ボックスで、次の情報を更新します。

   * **レコード名**：必要に応じて、レコードタイプ名を編集します。 <!--correct this - I asked Garik to change this field to "Record type name"-->
   * **外観**：レコードタイプに関連付けられたアイコンの色と形状を編集します。 次の操作を実行します。
      * レコードの種類を識別する色を選択します。 これは、レコードタイプアイコンの色です。 デフォルトでは「グレー」が選択されています。
      * リストからアイコンを選択するか、アイコンの名前を入力して内容を説明し、表示されたときに選択します。 これは、レコードタイプのアイコンです。 デフォルトでは、ファイルアイコンが選択されています。

     ![](assets/update-record-type-box.png)

1. 「レコードタイプを更新」ボックスの外側をクリックして、変更を保存します。
1. （オプション）ワークスペース領域でレコードタイプカードをクリックして、レコードタイプのページを開きます。
1. 次をクリック： **その他** レコードタイプ名の右にあるメニューをクリックし、 **名前を変更** レコードタイプの名前を変更するには

   または

   ヘッダーのレコードタイプの名前を変更します。  <!--check to see if they renamed this to "Rename" - it kept going back and forth between Rename and Edit-->

   ![](assets/more-menu-options-from-record-details-page.png) <!--check this screen shot - not sure this is valid ???-->

   レコードタイプのページのヘッダーでレコードタイプの名前を変更することもできます。

