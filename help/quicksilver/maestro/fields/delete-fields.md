---
title: フィールドの削除
description: Adobe Workfront Planning では、関係なくなったカスタムフィールドを削除できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ec48db42-2395-4439-97ae-e4f5242170b7
source-git-commit: 1369269bcb64bd32f26603608782dc996b079cb9
workflow-type: tm+mt
source-wordcount: '323'
ht-degree: 95%

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

# フィールドの削除

{{planning-important-intro}}

Adobe Workfront Planning では、カスタムフィールドを作成して、レコードに関する情報を格納できます。

Workfront Planning でのカスタムフィールドの作成について詳しくは、[フィールドの作成](../fields/create-fields.md)を参照してください。

関係がなくなった Workfront Planning フィールドは削除できます。

## Workfront Planning フィールドの削除に関する考慮事項：

* レコードタイプのテーブルビューでのみフィールドを削除できます。
* レコードの主フィールドは削除できません。
* フィールドに格納されている情報はすべて削除され、復元できません。
* リンクされたレコードフィールドを削除すると、リンクされたすべてのルックアップフィールドもリンク元のレコードタイプから削除されます。リンク先のレコードタイプのリンクされたレコードフィールドは削除されません。

  詳しくは、[レコードタイプの接続](../architecture/connect-record-types.md)を参照してください。

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
 <td role="rowheader"><p>Adobe Workfront の契約</p></td>
   <td>
<p>Workfront Planning の早期アクセス段階に登録されている必要があります </p>
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
   <td> <p>Workfront Planning に対するアクセスレベルのコントロールはありません</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront 管理者やグループ管理者は、レイアウトテンプレートに Planning エリアを追加する必要があります。詳しくは、<a href="../access/access-overview.md">アクセス権の概要</a>を参照してください。 </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する権限を管理</a> </p>  
   <p>システム管理者は、自身が作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>
</td>
  </tr>
 </tbody>
</table>



<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## フィールドの削除

<!--When they release the sharing of fields between other records, revise this section.  -->

{{step1-to-maestro}}

これにより、Workfront Planning で最後にアクセスしたワークスペースが開きます。
1. フィールドを削除するレコードタイプのカードをクリックします。
1. （条件付き）レコードタイプページの右上隅にある&#x200B;**表示**&#x200B;ドロップダウンメニューから「**テーブルビュー**」を選択します。
1. 削除するフィールドを列ヘッダーで見つけてその上にポインタを合わせ、フィールド名の後の下向き矢印をクリックします。

   ![](assets/arrow-menu-after-name-of-field-in-table-header-highlighted.png)

1. 「**削除**」をクリックします。<!-- check this: they might replace it with **Delete field**-->

   <!--insert screen shot when finalized-->

1. 「**削除**」をクリックして確定します。

   フィールドが削除され、復元できなくなり、レコードと関連付けられなくなります。
