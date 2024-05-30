---
title: レコードの削除
description: 自分または別のユーザーが作成したレコードを削除できます。削除したレコードは復元できません。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: 1369269bcb64bd32f26603608782dc996b079cb9
workflow-type: tm+mt
source-wordcount: '478'
ht-degree: 97%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# レコードの削除

{{planning-important-intro}}

Adobe Workfront Planning で関係がなくなったレコードを削除できます。

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
   <td role="rowheader"><p>Adobe Workfront ライセンス</p>
   </td>
   <td>
   <p>任意</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベル設定</p></td>
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。 </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する参加以上の権限</a> </p>  
   <p>システム管理者は、自身が作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront 管理者やグループ管理者は、レイアウトテンプレートに Planning エリアを追加する必要があります。詳しくは、<a href="../access/access-overview.md">アクセス権の概要</a>を参照してください。 </p>  
</td>
  </tr>

</tbody>
</table>


<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## レコードの削除に関する考慮事項

* 自分または別のユーザーが作成したレコードを削除できます。
* 削除したレコードを元に戻すことはできません。<!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* 削除されたレコードが他のレコードにリンクされている場合、リンクされているレコードは削除されませんが、削除されたレコードの情報も削除されます。
* レコードを一括で削除できません。<!--this will probably change-->
* タイムラインビューからレコードを削除できません。

## レコードの削除

次のエリアからレコードを削除できます。

* [レコードのページから](#delete-a-record-from-the-records-page)
* [レコードタイプのテーブルビューから](#delete-a-record-from-the-record-type-table-view)

### レコードのページからのレコードの削除

{{step1-to-maestro}}

最後にアクセスしたワークスペースが開きます。

1. レコードタイプをクリックします。

   レコードタイプのページが開きます。
1. 次のいずれかの操作を行います。

   * テーブルビューで、レコードの名前をクリックします。
   * テーブルビューで、レコードの名前にポインタを合わせ、「**詳細**」メニュー![](assets/more-menu.png)、「**表示**」の順にクリックします。

     ![](assets/contextual-menu-for-record-row.png)
   * タイムラインビューで、レコードバーをクリックします。

   レコードページが開きます。

1. レコード名の右側にある「**詳細**」メニュー ![](assets/more-menu.png) をクリックし、「**削除**」をクリックします。再度「**削除**」をクリックして確認します。

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
レコードが削除されます。これは復元できません。

### レコードタイプのテーブルビューからのレコードの削除

{{step1-to-maestro}}

最後にアクセスしたワークスペースが開きます。

1. レコードタイプをクリックします。

   レコードタイプのページが開きます。
1. （条件付き）テーブルの左上隅にある&#x200B;**ビュー**&#x200B;ドロップダウンメニューから、テーブルビューを選択します。最後にアクセスしたときにタイムラインビューでレコードタイプを表示した場合を除き、これがデフォルトのビューになります。

   選択したレコードタイプに関連付けられているレコードが、テーブルビューに表示されます。
1. 次のいずれかの操作を行います。

   * レコード行を右クリックし、「**削除**」をクリックします。
   * レコード名の右側にある&#x200B;**詳細**&#x200B;メニュー ![](assets/more-menu.png) をクリックし、「**削除**」をクリックします。

     ![](assets/contextual-menu-for-record-row.png)

   * **詳細を開く**&#x200B;アイコン ![](assets/open-details-icon-in-table-name-field.png) をクリックしてレコードの詳細情報を含むボックスを開き、レコード名の右側にある「**詳細**」![](assets/more-menu.png) をクリックして、「**削除**」をクリックします。

   レコードが削除されました。これは復元できません。

1. （任意）次のキーボードショートカットを使用すると、レコードの削除を取り消したり、やり直したりすることができます。

   * Ctrl + Z（Mac の場合は ⌘ + z）で、変更を取り消します
   * Ctrl + Shift + Z（Mac の場合は ⌘ + Shift + Z）で、変更を元に戻します
