---
title: レコードを削除
description: 自分または別のユーザーが作成したレコードを削除できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: e26a3d0e283182e08902c263252c8d067838c23a
workflow-type: tm+mt
source-wordcount: '617'
ht-degree: 35%

---


# レコードの削除

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>  -->

{{planning-important-intro}}

Adobe Workfront Planning 内で関係がなくなったレコードを削除できます。 削除されたレコードは、削除後 30 日間復元できます。 削除されたレコードのリカバリの詳細については、「[ 削除されたレコードのリカバリ ](/help/quicksilver/planning/records/restore-deleted-records.md)」を参照してください。

## アクセス要件

+++ 展開して、この記事の機能のアクセス要件を表示します。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>任意のWorkfrontと任意の Planning パッケージ</p> <p>任意のワークフローおよび任意の計画パッケージ</p>
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースおよびレコードタイプへの投稿以上の権限  </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p> </td> 
  </tr>   
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++   


<!--Old:
<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
<td> 
   <p> Products</p> </td> 
   <td> 
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfront Planning<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> 
<p>Any of the following Workfront plans:</p> 
<ul><li>Select</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning is not available for legacy Workfront plans</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning package*</p></td> 
   <td> 
<p>Any </p> 
<p>For more information about what is included in each Workfront Planning plan, contact your Workfront account manager. </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Your organization's instance of Workfront must be onboarded to the Adobe Unified Experience to be able to access Workfront Planning.</p> 
<p>For more information, see <a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Adobe Unified Experience for Workfront</a>. </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td><p> Standard</p>
   <p>Workfront Planning is not available for legacy Workfront licenses</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Access level configuration</p></td> 
   <td> <p>There are no access level controls for Adobe Workfront Planning</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Object permissions</p></td> 
   <td>   <p>Contribute or higher permissions to a workspace and record type </a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p> </td> 
  </tr> 
</tbody> 
</table> -->

## レコードの削除に関する考慮事項

* 自分または別のユーザーが作成したレコードを削除できます。
* 自分または他のユーザーが削除した削除済みレコードを復元できます。
* 削除したレコードが別のレコードにリンクされている場合、リンクされているレコードは削除されませんが、削除したレコードの情報は削除されます。
* タイムラインビューやカレンダービューからレコードを削除することはできません。

## レコードの削除

次のエリアからレコードを削除できます。

* [レコードのページから](#delete-a-record-from-the-records-page)
* [レコードタイプのテーブルビューから](#delete-a-record-from-the-record-type-table-view)

### レコードのページからのレコードの削除

{{step1-to-planning}}

1. レコードを削除するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。
1. 次のいずれかの操作を行います。

   * テーブルビューで、レコードの名前をクリックします。
   * テーブル表示で、レコード名の上にマウスポインターを置き、**詳細** メニュー ![ 詳細メニュー ](assets/more-menu.png) をクリックしてから、**表示** をクリックします

     ![ レコード行のコンテキストメニュー ](assets/contextual-menu-for-record-row.png)
   * タイムラインビューで、レコードバーをクリックします。

   レコードページが開きます。

1. レコード名の右側にある **その他** メニュー ![ その他メニュー ](assets/more-menu.png) をクリックし、もう一度 **削除** をクリックして **削除** をクリックして確認します。

   ![ レコードの詳細ページのその他のメニューオプション ](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->
レコードが削除されます。
1. （オプション）レコードページのテーブルビューに移動して、ビューの右上隅にある **取り消し** アイコン ![ 取り消しアイコン ](assets/undo-icon.png) をクリックしてから、**最近削除されたレコード** をクリックして削除したレコードを復元します。

削除されたレコードのリカバリの詳細については、「[ 削除されたレコードのリカバリ ](/help/quicksilver/planning/records/restore-deleted-records.md)」を参照してください。

### レコードタイプのテーブルビューからレコードを削除する

{{step1-to-planning}}

1. レコードを削除するワークスペースをクリックします。

   ワークスペースが開き、レコードタイプがカードとして表示されます。

1. レコードタイプのカードをクリックします。

   レコードタイプのページが開きます。
1. （条件付き）テーブルの左上隅にある&#x200B;**ビュー**&#x200B;ドロップダウンメニューから、テーブルビューを選択します。最後にアクセスしたときにタイムラインビューでレコードタイプを表示した場合を除き、これがデフォルトのビューになります。

   選択したレコードタイプに関連付けられているレコードが、テーブルビューに表示されます。
1. 次のいずれかの操作を行います。

   * レコード行を右クリックし、「**削除**」をクリックします。
   * レコード名の右側にある **その他** メニュー ![ その他メニュー ](assets/more-menu.png) をクリックし、「**削除**」をクリックします。

     ![ レコード行のコンテキストメニュー ](assets/contextual-menu-for-record-row.png)

   * **詳細を開く** アイコン ![ テーブル名フィールドで詳細を開くアイコン ](assets/open-details-icon-in-table-name-field.png) をクリックしてレコードの詳細情報を含むボックスを開き、レコード名の右側にある **詳細**![ 詳細メニュー ](assets/more-menu.png) をクリックしてから、**削除** をクリックします。

   レコードが削除されます。

1. （オプション）レコードの削除を取り消すまたはやり直すには、次のいずれかの操作を行います。

   * **取り消し** アイコン ![ 取り消しアイコン ](assets/undo-icon.png) をクリックし、**最近削除された項目** をクリックすると、削除されたレコードを復元できます。 削除されたレコードのリカバリの詳細については、「[ 削除されたレコードのリカバリ ](/help/quicksilver/planning/records/restore-deleted-records.md)」を参照してください。
   * レコードの削除の取り消しまたはやり直しには、次のキーボードショートカットを使用します。

      * レコードの削除を元に戻すには CTRL + Z （Macの場合は ⌘ + Z）
      * レコードの削除をやり直すには、Ctrl + Shift + Z （Macの場合は ⌘ + Shift + Z）




