---
title: レコードタイプを編集
description: 保存後にレコードタイプを編集できます。レコードタイプは、Adobe Workfront Planning のオブジェクトタイプです。
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 5d326776b9c5b4d9d24e802375df4630508c8bd0
workflow-type: tm+mt
source-wordcount: '571'
ht-degree: 26%

---


# レコードタイプの編集

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

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
または
<li><p>任意のワークフローと Planning PrimeまたはUltimate パッケージ</p></li></ul>


<p>グローバルレコードタイプを設定するには：</p>

<ul> 
<li><p>任意のWorkfront パッケージと Planning Plus パッケージ</p></li>
または
<li><p>任意のワークフローと Planning PrimeまたはUltimate パッケージ</p></li></ul>
<p>各Workfront Planning パッケージに含まれる内容について詳しくは、Workfront アカウント担当者にお問い合わせください。 </p>

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

   * レコードタイプのカードにポインタを合わせ、レコードタイプのカードの右上隅にある **その他** メニュー ![ その他のメニュー ](assets/more-menu.png) をクリックしてから、**編集** または **設定** をクリックします。
または
   * レコードタイプカードをクリックしてレコードタイプページを開き、レコードタイプ名の右側にある **詳細** メニュー ![ 詳細メニュー ](assets/more-menu.png) をクリックしてから、**編集** または **設定** をクリックします。

   ![ 設定付きレコードタイプカードのその他のメニューオプション ](assets/more-menu-options-from-record-type-card-with-settings-link.png)

1. **レコードタイプを編集** ボックスで、「**外観** タブがデフォルトで開きます。

   ![ レコードタイプを編集ボックスの「外観」タブ ](assets/edit-record-type-box-appearance-tab.png)

   「**外観**」タブで次の情報を更新します。

   * 必要に応じて、レコードタイプ名を編集します。<!--did they add a field label for this?-->
   * **説明**：詳しい情報を含むレコードタイプの説明を編集または追加します。
   * レコードタイプに関連付けられたアイコンの色と形状を編集します。 次の操作を実行します。
      * レコードタイプを識別するための色を選択します。これは、レコードタイプアイコンの色です。
      * リストからアイコンを選択するか、アイコンの名前を入力して何を表しているか説明し、表示されたら選択します。これは、レコードタイプのアイコンです。ファイルのアイコンはデフォルトで選択されています。

1. （オプションおよび条件付き）システム管理者の場合は、「**クロスワークスペース設定**」タブをクリックして、レコードタイプのクロスワークスペース機能に関する情報を更新します。

   詳しくは、[ レコードタイプに対するクロスワークスペース機能の設定 ](/help/quicksilver/planning/architecture/configure-record-type-cross-workspace-capabilities.md) を参照してください。

   ![ クロスワークスペース設定タブを使用してレコードタイプを編集ボックス ](assets/edit-record-type-box-advanced-settings-tab.png)

1. 「**保存**」をクリックします。

   このレコードを他のワークスペースから接続することを選択した場合、レコード カードに **接続可能なレコード** アイコン ![ 他のスペースから接続アイコン ](assets/connect-from-other-workspaces-icon.png) が表示されます。

   このレコードを他のワークスペースに追加することを許可した場合、レコードカードに **グローバルレコード** アイコン ![ グローバルレコードタイプアイコン ](assets/global-icon.png) が表示されます。

1. （オプション）ワークスペース領域からレコードタイプカードをクリックしてレコードタイプのページを開き、ヘッダーでレコードタイプの名前を変更します。

1. （オプション）別のレコードの種類を編集するには、レコードの種類のページで、レコードの種類名の右側にある下向き矢印を展開し、レコードの種類を検索してから、一覧に表示されるときにその種類を選択します。

   ![ 検索ボックス付きレコードタイプページのレコードタイプドロップダウン ](assets/record-type-drop-down-on-record-type-page-with-search-box.png)
