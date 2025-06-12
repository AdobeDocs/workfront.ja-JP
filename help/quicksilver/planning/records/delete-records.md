---
title: レコードを削除
description: 自分または別のユーザーが作成したレコードを削除できます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 3f7a3667-8a9f-462a-b706-cf15850a0d1c
source-git-commit: 939f3d9a4fac609c014acfc3be3d1485f469e947
workflow-type: tm+mt
source-wordcount: '808'
ht-degree: 38%

---


# レコードの削除

<!--take Preview and Production references out at release-->

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

Adobe Workfront Planning 内で関係がなくなったレコードを削除できます。 削除されたレコードは、削除後 30 日間復元できます。 削除されたレコードのリカバリの詳細については、「[ 削除されたレコードのリカバリ ](/help/quicksilver/planning/records/restore-deleted-records.md)」を参照してください。

## アクセス要件

+++ 展開すると、アクセス要件が表示されます。

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
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfrontの計画<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td> 
<p>次のいずれかのWorkfront プラン：</p> 
<ul><li>選択</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning は、従来のWorkfront プランでは使用できません</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront Planning パッケージ*</p></td> 
   <td> 
<p>任意 </p> 
<p>各Workfront Planning プランに含まれる内容について詳しくは、Workfront担当営業または販売店にお問い合わせください。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>Workfront Planning にアクセスするには、組織のWorkfront インスタンスをAdobe Unified Experience にオンボーディングする必要があります。</p> 
<p>詳しくは、<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront の Adobe Unified Experience</a> を参照してください。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td><p> 標準</p>
   <p>Workfront Planning は、従来のWorkfront ライセンスでは使用できません</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペース <span class="preview"> およびレコードタイプ </span> に対する投稿以上の権限 </a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> <p>実稼動環境では、システム管理者を含むすべてのユーザーを、Planning を含むレイアウト・テンプレートに割り当てる必要があります。</p>
<p><span class="preview">プレビュー環境では、標準ユーザーとシステム管理者は、デフォルトで計画を有効にしています。</span></p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## レコードの削除に関する考慮事項

* 自分または別のユーザーが作成したレコードを削除できます。
* 実稼動環境では、削除したレコードを復元できません。 プレビュー環境で、削除されたレコードを復元できます。
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
1. （オプションおよび条件付き）プレビュー環境でレコードを削除した場合、レコードページのテーブルビューに移動して、ビューの右上隅にある **取り消し** アイコン ![ 取り消しアイコン ](assets/undo-icon.png) をクリックしてから、**最近削除されたレコード** をクリックして復元します。

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




