---
title: レコードタイプを削除
description: 関係がなくなったレコードタイプは削除できます。レコードタイプを削除すると、レコード、フィールド、ビューなど、レコードタイプに関連付けられているすべての情報も削除されます。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 70fd3887-3871-45b5-9c21-f57da63662aa
source-git-commit: 5bccad02f90fd99135b50c5a929913b16cc5b809
workflow-type: tm+mt
source-wordcount: '1071'
ht-degree: 21%

---


<!--keep the global record type reference in yellow till January 2026-->

# レコードタイプの削除

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

関係がなくなったレコードタイプは削除できます。

ただし、レコードタイプを削除すると、そのレコードタイプに関連付けられているすべての情報も削除されます。詳しくは、この記事で[レコードタイプを削除する際の考慮事項](#considerations-when-deleting-record-types)の節を参照してください。

レコードタイプについて詳しくは、[&#x200B; レコードタイプの概要 &#x200B;](/help/quicksilver/planning/architecture/overview-of-record-types.md) を参照してください。

<!-- last sentence might need to be deleted when we can recover or replace deleted record types-->

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
<ul> 
<li><p>任意のWorkfrontと任意の Planning パッケージ</p></li>
または
<li><p>任意のワークフローおよび任意の計画パッケージ</p></li></ul>

<p>グローバル・レコード・タイプを削除する手順は、次のとおりです。</p>
<ul><li><p>任意のWorkfront パッケージと Planning Plus パッケージ</p></li>
または
<li><p>任意のワークフローと Planning PrimeまたはUltimate パッケージ</p></li></ul>

<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。 </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td><p>標準</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースに対する権限の管理</p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>  </td> 
  </tr>  
</tbody> 
</table>

Workfrontのアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件 &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

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
   <td>   <p>Manage permissions to a workspace and record type</p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p></td> 
  </tr> 
</tbody> 
</table> 
-->


## レコードタイプを削除する際の考慮事項

<!--check this and ensure these are still true - some things might change with / after closed beta-->

* 自分が管理権限を持つワークスペースからは、レコードタイプのみを削除できます。
* レコードタイプを削除すると、それに関連付けられている次の情報が削除されます。

   * そのタイプのすべてのレコード。
   * そのレコードタイプに関連付けられているすべてのフィールド。
   * そのレコードタイプのすべてのビュー（フィルター、グループ化、並べ替え条件を含む）。
* そのレコードタイプは、ワークスペースにアクセスするすべてのユーザーから削除されます。
* 削除したレコードタイプやその情報は復元できません。
* 削除するレコードタイプに関連付けられているフィールドとレコードを別のレコードタイプで再作成してから削除することをお勧めします。

* 他のワークスペースに追加されているグローバル レコード タイプは削除できません。

  詳細については、この記事の「グローバル レコード タイプを削除する [&#x200B; を参照し &#x200B;](#delete-global-record-types) ください。

## レコードタイプの削除

{{step1-to-planning}}

1. レコードタイプを削除するワークスペースをクリックします。

   または

   ワークスペースから、既存のワークスペース名の右側にある下向き矢印を展開してワークスペースを検索し、リストに表示されたら選択します。

   ワークスペースが開き、レコードタイプが表示されます。
1. 次のいずれかの操作を行います。

   * レコードタイプカードにポインタを合わせ、「**詳細**」メニューをクリックしてから **削除** をクリックします。
   * 削除するレコードの種類のカードをクリックし、レコードの種類ページで、レコードの種類名の右側にある **その他** メニュー ![&#x200B; その他のメニュー &#x200B;](assets/more-menu.png) をクリックし、[**削除**] をクリックします。

     >[!TIP]
     >
     >グローバルレコードタイプは、追加されたセカンダリワークスペースからレコードタイプページから削除することはできません。 ワークスペースのレコードタイプカードからのみ削除できます。

     ![&#x200B; レコードタイプを完全に削除する確認 &#x200B;](assets/permanently-delete-record-type-confirmation.png)


1. 確認ボックスに **削除** と入力し、「**完全に削除**」をクリックします。 これは、大文字と小文字を区別しません。

   選択したレコードタイプは、フィールド、関連レコード、ビューと共に削除され、復元できません。

## グローバル レコード タイプの削除

グローバル レコード タイプを削除する場合は、次のシナリオが発生します。

* グローバルとして設定されたレコードタイプがまだ別のワークスペースに追加されていない場合は、元のワークスペースから削除できます。

* グローバルレコードタイプとして設定されたレコードタイプが 1 つ以上の他のワークスペースに追加されている場合、元のワークスペースから削除することはできません。 まず、グローバル レコード タイプを追加先のセカンダリ ワークスペースから削除する（削除する）必要があります。その後、グローバル レコード タイプを元のワークスペースから完全に削除できます。

### グローバルレコードタイプの元のワークスペースからの削除

関係がなくなったレコードタイプは、元のワークスペースから削除できます。

すべてのレコードとフィールドも削除され、復元できません。

1. 元のワークスペースのグローバルレコードタイプに移動します。

1. （条件付き）グローバルレコードタイプがセカンダリワークスペースに追加されているかどうかに応じて、次のいずれかの操作をおこないます。

   * レコードの種類がセカンダリ ワークスペースに追加されなかった場合、レコードの種類のカードの **その他** メニュー ![&#x200B; その他のメニュー &#x200B;](assets/more-menu.png)、またはページ上のレコードの種類の名前の右側をクリックし、[**削除**] をクリックします。
   * レコードタイプが 1 つ以上の他のセカンダリワークスペースに追加された場合、最初にセカンダリワークスペースに移動し、そのスペースからグローバルレコードを削除します。

     詳しくは、この記事の [&#x200B; セカンダリワークスペースからグローバルレコードタイプを削除する &#x200B;](#delete-a-global-record-type-from-a-secondary-workspace) を参照してください。

1. （条件付き）この記事の「レコードタイプを削除 [&#x200B; の節で説明しているように、レコードタイプの削除を続行 &#x200B;](#delete-record-types-1) ます。

   次のことが発生します。

   * グローバルレコードタイプが元のワークスペースから削除され、レコードタイプ、そのレコードおよびフィールドは復元できません。
   * セカンダリワークスペースのすべてのグローバルレコードとそのレコードもこのワークスペースから削除されます。

### グローバルレコードタイプのセカンダリワークスペースからの削除

追加したレコードタイプは、不要になったら別のワークスペースから削除できます。

次の点に注意してください。

* グローバルレコードタイプをセカンダリワークスペースから削除しても、レコードタイプは元のワークスペースに残ります。

* グローバルレコードタイプをセカンダリワークスペースから削除すると、次の項目も削除されます。

   * セカンダリワークスペースから追加されたレコードは、セカンダリワークスペースと元のワークスペースから削除され、復元できません。

  <!--Coming later: * The fields added from the secondary workspace.-->

* セカンダリ ワークスペースから削除されたグローバル レコード タイプはリカバリできません。

* 元のレコードタイプは、元のワークスペースと、それが追加された他のワークスペースに残ります。

* セカンダリワークスペースのレコードタイプに追加されたビューは保持され、共有されている場合は他のワークスペースに表示されます。

セカンダリワークスペースからグローバルレコードタイプを削除するには：

1. セカンダリワークスペースのグローバルレコードタイプに移動します。

1. （オプション）レコードタイプのカードの **詳細** メニュー ![&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックしてから、「**削除**」をクリックします。
1. （条件付き）表示されたフィールドに **削除** と入力し、「**完全に削除**」をクリックします。

   ![&#x200B; セカンダリ グローバル レコード タイプの削除の確認ボックス &#x200B;](assets/delete-secondary-global-record-type.png)

   次のことが発生します。

   * グローバル レコード タイプから作成されたレコード タイプは、選択したセカンダリ ワークスペースから削除されます。
   * フィールドを含む元のレコードタイプは、元のワークスペースに残ります。
   * レコードタイプは、追加された他のすべてのワークスペースに残ります。
   * セカンダリワークスペースからレコードタイプに追加されたレコード <!--and fields--> が削除されます。 グローバルレコードタイプが追加された追加のワークスペースから追加された他のすべてのレコードは、それぞれのワークスペースと元のワークスペースに保持されます。 &lt;!- フィールドが追加されたワークスペースに保持されます。


