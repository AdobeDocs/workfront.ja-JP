---
title: レコードを削除
description: 自分または別のユーザーが作成したレコードを削除できます。 削除したレコードは復元できません。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: a0f12a016ae8ac73136f05bf3255f9882e2ce6d4
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 7%

---

<!--update the metadata with real information when making this available in TOC and in the left nav-->

# レコードを削除

{{maestro-important-intro}}

Adobe Workfrontの計画で関連性がなくなったレコードは削除できます。

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
<p>組織がAdobe Workfront Planning ベータプログラムに登録されている必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
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
   <td> <p>Adobe Workfront Planning には、アクセスレベルの制御はありません </p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに権限を付与する（またはそれ以上の場合）</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfrontまたはグループ管理者は、レイアウトテンプレートに計画領域を追加する必要があります。 詳しくは、 <a href="../access/access-overview.md">アクセスの概要</a>. </p>  
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
* 削除したレコードは復元できません。 <!--the above statements (and in the metadata description) will change with access levels and recycle bin??-->
* 削除したレコードが他のレコードにリンクされている場合、リンクされたレコードは削除されませんが、削除したレコードの情報も削除されます。
* レコードは一括で削除できません。 <!--this will probably change-->
* タイムラインビューからレコードを削除することはできません。

## レコードを削除

次の領域からレコードを削除できます。

* [レコードの詳細ページから](#delete-a-record-from-the-records-details-page)
* [レコードタイプのテーブルビューから](#delete-a-record-from-the-record-type-table-view)

### レコードの詳細ページからレコードを削除する

{{step1-to-maestro}}

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

{{step1-to-maestro}}

最後にアクセスしたワークスペースが開きます。

1. レコードタイプをクリックします。

   レコードタイプのページが開きます。
1. （条件付き） **表示** テーブルの左上隅にあるドロップダウンメニューから、テーブルビューを選択します。 最後にアクセスしたときにタイムラインビューでレコードタイプを表示した場合を除き、これがデフォルトのビューになります。

   選択したレコードタイプに関連付けられているレコードが、テーブルビューに表示されます。
1. 次のいずれかの操作を行います。

   * レコード行を右クリックし、 **削除**.
   * 次をクリック： **その他** メニュー ![](assets/more-menu.png) をクリックし、 **削除**

     ![](assets/contextual-menu-for-record-row.png)

   * 次をクリック： **詳細を開く** アイコン ![](assets/open-details-icon-in-table-name-field.png) をクリックして [ 詳細 ] ボックスを開き、 **その他** ![](assets/more-menu.png) をレコード名の右に追加し、 **削除**.

   レコードは削除されているため、復元できません。

1. （オプション）次のキーボードショートカットを使用して、レコードの削除の取り消しとやり直しを行います。

   * Ctrl + Z( Macの場合は⌘ + Z)：変更を元に戻します。
   * Ctrl + Shift + Z(Macの場合は⌘ + Shift + Z)：変更をやり直します。
