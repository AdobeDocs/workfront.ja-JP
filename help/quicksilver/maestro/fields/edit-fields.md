---
title: フィールドの編集
description: Adobe Workfront Planning では、作成済みのフィールドのフィールド設定を編集できます。 ここでは、Workfront計画フィールドの設定を編集する方法について説明します。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 6c35c313-d6ed-428b-b70d-2ea242da4e8f
source-git-commit: 6ec985d10a5fd7a4a9307b705f48734d76aec181
workflow-type: tm+mt
source-wordcount: '469'
ht-degree: 23%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!---
title: Edit foelds
description: In Adobe Maestro, you can edit the field settings for fields that are already created.
hidefromtoc: yes
hide: yes
author: Alina
feature: (*******************WE NEED A NEW ONE*******************)
role: User, Administrator (************is this right???************)
recommendations: noDisplay, noCatalog
--->

# フィールドの編集

{{maestro-important-intro}}

Adobe Workfront Planning で既に作成されているフィールドのフィールド設定を編集できます。

Adobe Workfront Planning フィールドの作成の詳細は、次を参照してください： [フィールドの作成](../fields/create-fields.md).

ここでは、Workfront計画フィールドの設定を編集する方法について説明します。 レコードのフィールド値の編集については、を参照してください [レコードを編集](/help/quicksilver/maestro/records/edit-records.md).

## フィールド設定の編集に関する考慮事項

フィールドの設定を変更する前に、次の点を考慮する必要があります。

* フィールドが属するワークスペースへの管理権限がある場合は、自分が作成したフィールドや、他のユーザーが作成したフィールドを編集できます。
* レコードタイプ テーブルのフィールドを編集できます。
* レコード ページまたはテーブル ビュー以外の他のビューでフィールドを編集することはできません。
* フィールドの保存後にフィールドタイプを編集することはできません。
* 「数値」、「パーセント」または「通貨」フィールドで、添付対象のレコードにマイナスの値が格納されている場合は、以前に選択した「マイナスの値を許可」設定を選択解除できません。

<!--this is not true yet, but will be with the release of RTBE for field configuration changes: 

* You can edit the configuration of the following fields, after they are saved:

    * The Name or the Description of any field
    * The Options of a Single-select or a Multi-select field.
    * The expression of a Formula field.-->

<!--this is not yet true, but it might come later:
* You can deselect Allow negative numbers option from a Number, Percentage, or Currency field after you save the field. 
-->

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
   <td role="rowheader"><p>アクセスレベルの設定</p></td>
   <td> <p>Workfront Planning にはアクセス制御はありません</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する権限を管理</a> </p>  
   <p>システム管理者は、自身が作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront管理者またはグループ管理者が、レイアウトテンプレートにプランニング エリアを追加する必要があります。 詳しくは、<a href="../access/access-overview.md">アクセス権の概要</a>を参照してください。 </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## フィールド設定を編集

{{step1-to-maestro}}

    最後にアクセスしたワークスペースは、デフォルトで開きます。

1. （オプション）既存のワークスペース名の右側にある下向き矢印を展開し、レコードタイプを削除するワークスペースを選択します。

   ワークスペースが開き、それに関連付けられたレコードタイプが表示されます。
1. 編集するフィールドを持つレコードタイプのカードをクリックします。

   レコードタイプのページが開きます。
1. （条件付き）のタブをクリック **テーブル表示**.
1. 編集するフィールドの列見出しにポインタを合わせ、フィールド名の後の下向き矢印をクリックして、クリックします **フィールドを編集**

   または

   フィールドの列見出しをダブルクリックします。

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. フィールドに関する情報を更新し、をクリックします **保存**.

   <!--insert screen shot when finalized-->

   >[!TIP]
   >
   >フィールドを保存した後は、フィールドタイプを更新できません。

   フィールド情報は、ワークスペースを表示するアクセス権を持つすべてのユーザーに対して更新されます。

   <!--After the release of the RTBE for field configurations, replace the tip with this:

    >[!TIP]
    >
    >* You cannot update the field type after the field is saved.
    >
    >* When you modify field configurations (field options or formula expressions), records that already contain information in the modified fields will update their values in real-time. There is no warning and no audit log for the value changes triggered by field configuration changes. All users who view the fields will immediately see the new values with the modifications. 
    -->


1. （条件付き）リンクされたレコードフィールドで、 **参照フィールドを編集** また、リンクされたレコードタイプにフィールドを追加したり、いずれかのフィールドをリンクされたレコードタイプから削除したりできます。

   詳しくは、[レコードタイプの接続](../architecture/connect-record-types.md)を参照してください。
