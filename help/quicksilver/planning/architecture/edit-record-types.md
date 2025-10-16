---
title: レコードタイプを編集
description: 保存後にレコードタイプを編集できます。レコードタイプは、Adobe Workfront Planning のオブジェクトタイプです。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 2fb95d37c32984e248767993c4858038d27e0590
workflow-type: tm+mt
source-wordcount: '634'
ht-degree: 27%

---


# レコードタイプの編集

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{planning-important-intro}}

レコードタイプは、Adobe Workfront Planning のオブジェクトタイプです。自分または他のユーザーが作成したレコードタイプの外観を編集できます。Workfront Planning レコードタイプの作成について詳しくは、[レコードタイプの作成](/help/quicksilver/planning/architecture/create-record-types.md)を参照してください。

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
<p>任意のWorkfrontおよび Planning パッケージ</p>
<p>任意のWorkfrontおよび Planning パッケージ</p>
<p><b>メモ</b></p>
<p>接続可能なレコード・タイプを構成する手順は、次のとおりです。 </p>
<ul> 
<li><p>任意のWorkfront パッケージと任意の Planning パッケージ</p></li>
<p>または</p>
<li><p>任意のワークフローと Planning PrimeまたはUltimate パッケージ</p></li></ul>

<div class="preview">
<p>グローバルレコードタイプを設定するには：</p>

<ul> 
<li><p>任意のWorkfront パッケージと Planning Plus パッケージ</p></li>
<p>または</p>
<li><p>任意のワークフローと Planning PrimeまたはUltimate パッケージ</p></li></ul>
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。 </p>

</div>
   </td> </tr>
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
   <td><p> Standard </p>
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
   <td>   <p>Manage permissions to a workspace and record type </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
   <p>Only system administrators can enable record types to connect from other workspaces</p> </td> 
  </tr> 

</tbody> 
</table> -->

## レコードタイプの編集

{{step1-to-planning}}

1. レコードタイプを編集するワークスペースをクリックします。

   ワークスペースページが開き、レコードタイプが表示されます。
1. 次のいずれかの操作を行います。

   * レコードタイプのカードにポインタを合わせ、レコードタイプのカードの右上隅にある **その他** メニュー ![&#x200B; その他のメニュー &#x200B;](assets/more-menu.png) をクリックしてから、**編集** をクリックします
     <span class="preview"> または **設定**</span>
または
   * レコードタイプカードをクリックしてレコードタイプページを開き、レコードタイプ名の右側にある **詳細** メニュー ![&#x200B; 詳細メニュー &#x200B;](assets/more-menu.png) をクリックしてから、**編集**<span class="preview"> または **設定**</span> をクリックします。

   <span class="preview">![&#x200B; 設定付きレコードタイプカードのその他のメニューオプション &#x200B;](assets/more-menu-options-from-record-type-card-with-settings-link.png)</span>

1. **レコードタイプを編集** ボックスで、「**外観** タブがデフォルトで開きます。<!--update screen shot below at production-->

   ![&#x200B; レコードタイプを編集ボックスの「外観」タブ &#x200B;](assets/edit-record-type-box-appearance-tab.png)

   「**外観**」タブで次の情報を更新します。

   * 必要に応じて、レコードタイプ名を編集します。<!--did they add a field label for this?-->
   * **説明**：詳しい情報を含むレコードタイプの説明を編集または追加します。
   * レコードタイプに関連付けられたアイコンの色と形状を編集します。 次の操作を実行します。
      * レコードタイプを識別するための色を選択します。これは、レコードタイプアイコンの色です。
      * リストからアイコンを選択するか、アイコンの名前を入力して何を表しているか説明し、表示されたら選択します。これは、レコードタイプのアイコンです。ファイルのアイコンはデフォルトで選択されています。

1. （オプションおよび条件付き）システム管理者の場合は、**詳細設定**<span class="preview"> または **クロスワークスペース設定**</span> タブをクリックして、レコードタイプのクロスワークスペース機能に関する情報を更新します。

   詳しくは、[&#x200B; レコードタイプのクロスワークスペース機能の設定 &#x200B;](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) を参照してください。<!--update screen shot at production - Jan 2026-->

   ![&#x200B; 「詳細設定」タブの「レコードタイプを編集」ボックス &#x200B;](assets/edit-record-type-box-advanced-settings-tab.png)

1. 「**保存**」をクリックします。

   このレコードを他のワークスペースから接続することを選択した場合、レコード カードに **接続可能なレコード** アイコン ![&#x200B; 他のスペースから接続アイコン &#x200B;](assets/connect-from-other-workspaces-icon.png) が表示されます。

   <span class="preview"> このレコードを他のワークスペースに追加することを許可するように選択した場合、レコードカードに **グローバルレコード** アイコン ![&#x200B; グローバルレコードタイプアイコン &#x200B;](assets/global-icon.png) が表示されます。</span>

1. （オプション）ワークスペース領域からレコードタイプカードをクリックしてレコードタイプのページを開き、ヘッダーでレコードタイプの名前を変更します。

1. （オプション）別のレコードの種類を編集するには、レコードの種類のページで、レコードの種類名の右側にある下向き矢印を展開し、レコードの種類を検索してから、一覧に表示されるときにその種類を選択します。

   ![&#x200B; 検索ボックス付きレコードタイプページのレコードタイプドロップダウン &#x200B;](assets/record-type-drop-down-on-record-type-page-with-search-box.png)
