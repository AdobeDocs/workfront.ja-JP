---
title: フィールドを削除
description: Adobeマエストロでは、不要になったカスタムフィールドを削除できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: ce015eba8291995eec1611917896a0e797f820cc
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Delete fields
description: In Adobe Maestro, you can delete custom fields that are no longer relevant.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# フィールドを削除

>[!IMPORTANT]
>
>この記事の情報は、Adobe Workfrontからの新しいオファーであるAdobe・マエストロを指します。
>
>現在、Adobe・マエストロは、限られた数の顧客に対してオープンなベータプログラムの一部です。 Maestro 機能を使用するには、Workfrontのお客様である必要があります。
>
>Maestro のベータプログラムへの参加について詳しくは、アカウント担当者にお問い合わせください。
>
>詳しくは、 [Adobeマエストロの概要](../maestro-overview.md).

Adobeマエストロでは、レコードに関する情報を格納するカスタムフィールドを作成できます。

Maestro でのカスタムフィールドの作成について詳しくは、 [フィールドの作成](../fields/create-fields.md).

関連性がなくなったマエストロフィールドは削除できます。

## マエストロフィールドの削除に関する考慮事項：

* フィールドを削除できるのは、レコードタイプのテーブルビューだけです。
* レコードの主フィールドは削除できません。
* フィールドに格納されている情報はすべて削除され、復元できません。
* リンクされたレコードフィールドを削除すると、リンク元のレコードの種類から、リンクされたすべての参照フィールドも削除されます。 リンク先のレコードタイプのリンクされたレコードフィールドは削除されません。

  詳しくは、 [レコードタイプを接続](../architecture/connect-record-types.md).

<!-- this is not possible yet, since fields cannot be shared yet; maybe move this up a bit, in this bullet list: * When you delete a field, it is deleted from all records associated with the field.-->

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
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfrontまたはグループ管理者は、レイアウトテンプレートに Maestro 領域を追加する必要があります。 詳しくは、 <a href="../access/access-overview.md">アクセスの概要</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する権限の管理</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています</p>
</td>
  </tr>
 </tbody>
</table>



<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## フィールドを削除

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-maestro}}

これにより、Maestro で最後にアクセスしたワークスペースが開きます。
1. フィールドを削除するレコードタイプのカードをクリックします。
1. （条件付き） **テーブル表示** から **表示** レコードタイプページの右上隅にあるドロップダウンメニュー。
1. 列ヘッダーで削除するフィールドを見つけ、列ヘッダーの上にマウスポインターを置き、フィールド名の後の下向き矢印をクリックします。

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. クリック **削除**. <!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. クリック **削除** をクリックして確定します。

   フィールドが削除され、復元できず、レコードと関連付けられなくなります。
